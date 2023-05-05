# Comparing `tmp/BBFinance-1.5.1.tar.gz` & `tmp/BBFinance-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.5.1.tar", last modified: Fri May  5 17:31:28 2023, max compression
+gzip compressed data, was "BBFinance-1.5.2.tar", last modified: Fri May  5 19:59:23 2023, max compression
```

## Comparing `BBFinance-1.5.1.tar` & `BBFinance-1.5.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:18.366284 BBFinance-1.5.1/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:11.333101 BBFinance-1.5.1/BBFdocs/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:11.442492 BBFinance-1.5.1/BBFdocs/docs/
--rw-rw-rw-   0        0        0     4250 2023-04-11 14:25:22.000000 BBFinance-1.5.1/BBFdocs/docs/index.md
--rw-rw-rw-   0        0        0       84 2023-04-10 19:53:10.000000 BBFinance-1.5.1/BBFdocs/mkdocs.yml
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:11.880039 BBFinance-1.5.1/BBFdocs/site/
--rw-rw-rw-   0        0        0     6094 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/404.html
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:12.895743 BBFinance-1.5.1/BBFdocs/site/css/
--rw-rw-rw-   0        0        0     5635 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/css/base.css
--rw-rw-rw-   0        0        0     3487 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/css/base.min.css
--rw-rw-rw-   0        0        0   132465 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/css/bootstrap-custom.css
--rw-rw-rw-   0        0        0   109468 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/css/bootstrap-custom.min.css
--rw-rw-rw-   0        0        0     2131 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/css/cinder.css
--rw-rw-rw-   0        0        0     1637 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/css/cinder.min.css
--rw-rw-rw-   0        0        0     1148 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/css/highlight.css
--rw-rw-rw-   0        0        0      866 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/css/highlight.min.css
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:13.177023 BBFinance-1.5.1/BBFdocs/site/fonts/
--rw-rw-rw-   0        0        0    38205 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   202148 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0    80652 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    44432 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/fonts/fontawesome-webfont.woff
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:16.053579 BBFinance-1.5.1/BBFdocs/site/img/
--rw-rw-rw-   0        0        0     1150 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/img/favicon.ico
--rw-rw-rw-   0        0        0      251 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/img/grid1.png
--rw-rw-rw-   0        0        0      495 2023-04-10 19:54:23.000000 BBFinance-1.5.1/BBFdocs/site/img/grid10.png
--rw-rw-rw-   0        0        0      253 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid11.png
--rw-rw-rw-   0        0        0      260 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid12.png
--rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid13.png
--rw-rw-rw-   0        0        0      240 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid14.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid15.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid16.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid17.png
--rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid18.png
--rw-rw-rw-   0        0        0      427 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid19.png
--rw-rw-rw-   0        0        0      271 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid2.png
--rw-rw-rw-   0        0        0      493 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid20.png
--rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid3.png
--rw-rw-rw-   0        0        0      244 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid4.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid5.png
--rw-rw-rw-   0        0        0      460 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid6.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid7.png
--rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid8.png
--rw-rw-rw-   0        0        0      456 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/img/grid9.png
--rw-rw-rw-   0        0        0    11272 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/index.html
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:16.428607 BBFinance-1.5.1/BBFdocs/site/js/
--rw-rw-rw-   0        0        0     5911 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/js/base.js
--rw-rw-rw-   0        0        0    27822 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/js/bootstrap-3.0.3.min.js
--rw-rw-rw-   0        0        0    54608 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/js/highlight.pack.js
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:16.913025 BBFinance-1.5.1/BBFdocs/site/search/
--rw-rw-rw-   0        0        0    99805 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/search/lunr.js
--rw-rw-rw-   0        0        0     3206 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/search/main.js
--rw-rw-rw-   0        0        0     9063 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/search/search_index.json
--rw-rw-rw-   0        0        0     3724 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/search/worker.js
--rw-rw-rw-   0        0        0      234 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/sitemap.xml
--rw-rw-rw-   0        0        0      189 2023-04-10 19:54:24.000000 BBFinance-1.5.1/BBFdocs/site/sitemap.xml.gz
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:16.991179 BBFinance-1.5.1/BBFinance/
--rw-rw-rw-   0        0        0    43714 2023-05-05 17:32:23.000000 BBFinance-1.5.1/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      340 2023-04-17 19:24:24.000000 BBFinance-1.5.1/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:17.553720 BBFinance-1.5.1/BBFinance/__pycache__/
--rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.5.1/BBFinance/__pycache__/BBFinance.cpython-311.pyc
--rw-rw-rw-   0        0        0    27392 2023-05-05 13:29:28.000000 BBFinance-1.5.1/BBFinance/__pycache__/BBFinance.cpython-39.pyc
--rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.5.1/BBFinance/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      446 2023-04-18 13:13:11.000000 BBFinance-1.5.1/BBFinance/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:17.475575 BBFinance-1.5.1/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     5071 2023-05-05 17:34:57.000000 BBFinance-1.5.1/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-05-05 17:35:08.000000 BBFinance-1.5.1/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 17:34:57.000000 BBFinance-1.5.1/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      283 2023-05-05 17:34:57.000000 BBFinance-1.5.1/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 17:34:57.000000 BBFinance-1.5.1/BBFinance.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:17.928749 BBFinance-1.5.1/Banco/
--rw-rw-rw-   0        0        0    12288 2023-04-18 14:50:54.000000 BBFinance-1.5.1/Banco/DataClients.db
--rw-rw-rw-   0        0        0      589 2023-04-10 16:16:08.000000 BBFinance-1.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5071 2023-05-05 17:35:18.350652 BBFinance-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4445 2023-04-11 17:27:42.000000 BBFinance-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:18.131882 BBFinance-1.5.1/__pycache__/
--rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.5.1/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.5.1/__pycache__/main.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-05 17:35:18.210012 BBFinance-1.5.1/docs/
--rw-rw-rw-   0        0        0       17 2023-04-11 17:09:57.000000 BBFinance-1.5.1/docs/CNAME
--rw-rw-rw-   0        0        0     1354 2023-05-05 17:33:45.000000 BBFinance-1.5.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 17:35:18.381912 BBFinance-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-05-05 17:34:14.000000 BBFinance-1.5.1/setup.py
--rw-rw-rw-   0        0        0      124 2023-05-05 14:50:14.000000 BBFinance-1.5.1/teste.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:12.997396 BBFinance-1.5.2/
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:06.490194 BBFinance-1.5.2/BBFdocs/
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:06.568328 BBFinance-1.5.2/BBFdocs/docs/
+-rw-rw-rw-   0        0        0     4250 2023-04-11 14:25:22.000000 BBFinance-1.5.2/BBFdocs/docs/index.md
+-rw-rw-rw-   0        0        0       84 2023-04-10 19:53:10.000000 BBFinance-1.5.2/BBFdocs/mkdocs.yml
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:06.787111 BBFinance-1.5.2/BBFdocs/site/
+-rw-rw-rw-   0        0        0     6094 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/404.html
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:06.927765 BBFinance-1.5.2/BBFdocs/site/css/
+-rw-rw-rw-   0        0        0     5635 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/css/base.css
+-rw-rw-rw-   0        0        0     3487 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/css/base.min.css
+-rw-rw-rw-   0        0        0   132465 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/css/bootstrap-custom.css
+-rw-rw-rw-   0        0        0   109468 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/css/bootstrap-custom.min.css
+-rw-rw-rw-   0        0        0     2131 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/css/cinder.css
+-rw-rw-rw-   0        0        0     1637 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/css/cinder.min.css
+-rw-rw-rw-   0        0        0     1148 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/css/highlight.css
+-rw-rw-rw-   0        0        0      866 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/css/highlight.min.css
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:08.302986 BBFinance-1.5.2/BBFdocs/site/fonts/
+-rw-rw-rw-   0        0        0    38205 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   202148 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0    80652 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    44432 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/fonts/fontawesome-webfont.woff
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:10.525493 BBFinance-1.5.2/BBFdocs/site/img/
+-rw-rw-rw-   0        0        0     1150 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/img/favicon.ico
+-rw-rw-rw-   0        0        0      251 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/img/grid1.png
+-rw-rw-rw-   0        0        0      495 2023-04-10 19:54:23.000000 BBFinance-1.5.2/BBFdocs/site/img/grid10.png
+-rw-rw-rw-   0        0        0      253 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid11.png
+-rw-rw-rw-   0        0        0      260 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid12.png
+-rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid13.png
+-rw-rw-rw-   0        0        0      240 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid14.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid15.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid16.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid17.png
+-rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid18.png
+-rw-rw-rw-   0        0        0      427 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid19.png
+-rw-rw-rw-   0        0        0      271 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid2.png
+-rw-rw-rw-   0        0        0      493 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid20.png
+-rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid3.png
+-rw-rw-rw-   0        0        0      244 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid4.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid5.png
+-rw-rw-rw-   0        0        0      460 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid6.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid7.png
+-rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid8.png
+-rw-rw-rw-   0        0        0      456 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/img/grid9.png
+-rw-rw-rw-   0        0        0    11272 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/index.html
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:10.838049 BBFinance-1.5.2/BBFdocs/site/js/
+-rw-rw-rw-   0        0        0     5911 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/js/base.js
+-rw-rw-rw-   0        0        0    27822 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/js/bootstrap-3.0.3.min.js
+-rw-rw-rw-   0        0        0    54608 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/js/highlight.pack.js
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:11.448695 BBFinance-1.5.2/BBFdocs/site/search/
+-rw-rw-rw-   0        0        0    99805 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/search/lunr.js
+-rw-rw-rw-   0        0        0     3206 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/search/main.js
+-rw-rw-rw-   0        0        0     9063 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/search/search_index.json
+-rw-rw-rw-   0        0        0     3724 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/search/worker.js
+-rw-rw-rw-   0        0        0      234 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/sitemap.xml
+-rw-rw-rw-   0        0        0      189 2023-04-10 19:54:24.000000 BBFinance-1.5.2/BBFdocs/site/sitemap.xml.gz
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:11.636225 BBFinance-1.5.2/BBFinance/
+-rw-rw-rw-   0        0        0    43714 2023-05-05 17:32:23.000000 BBFinance-1.5.2/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      340 2023-04-17 19:24:24.000000 BBFinance-1.5.2/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:12.199381 BBFinance-1.5.2/BBFinance/__pycache__/
+-rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.5.2/BBFinance/__pycache__/BBFinance.cpython-311.pyc
+-rw-rw-rw-   0        0        0    27396 2023-05-05 17:40:40.000000 BBFinance-1.5.2/BBFinance/__pycache__/BBFinance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.5.2/BBFinance/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      446 2023-04-18 13:13:11.000000 BBFinance-1.5.2/BBFinance/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:12.089419 BBFinance-1.5.2/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     5071 2023-05-05 20:02:57.000000 BBFinance-1.5.2/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-05-05 20:03:05.000000 BBFinance-1.5.2/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 20:02:57.000000 BBFinance-1.5.2/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      336 2023-05-05 20:02:57.000000 BBFinance-1.5.2/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 20:02:57.000000 BBFinance-1.5.2/BBFinance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:12.575452 BBFinance-1.5.2/Banco/
+-rw-rw-rw-   0        0        0    12288 2023-04-18 14:50:54.000000 BBFinance-1.5.2/Banco/DataClients.db
+-rw-rw-rw-   0        0        0      589 2023-04-10 16:16:08.000000 BBFinance-1.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5071 2023-05-05 20:03:12.981763 BBFinance-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4445 2023-04-11 17:27:42.000000 BBFinance-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:12.762976 BBFinance-1.5.2/__pycache__/
+-rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.5.2/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.5.2/__pycache__/main.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-05 20:03:12.872375 BBFinance-1.5.2/docs/
+-rw-rw-rw-   0        0        0       17 2023-04-11 17:09:57.000000 BBFinance-1.5.2/docs/CNAME
+-rw-rw-rw-   0        0        0     1504 2023-05-05 20:01:15.000000 BBFinance-1.5.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 20:03:13.013023 BBFinance-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1442 2023-05-05 20:02:22.000000 BBFinance-1.5.2/setup.py
+-rw-rw-rw-   0        0        0      124 2023-05-05 14:50:14.000000 BBFinance-1.5.2/teste.py
```

### Comparing `BBFinance-1.5.1/BBFdocs/docs/index.md` & `BBFinance-1.5.2/BBFdocs/docs/index.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/404.html` & `BBFinance-1.5.2/BBFdocs/site/404.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/css/base.css` & `BBFinance-1.5.2/BBFdocs/site/css/base.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/css/base.min.css` & `BBFinance-1.5.2/BBFdocs/site/css/base.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/css/bootstrap-custom.css` & `BBFinance-1.5.2/BBFdocs/site/css/bootstrap-custom.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/css/bootstrap-custom.min.css` & `BBFinance-1.5.2/BBFdocs/site/css/bootstrap-custom.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/css/cinder.css` & `BBFinance-1.5.2/BBFdocs/site/css/cinder.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/css/cinder.min.css` & `BBFinance-1.5.2/BBFdocs/site/css/cinder.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/css/highlight.css` & `BBFinance-1.5.2/BBFdocs/site/css/highlight.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/css/highlight.min.css` & `BBFinance-1.5.2/BBFdocs/site/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/fonts/fontawesome-webfont.eot` & `BBFinance-1.5.2/BBFdocs/site/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/fonts/fontawesome-webfont.svg` & `BBFinance-1.5.2/BBFdocs/site/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/fonts/fontawesome-webfont.ttf` & `BBFinance-1.5.2/BBFdocs/site/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/fonts/fontawesome-webfont.woff` & `BBFinance-1.5.2/BBFdocs/site/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/img/favicon.ico` & `BBFinance-1.5.2/BBFdocs/site/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/index.html` & `BBFinance-1.5.2/BBFdocs/site/index.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/js/base.js` & `BBFinance-1.5.2/BBFdocs/site/js/base.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/js/bootstrap-3.0.3.min.js` & `BBFinance-1.5.2/BBFdocs/site/js/bootstrap-3.0.3.min.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/js/highlight.pack.js` & `BBFinance-1.5.2/BBFdocs/site/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/search/lunr.js` & `BBFinance-1.5.2/BBFdocs/site/search/lunr.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/search/main.js` & `BBFinance-1.5.2/BBFdocs/site/search/main.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/search/search_index.json` & `BBFinance-1.5.2/BBFdocs/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFdocs/site/search/worker.js` & `BBFinance-1.5.2/BBFdocs/site/search/worker.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFinance/BBFinance.py` & `BBFinance-1.5.2/BBFinance/BBFinance.py`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFinance/__pycache__/BBFinance.cpython-311.pyc` & `BBFinance-1.5.2/BBFinance/__pycache__/BBFinance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/BBFinance/__pycache__/BBFinance.cpython-39.pyc` & `BBFinance-1.5.2/BBFinance/__pycache__/BBFinance.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 19 19:37:15 2023 UTC, .py size: 43596 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 eb42 4064 4caa 0000  a........B@dL...
+00000000: 610d 0d0a 0000 0000 a73d 5564 c2aa 0000  a........=Ud....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4206 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6400 6401 6c08  d.l.m.Z...d.d.l.
 00000060: 5a09 6400 6405 6c0a 6d0b 5a0b 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6400 6407 6c0e  d.l.m.Z...d.d.l.
@@ -139,1574 +139,1575 @@
 000008a0: 6573 4e75 6d65 726f 4200 0000 730a 0000  esNumeroB...s...
 000008b0: 0000 0118 0118 0118 0112 0272 2100 0000  ...........r!...
 000008c0: 7a15 2f73 746f 636b 732f 7b73 796d 626f  z./stocks/{symbo
 000008d0: 6c7d 2f69 6e66 6f29 015a 0e72 6573 706f  l}/info).Z.respo
 000008e0: 6e73 655f 6d6f 6465 6c29 02da 0673 796d  nse_model)...sym
 000008f0: 626f 6cda 0672 6574 7572 6e63 0100 0000  bol..returnc....
 00000900: 0000 0000 0000 0000 0800 0000 0500 0000  ................
-00000910: 4300 0000 7368 0000 0074 00a0 0164 01a1  C...sh...t...d..
+00000910: 4300 0000 7368 0000 0074 00a0 017c 00a1  C...sh...t...|..
 00000920: 017d 017c 016a 027d 0274 037c 0283 017d  .}.|.j.}.t.|...}
-00000930: 037c 0374 046b 0272 226e 0874 0564 0283  .|.t.k.r"n.t.d..
-00000940: 0101 007c 016a 0264 0319 007d 047c 016a  ...|.j.d...}.|.j
-00000950: 0264 0419 007d 057c 016a 067d 067c 066a  .d...}.|.j.}.|.j
-00000960: 0764 0564 0685 0219 00a0 08a1 007d 067c  .d.d.........}.|
-00000970: 007c 047c 057c 0664 079c 047d 077c 0753  .|.|.|.d...}.|.S
-00000980: 0029 0875 bf00 0000 0a20 2020 2023 2320  .).u.....    ## 
+00000930: 037c 0374 046b 0272 226e 0874 0564 0183  .|.t.k.r"n.t.d..
+00000940: 0101 007c 016a 0264 0219 007d 047c 016a  ...|.j.d...}.|.j
+00000950: 0264 0319 007d 057c 016a 067d 067c 066a  .d...}.|.j.}.|.j
+00000960: 0764 0464 0585 0219 00a0 08a1 007d 067c  .d.d.........}.|
+00000970: 007c 047c 057c 0664 069c 047d 077c 0753  .|.|.|.d...}.|.S
+00000980: 0029 0775 bf00 0000 0a20 2020 2023 2320  .).u.....    ## 
 00000990: 5573 6162 696c 6964 6164 6520 0a20 2020  Usabilidade .   
 000009a0: 202d 2042 7573 6361 2061 7320 7072 696e   - Busca as prin
 000009b0: 6369 7061 6973 2069 6e66 6f72 6d61 c3a7  cipais informa..
 000009c0: 6f65 7320 736f 6272 6520 6f20 6174 6976  oes sobre o ativ
 000009d0: 6f20 7365 6c65 6369 6f6e 6164 6f20 636f  o selecionado co
 000009e0: 6d6f 2050 7265 c3a7 6f20 6520 4469 7669  mo Pre..o e Divi
 000009f0: 6465 6e64 6f73 200a 0a20 2020 200a 2020  dendos ..    .  
 00000a00: 2020 2323 2050 6172 c3a2 6d65 7472 6f73    ## Par..metros
 00000a10: 0a20 2020 202d 2073 796d 626f 6c20 2d3e  .    - symbol ->
 00000a20: 204e 6f6d 6520 646f 2041 7469 766f 2070   Nome do Ativo p
 00000a30: 6172 6120 6120 6275 7363 6120 0a0a 2020  ara a busca ..  
-00000a40: 2020 0a20 2020 207a 0850 4554 5234 2e53    .    z.PETR4.S
-00000a50: 41fa 0f54 6963 6b65 7220 496e 7661 6c69  A..Ticker Invali
-00000a60: 646f da12 7265 6775 6c61 724d 6172 6b65  do..regularMarke
-00000a70: 7450 7269 6365 5a08 6c6f 6e67 4e61 6d65  tPriceZ.longName
-00000a80: e9ff ffff ff4e 2904 7222 0000 00da 0d63  .....N).r".....c
-00000a90: 7572 7265 6e74 5f70 7269 6365 da0c 636f  urrent_price..co
-00000aa0: 6d70 616e 795f 6e61 6d65 da09 6469 7669  mpany_name..divi
-00000ab0: 6465 6e64 7329 09da 0279 66da 0654 6963  dends)...yf..Tic
-00000ac0: 6b65 72da 0469 6e66 6fda 0474 7970 65da  ker..info..type.
-00000ad0: 0464 6963 74da 0570 7269 6e74 7229 0000  .dict..printr)..
-00000ae0: 00da 0469 6c6f 63da 0373 756d 2908 7222  ...iloc..sum).r"
-00000af0: 0000 00da 0573 746f 636b 722c 0000 00da  .....stockr,....
-00000b00: 0874 6970 6f49 6e66 6f72 2700 0000 7228  .tipoInfor'...r(
-00000b10: 0000 005a 0864 6976 6964 656e 64da 096a  ...Z.dividend..j
-00000b20: 736f 6e5f 6461 7461 721f 0000 0072 1f00  son_datar....r..
-00000b30: 0000 7220 0000 00da 0867 6574 5f69 6e66  ..r .....get_inf
-00000b40: 6f4b 0000 0073 2000 0000 000c 0a01 0601  oK...s .........
-00000b50: 0801 0801 0202 0802 0a03 0a03 0601 1203  ................
-00000b60: 0201 0201 0201 02fd 0607 7235 0000 00da  ..........r5....
-00000b70: 085f 5f6d 6169 6e5f 5f7a 086d 6169 6e3a  .__main__z.main:
-00000b80: 6170 707a 0931 3237 2e30 2e30 2e31 6940  appz.127.0.0.1i@
-00000b90: 1f00 007a 1473 746f 636b 732f 7b73 796d  ...z.stocks/{sym
-00000ba0: 626f 6c7d 2f69 6e66 6f29 03da 0468 6f73  bol}/info)...hos
-00000bb0: 74da 0470 6f72 74da 0764 6566 6175 6c74  t..port..default
-00000bc0: 7a10 6170 706c 6963 6174 696f 6e2f 6a73  z.application/js
-00000bd0: 6f6e 2901 5a0a 6d65 6469 615f 7479 7065  on).Z.media_type
-00000be0: 7a18 2f73 746f 636b 732f 7b73 796d 626f  z./stocks/{symbo
-00000bf0: 6c7d 2f68 6973 746f 7279 da02 3179 2903  l}/history..1y).
-00000c00: 7222 0000 00da 0670 6572 696f 6472 2300  r".....periodr#.
-00000c10: 0000 6302 0000 0000 0000 0000 0000 0008  ..c.............
-00000c20: 0000 0003 0000 0043 0000 0073 7000 0000  .......C...sp...
-00000c30: 7400 a001 7c00 a101 7d02 7c02 6a02 7d03  t...|...}.|.j.}.
-00000c40: 7403 7c03 8301 7d04 7c04 7404 6b02 7222  t.|...}.|.t.k.r"
-00000c50: 6e08 7405 6401 8301 0100 7c02 6a06 7c01  n.t.d.....|.j.|.
-00000c60: 6402 8d01 7d05 7c05 6a07 7248 6403 7405  d...}.|.j.rHd.t.
-00000c70: 6404 8301 6901 5300 7c05 6a08 6405 6406  d...i.S.|.j.d.d.
-00000c80: 8d01 7d06 7409 6a0a a00b 7c06 a101 6a0c  ..}.t.j...|...j.
-00000c90: 6407 6408 8d01 7d07 7c07 5300 6409 5300  d.d...}.|.S.d.S.
-00000ca0: 290a 75ff 0000 000a 2020 2020 2323 2055  ).u.....    ## U
-00000cb0: 7361 6269 6c69 6461 6465 200a 2020 2020  sabilidade .    
-00000cc0: 2d20 5573 6164 6120 7061 7261 2076 6572  - Usada para ver
-00000cd0: 6966 6963 6172 206f 2068 6973 74c3 b372  ificar o hist..r
-00000ce0: 6963 6f20 6461 2061 c3a7 616f 2073 656c  ico da a..ao sel
-00000cf0: 6563 696f 6e61 6461 2065 2065 6d20 7175  ecionada e em qu
-00000d00: 616c 2070 6572 696f 646f 200a 0a20 2020  al periodo ..   
-00000d10: 200a 2020 2020 2323 2050 6172 c3a2 6d65   .    ## Par..me
-00000d20: 7472 6f73 0a20 2020 200a 2020 2020 2d20  tros.    .    - 
-00000d30: 7379 6d62 6f6c 202d 3e20 4e6f 6d65 2064  symbol -> Nome d
-00000d40: 6f20 4174 6976 6f20 7061 7261 2061 2062  o Ativo para a b
-00000d50: 7573 6361 200a 0a20 2020 202d 2070 6572  usca ..    - per
-00000d60: 696f 6420 2d3e 2044 6174 6120 656d 2041  iod -> Data em A
-00000d70: 4e4f 5320 7061 7261 2061 2062 7573 6361  NOS para a busca
-00000d80: 2064 6173 2069 6e66 6f72 6d61 c3a7 6f65   das informa..oe
-00000d90: 7320 646f 2041 7469 766f 200a 0a20 2020  s do Ativo ..   
-00000da0: 200a 2020 2020 7224 0000 00a9 0172 3b00   .    r$.....r;.
-00000db0: 0000 da05 6572 726f 727a 0d4e 6f20 6461  ....errorz.No da
-00000dc0: 7461 2066 6f75 6e64 da04 6c69 7374 2901  ta found..list).
-00000dd0: 5a06 6f72 6965 6e74 4629 01da 0464 726f  Z.orientF)...dro
-00000de0: 704e 290d 722a 0000 0072 2b00 0000 722c  pN).r*...r+...r,
-00000df0: 0000 0072 2d00 0000 722e 0000 0072 2f00  ...r-...r....r/.
-00000e00: 0000 da07 6869 7374 6f72 79da 0565 6d70  ....history..emp
-00000e10: 7479 da07 746f 5f64 6963 74da 0270 64da  ty..to_dict..pd.
-00000e20: 0944 6174 6146 7261 6d65 da09 6672 6f6d  .DataFrame..from
-00000e30: 5f64 6963 74da 0b72 6573 6574 5f69 6e64  _dict..reset_ind
-00000e40: 6578 2908 7222 0000 0072 3b00 0000 7232  ex).r"...r;...r2
-00000e50: 0000 0072 2c00 0000 7233 0000 0072 4000  ...r,...r3...r@.
-00000e60: 0000 5a0c 6869 7374 6f72 795f 6469 6374  ..Z.history_dict
-00000e70: 5a0a 6869 7374 6f72 795f 6466 721f 0000  Z.history_dfr...
-00000e80: 0072 1f00 0000 7220 0000 00da 1167 6574  .r....r .....get
-00000e90: 5f73 746f 636b 5f68 6973 746f 7279 7900  _stock_historyy.
-00000ea0: 0000 7318 0000 0000 0e0a 0106 0108 0108  ..s.............
-00000eb0: 0102 0208 020c 0206 010c 020c 0114 0272  ...............r
-00000ec0: 4700 0000 7a17 7374 6f63 6b73 2f7b 7379  G...z.stocks/{sy
-00000ed0: 6d62 6f6c 7d2f 6869 7374 6f72 797a 152f  mbol}/historyz./
-00000ee0: 7374 6f63 6b2f 7b73 796d 626f 6c7d 2f74  stock/{symbol}/t
-00000ef0: 7265 6e64 6301 0000 0000 0000 0000 0000  rendc...........
-00000f00: 0008 0000 0003 0000 0043 0000 0073 6800  .........C...sh.
-00000f10: 0000 7400 a001 7c00 a101 7d01 7c01 6a02  ..t...|...}.|.j.
-00000f20: 7d02 7403 7c02 8301 7d03 7c03 7404 6b02  }.t.|...}.|.t.k.
-00000f30: 7222 6e08 7405 6401 8301 0100 7c01 6a06  r"n.t.d.....|.j.
-00000f40: 6402 6403 8d01 7d04 7c04 6404 1900 7d05  d.d...}.|.d...}.
-00000f50: 7c05 6a07 6405 1900 7c05 6a07 6406 1900  |.j.d...|.j.d...
-00000f60: 6b04 7256 6407 6e02 6408 7d06 7c00 7c06  k.rVd.n.d.}.|.|.
-00000f70: 6409 9c02 7d07 7c07 5300 290a 75b9 0000  d...}.|.S.).u...
-00000f80: 000a 2020 2020 2323 2055 7361 6269 6c69  ..    ## Usabili
-00000f90: 6461 6465 200a 2020 2020 2d20 4964 656e  dade .    - Iden
-00000fa0: 7469 6669 6361 2061 2074 656e 6465 6e63  tifica a tendenc
-00000fb0: 6961 2064 6520 7072 65c3 a76f 2064 6520  ia de pre..o de 
-00000fc0: 756d 6120 61c3 a761 6f2c 2073 6520 6972  uma a..ao, se ir
-00000fd0: 6120 7365 7220 6465 2041 4c54 4120 6f75  a ser de ALTA ou
-00000fe0: 2042 4149 5841 0a20 2020 200a 2020 2020   BAIXA.    .    
-00000ff0: 2323 2050 6172 c3a2 6d65 7472 6f73 0a20  ## Par..metros. 
-00001000: 2020 200a 2020 2020 2d20 7379 6d62 6f6c     .    - symbol
-00001010: 202d 3e20 4e6f 6d65 2064 6f20 4174 6976   -> Nome do Ativ
-00001020: 6f20 7061 7261 2061 2062 7573 6361 200a  o para a busca .
-00001030: 0a20 2020 200a 2020 2020 7224 0000 005a  .    .    r$...Z
-00001040: 0231 6472 3c00 0000 da05 436c 6f73 6572  .1dr<.....Closer
-00001050: 2600 0000 7201 0000 00da 0275 70da 0464  &...r......up..d
-00001060: 6f77 6e29 0272 2200 0000 da05 7472 656e  own).r".....tren
-00001070: 6429 0872 2a00 0000 722b 0000 0072 2c00  d).r*...r+...r,.
-00001080: 0000 722d 0000 0072 2e00 0000 722f 0000  ..r-...r....r/..
-00001090: 0072 4000 0000 7230 0000 0029 0872 2200  .r@...r0...).r".
-000010a0: 0000 7232 0000 0072 2c00 0000 7233 0000  ..r2...r,...r3..
-000010b0: 0072 4000 0000 da0c 636c 6f73 655f 7072  .r@.....close_pr
-000010c0: 6963 6573 724b 0000 0072 3400 0000 721f  icesrK...r4...r.
-000010d0: 0000 0072 1f00 0000 7220 0000 00da 0f67  ...r....r .....g
-000010e0: 6574 5f73 746f 636b 5f74 7265 6e64 a700  et_stock_trend..
-000010f0: 0000 731a 0000 0000 0d0a 0106 0108 0108  ..s.............
-00001100: 0102 0208 020c 0108 011c 0202 0102 ff06  ................
-00001110: 0672 4d00 0000 7a15 7374 6f63 6b73 2f7b  .rM...z.stocks/{
-00001120: 7379 6d62 6f6c 7d2f 7472 656e 647a 192f  symbol}/trendz./
-00001130: 7374 6f63 6b2f 7b73 796d 626f 6c7d 2f74  stock/{symbol}/t
-00001140: 6563 686e 6963 616c 6301 0000 0000 0000  echnicalc.......
-00001150: 0000 0000 0011 0000 0006 0000 0043 0000  .............C..
-00001160: 0073 f800 0000 7400 a001 7c00 a101 7d01  .s....t...|...}.
-00001170: 7c01 6a02 7d02 7403 7c02 8301 7d03 7c03  |.j.}.t.|...}.|.
-00001180: 7404 6b02 7222 6e08 7405 6401 8301 0100  t.k.r"n.t.d.....
-00001190: 7c01 6a06 6402 6403 8d01 7d04 7c04 6404  |.j.d.d...}.|.d.
-000011a0: 1900 7d05 7c05 6a07 6405 6406 8d01 a008  ..}.|.j.d.d.....
-000011b0: a100 6a09 6407 1900 7d06 7c05 6a07 6408  ..j.d...}.|.j.d.
-000011c0: 6406 8d01 a008 a100 6a09 6407 1900 7d07  d.......j.d...}.
-000011d0: 7c05 a00a a100 7d08 7c08 a00b 7c08 6409  |.....}.|...|.d.
-000011e0: 6b04 6409 a102 7d09 7c08 a00b 7c08 6409  k.d...}.|...|.d.
-000011f0: 6b00 6409 a102 0b00 7d0a 7c09 6a07 640a  k.d.....}.|.j.d.
-00001200: 6406 8d01 a008 a100 7d0b 7c0a 6a07 640a  d.......}.|.j.d.
-00001210: 6406 8d01 a008 a100 7d0c 7c0b 7c0c 1b00  d.......}.|.|...
-00001220: 7d0d 640b 640b 640c 7c0d 1700 1b00 6a09  }.d.d.d.|.....j.
-00001230: 6407 1900 1800 7d0e 7c0e 640d 6b05 72e0  d.....}.|.d.k.r.
-00001240: 640e 7d0f 6e04 640f 7d0f 7c00 7c06 7c07  d.}.n.d.}.|.|.|.
-00001250: 7c0e 7c0f 6410 9c05 7d10 7c10 5300 2911  |.|.d...}.|.S.).
-00001260: 7579 0200 000a 2020 2020 2323 2055 7361  uy....    ## Usa
-00001270: 6269 6c69 6461 6465 200a 2020 2020 2d20  bilidade .    - 
-00001280: 63c3 a16c 6375 6c6f 2065 6e76 6f6c 7665  c..lculo envolve
-00001290: 2061 2063 6f6d 7061 7261 c3a7 c3a3 6f20   a compara....o 
-000012a0: 6461 206d c3a9 6469 6120 6465 2067 616e  da m..dia de gan
-000012b0: 686f 7320 656d 2075 6d20 7065 72c3 ad6f  hos em um per..o
-000012c0: 646f 2064 6520 7465 6d70 6f20 636f 6d20  do de tempo com 
-000012d0: 6120 6dc3 a964 6961 2064 6520 7065 7264  a m..dia de perd
-000012e0: 6173 2065 6d20 756d 2070 6572 c3ad 6f64  as em um per..od
-000012f0: 6f20 6465 2074 656d 706f 2e20 0a0a 2020  o de tempo. ..  
-00001300: 2020 0a20 2020 2023 2320 436f 6d6f 2069    .    ## Como i
-00001310: 6e74 6572 7072 6574 6172 200a 2020 2020  nterpretar .    
-00001320: 2d20 5175 616e 646f 206f 2052 5349 2065  - Quando o RSI e
-00001330: 7374 c3a1 2061 6369 6d61 2064 6520 3730  st.. acima de 70
-00001340: 2c20 6f20 6174 6976 6f20 c3a9 2063 6f6e  , o ativo .. con
-00001350: 7369 6465 7261 646f 2073 6f62 7265 636f  siderado sobreco
-00001360: 6d70 7261 646f 2c20 6f20 7175 6520 7369  mprado, o que si
-00001370: 676e 6966 6963 6120 7175 6520 706f 6465  gnifica que pode
-00001380: 2065 7374 6172 2070 7265 7374 6573 2061   estar prestes a
-00001390: 2073 6f66 7265 7220 756d 6120 636f 7272   sofrer uma corr
-000013a0: 65c3 a7c3 a36f 2070 6172 6120 6261 6978  e....o para baix
-000013b0: 6f2e 200a 2020 2020 5175 616e 646f 206f  o. .    Quando o
-000013c0: 2052 5349 2065 7374 c3a1 2061 6261 6978   RSI est.. abaix
-000013d0: 6f20 6465 2033 302c 206f 2061 7469 766f  o de 30, o ativo
-000013e0: 20c3 a920 636f 6e73 6964 6572 6164 6f20   .. considerado 
-000013f0: 736f 6272 6576 656e 6469 646f 2c20 6f20  sobrevendido, o 
-00001400: 7175 6520 7369 676e 6966 6963 6120 7175  que significa qu
-00001410: 6520 706f 6465 2065 7374 6172 2070 7265  e pode estar pre
-00001420: 7374 6573 2061 2073 7562 6972 206e 6f76  stes a subir nov
-00001430: 616d 656e 7465 2e20 0a20 0a20 2020 202d  amente. . .    -
-00001440: 2073 6d61 5f35 3020 2d3e 204d 6564 6961   sma_50 -> Media
-00001450: 206d 6f76 656c 2064 6f73 2035 3020 7065   movel dos 50 pe
-00001460: 7269 6f64 6f73 0a20 2020 202d 2073 6d61  riodos.    - sma
-00001470: 5f32 3030 202d 3e20 6d65 6469 6120 6d6f  _200 -> media mo
-00001480: 7665 6c20 646f 7320 3230 3020 7065 7269  vel dos 200 peri
-00001490: 646f 730a 0a20 2020 2023 2320 5061 72c3  dos..    ## Par.
-000014a0: a26d 6574 726f 730a 2020 2020 2d20 7379  .metros.    - sy
-000014b0: 6d62 6f6c 202d 3e20 4e6f 6d65 2064 6f20  mbol -> Nome do 
-000014c0: 4174 6976 6f20 7061 7261 2061 2062 7573  Ativo para a bus
-000014d0: 6361 200a 0a20 2020 200a 2020 2020 7224  ca ..    .    r$
-000014e0: 0000 00da 036d 6178 723c 0000 0072 4800  .....maxr<...rH.
-000014f0: 0000 e932 0000 0029 01da 0677 696e 646f  ...2...)...windo
-00001500: 7772 2600 0000 e9c8 0000 0072 0100 0000  wr&........r....
-00001510: e90e 0000 00e9 6400 0000 7216 0000 00e9  ......d...r.....
-00001520: 4600 0000 7a1f 4120 6368 616e 6365 2064  F...z.A chance d
-00001530: 6f20 7072 6563 6f20 646f 2061 7469 766f  o preco do ativo
-00001540: 2043 4149 527a 2041 2063 6861 6e63 6520   CAIRz A chance 
-00001550: 646f 2070 7265 636f 2064 6f20 6174 6976  do preco do ativ
-00001560: 6f20 5355 4249 5229 0572 2200 0000 da06  o SUBIR).r".....
-00001570: 736d 615f 3530 da07 736d 615f 3230 30da  sma_50..sma_200.
-00001580: 0372 7369 5a08 7465 6e64 656e 6379 290c  .rsiZ.tendency).
-00001590: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
-000015a0: 2d00 0000 722e 0000 0072 2f00 0000 7240  -...r....r/...r@
-000015b0: 0000 005a 0772 6f6c 6c69 6e67 da04 6d65  ...Z.rolling..me
-000015c0: 616e 7230 0000 00da 0464 6966 66da 0577  anr0.....diff..w
-000015d0: 6865 7265 2911 7222 0000 0072 3200 0000  here).r"...r2...
-000015e0: 722c 0000 0072 3300 0000 7240 0000 0072  r,...r3...r@...r
-000015f0: 4c00 0000 7255 0000 0072 5600 0000 da05  L...rU...rV.....
-00001600: 6465 6c74 615a 0467 6169 6eda 046c 6f73  deltaZ.gain..los
-00001610: 735a 0861 7667 5f67 6169 6e5a 0861 7667  sZ.avg_gainZ.avg
-00001620: 5f6c 6f73 73da 0272 7372 5700 0000 da06  _loss..rsrW.....
-00001630: 7374 6174 7573 7234 0000 0072 1f00 0000  statusr4...r....
-00001640: 721f 0000 0072 2000 0000 da14 6765 745f  r....r .....get_
-00001650: 7374 6f63 6b5f 7465 6368 6e69 6361 6c73  stock_technicals
-00001660: cf00 0000 7336 0000 0000 120a 0106 0108  ....s6..........
-00001670: 0108 0102 0208 020c 0108 0316 0116 0308  ................
-00001680: 0110 0112 0110 0110 0108 0116 0208 0106  ................
-00001690: 0204 0302 0102 0102 0102 0102 fb06 0a72  ...............r
-000016a0: 5f00 0000 7a19 7374 6f63 6b73 2f7b 7379  _...z.stocks/{sy
-000016b0: 6d62 6f6c 7d2f 7465 6368 6e69 6361 6c7a  mbol}/technicalz
-000016c0: 1a73 746f 636b 732f 7b73 796d 626f 6c7d  .stocks/{symbol}
-000016d0: 2f76 6f6c 6174 696c 6974 7929 0472 2200  /volatility).r".
-000016e0: 0000 da0a 7374 6172 745f 6461 7465 da08  ....start_date..
-000016f0: 656e 645f 6461 7465 7223 0000 0063 0300  end_dater#...c..
-00001700: 0000 0000 0000 0000 0000 0600 0000 0600  ................
-00001710: 0000 4300 0000 7368 0000 007a 2874 006a  ..C...sh...z(t.j
-00001720: 017c 007c 017c 0264 018d 037d 037c 036a  .|.|.|.d...}.|.j
-00001730: 0272 2664 0274 0364 0383 0169 0157 0053  .r&d.t.d...i.W.S
-00001740: 0057 006e 0c01 0001 0001 0059 006e 0230  .W.n.......Y.n.0
-00001750: 0074 04a0 057c 0364 0419 007c 0364 0419  .t...|.d...|.d..
-00001760: 00a0 0664 05a1 011b 00a1 017d 0474 04a0  ...d.......}.t..
-00001770: 0764 067c 04a0 08a1 0014 00a1 017d 057c  .d.|.........}.|
-00001780: 0553 0029 0775 6e01 0000 0a20 2020 2023  .S.).un....    #
-00001790: 2320 5573 6162 696c 6964 6164 6520 0a20  # Usabilidade . 
-000017a0: 2020 202d 204d c3a9 746f 646f 2075 7361     - M..todo usa
-000017b0: 646f 2070 6172 6120 7665 7269 6669 6361  do para verifica
-000017c0: 7220 6120 766f 6c61 7469 6c69 6461 6465  r a volatilidade
-000017d0: 2064 6520 756d 2061 7469 766f 2065 6d20   de um ativo em 
-000017e0: 636f 6d70 6172 6163 616f 2061 6f20 6d65  comparacao ao me
-000017f0: 7263 6164 6f20 656d 2071 7565 2065 7374  rcado em que est
-00001800: 6120 200a 0a20 2020 200a 2020 2020 2323  a  ..    .    ##
-00001810: 2050 6172 c3a2 6d65 7472 6f73 0a20 2020   Par..metros.   
-00001820: 202d 2073 796d 626f 6c20 2d3e 204e 6f6d   - symbol -> Nom
-00001830: 6520 646f 2041 7469 766f 2070 6172 6120  e do Ativo para 
-00001840: 6120 6275 7363 6120 0a0a 2020 2020 2d20  a busca ..    - 
-00001850: 7374 6172 745f 6461 7465 202d 3e20 4461  start_date -> Da
-00001860: 7461 2064 6520 496e 6963 696f 2064 6120  ta de Inicio da 
-00001870: 6275 7363 6120 6461 7320 696e 666f 7320  busca das infos 
-00001880: 2870 7265 636f 2c20 766f 6c75 6d65 2c20  (preco, volume, 
-00001890: 6574 6329 2064 6f20 6174 6976 6f20 0a0a  etc) do ativo ..
-000018a0: 2020 2020 2d20 656e 645f 6461 7465 202d      - end_date -
-000018b0: 3e20 4461 7461 2046 696e 616c 2070 6172  > Data Final par
-000018c0: 6120 6120 6275 7363 6120 6461 7320 696e  a a busca das in
-000018d0: 666f 7320 2870 7265 636f 2c20 766f 6c75  fos (preco, volu
-000018e0: 6d65 2c20 6574 6329 2064 6f20 6174 6976  me, etc) do ativ
-000018f0: 6f20 0a0a 2020 2020 a902 da05 7374 6172  o ..    ....star
-00001900: 74da 0365 6e64 723d 0000 007a 384e 616f  t..endr=...z8Nao
-00001910: 2066 6f69 2065 6e63 6f6e 7472 6164 6f20   foi encontrado 
-00001920: 6f20 6869 7374 6f72 6963 6f20 6e65 7373  o historico ness
-00001930: 6520 7065 7269 6f64 6f2c 2076 6572 6966  e periodo, verif
-00001940: 6963 6172 2e72 4800 0000 7216 0000 00e9  icar.rH...r.....
-00001950: fc00 0000 2909 722a 0000 00da 0864 6f77  ....).r*.....dow
-00001960: 6e6c 6f61 6472 4100 0000 722f 0000 00da  nloadrA...r/....
-00001970: 026e 70da 036c 6f67 da05 7368 6966 74da  .np..log..shift.
-00001980: 0473 7172 74da 0376 6172 2906 7222 0000  .sqrt..var).r"..
-00001990: 0072 6000 0000 7261 0000 005a 0a73 746f  .r`...ra...Z.sto
-000019a0: 636b 5f64 6174 615a 0b6c 6f67 5f72 6574  ck_dataZ.log_ret
-000019b0: 7572 6e73 5a0a 766f 6c61 7469 6c69 7479  urnsZ.volatility
-000019c0: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
-000019d0: 0e67 6574 5f76 6f6c 6174 696c 6974 7911  .get_volatility.
-000019e0: 0100 0073 1200 0000 000d 0201 1001 0601  ...s............
-000019f0: 1201 0601 0602 1c01 1202 726c 0000 007a  ..........rl...z
-00001a00: 1473 746f 636b 732f 7b73 796d 626f 6c7d  .stocks/{symbol}
-00001a10: 2f62 6574 6163 0100 0000 0000 0000 0000  /betac..........
-00001a20: 0000 0f00 0000 0300 0000 4300 0000 73be  ..........C...s.
-00001a30: 0000 0074 00a0 017c 00a1 017d 0174 00a0  ...t...|...}.t..
-00001a40: 0164 01a1 017d 027c 016a 027d 037c 026a  .d...}.|.j.}.|.j
-00001a50: 027d 0474 037c 0383 017d 057c 0574 046b  .}.t.|...}.|.t.k
-00001a60: 0273 427c 0474 046b 0272 3a6e 0874 0564  .sB|.t.k.r:n.t.d
-00001a70: 0283 0101 007c 016a 0664 0364 048d 017d  .....|.j.d.d...}
-00001a80: 067c 026a 0664 0364 048d 017d 077c 0664  .|.j.d.d...}.|.d
-00001a90: 0519 00a0 07a1 007d 087c 0764 0519 00a0  .......}.|.d....
-00001aa0: 07a1 007d 097c 08a0 087c 09a1 017d 0a7c  ...}.|...|...}.|
-00001ab0: 09a0 09a1 007d 0b7c 0a7c 0b1b 007d 0c7c  .....}.|.|...}.|
-00001ac0: 0c64 066b 0472 9864 077d 0d7c 0c64 066b  .d.k.r.d.}.|.d.k
-00001ad0: 0072 a464 087d 0d7c 0c64 066b 0272 b064  .r.d.}.|.d.k.r.d
-00001ae0: 097d 0d7c 0c7c 0d64 0a9c 027d 0e7c 0e53  .}.|.|.d...}.|.S
-00001af0: 0029 0b75 9501 0000 0a20 2020 2023 2320  .).u.....    ## 
-00001b00: 5573 6162 696c 6964 6164 6520 0a20 2020  Usabilidade .   
-00001b10: 202d 204f 2062 6574 6120 c3a9 2075 6d61   - O beta .. uma
-00001b20: 206d 6564 6964 6120 6573 7461 74c3 ad73   medida estat..s
-00001b30: 7469 6361 2071 7565 2069 6e64 6963 6120  tica que indica 
-00001b40: 6120 7265 6c61 c3a7 c3a3 6f20 656e 7472  a rela....o entr
-00001b50: 6520 6120 766f 6c61 7469 6c69 6461 6465  e a volatilidade
-00001b60: 2064 6520 756d 6120 61c3 a7c3 a36f 2065   de uma a....o e
-00001b70: 2061 2076 6f6c 6174 696c 6964 6164 6520   a volatilidade 
-00001b80: 646f 206d 6572 6361 646f 2063 6f6d 6f20  do mercado como 
-00001b90: 756d 2074 6f64 6f2e 0a20 2020 204f 2076  um todo..    O v
-00001ba0: 616c 6f72 2064 6f20 6265 7461 20c3 a920  alor do beta .. 
-00001bb0: 7574 696c 697a 6164 6f20 7061 7261 206d  utilizado para m
-00001bc0: 6564 6972 206f 2072 6973 636f 2064 6520  edir o risco de 
-00001bd0: 756d 6120 61c3 a7c3 a36f 2065 6d20 7265  uma a....o em re
-00001be0: 6c61 c3a7 c3a3 6f20 616f 206d 6572 6361  la....o ao merca
-00001bf0: 646f 2065 6d20 7175 6520 656c 6120 c3a9  do em que ela ..
-00001c00: 206e 6567 6f63 6961 6461 2e20 0a0a 2020   negociada. ..  
-00001c10: 2020 0a20 2020 2023 2320 5061 72c3 a26d    .    ## Par..m
-00001c20: 6574 726f 730a 2020 2020 2d20 7379 6d62  etros.    - symb
-00001c30: 6f6c 202d 3e20 4e6f 6d65 2064 6f20 4174  ol -> Nome do At
-00001c40: 6976 6f20 7061 7261 2061 2062 7573 6361  ivo para a busca
-00001c50: 200a 0a20 2020 202d 206d 6172 6b65 7420   ..    - market 
-00001c60: 2d3e 2043 6f6d 6f20 7061 6472 616f 2c20  -> Como padrao, 
-00001c70: 4d65 7263 6164 6f3a 2049 424f 5645 5350  Mercado: IBOVESP
-00001c80: 4120 2f20 4256 5350 0a20 2020 207a 055e  A / BVSP.    z.^
-00001c90: 4256 5350 7224 0000 0072 4e00 0000 723c  BVSPr$...rN...r<
-00001ca0: 0000 0072 4800 0000 7216 0000 007a 2841  ...rH...r....z(A
-00001cb0: 6361 6f20 6d61 6973 2056 6f6c 6174 696c  cao mais Volatil
-00001cc0: 2071 7565 206f 206d 6572 6361 646f 2065   que o mercado e
-00001cd0: 6d20 6765 7261 6c7a 2941 6361 6f20 6d65  m geralz)Acao me
-00001ce0: 6e6f 7320 566f 6c61 7469 6c20 7175 6520  nos Volatil que 
-00001cf0: 6f20 6d65 7263 6164 6f20 656d 2067 6572  o mercado em ger
-00001d00: 616c 7a34 4163 616f 2063 6f6d 2061 206d  alz4Acao com a m
-00001d10: 6573 6d61 2056 6f6c 6174 696c 6964 6164  esma Volatilidad
-00001d20: 6520 7175 6520 6f20 6d65 7263 6164 6f20  e que o mercado 
-00001d30: 656d 2067 6572 616c 2902 da04 6265 7461  em geral)...beta
-00001d40: 725e 0000 0029 0a72 2a00 0000 722b 0000  r^...).r*...r+..
-00001d50: 0072 2c00 0000 722d 0000 0072 2e00 0000  .r,...r-...r....
-00001d60: 722f 0000 0072 4000 0000 da0a 7063 745f  r/...r@.....pct_
-00001d70: 6368 616e 6765 da03 636f 7672 6b00 0000  change..covrk...
-00001d80: 290f 7222 0000 005a 0561 7373 6574 5a06  ).r"...Z.assetZ.
-00001d90: 6d61 726b 6574 722c 0000 005a 0a69 6e66  marketr,...Z.inf
-00001da0: 6f4d 6172 6b65 7472 3300 0000 5a0d 6173  oMarketr3...Z.as
-00001db0: 7365 745f 6869 7374 6f72 795a 0e6d 6172  set_historyZ.mar
-00001dc0: 6b65 745f 6869 7374 6f72 795a 0d61 7373  ket_historyZ.ass
-00001dd0: 6574 5f72 6574 7572 6e73 5a0e 6d61 726b  et_returnsZ.mark
-00001de0: 6574 5f72 6574 7572 6e73 726f 0000 0072  et_returnsro...r
-00001df0: 6b00 0000 726d 0000 0072 5e00 0000 7234  k...rm...r^...r4
-00001e00: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
-00001e10: 0000 da08 6765 745f 6265 7461 3101 0000  ....get_beta1...
-00001e20: 7332 0000 0000 0e0a 010a 0106 0106 0108  s2..............
-00001e30: 0110 0102 0208 020c 010c 030c 010c 030a  ................
-00001e40: 0108 0108 0208 0104 0108 0104 0108 0104  ................
-00001e50: 0302 0102 ff06 0572 7000 0000 7a13 7374  .......rp...z.st
-00001e60: 6f63 6b73 2f7b 7379 6d62 6f6c 7d2f 5661  ocks/{symbol}/Va
-00001e70: 5229 0472 2200 0000 da10 636f 6e66 6964  R).r".....confid
-00001e80: 656e 6365 5f6c 6576 656c da0f 6c6f 6f6b  ence_level..look
-00001e90: 6261 636b 5f70 6572 696f 6472 2300 0000  back_periodr#...
-00001ea0: 6303 0000 0000 0000 0000 0000 000b 0000  c...............
-00001eb0: 0006 0000 0043 0000 0073 9e00 0000 7400  .....C...s....t.
-00001ec0: a001 7c00 a101 7d03 7c03 6a02 7d04 7403  ..|...}.|.j.}.t.
-00001ed0: 7c04 8301 7d05 7c05 7404 6b02 7222 6e08  |...}.|.t.k.r"n.
-00001ee0: 7405 6401 8301 0100 7c03 6a06 7c02 9b00  t.d.....|.j.|...
-00001ef0: 6402 9d02 6403 8d01 6404 1900 7d06 7407  d...d...d...}.t.
-00001f00: a008 7c06 7c06 a009 6405 a101 1b00 a101  ..|.|...d.......
-00001f10: 7d07 7c07 a00a a100 7d08 7c08 740b a00c  }.|.....}.|.t...
-00001f20: 6405 7c01 1800 a101 1400 7d09 7405 6406  d.|.......}.t.d.
-00001f30: 740d 7c09 7c06 6407 1900 1400 6408 8302  t.|.|.d.....d...
-00001f40: 6901 8301 0100 740d 7c09 7c06 6407 1900  i.....t.|.|.d...
-00001f50: 1400 6408 8302 7d0a 7c0a 5300 2909 75c8  ..d...}.|.S.).u.
-00001f60: 0100 000a 2020 2020 2323 2055 7361 6269  ....    ## Usabi
-00001f70: 6c69 6461 6465 200a 2020 2020 2d20 4f20  lidade .    - O 
-00001f80: 5661 6c75 6520 6174 2052 6973 6b20 2856  Value at Risk (V
-00001f90: 6152 2920 c3a9 2075 6d61 206d 6564 6964  aR) .. uma medid
-00001fa0: 6120 6465 2072 6973 636f 2071 7565 2069  a de risco que i
-00001fb0: 6e64 6963 6120 6120 7065 7264 6120 6dc3  ndica a perda m.
-00001fc0: a178 696d 6120 6573 7065 7261 6461 2c20  .xima esperada, 
-00001fd0: 636f 6d20 756d 2064 6574 6572 6d69 6e61  com um determina
-00001fe0: 646f 206e c3ad 7665 6c20 6465 2063 6f6e  do n..vel de con
-00001ff0: 6669 616e c3a7 612c 2065 6d20 756d 2069  fian..a, em um i
-00002000: 6e74 6572 7661 6c6f 2064 6520 7465 6d70  ntervalo de temp
-00002010: 6f20 7072 c3a9 2d64 6574 6572 6d69 6e61  o pr..-determina
-00002020: 646f 2e20 0a0a 2020 2020 0a20 2020 2023  do. ..    .    #
-00002030: 2320 5061 72c3 a26d 6574 726f 730a 2020  # Par..metros.  
-00002040: 2020 0a20 2020 202d 2073 796d 626f 6c20    .    - symbol 
-00002050: 2d3e 204e 6f6d 6520 646f 2041 7469 766f  -> Nome do Ativo
-00002060: 2070 6172 6120 6661 7a65 7220 6120 6275   para fazer a bu
-00002070: 7363 6120 0a0a 2020 2020 2d20 636f 6e66  sca ..    - conf
-00002080: 6964 656e 6365 5f6c 6576 656c 202d 3e20  idence_level -> 
-00002090: 4e69 7665 6c20 6465 2063 6f6e 6669 616e  Nivel de confian
-000020a0: c3a7 6120 7061 7261 206f 2056 4152 2028  ..a para o VAR (
-000020b0: 3020 6120 3129 2c20 6e6f 726d 616c 6d65  0 a 1), normalme
-000020c0: 6e74 6520 7573 6164 6f20 656d 2030 2e39  nte usado em 0.9
-000020d0: 3520 0a0a 2020 2020 2d20 6c6f 6f6b 6261  5 ..    - lookba
-000020e0: 636b 5f70 6572 696f 6420 2d3e 2050 6572  ck_period -> Per
-000020f0: 696f 646f 2045 4d20 4449 4153 2061 2073  iodo EM DIAS a s
-00002100: 6572 2063 6f6e 7369 6465 7261 646f 2070  er considerado p
-00002110: 6172 6120 6f20 63c3 a16c 6375 6c6f 2064  ara o c..lculo d
-00002120: 6f20 5661 520a 0a20 2020 2072 2400 0000  o VaR..    r$...
-00002130: da01 6472 3c00 0000 7248 0000 0072 1600  ..dr<...rH...r..
-00002140: 0000 5a03 5661 5272 2600 0000 e902 0000  ..Z.VaRr&.......
-00002150: 0029 0e72 2a00 0000 722b 0000 0072 2c00  .).r*...r+...r,.
-00002160: 0000 722d 0000 0072 2e00 0000 722f 0000  ..r-...r....r/..
-00002170: 0072 4000 0000 7267 0000 0072 6800 0000  .r@...rg...rh...
-00002180: 7269 0000 00da 0373 7464 7202 0000 005a  ri.....stdr....Z
-00002190: 0370 7066 da05 726f 756e 6429 0b72 2200  .ppf..round).r".
-000021a0: 0000 7271 0000 0072 7200 0000 7232 0000  ..rq...rr...r2..
-000021b0: 0072 2c00 0000 7233 0000 005a 0670 7269  .r,...r3...Z.pri
-000021c0: 6365 73da 0772 6574 7572 6e73 5a07 7374  ces..returnsZ.st
-000021d0: 645f 6465 7672 6b00 0000 5a03 5661 7272  d_devrk...Z.Varr
-000021e0: 1f00 0000 721f 0000 0072 2000 0000 da07  ....r....r .....
-000021f0: 6765 745f 7661 726b 0100 0073 1a00 0000  get_vark...s....
-00002200: 000f 0a01 0601 0801 0801 0202 0803 1603  ................
-00002210: 1403 0801 1201 1a01 1201 7278 0000 007a  ..........rx...z
-00002220: 1c73 746f 636b 732f 7b73 796d 626f 6c7d  .stocks/{symbol}
-00002230: 2f41 6e6e 7561 6c52 6574 7572 6e29 04da  /AnnualReturn)..
-00002240: 0773 796d 626f 6c73 7260 0000 0072 6100  .symbolsr`...ra.
-00002250: 0000 7223 0000 0063 0300 0000 0000 0000  ..r#...c........
-00002260: 0000 0000 1100 0000 0700 0000 4300 0000  ............C...
-00002270: 7392 0100 0074 007c 0074 0183 0272 c874  s....t.|.t...r.t
-00002280: 0264 017c 009b 009d 0283 0101 0074 036a  .d.|.........t.j
-00002290: 047c 007c 017c 0264 0264 038d 047d 037a  .|.|.|.d.d...}.z
-000022a0: 8674 03a0 057c 00a1 016a 067d 047c 0464  .t...|...j.}.|.d
-000022b0: 0419 007d 057c 0364 0519 007d 067c 06a0  ...}.|.d...}.|..
-000022c0: 07a1 007d 077c 07a0 08a1 0064 0614 007d  ...}.|.....d...}
-000022d0: 087c 07a0 09a1 0064 0714 007d 097c 066a  .|.....d...}.|.j
-000022e0: 0a64 0819 0064 0914 007d 0a7c 066a 0a64  .d...d...}.|.j.d
-000022f0: 0a19 0064 0914 007d 0b7c 0b7c 0a18 007c  ...d...}.|.|...|
-00002300: 0a1b 007d 0c74 0b6a 0c7c 007c 057c 087c  ...}.t.j.|.|.|.|
-00002310: 097c 0c64 0b9c 0564 0c67 0164 0d8d 027d  .|.d...d.g.d...}
-00002320: 0d7c 0d57 0053 0001 0001 0001 0074 0264  .|.W.S.......t.d
-00002330: 0e83 0101 0059 006e 0230 006e c674 007c  .....Y.n.0.n.t.|
-00002340: 0074 0d83 0290 0172 8674 0ba0 0ca1 007d  .t.....r.t.....}
-00002350: 0e74 0264 0f7c 009b 009d 0283 0101 007c  .t.d.|.........|
-00002360: 0044 005d 927d 0f74 036a 047c 0f7c 017c  .D.].}.t.j.|.|.|
-00002370: 0264 0264 038d 047d 037c 0364 0519 007d  .d.d...}.|.d...}
-00002380: 067c 06a0 07a1 007d 077c 07a0 08a1 0064  .|.....}.|.....d
-00002390: 0614 007d 087c 07a0 09a1 0064 0714 007d  ...}.|.....d...}
-000023a0: 097c 066a 0a64 0819 0064 0914 007d 0a7c  .|.j.d...d...}.|
-000023b0: 066a 0a64 0a19 0064 0914 007d 0b7c 0b7c  .j.d...d...}.|.|
-000023c0: 0a18 007c 0a1b 007d 0c74 0b6a 0c7c 0f7c  ...|...}.t.j.|.|
-000023d0: 087c 097c 0c64 109c 0474 0e7c 0083 0167  .|.|.d...t.|...g
-000023e0: 0164 0d8d 027d 1074 0ba0 0f7c 107c 0e67  .d...}.t...|.|.g
-000023f0: 02a1 017d 0e71 ee7c 0e53 0074 0264 1183  ...}.q.|.S.t.d..
-00002400: 0101 0064 1253 0029 1375 9b01 0000 0a20  ...d.S.).u..... 
-00002410: 2020 2023 2320 5573 6162 696c 6964 6164     ## Usabilidad
-00002420: 650a 2020 2020 2d20 5265 6365 6265 2075  e.    - Recebe u
-00002430: 6d61 206c 6973 7461 2065 2072 6574 6f72  ma lista e retor
-00002440: 6e61 2075 6d20 4461 7461 4672 616d 6520  na um DataFrame 
-00002450: 636f 6d20 6173 2069 6e66 6f72 6d61 c3a7  com as informa..
-00002460: c3b5 6573 2064 6f73 2061 7469 766f 7320  ..es dos ativos 
-00002470: 6520 616c 6775 6d61 7320 6573 7461 74c3  e algumas estat.
-00002480: ad73 7469 6361 7320 62c3 a173 6963 6173  .sticas b..sicas
-00002490: 2e20 0a0a 2020 2020 0a20 2020 2023 2320  . ..    .    ## 
-000024a0: 5061 72c3 a26d 6574 726f 730a 2020 2020  Par..metros.    
-000024b0: 2d20 7379 6d62 6f6c 7320 2d3e 2052 6563  - symbols -> Rec
-000024c0: 6562 6520 756d 6120 6c69 7374 6120 6f75  ebe uma lista ou
-000024d0: 2075 6d20 756e 6963 6f20 6174 6976 6f20   um unico ativo 
-000024e0: 7061 7261 2062 7573 6361 7220 6e61 2062  para buscar na b
-000024f0: 6173 6520 0a0a 2020 2020 2d20 7374 6172  ase ..    - star
-00002500: 745f 6461 7465 202d 3e20 4461 7461 2064  t_date -> Data d
-00002510: 6520 496e 6963 696f 2064 6120 6275 7363  e Inicio da busc
-00002520: 6120 6461 7320 696e 666f 7320 2870 7265  a das infos (pre
-00002530: 636f 2c20 766f 6c75 6d65 2c20 6574 6329  co, volume, etc)
-00002540: 2064 6f20 6174 6976 6f20 0a0a 2020 2020   do ativo ..    
-00002550: 2d20 656e 645f 6461 7465 202d 3e20 4461  - end_date -> Da
-00002560: 7461 2046 696e 616c 2070 6172 6120 6120  ta Final para a 
-00002570: 6275 7363 6120 6461 7320 696e 666f 7320  busca das infos 
-00002580: 2870 7265 636f 2c20 766f 6c75 6d65 2c20  (preco, volume, 
-00002590: 6574 6329 2064 6f20 6174 6976 6f20 0a0a  etc) do ativo ..
-000025a0: 2020 2020 0a20 2020 2075 1a00 0000 566f      .    u....Vo
-000025b0: 63c3 aa20 6469 6769 746f 7520 756d 6120  c.. digitou uma 
-000025c0: 7374 7269 6e67 3a20 da06 7469 636b 6572  string: ..ticker
-000025d0: 2904 5a07 7469 636b 6572 7372 6300 0000  ).Z.tickersrc...
-000025e0: 7264 0000 005a 0867 726f 7570 5f62 7972  rd...Z.group_byr
-000025f0: 2500 0000 7248 0000 0072 6500 0000 675f  %...rH...re...g_
-00002600: 75bc 7ebf bf2f 4072 0100 0000 7253 0000  u.~../@r....rS..
-00002610: 0072 2600 0000 2905 da05 4174 6976 6f75  .r&...)...Ativou
-00002620: 1000 0000 5072 65c3 a76f 2061 204d 6572  ....Pre..o a Mer
-00002630: 6361 646f fa0d 5265 746f 726e 6f20 616e  cado..Retorno an
-00002640: 7561 6cf5 1400 0000 4465 7376 696f 2070  ual.....Desvio p
-00002650: 6164 72c3 a36f 2061 6e75 616c fa0d 5265  adr..o anual..Re
-00002660: 746f 726e 6f20 746f 7461 6c72 1600 0000  torno totalr....
-00002670: a901 da05 696e 6465 7875 1000 0000 5469  ....indexu....Ti
-00002680: 636b 6572 2069 6e76 c3a1 6c69 646f 7519  cker inv..lidou.
-00002690: 0000 0056 6f63 c3aa 2064 6967 6974 6f75  ...Voc.. digitou
-000026a0: 2075 6d61 206c 6973 7461 3a20 2904 727b   uma lista: ).r{
-000026b0: 0000 0072 7c00 0000 727d 0000 0072 7e00  ...r|...r}...r~.
-000026c0: 0000 752f 0000 0054 6970 6f20 696e 76c3  ..u/...Tipo inv.
-000026d0: a16c 6964 6f2e 2044 6967 6974 6520 756d  .lido. Digite um
-000026e0: 6120 7374 7269 6e67 206f 7520 756d 6120  a string ou uma 
-000026f0: 6c69 7374 612e 4e29 10da 0a69 7369 6e73  lista.N)...isins
-00002700: 7461 6e63 65da 0373 7472 722f 0000 0072  tance..strr/...r
-00002710: 2a00 0000 7266 0000 0072 2b00 0000 722c  *...rf...r+...r,
-00002720: 0000 0072 6e00 0000 7258 0000 0072 7500  ...rn...rX...ru.
-00002730: 0000 7230 0000 0072 4300 0000 7244 0000  ..r0...rC...rD..
-00002740: 0072 3e00 0000 da03 6c65 6eda 0663 6f6e  .r>.....len..con
-00002750: 6361 7429 1172 7900 0000 7260 0000 0072  cat).ry...r`...r
-00002760: 6100 0000 da05 6461 646f 73da 0464 6174  a.....dados..dat
-00002770: 615a 0b76 616c 7565 4d61 726b 6574 da05  aZ.valueMarket..
-00002780: 636c 6f73 655a 0e72 6574 6f72 6e6f 5f64  closeZ.retorno_d
-00002790: 6961 7269 6f5a 0d72 6574 6f72 6e6f 5f61  iarioZ.retorno_a
-000027a0: 6e75 616c 5a13 6465 7376 696f 5f70 6164  nualZ.desvio_pad
-000027b0: 7261 6f5f 616e 7561 6c5a 0f76 616c 6f72  rao_anualZ.valor
-000027c0: 5f69 6e76 6573 7469 646f 5a0b 7661 6c6f  _investidoZ.valo
-000027d0: 725f 6174 7561 6c5a 0d72 6574 6f72 6e6f  r_atualZ.retorno
-000027e0: 5f74 6f74 616c 5a0c 7661 6c75 6553 796d  _totalZ.valueSym
-000027f0: 626f 6c73 5a07 7661 6c75 6544 465a 0773  bolsZ.valueDFZ.s
-00002800: 696d 626f 6c6f 5a0d 7265 7475 726e 5379  imboloZ.returnSy
-00002810: 6d62 6f6c 7372 1f00 0000 721f 0000 0072  mbolsr....r....r
-00002820: 2000 0000 da0f 6173 7365 745f 706f 7274   .....asset_port
-00002830: 666f 6c69 6f96 0100 0073 6000 0000 000e  folio....s`.....
-00002840: 0a01 0e01 1202 0202 0c01 0803 0803 0803  ................
-00002850: 0c03 0c03 0e03 0e03 0c03 0401 0201 0201  ................
-00002860: 0201 0201 02fb 0406 04fa 0608 0602 0601  ................
-00002870: 1002 0c01 0801 0e01 0801 1203 0803 0803  ................
-00002880: 0c03 0c03 0e03 0e03 0c03 0401 0201 0201  ................
-00002890: 0201 02fc 0405 08fb 0607 1002 0402 7288  ..............r.
-000028a0: 0000 007a 2473 746f 636b 732f 7b73 796d  ...z$stocks/{sym
-000028b0: 626f 6c7d 2f4d 6172 6b6f 7769 747a 416c  bol}/MarkowitzAl
-000028c0: 6c6f 6361 7469 6f6e 6e29 0472 7900 0000  locationn).ry...
-000028d0: da09 7374 6172 5f64 6174 6572 6100 0000  ..star_datera...
-000028e0: 7223 0000 0063 0300 0000 0000 0000 0000  r#...c..........
-000028f0: 0000 1100 0000 0900 0000 4300 0000 733a  ..........C...s:
-00002900: 0100 0074 006a 017c 007c 017c 0264 018d  ...t.j.|.|.|.d..
-00002910: 0364 0219 007d 037c 03a0 02a1 00a0 03a1  .d...}.|........
-00002920: 007d 047c 04a0 04a1 007d 0574 05a0 0664  .}.|.....}.t...d
-00002930: 0374 077c 0083 011b 0067 0174 077c 0083  .t.|.....g.t.|..
-00002940: 0114 00a1 017d 0674 05a0 087c 04a0 09a1  .....}.t...|....
-00002950: 007c 0614 00a1 0164 0414 007d 0774 05a0  .|.....d...}.t..
-00002960: 0a74 05a0 0b7c 066a 0c74 05a0 0b7c 057c  .t...|.j.t...|.|
-00002970: 06a1 02a1 02a1 0174 05a0 0a64 04a1 0114  .......t...d....
-00002980: 007d 0864 0574 05a0 0d7c 05a1 0114 007d  .}.d.t...|.....}
-00002990: 0974 056a 0ea0 0f7c 057c 0974 05a0 107c  .t.j...|.|.t...|
-000029a0: 056a 1164 0619 00a1 0114 0017 00a1 017d  .j.d...........}
-000029b0: 0a74 05a0 1274 077c 0083 0164 0366 02a1  .t...t.|...d.f..
-000029c0: 017d 0b74 05a0 0b7c 0a7c 0ba1 0274 05a0  .}.t...|.|...t..
-000029d0: 0b74 05a0 0b7c 0b6a 0c7c 0aa1 027c 0ba1  .t...|.j.|...|..
-000029e0: 021b 007d 0c7c 0ca0 13a1 007d 0c67 007d  ...}.|.....}.g.}
-000029f0: 0d74 1474 077c 0083 0183 0144 005d 2e7d  .t.t.|.....D.].}
-00002a00: 0e64 077c 007c 0e19 009b 0064 087c 0c7c  .d.|.|.....d.|.|
-00002a10: 0e19 0064 0914 0064 0a9b 0464 0b9d 057d  ...d...d...d...}
-00002a20: 0f7c 0da0 157c 0fa1 0101 0071 fa7c 077c  .|...|.....q.|.|
-00002a30: 087c 0d64 0c9c 037d 107c 1053 0029 0d75  .|.d...}.|.S.).u
-00002a40: 2403 0000 0a20 2020 2023 2320 5573 6162  $....    ## Usab
-00002a50: 696c 6964 6164 6573 200a 2020 2020 2d20  ilidades .    - 
-00002a60: 416c 6f63 61c3 a7c3 a36f 2064 6520 4d61  Aloca....o de Ma
-00002a70: 726b 6f77 6974 7a20 c3a9 2075 6d61 2074  rkowitz .. uma t
-00002a80: c3a9 636e 6963 6120 6465 206f 7469 6d69  ..cnica de otimi
-00002a90: 7a61 c3a7 c3a3 6f20 6465 2070 6f72 7466  za....o de portf
-00002aa0: c3b3 6c69 6f20 7175 6520 7669 7361 2065  ..lio que visa e
-00002ab0: 6e63 6f6e 7472 6172 2061 2063 6f6d 6269  ncontrar a combi
-00002ac0: 6e61 c3a7 c3a3 6f20 6964 6561 6c20 6465  na....o ideal de
-00002ad0: 2061 7469 766f 7320 7061 7261 206d 6178   ativos para max
-00002ae0: 696d 697a 6172 206f 2072 6574 6f72 6e6f  imizar o retorno
-00002af0: 2064 6f20 696e 7665 7374 696d 656e 746f   do investimento
-00002b00: 2065 6e71 7561 6e74 6f20 6d69 6e69 6d69   enquanto minimi
-00002b10: 7a61 206f 2072 6973 636f 2e20 0a0a 0a20  za o risco. ... 
-00002b20: 2020 2023 2320 4f20 5265 746f 726e 6f20     ## O Retorno 
-00002b30: 4573 7065 7261 646f 0a20 2020 202d 2072  Esperado.    - r
-00002b40: 6570 7265 7365 6e74 6120 6120 7461 7861  epresenta a taxa
-00002b50: 2064 6520 7265 746f 726e 6f20 6dc3 a964   de retorno m..d
-00002b60: 6961 2071 7565 2073 6520 6573 7065 7261  ia que se espera
-00002b70: 206f 6274 6572 2064 6f20 706f 7274 66c3   obter do portf.
-00002b80: b36c 696f 2064 6520 696e 7665 7374 696d  .lio de investim
-00002b90: 656e 746f 7320 0a0a 2020 2020 2323 204f  entos ..    ## O
-00002ba0: 2052 6973 636f 200a 2020 2020 2d20 7265   Risco .    - re
-00002bb0: 7072 6573 656e 7461 2061 206d 6564 6964  presenta a medid
-00002bc0: 6120 6465 2076 6f6c 6174 696c 6964 6164  a de volatilidad
-00002bd0: 6520 646f 2070 6f72 7466 c3b3 6c69 6f2c  e do portf..lio,
-00002be0: 206f 7520 7365 6a61 2c20 0a20 2020 2071   ou seja, .    q
-00002bf0: 7561 6e74 6f20 6d61 6973 2069 6e73 74c3  uanto mais inst.
-00002c00: a176 656c 2066 6f72 206f 2072 6574 6f72  .vel for o retor
-00002c10: 6e6f 2064 6f73 2061 7469 766f 732c 206d  no dos ativos, m
-00002c20: 6169 6f72 2073 6572 c3a1 206f 2072 6973  aior ser.. o ris
-00002c30: 636f 2064 6f20 706f 7274 66c3 b36c 696f  co do portf..lio
-00002c40: 2063 6f6d 6f20 756d 2074 6f64 6f20 0a0a   como um todo ..
-00002c50: 2020 2020 0a20 2020 200a 2020 2020 0a20      .    .    . 
-00002c60: 2020 2023 2320 5061 72c3 a26d 6574 726f     ## Par..metro
-00002c70: 730a 2020 2020 0a20 2020 202d 2073 796d  s.    .    - sym
-00002c80: 626f 6c73 202d 3e20 5265 6365 6265 2075  bols -> Recebe u
-00002c90: 6d61 206c 6973 7461 2064 6520 6174 6976  ma lista de ativ
-00002ca0: 6f73 2070 6172 6120 6275 7363 6172 206e  os para buscar n
-00002cb0: 6120 6261 7365 200a 0a20 2020 202d 2073  a base ..    - s
-00002cc0: 7461 7274 5f64 6174 6520 2d3e 2044 6174  tart_date -> Dat
-00002cd0: 6120 6465 2049 6e69 6369 6f20 6461 2062  a de Inicio da b
-00002ce0: 7573 6361 2064 6173 2069 6e66 6f73 2028  usca das infos (
-00002cf0: 7072 6563 6f2c 2076 6f6c 756d 652c 2065  preco, volume, e
-00002d00: 7463 2920 646f 2061 7469 766f 200a 0a20  tc) do ativo .. 
-00002d10: 2020 202d 2065 6e64 5f64 6174 6520 2d3e     - end_date ->
-00002d20: 2044 6174 6120 4669 6e61 6c20 7061 7261   Data Final para
-00002d30: 2061 2062 7573 6361 2064 6173 2069 6e66   a busca das inf
-00002d40: 6f73 2028 7072 6563 6f2c 2076 6f6c 756d  os (preco, volum
-00002d50: 652c 2065 7463 2920 646f 2061 7469 766f  e, etc) do ativo
-00002d60: 200a 0a0a 2020 2020 7262 0000 007a 0941   ...    rb...z.A
-00002d70: 646a 2043 6c6f 7365 7216 0000 0072 6500  dj Closer....re.
-00002d80: 0000 679a 9999 9999 99b9 3f72 0100 0000  ..g.......?r....
-00002d90: 7a08 4f20 6174 6976 6f20 7a15 2064 6576  z.O ativo z. dev
-00002da0: 6520 7365 7220 616c 6f63 6164 6f20 656d  e ser alocado em
-00002db0: 2072 5300 0000 7a03 2e32 667a 0d25 2064   rS...z..2fz.% d
-00002dc0: 6120 6361 7274 6569 7261 2903 fa10 5265  a carteira)...Re
-00002dd0: 746f 726e 6f20 4573 7065 7261 646f fa11  torno Esperado..
-00002de0: 5269 7363 6f20 6461 2043 6172 7465 6972  Risco da Carteir
-00002df0: 61fa 1241 6c6f 6361 6361 6f20 4d61 726b  a..Alocacao Mark
-00002e00: 6f77 6974 7a29 1672 2a00 0000 7266 0000  owitz).r*...rf..
-00002e10: 0072 6e00 0000 da06 6472 6f70 6e61 726f  .rn.....dropnaro
-00002e20: 0000 0072 6700 0000 da05 6172 7261 7972  ...rg.....arrayr
-00002e30: 8300 0000 7231 0000 0072 5800 0000 726a  ....r1...rX...rj
-00002e40: 0000 00da 0364 6f74 da01 54da 0574 7261  .....dot..T..tra
-00002e50: 6365 5a06 6c69 6e61 6c67 da03 696e 76da  ceZ.linalg..inv.
-00002e60: 0365 7965 da05 7368 6170 65da 046f 6e65  .eye..shape..one
-00002e70: 73da 0766 6c61 7474 656e da05 7261 6e67  s..flatten..rang
-00002e80: 65da 0661 7070 656e 6429 1172 7900 0000  e..append).ry...
-00002e90: 7289 0000 0072 6100 0000 7285 0000 005a  r....ra...r....Z
-00002ea0: 0872 6574 6f72 6e6f 735a 126d 6174 7269  .retornosZ.matri
-00002eb0: 7a5f 636f 7661 7269 616e 6369 615a 0570  z_covarianciaZ.p
-00002ec0: 6573 6f73 da10 7265 746f 726e 6f5f 6573  esos..retorno_es
-00002ed0: 7065 7261 646f da05 7269 7363 6f5a 076c  perado..riscoZ.l
-00002ee0: 616d 6264 615f 5a07 636f 765f 696e 765a  ambda_Z.cov_invZ
-00002ef0: 0976 6574 6f72 5f75 6e73 5a0b 775f 6d61  .vetor_unsZ.w_ma
-00002f00: 726b 6f77 6974 7a5a 0d6d 6172 6b6f 7769  rkowitzZ.markowi
-00002f10: 747a 4c69 7374 da01 695a 0574 6178 6173  tzList..iZ.taxas
-00002f20: 7234 0000 0072 1f00 0000 721f 0000 0072  r4...r....r....r
-00002f30: 2000 0000 da14 6d61 726b 6f77 6974 7a5f   .....markowitz_
-00002f40: 616c 6c6f 6361 7469 6f6e 0002 0000 7328  allocation....s(
-00002f50: 0000 0000 1614 030c 0308 031c 0316 0326  ...............&
-00002f60: 030e 0120 0112 0122 0108 0304 0110 0120  ... ..."....... 
-00002f70: 010c 0102 0102 0102 fe06 0672 9c00 0000  ...........r....
-00002f80: 7a23 7374 6f63 6b73 2f7b 7379 6d62 6f6c  z#stocks/{symbol
-00002f90: 7d2f 4d61 726b 6f77 6974 7a41 6c6c 6f63  }/MarkowitzAlloc
-00002fa0: 6174 696f 6e7a 0a2f 696e 666f 4675 6e64  ationz./infoFund
-00002fb0: 7363 0100 0000 0000 0000 0000 0000 0700  sc..............
-00002fc0: 0000 0400 0000 4300 0000 7372 0000 0064  ......C...sr...d
-00002fd0: 017d 0174 00a0 017c 01a1 017d 0274 027c  .}.t...|...}.t.|
-00002fe0: 026a 0364 0283 027d 037c 03a0 0464 03a1  .j.d...}.|...d..
-00002ff0: 0164 0419 007d 0474 05a0 0674 077c 0483  .d...}.t...t.|..
-00003000: 01a1 0164 0419 007d 057c 0564 0519 00a0  ...d...}.|.d....
-00003010: 0864 0664 0784 00a1 017c 0564 053c 007c  .d.d.....|.d.<.|
-00003020: 056a 097c 0564 0519 007c 006b 0219 007d  .j.|.d...|.k...}
-00003030: 067c 0667 0064 08a2 0119 007d 067c 0653  .|.g.d.....}.|.S
-00003040: 0029 0975 ca00 0000 0a20 2020 2023 2320  .).u.....    ## 
-00003050: 5573 6162 696c 6964 6164 650a 2020 2020  Usabilidade.    
-00003060: 2d20 4675 6ec3 a761 6f20 7574 696c 697a  - Fun..ao utiliz
-00003070: 6164 6120 7061 7261 2061 6471 7569 7269  ada para adquiri
-00003080: 7220 6173 2070 7269 6e63 6970 6169 7320  r as principais 
-00003090: 6361 7261 6374 6572 6973 7469 6361 7320  caracteristicas 
-000030a0: 6520 696e 666f 726d 61c3 a7c3 b565 7320  e informa....es 
-000030b0: 646f 2066 756e 646f 2073 656c 6563 696f  do fundo selecio
-000030c0: 6e61 646f 0a0a 2020 2020 2323 2050 6172  nado..    ## Par
-000030d0: c3a2 6d65 7472 6f73 0a0a 2020 2020 2d20  ..metros..    - 
-000030e0: 7379 6d62 6f6c 202d 3e20 4e6f 6d65 2064  symbol -> Nome d
-000030f0: 6f20 4675 6e64 6f20 7061 7261 2066 617a  o Fundo para faz
-00003100: 6572 2061 2062 7573 6361 200a 0a0a 2020  er a busca ...  
-00003110: 2020 fa28 6874 7470 733a 2f2f 7777 772e    .(https://www.
-00003120: 6675 6e64 7365 7870 6c6f 7265 722e 636f  fundsexplorer.co
-00003130: 6d2e 6272 2f72 616e 6b69 6e67 fa0b 6874  m.br/ranking..ht
-00003140: 6d6c 2e70 6172 7365 72da 0574 6162 6c65  ml.parser..table
-00003150: 7201 0000 00f5 1000 0000 43c3 b364 6967  r.........C..dig
-00003160: 6f20 646f 2066 756e 646f 6301 0000 0000  o do fundoc.....
-00003170: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
-00003180: 0000 0073 0800 0000 7c00 6401 1700 5300  ...s....|.d...S.
-00003190: a902 4efa 032e 5341 721f 0000 00a9 01da  ..N...SAr.......
-000031a0: 0178 721f 0000 0072 1f00 0000 7220 0000  .xr....r....r ..
-000031b0: 00da 083c 6c61 6d62 6461 3e54 0200 00f3  ...<lambda>T....
-000031c0: 0000 0000 7a1b 6765 745f 6675 6e64 732e  ....z.get_funds.
-000031d0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-000031e0: 3ea9 0672 a000 0000 da05 5365 746f 72f5  >..r......Setor.
-000031f0: 0c00 0000 5072 65c3 a76f 2041 7475 616c  ....Pre..o Atual
-00003200: da09 4469 7669 6465 6e64 6ff5 1100 0000  ..Dividendo.....
-00003210: 5661 7269 61c3 a7c3 a36f 2050 7265 c3a7  Varia....o Pre..
-00003220: 6ff5 1000 0000 5265 6e74 6162 2e20 5065  o.....Rentab. Pe
-00003230: 72c3 ad6f 646f 290a da08 7265 7175 6573  r..odo)...reques
-00003240: 7473 da03 6765 7472 0a00 0000 da07 636f  ts..getr......co
-00003250: 6e74 656e 74da 0866 696e 645f 616c 6c72  ntent..find_allr
-00003260: 4300 0000 da09 7265 6164 5f68 746d 6c72  C.....read_htmlr
-00003270: 8200 0000 da05 6170 706c 79da 036c 6f63  ......apply..loc
-00003280: 2907 7222 0000 00da 0375 726c da08 7265  ).r".....url..re
-00003290: 7370 6f6e 7365 da04 736f 7570 729f 0000  sponse..soupr...
-000032a0: 00da 0766 756e 6473 4446 da08 7661 6c75  ...fundsDF..valu
-000032b0: 6573 4649 721f 0000 0072 1f00 0000 7220  esFIr....r....r 
-000032c0: 0000 00da 0967 6574 5f66 756e 6473 4202  .....get_fundsB.
-000032d0: 0000 7312 0000 0000 0d04 010a 010c 010e  ..s.............
-000032e0: 0112 0116 0212 010c 0272 b900 0000 7a12  .........r....z.
-000032f0: 2f63 6f6d 7061 7265 5365 746f 7246 756e  /compareSetorFun
-00003300: 6473 2902 da05 7365 746f 7272 2300 0000  ds)...setorr#...
-00003310: 6302 0000 0000 0000 0000 0000 000c 0000  c...............
-00003320: 0006 0000 0043 0000 0073 1e01 0000 6401  .....C...s....d.
-00003330: 7d02 7400 a001 7c02 a101 7d03 7402 7c03  }.t...|...}.t.|.
-00003340: 6a03 6402 8302 7d04 7c04 a004 6403 a101  j.d...}.|...d...
-00003350: 6404 1900 7d05 7405 a006 7407 7c05 8301  d...}.t...t.|...
-00003360: a101 6404 1900 7d06 7408 7c06 6405 8302  ..d...}.t.|.d...
-00003370: 0100 7c01 6406 1b00 7d01 7c06 6a09 7c06  ..|.d...}.|.j.|.
-00003380: 6405 1900 6406 1b00 7c01 6b04 1900 7d07  d...d...|.k...}.
-00003390: 7c07 6700 6407 a201 1900 7d07 7c07 a00a  |.g.d.....}.|...
-000033a0: a100 7d07 7c07 6405 1900 a00b a100 7d08  ..}.|.d.......}.
-000033b0: 7c00 6408 6b02 72aa 6409 7d00 7c07 6a09  |.d.k.r.d.}.|.j.
-000033c0: 7c07 640a 1900 7c00 6b02 1900 6405 1900  |.d...|.k...d...
-000033d0: a00b a100 7d09 6e42 7c00 640b 6b02 72d2  ....}.nB|.d.k.r.
-000033e0: 640c 7d00 7c07 6a09 7c07 640a 1900 7c00  d.}.|.j.|.d...|.
-000033f0: 6b02 1900 6405 1900 a00b a100 7d09 6e1a  k...d.......}.n.
-00003400: 7c07 6a09 7c07 640a 1900 7c00 6b02 1900  |.j.|.d...|.k...
-00003410: 6405 1900 a00b a100 7d09 7c07 6405 1900  d.......}.|.d...
-00003420: a00c a100 7d0a 7405 a00d 7c08 6701 7c09  ....}.t...|.g.|.
-00003430: 6701 7c0a 6701 640d 9c03 a101 7d0b 7c0b  g.|.g.d.....}.|.
-00003440: a00e 640e a101 7d0b 7c0b 5300 290f 7506  ..d...}.|.S.).u.
-00003450: 0300 000a 2020 2020 2323 2055 7361 6269  ....    ## Usabi
-00003460: 6c69 6461 6465 0a20 2020 200a 2020 2020  lidade.    .    
-00003470: 2d20 4675 6ec3 a761 6f20 7175 6520 7574  - Fun..ao que ut
-00003480: 696c 697a 6120 6173 206d 6574 7269 6361  iliza as metrica
-00003490: 7320 6520 6d65 6469 6173 2064 6f73 2066  s e medias dos f
-000034a0: 756e 646f 2063 6f6d 2062 6173 6520 6e6f  undo com base no
-000034b0: 2073 6575 2053 6574 6f72 2070 6172 6120   seu Setor para 
-000034c0: 756d 6120 616e 616c 6973 6520 6d61 6973  uma analise mais
-000034d0: 2072 6573 7472 6974 610a 2020 2020 0a20   restrita.    . 
-000034e0: 2020 2023 2320 5061 72c3 a26d 6574 726f     ## Par..metro
-000034f0: 730a 2020 2020 0a20 2020 202d 2072 656e  s.    .    - ren
-00003500: 7461 6269 6c69 6461 6465 5f6d 696e 202d  tabilidade_min -
-00003510: 3e20 5661 6c6f 7220 656d 2025 2070 6172  > Valor em % par
-00003520: 6120 6275 7363 6172 2061 2072 656e 7461  a buscar a renta
-00003530: 6269 6c69 6461 6465 206d 696e 696d 6120  bilidade minima 
-00003540: 646f 2066 756e 646f 2065 7363 6f6c 6869  do fundo escolhi
-00003550: 646f 0a20 2020 202d 2073 6574 6f72 202d  do.    - setor -
-00003560: 3e20 5365 746f 7265 7320 6465 2066 756e  > Setores de fun
-00003570: 646f 7320 7175 6520 706f 6465 7261 6d20  dos que poderam 
-00003580: 7365 7220 6573 636f 6c68 6964 6f73 2c20  ser escolhidos, 
-00003590: 7365 6775 6520 6120 6c69 7374 613a 0a20  segue a lista:. 
-000035a0: 2020 200a 2020 2020 6060 600a 2020 2020     .    ```.    
-000035b0: 5469 706f 7353 6574 6f72 6573 3a0a 2020  TiposSetores:.  
-000035c0: 2020 2d20 436f 7270 6f72 6174 6976 6173    - Corporativas
-000035d0: 203d 2022 4c61 6a65 7320 436f 7270 6f72   = "Lajes Corpor
-000035e0: 6174 6976 6173 2220 0a20 2020 202d 204d  ativas" .    - M
-000035f0: 6f62 696c 6961 7269 6f73 203d 2022 54c3  obiliarios = "T.
-00003600: ad74 756c 6f73 2065 2056 616c 2e20 4d6f  .tulos e Val. Mo
-00003610: 622e 220a 2020 2020 2d20 5368 6f70 7069  b.".    - Shoppi
-00003620: 6e67 7320 3d20 2253 686f 7070 696e 6773  ngs = "Shoppings
-00003630: 220a 2020 2020 2d20 48c3 ad62 7269 646f  ".    - H..brido
-00003640: 203d 2027 48c3 ad62 7269 646f 270a 2020   = 'H..brido'.  
-00003650: 2020 2d20 5265 6e64 6120 3d20 2752 656e    - Renda = 'Ren
-00003660: 6461 270a 2020 2020 2d20 4c6f 67c3 ad73  da'.    - Log..s
-00003670: 7469 6361 203d 2027 4c6f 67c3 ad73 7469  tica = 'Log..sti
-00003680: 6361 270a 2020 2020 2d20 486f 7370 6974  ca'.    - Hospit
-00003690: 616c 203d 2027 486f 7370 6974 616c 270a  al = 'Hospital'.
-000036a0: 2020 2020 2d20 5265 7369 6465 6e63 6961      - Residencia
-000036b0: 6c20 3d20 2752 6573 6964 656e 6369 616c  l = 'Residencial
-000036c0: 270a 2020 2020 2d20 4f75 7472 6f73 203d  '.    - Outros =
-000036d0: 2027 4f75 7472 6f73 270a 0a20 2020 2060   'Outros'..    `
-000036e0: 6060 0a20 2020 2023 2320 4578 656d 706c  ``.    ## Exempl
-000036f0: 6f3a 0a20 2020 200a 2020 2020 6060 600a  o:.    .    ```.
-00003700: 2020 2020 3e3e 3e20 6262 2e63 6f6d 7061      >>> bb.compa
-00003710: 7265 5f73 6574 6f72 5f66 756e 6473 2873  re_setor_funds(s
-00003720: 6574 6f72 3d27 436f 7270 6f72 6174 6976  etor='Corporativ
-00003730: 6173 272c 2072 656e 7461 6269 6c69 6461  as', rentabilida
-00003740: 6465 5f6d 696e 203d 2033 290a 2020 2020  de_min = 3).    
-00003750: 6060 600a 0a20 2020 2072 9d00 0000 729e  ```..    r....r.
-00003760: 0000 0072 9f00 0000 7201 0000 0072 ac00  ...r....r....r..
-00003770: 0000 7253 0000 0072 a700 0000 5a0c 436f  ..rS...r....Z.Co
-00003780: 7270 6f72 6174 6976 6173 7a12 4c61 6a65  rporativasz.Laje
-00003790: 7320 436f 7270 6f72 6174 6976 6173 72a8  s Corporativasr.
-000037a0: 0000 005a 0b4d 6f62 696c 6961 7269 6f73  ...Z.Mobiliarios
-000037b0: 7514 0000 0054 c3ad 7475 6c6f 7320 6520  u....T..tulos e 
-000037c0: 5661 6c2e 204d 6f62 2e29 0375 2a00 0000  Val. Mob.).u*...
-000037d0: 5265 6e74 6162 696c 6964 6164 6520 4dc3  Rentabilidade M.
-000037e0: a964 6961 2064 6f73 2046 4949 7320 5365  .dia dos FIIs Se
-000037f0: 6c65 6369 6f6e 6164 6f73 751f 0000 0052  lecionadosu....R
-00003800: 656e 7461 6269 6c69 6461 6465 204d c3a9  entabilidade M..
-00003810: 6469 6120 646f 204d 6572 6361 646f 7537  dia do Mercadou7
-00003820: 0000 0044 6573 7669 6f20 5061 6472 c3a3  ...Desvio Padr..
-00003830: 6f20 6461 7320 5265 6e74 6162 696c 6964  o das Rentabilid
-00003840: 6164 6573 2064 6f73 2046 4949 7320 5365  ades dos FIIs Se
-00003850: 6c65 6369 6f6e 6164 6f73 7a20 4f20 7365  lecionadosz O se
-00003860: 746f 722f 7661 6c6f 7220 6e61 6f20 666f  tor/valor nao fo
-00003870: 6920 656e 636f 6e74 7261 646f 290f 72ad  i encontrado).r.
-00003880: 0000 0072 ae00 0000 720a 0000 0072 af00  ...r....r....r..
-00003890: 0000 72b0 0000 0072 4300 0000 72b1 0000  ..r....rC...r...
-000038a0: 0072 8200 0000 7221 0000 0072 b300 0000  .r....r!...r....
-000038b0: 728d 0000 0072 5800 0000 7275 0000 0072  r....rX...ru...r
-000038c0: 4400 0000 5a06 6669 6c6c 6e61 290c 72ba  D...Z.fillna).r.
-000038d0: 0000 005a 1172 656e 7461 6269 6c69 6461  ...Z.rentabilida
-000038e0: 6465 5f6d 696e 72b4 0000 0072 b500 0000  de_minr....r....
-000038f0: 72b6 0000 0072 9f00 0000 72b7 0000 0072  r....r....r....r
-00003900: b800 0000 5a13 7265 6e74 6162 696c 6964  ....Z.rentabilid
-00003910: 6164 655f 6d65 6469 615a 1572 656e 7461  ade_mediaZ.renta
-00003920: 6269 6c69 6461 6465 5f6d 6572 6361 646f  bilidade_mercado
-00003930: da0d 6465 7376 696f 5f70 6164 7261 6f5a  ..desvio_padraoZ
-00003940: 0a72 6573 756c 7461 646f 7372 1f00 0000  .resultadosr....
-00003950: 721f 0000 0072 2000 0000 da13 636f 6d70  r....r .....comp
-00003960: 6172 655f 7365 746f 725f 6675 6e64 7362  are_setor_fundsb
-00003970: 0200 0073 3400 0000 0022 0401 0a01 0c01  ...s4...."......
-00003980: 0e01 1202 0a01 0801 1601 0c01 0801 0c01  ................
-00003990: 0801 0401 1c01 0801 0401 1c02 1a02 0c02  ................
-000039a0: 0401 0401 0401 04fd 0806 0a02 72bc 0000  ............r...
-000039b0: 007a 0d2f 636f 6d70 6172 6546 756e 6473  .z./compareFunds
-000039c0: 2901 7223 0000 0063 0300 0000 0000 0000  ).r#...c........
-000039d0: 0000 0000 1200 0000 0400 0000 4300 0000  ............C...
-000039e0: 734a 0100 007c 0172 bc7c 0264 016b 0372  sJ...|.r.|.d.k.r
-000039f0: bc64 027d 0374 00a0 017c 03a1 017d 0474  .d.}.t...|...}.t
-00003a00: 027c 046a 0364 0383 027d 057c 05a0 0464  .|.j.d...}.|...d
-00003a10: 04a1 0164 0519 007d 0674 05a0 0674 077c  ...d...}.t...t.|
-00003a20: 0683 01a1 0164 0519 007d 077c 0764 0619  .....d...}.|.d..
-00003a30: 00a0 0864 0764 0884 00a1 017c 0764 063c  ...d.d.....|.d.<
-00003a40: 007c 0767 0064 09a2 0119 007d 077c 076a  .|.g.d.....}.|.j
-00003a50: 0964 0667 0164 0a8d 017d 077c 076a 0a7c  .d.g.d...}.|.j.|
-00003a60: 0764 0619 007c 016b 0219 007d 087c 076a  .d...|.k...}.|.j
-00003a70: 0a7c 0764 0619 007c 026b 0219 007d 0974  .|.d...|.k...}.t
-00003a80: 05a0 0b7c 087c 0967 02a1 017d 0a7c 0a6a  ...|.|.g...}.|.j
-00003a90: 0c72 b874 0d64 0b83 0101 006e 047c 0a53  .r.t.d.....n.|.S
-00003aa0: 007c 0064 0175 0072 ca67 007d 006e 7c64  .|.d.u.r.g.}.n|d
-00003ab0: 0c7d 0b64 0d7d 0c7c 0044 005d 3a7d 0d74  .}.d.}.|.D.]:}.t
-00003ac0: 0ea0 0f7c 0da1 017d 0e7c 0e6a 1064 0e64  ...|...}.|.j.d.d
-00003ad0: 0f8d 017d 0f7c 0f64 1019 00a0 11a1 00a0  ...}.|.d........
-00003ae0: 12a1 007d 107c 107c 0b6b 0472 d67c 107d  ...}.|.|.k.r.|.}
-00003af0: 0b7c 0d7d 0c71 d674 056a 137c 0c7c 0b64  .|.}.q.t.j.|.|.d
-00003b00: 1114 0064 129c 0274 147c 0083 0167 0164  ...d...t.|...g.d
-00003b10: 138d 027d 117c 116a 0c90 0172 4274 0d64  ...}.|.j...rBt.d
-00003b20: 1483 0101 006e 047c 1153 0064 0153 0029  .....n.|.S.d.S.)
-00003b30: 1575 2403 0000 0a20 2020 2023 2320 5573  .u$....    ## Us
-00003b40: 6162 696c 6964 6164 650a 2020 2020 0a20  abilidade.    . 
-00003b50: 2020 202d 2046 756e c3a7 616f 2071 7565     - Fun..ao que
-00003b60: 2072 6561 6c69 7a61 2061 2063 6f6d 7061   realiza a compa
-00003b70: 7261 c3a7 616f 2065 6e74 7265 2064 6f69  ra..ao entre doi
-00003b80: 7320 6675 6e64 6f73 2c20 7365 6a61 2066  s fundos, seja f
-00003b90: 6569 7461 2061 2072 6571 7569 7369 c3a7  eita a requisi..
-00003ba0: 616f 2064 6f73 2066 756e 646f 7320 7669  ao dos fundos vi
-00003bb0: 6120 6c69 7374 6120 6f75 2075 6e69 636f  a lista ou unico
-00003bc0: 7320 0a20 2020 202d 2052 6571 7569 7369  s .    - Requisi
-00003bd0: c3a7 616f 204c 6973 7461 733a 2052 6574  ..ao Listas: Ret
-00003be0: 6f72 6e61 206f 2066 756e 646f 2063 6f6d  orna o fundo com
-00003bf0: 206d 6169 6f72 2070 6f72 6365 6e74 6167   maior porcentag
-00003c00: 656d 2064 6520 7269 7363 6f20 2861 2076  em de risco (a v
-00003c10: 6172 6961 c3a7 c3a3 6f20 7065 7263 656e  aria....o percen
-00003c20: 7475 616c 2064 6f73 2070 7265 c3a7 6f73  tual dos pre..os
-00003c30: 2064 6f73 2061 7469 766f 732c 2063 616c   dos ativos, cal
-00003c40: 6375 6c6f 2072 6561 6c69 7a61 646f 2063  culo realizado c
-00003c50: 6f6d 2062 6173 6520 6e6f 2064 6573 7669  om base no desvi
-00003c60: 6f20 7061 6472 c3a3 6f29 0a20 2020 202d  o padr..o).    -
-00003c70: 2052 6571 7569 7369 c3a7 616f 2055 6e69   Requisi..ao Uni
-00003c80: 6361 3a20 5265 746f 726e 6120 756d 2044  ca: Retorna um D
-00003c90: 6174 6166 7261 6d65 2063 6f6d 2061 7320  ataframe com as 
-00003ca0: 7072 696e 6369 7061 6973 2069 6e66 6f72  principais infor
-00003cb0: 6d61 c3a7 6f65 7320 646f 7320 6675 6e64  ma..oes dos fund
-00003cc0: 6f73 2c20 6166 696d 2064 6520 756d 6120  os, afim de uma 
-00003cd0: 636f 6d70 6172 61c3 a761 6f20 656e 7472  compara..ao entr
-00003ce0: 6520 7365 7573 2076 616c 6f72 6573 200a  e seus valores .
-00003cf0: 0a20 2020 200a 2020 2020 2323 2050 6172  .    .    ## Par
-00003d00: c3a2 6d65 7472 6f73 0a20 2020 200a 2020  ..metros.    .  
-00003d10: 2020 2d20 6c69 7374 6675 6e64 202d 3e20    - listfund -> 
-00003d20: 4c69 7374 6120 646f 7320 6675 6e64 6f73  Lista dos fundos
-00003d30: 2070 6172 6120 616e 616c 6973 6520 6465   para analise de
-00003d40: 2072 6973 636f 0a20 2020 202d 2066 756e   risco.    - fun
-00003d50: 645f 3120 2d3e 2050 7269 6d65 6972 6f20  d_1 -> Primeiro 
-00003d60: 6675 6e64 6f20 7061 7261 2061 6e61 6c69  fundo para anali
-00003d70: 7365 2075 6e69 6361 0a20 2020 202d 2066  se unica.    - f
-00003d80: 756e 645f 3220 2d3e 2053 6567 756e 646f  und_2 -> Segundo
-00003d90: 2066 756e 646f 2070 6172 6120 616e 616c   fundo para anal
-00003da0: 6973 6520 756e 6963 610a 2020 2020 0a20  ise unica.    . 
-00003db0: 2020 2023 2320 4578 656d 706c 6f73 3a0a     ## Exemplos:.
-00003dc0: 2020 2020 0a20 2020 2060 6060 0a20 2020      .    ```.   
-00003dd0: 203e 3e3e 2062 622e 636f 6d70 6172 655f   >>> bb.compare_
-00003de0: 6675 6e64 7328 6c69 7374 6675 6e64 3d20  funds(listfund= 
-00003df0: 6c69 7374 2920 0a20 2020 2020 2020 2020  list) .         
-00003e00: 2020 2020 2020 2020 2020 206f 750a 2020             ou.  
-00003e10: 2020 3e3e 3e20 6262 2e63 6f6d 7061 7265    >>> bb.compare
-00003e20: 5f66 756e 6473 2866 756e 645f 313d 2027  _funds(fund_1= '
-00003e30: 6675 6e64 3127 2c20 6675 6e64 5f32 3d20  fund1', fund_2= 
-00003e40: 2766 756e 6432 2729 0a20 2020 2060 6060  'fund2').    ```
-00003e50: 0a20 2020 200a 2020 2020 4e72 9d00 0000  .    .    Nr....
-00003e60: 729e 0000 0072 9f00 0000 7201 0000 0072  r....r....r....r
-00003e70: a000 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00003e80: 0001 0000 0002 0000 0053 0000 0073 0800  .........S...s..
-00003e90: 0000 7c00 6401 1700 5300 72a1 0000 0072  ..|.d...S.r....r
-00003ea0: 1f00 0000 72a3 0000 0072 1f00 0000 721f  ....r....r....r.
-00003eb0: 0000 0072 2000 0000 72a5 0000 00cb 0200  ...r ...r.......
-00003ec0: 0072 a600 0000 7a1f 636f 6d70 6172 655f  .r....z.compare_
-00003ed0: 6675 6e64 732e 3c6c 6f63 616c 733e 2e3c  funds.<locals>.<
-00003ee0: 6c61 6d62 6461 3e29 0872 a000 0000 72a8  lambda>).r....r.
-00003ef0: 0000 0072 a900 0000 72aa 0000 0072 ab00  ...r....r....r..
-00003f00: 0000 72ac 0000 007a 0e44 6976 6964 656e  ..r....z.Dividen
-00003f10: 6420 5969 656c 647a 1144 5920 2833 4d29  d Yieldz.DY (3M)
-00003f20: 2041 6375 6d75 6c61 646f 2901 5a06 7375   Acumulado).Z.su
-00003f30: 6273 6574 753e 0000 004e 616f 2066 6f72  bsetu>...Nao for
-00003f40: 616d 2061 7072 6573 656e 7461 646f 2064  am apresentado d
-00003f50: 6164 6f73 2064 6f73 2066 756e 646f 7320  ados dos fundos 
-00003f60: 7061 7261 2076 6572 6966 6963 61c3 a761  para verifica..a
-00003f70: 6f20 756e 6963 6172 2600 0000 7218 0000  o unicar&...r...
-00003f80: 0072 4e00 0000 723c 0000 0072 4800 0000  .rN...r<...rH...
-00003f90: 7253 0000 0029 025a 0446 756e 647a 0c4d  rS...).Z.Fundz.M
-00003fa0: 6178 2072 6973 6b20 2825 2972 7f00 0000  ax risk (%)r....
-00003fb0: 7542 0000 004e 616f 2066 6f72 616d 2061  uB...Nao foram a
-00003fc0: 7072 6573 656e 7461 646f 2064 6164 6f73  presentado dados
-00003fd0: 2064 6f73 2066 756e 646f 7320 7061 7261   dos fundos para
-00003fe0: 2076 6572 6966 6963 61c3 a761 6f20 6dc3   verifica..ao m.
-00003ff0: ba6c 7469 706c 6129 1572 ad00 0000 72ae  .ltipla).r....r.
-00004000: 0000 0072 0a00 0000 72af 0000 0072 b000  ...r....r....r..
-00004010: 0000 7243 0000 0072 b100 0000 7282 0000  ..rC...r....r...
-00004020: 0072 b200 0000 da0f 6472 6f70 5f64 7570  .r......drop_dup
-00004030: 6c69 6361 7465 7372 b300 0000 7284 0000  licatesr....r...
-00004040: 0072 4100 0000 722f 0000 0072 2a00 0000  .rA...r/...r*...
-00004050: 722b 0000 0072 4000 0000 726e 0000 0072  r+...r@...rn...r
-00004060: 7500 0000 7244 0000 0072 8300 0000 2912  u...rD...r....).
-00004070: 5a08 6c69 7374 6675 6e64 5a06 6675 6e64  Z.listfundZ.fund
-00004080: 5f31 5a06 6675 6e64 5f32 72b4 0000 0072  _1Z.fund_2r....r
-00004090: b500 0000 72b6 0000 0072 9f00 0000 72b7  ....r....r....r.
-000040a0: 0000 005a 0566 756e 6431 5a05 6675 6e64  ...Z.fund1Z.fund
-000040b0: 32da 0475 6e69 745a 096d 6178 5f72 6973  2..unitZ.max_ris
-000040c0: 636f 5a10 7469 636b 6572 5f6d 6178 5f72  coZ.ticker_max_r
-000040d0: 6973 636f 727a 0000 005a 0566 756e 646f  iscorz...Z.fundo
-000040e0: 721e 0000 0072 bb00 0000 5a09 7661 6c75  r....r....Z.valu
-000040f0: 6572 6973 6b72 1f00 0000 721f 0000 0072  eriskr....r....r
-00004100: 2000 0000 da0d 636f 6d70 6172 655f 6675   .....compare_fu
-00004110: 6e64 73ac 0200 0073 4400 0000 0019 0c01  nds....sD.......
-00004120: 0401 0a01 0c01 0e01 1201 1601 0c01 0e02  ................
-00004130: 1201 1202 0e01 0601 0a02 0402 0801 0602  ................
-00004140: 0401 0401 0801 0a01 0c01 1001 0801 0401  ................
-00004150: 0602 0601 06ff 0401 08ff 0603 0801 0a02  ................
-00004160: 72bf 0000 007a 0b2f 6265 7374 4173 7365  r....z./bestAsse
-00004170: 7473 6301 0000 0000 0000 0000 0000 0019  tsc.............
-00004180: 0000 0005 0000 0043 0000 0073 fa02 0000  .......C...s....
-00004190: 6401 7d01 7400 a001 7c01 a101 7d02 7c02  d.}.t...|...}.|.
-000041a0: 6a02 6402 6b03 7224 7403 6403 8301 0100  j.d.k.r$t.d.....
-000041b0: 9002 6ed2 7404 7c02 6a05 6404 8302 7d03  ..n.t.|.j.d...}.
-000041c0: 7c03 a006 6405 a101 6406 1900 7d04 7407  |...d...d...}.t.
-000041d0: 6a08 7409 7c04 8301 6407 6408 6409 8d03  j.t.|...d.d.d...
-000041e0: 6406 1900 7d05 7c05 640a 1900 a00a 640b  d...}.|.d.....d.
-000041f0: 640c 8400 a101 7c05 640a 3c00 7403 640d  d.....|.d.<.t.d.
-00004200: 8301 0100 740b 6a0c 7c05 640a 1900 a00d  ....t.j.|.d.....
-00004210: a100 640e 640f 8d02 6410 1900 7d06 6411  ..d.d...d...}.d.
-00004220: 6412 8400 7d07 6413 6414 8400 7d08 6900  d...}.d.d...}.i.
-00004230: 7d09 6900 7d0a 7c06 6a0e 4400 5d24 7d0b  }.i.}.|.j.D.]$}.
-00004240: 7c06 7c0b 1900 7d0c 7c07 7c0c 8301 7c09  |.|...}.|.|...|.
-00004250: 7c0b 3c00 7c08 7c0c 8301 7c0a 7c0b 3c00  |.<.|.|...|.|.<.
-00004260: 71ac 7c00 6415 6b02 9001 7288 6700 7d0d  q.|.d.k...r.g.}.
-00004270: 7c06 6a0e 4400 5d26 7d0b 7c09 7c0b 1900  |.j.D.]&}.|.|...
-00004280: 6416 6b04 72e6 7c0a 7c0b 1900 6417 6b04  d.k.r.|.|...d.k.
-00004290: 72e6 7c0d a00f 7c0b a101 0100 71e6 7407  r.|...|.....q.t.
-000042a0: 6a10 7c0d 6418 6701 6419 8d02 7d0e 7403  j.|.d.g.d...}.t.
-000042b0: 641a 8301 0100 7411 7c0d 7412 7413 641b  d.....t.|.t.t.d.
-000042c0: 8d03 7d0f 7c0f 6701 7d0f 7407 a010 7c0f  ..}.|.g.}.t...|.
-000042d0: a101 7d10 7c10 a014 641c a101 7d10 7c10  ..}.|...d...}.|.
-000042e0: 641d 1900 a015 a100 a016 a100 7c10 641d  d...........|.d.
-000042f0: 3c00 7c10 641e 1900 a015 a100 a016 a100  <.|.d...........
-00004300: 7c10 641e 3c00 7c10 6a17 9001 7280 6e04  |.d.<.|.j...r.n.
-00004310: 7c10 5300 9001 6e6e 7c00 641f 6b02 9002  |.S...nn|.d.k...
-00004320: 7242 6700 7d11 7c06 6a0e 4400 5d2c 7d0b  rBg.}.|.j.D.],}.
-00004330: 7c09 7c0b 1900 6420 6b04 9001 729c 7c0a  |.|...d k...r.|.
-00004340: 7c0b 1900 6421 6b00 9001 729c 7c11 a00f  |...d!k...r.|...
-00004350: 7c0b a101 0100 9001 719c 7407 6a10 7c11  |.......q.t.j.|.
-00004360: 6422 6701 6419 8d02 7d12 7403 641a 8301  d"g.d...}.t.d...
-00004370: 0100 7411 7c11 7412 7413 641b 8d03 7d13  ..t.|.t.t.d...}.
-00004380: 7c13 6701 7d13 7407 a010 7c13 a101 7d14  |.g.}.t...|...}.
-00004390: 7c14 a014 641c a101 7d14 7c14 641d 1900  |...d...}.|.d...
-000043a0: a015 a100 a016 a100 7c14 641d 3c00 7c14  ........|.d.<.|.
-000043b0: 641e 1900 a015 a100 a016 a100 7c14 641e  d...........|.d.
-000043c0: 3c00 7c14 6a17 9002 723c 6e04 7c14 5300  <.|.j...r<n.|.S.
-000043d0: 6eb4 7c00 6423 6b02 9002 72ee 6700 7d15  n.|.d#k...r.g.}.
-000043e0: 7c06 6a0e 4400 5d1e 7d0b 7c0a 7c0b 1900  |.j.D.].}.|.|...
-000043f0: 6417 6b00 9002 7256 7c15 a00f 7c0b a101  d.k...rV|...|...
-00004400: 0100 9002 7156 7407 6a10 7c15 6424 6701  ....qVt.j.|.d$g.
-00004410: 6419 8d02 7d16 7403 641a 8301 0100 7411  d...}.t.d.....t.
-00004420: 7c15 7412 7413 641b 8d03 7d17 7c17 6701  |.t.t.d...}.|.g.
-00004430: 7d17 7407 a010 7c17 a101 7d18 7c18 a014  }.t...|...}.|...
-00004440: 641c a101 7d18 7c18 641d 1900 a015 a100  d...}.|.d.......
-00004450: a016 a100 7c18 641d 3c00 7c18 641e 1900  ....|.d.<.|.d...
-00004460: a015 a100 a016 a100 7c18 641e 3c00 7c18  ........|.d.<.|.
-00004470: 6a17 9002 72e8 6e04 7c18 5300 6e08 7403  j...r.n.|.S.n.t.
-00004480: 6425 8301 0100 6426 5300 2927 750c 0200  d%....d&S.)'u...
-00004490: 000a 2020 2020 2323 2055 7361 6269 6c69  ..    ## Usabili
-000044a0: 6461 6465 0a20 2020 202d 2046 756e c3a7  dade.    - Fun..
-000044b0: c3a3 6f20 7175 6520 616e 616c 6973 6120  ..o que analisa 
-000044c0: 6f73 2070 7269 6e63 6970 6169 7320 6174  os principais at
-000044d0: 6976 6f73 206c 6973 7461 646f 7320 6e6f  ivos listados no
-000044e0: 206d 6572 6361 646f 2071 7565 2063 6f6d   mercado que com
-000044f0: 2062 6173 6520 6e6f 2070 6572 6669 6c20   base no perfil 
-00004500: 6573 636f 6c68 6964 6f20 6d6f 7374 7261  escolhido mostra
-00004510: 2071 7561 6973 2070 6f64 656d 2073 6572   quais podem ser
-00004520: 2073 7561 7320 6573 636f 6c68 6173 2065   suas escolhas e
-00004530: 2071 7561 6e74 6f73 2070 6f72 6365 6e74   quantos porcent
-00004540: 6f20 7365 2064 6576 6520 7465 7220 6e61  o se deve ter na
-00004550: 2063 6172 7465 6972 610a 2020 2020 0a20   carteira.    . 
-00004560: 2020 2023 2320 5061 72c3 a26d 6574 726f     ## Par..metro
-00004570: 730a 2020 2020 0a20 2020 202d 2070 6572  s.    .    - per
-00004580: 6669 6c20 2d3e 2050 6572 6669 7320 7175  fil -> Perfis qu
-00004590: 6520 706f 6465 6d20 7365 7220 6573 636f  e podem ser esco
-000045a0: 6c68 6964 6f73 2070 6172 6120 7265 616c  lhidos para real
-000045b0: 697a 6172 2061 2061 6ec3 a16c 6973 652c  izar a an..lise,
-000045c0: 2073 6567 7565 2061 206c 6973 7461 3a20   segue a lista: 
-000045d0: 0a0a 2020 2020 0a20 2020 2060 6060 0a20  ..    .    ```. 
-000045e0: 2020 2054 6970 6f50 6572 6669 733a 0a20     TipoPerfis:. 
-000045f0: 2020 202a 2041 6772 6573 7369 766f 0a20     * Agressivo. 
-00004600: 2020 202a 204d 6f64 6572 6164 6f0a 2020     * Moderado.  
-00004610: 2020 2a20 436f 6e73 6572 7661 646f 720a    * Conservador.
-00004620: 2020 2020 0a20 2020 2060 6060 0a20 2020      .    ```.   
-00004630: 200a 2020 2020 2323 2045 7865 6d70 6c6f   .    ## Exemplo
-00004640: 0a20 2020 200a 2020 2020 6060 600a 2020  .    .    ```.  
-00004650: 2020 0a20 2020 203e 3e3e 2061 6c6f 6361    .    >>> aloca
-00004660: 7469 6f6e 203d 2062 6573 745f 6173 7365  tion = best_asse
-00004670: 7473 2870 6572 6669 6c3d 2741 6772 6573  ts(perfil='Agres
-00004680: 7369 766f 2729 0a20 2020 200a 2020 2020  sivo').    .    
-00004690: 6060 600a 2020 2020 0a20 2020 207a 2d68  ```.    .    z-h
-000046a0: 7474 7073 3a2f 2f77 7777 2e64 6164 6f73  ttps://www.dados
-000046b0: 6465 6d65 7263 6164 6f2e 636f 6d2e 6272  demercado.com.br
-000046c0: 2f62 6f6c 7361 2f61 636f 6573 7251 0000  /bolsa/acoesrQ..
-000046d0: 007a 3141 6365 7373 6f20 6e65 6761 646f  .z1Acesso negado
-000046e0: 2061 2062 6173 652c 2074 656e 7465 206e   a base, tente n
-000046f0: 6f76 616d 656e 7465 206d 6169 7320 7461  ovamente mais ta
-00004700: 7264 652e 729e 0000 0072 9f00 0000 7201  rde.r....r....r.
-00004710: 0000 00fa 012c 721a 0000 00a9 02da 0764  .....,r........d
-00004720: 6563 696d 616c 5a09 7468 6f75 7361 6e64  ecimalZ.thousand
-00004730: 73f5 0700 0000 43c3 b364 6967 6f63 0100  s.....C..digoc..
-00004740: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00004750: 0000 5300 0000 7308 0000 007c 0064 0117  ..S...s....|.d..
-00004760: 0053 0072 a100 0000 721f 0000 0072 a300  .S.r....r....r..
-00004770: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00004780: 0072 a500 0000 1a03 0000 72a6 0000 007a  .r........r....z
-00004790: 1d62 6573 745f 6173 7365 7473 2e3c 6c6f  .best_assets.<lo
-000047a0: 6361 6c73 3e2e 3c6c 616d 6264 613e 7a13  cals>.<lambda>z.
-000047b0: 4275 7363 616e 646f 2061 7469 766f 732e  Buscando ativos.
-000047c0: 2e2e 2e72 3a00 0000 723c 0000 0072 4800  ...r:...r<...rH.
-000047d0: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
-000047e0: 0000 0002 0000 0053 0000 0073 1400 0000  .......S...s....
-000047f0: 7c00 a000 a100 7d01 7c01 a001 a100 7d02  |.....}.|.....}.
-00004800: 7c02 5300 a901 4e29 0272 6e00 0000 7258  |.S...N).rn...rX
-00004810: 0000 0029 03da 0670 7265 636f 73da 0772  ...)...precos..r
-00004820: 6574 6f72 6e6f 5a0d 7265 746f 726e 6f5f  etornoZ.retorno_
-00004830: 6d65 6469 6f72 1f00 0000 721f 0000 0072  medior....r....r
-00004840: 2000 0000 da10 6361 6c63 756c 6172 5f72   .....calcular_r
-00004850: 6574 6f72 6e6f 1f03 0000 7306 0000 0000  etorno....s.....
-00004860: 0108 0108 017a 2562 6573 745f 6173 7365  .....z%best_asse
-00004870: 7473 2e3c 6c6f 6361 6c73 3e2e 6361 6c63  ts.<locals>.calc
-00004880: 756c 6172 5f72 6574 6f72 6e6f 6301 0000  ular_retornoc...
-00004890: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-000048a0: 0053 0000 0073 1400 0000 7c00 a000 a100  .S...s....|.....
-000048b0: 7d01 7c01 a001 a100 7d02 7c02 5300 72c4  }.|.....}.|.S.r.
-000048c0: 0000 0029 0272 6e00 0000 7275 0000 0029  ...).rn...ru...)
-000048d0: 0372 c500 0000 72c6 0000 0072 9a00 0000  .r....r....r....
-000048e0: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
-000048f0: 0e63 616c 6375 6c61 725f 7269 7363 6f25  .calcular_risco%
-00004900: 0300 0073 0600 0000 0001 0801 0801 7a23  ...s..........z#
-00004910: 6265 7374 5f61 7373 6574 732e 3c6c 6f63  best_assets.<loc
-00004920: 616c 733e 2e63 616c 6375 6c61 725f 7269  als>.calcular_ri
-00004930: 7363 6f5a 0941 6772 6573 7369 766f 672d  scoZ.Agressivog-
-00004940: 431c ebe2 361a 3f67 7b14 ae47 e17a 843f  C...6.?g{..G.z.?
-00004950: 7a12 4174 6976 6f73 2050 2f41 6772 6573  z.Ativos P/Agres
-00004960: 7369 766f a901 da07 636f 6c75 6d6e 737a  sivo....columnsz
-00004970: 3f52 6561 6c69 7a61 6e64 6f20 6361 6c63  ?Realizando calc
-00004980: 756c 6f73 2070 6172 6120 6120 7375 6120  ulos para a sua 
-00004990: 6361 7274 6569 7261 2063 6f6d 2062 6173  carteira com bas
-000049a0: 6520 6e6f 2073 6575 2070 6572 6669 6c2e  e no seu perfil.
-000049b0: 2902 7289 0000 0072 6100 0000 728c 0000  ).r....ra...r...
-000049c0: 0072 8a00 0000 728b 0000 005a 084d 6f64  .r....r....Z.Mod
-000049d0: 6572 6164 6f67 6132 5530 2aa9 333f 67b8  eradoga2U0*.3?g.
-000049e0: 1e85 eb51 b89e 3f7a 1141 7469 766f 7320  ...Q..?z.Ativos 
-000049f0: 502f 4d6f 6465 7261 646f 5a0b 436f 6e73  P/ModeradoZ.Cons
-00004a00: 6572 7661 646f 727a 1441 7469 766f 7320  ervadorz.Ativos 
-00004a10: 502f 436f 6e73 6572 7661 646f 7275 5a00  P/ConservadoruZ.
-00004a20: 0000 5065 7266 696c 206e c3a3 6f20 7265  ..Perfil n..o re
-00004a30: 636f 6e68 6563 6964 6f2c 206f 7320 7065  conhecido, os pe
-00004a40: 7266 6973 2064 6973 706f 6e69 7665 6973  rfis disponiveis
-00004a50: 2065 7374 616f 2070 7265 7365 6e74 6573   estao presentes
-00004a60: 206e 6120 6578 706c 6963 61c3 a7c3 a36f   na explica....o
-00004a70: 2064 6120 6675 6ec3 a7c3 a36f 4e29 1872   da fun....oN).r
-00004a80: ad00 0000 72ae 0000 005a 0b73 7461 7475  ....r....Z.statu
-00004a90: 735f 636f 6465 722f 0000 0072 0a00 0000  s_coder/...r....
-00004aa0: 72af 0000 0072 b000 0000 7243 0000 0072  r....r....rC...r
-00004ab0: b100 0000 7282 0000 0072 b200 0000 722a  ....r....r....r*
-00004ac0: 0000 0072 6600 0000 da06 746f 6c69 7374  ...rf.....tolist
-00004ad0: 72ca 0000 0072 9800 0000 7244 0000 0072  r....r....rD...r
-00004ae0: 9c00 0000 da04 6f6e 6559 da09 6375 7272  ......oneY..curr
-00004af0: 656e 746c 795a 0765 7870 6c6f 6465 72bd  entlyZ.exploder.
-00004b00: 0000 0072 8d00 0000 7241 0000 0029 195a  ...r....rA...).Z
-00004b10: 0670 6572 6669 6c72 b400 0000 72b5 0000  .perfilr....r...
-00004b20: 0072 b600 0000 729f 0000 0072 b700 0000  .r....r....r....
-00004b30: 72c5 0000 0072 c700 0000 72c8 0000 0072  r....r....r....r
-00004b40: c600 0000 729a 0000 00da 0561 7469 766f  ....r......ativo
-00004b50: 5a0c 7072 6563 6f73 5f61 7469 766f 5a09  Z.precos_ativoZ.
-00004b60: 6167 7265 7373 6976 6f5a 0b44 6641 6772  agressivoZ.DfAgr
-00004b70: 6573 7369 766f 5a13 616c 6f63 6174 696f  essivoZ.alocatio
-00004b80: 6e5f 4167 7265 7373 6976 655a 1764 6174  n_AgressiveZ.dat
-00004b90: 6141 6c6f 6361 7469 6f6e 5f41 6772 6573  aAlocation_Agres
-00004ba0: 7369 7665 5a08 6d6f 6465 7261 646f 5a0a  siveZ.moderadoZ.
-00004bb0: 4466 4d6f 6465 7261 646f 5a12 616c 6f63  DfModeradoZ.aloc
-00004bc0: 6174 696f 6e5f 4d6f 6465 7261 6465 5a16  ation_ModeradeZ.
-00004bd0: 6461 7461 416c 6f63 6174 696f 6e5f 4d6f  dataAlocation_Mo
-00004be0: 6465 7261 6465 5a0b 636f 6e73 6572 7661  deradeZ.conserva
-00004bf0: 646f 725a 0d44 6643 6f6e 7365 7276 6164  dorZ.DfConservad
-00004c00: 6f72 5a16 616c 6f63 6174 696f 6e5f 436f  orZ.alocation_Co
-00004c10: 6e73 6572 7661 7469 7665 5a1a 6461 7461  nservativeZ.data
-00004c20: 416c 6f63 6174 696f 6e5f 436f 6e73 6572  Alocation_Conser
-00004c30: 7661 7469 7665 721f 0000 0072 1f00 0000  vativer....r....
-00004c40: 7220 0000 00da 0b62 6573 745f 6173 7365  r .....best_asse
-00004c50: 7473 f402 0000 7386 0000 0000 1e04 010a  ts....s.........
-00004c60: 010a 010c 020c 010e 0118 0116 0108 011a  ................
-00004c70: 0308 0608 0604 0104 010a 0108 010c 010e  ................
-00004c80: 030a 0104 010a 0118 010c 0210 0108 010e  ................
-00004c90: 0106 010a 010a 0414 0114 0208 0102 0208  ................
-00004ca0: 020a 0204 010a 011c 010e 0210 0108 010e  ................
-00004cb0: 0106 010a 010a 0414 0114 0208 0102 0206  ................
-00004cc0: 020a 0204 010a 010e 010e 0110 0208 010e  ................
-00004cd0: 0106 010a 010a 0314 0114 0208 0102 0206  ................
-00004ce0: 0272 cf00 0000 7a11 2f62 6573 7441 7373  .r....z./bestAss
-00004cf0: 6574 7356 616c 7565 7363 0100 0000 0000  etsValuesc......
-00004d00: 0000 0000 0000 1100 0000 0600 0000 0300  ................
-00004d10: 0000 7344 0200 0074 00a0 01a1 0001 0074  ..sD...t.......t
-00004d20: 0283 007d 017c 01a0 0364 01a1 0101 0074  ...}.|...d.....t
-00004d30: 046a 057c 0164 028d 017d 0264 037d 037c  .j.|.d...}.d.}.|
-00004d40: 02a0 067c 03a1 0101 0074 07a0 0864 04a1  ...|.....t...d..
-00004d50: 0101 007c 02a0 0974 0a6a 0b64 05a1 02a0  ...|...t.j.d....
-00004d60: 0ca1 007d 047c 026a 0da0 0e7c 02a0 0974  ...}.|.j...|...t
-00004d70: 0a6a 0f64 06a1 02a1 0101 007c 02a0 0974  .j.d.......|...t
-00004d80: 0a6a 0f64 07a1 02a0 0ca1 007d 057c 02a0  .j.d.......}.|..
-00004d90: 0974 0a6a 1064 08a1 02a0 0ca1 007d 0674  .t.j.d.......}.t
-00004da0: 07a0 0864 09a1 0101 007c 02a0 0974 0a6a  ...d.....|...t.j
-00004db0: 1064 0aa1 027d 077c 07a0 1164 0ba1 017d  .d...}.|...d...}
-00004dc0: 0874 126a 1374 147c 0883 0164 0c64 0d64  .t.j.t.|...d.d.d
-00004dd0: 0e8d 037d 097c 0964 0f19 007d 097c 0964  ...}.|.d...}.|.d
-00004de0: 1064 1167 0219 007d 097c 09a0 1564 1264  .d.g...}.|...d.d
-00004df0: 1367 02a1 017d 097c 0964 1019 00a0 1664  .g...}.|.d.....d
-00004e00: 1464 1584 00a1 017c 0964 103c 0074 176a  .d.....|.d.<.t.j
-00004e10: 187c 0964 1019 00a0 19a1 0064 1664 178d  .|.d.......d.d..
-00004e20: 0264 1819 007d 0a7c 0a6a 1a64 1964 1a8d  .d...}.|.j.d.d..
-00004e30: 017d 0a7c 0aa0 1ba1 00a0 1ca1 0064 1b14  .}.|.........d..
-00004e40: 0089 007c 0aa0 1ba1 00a0 1da1 0074 1ea0  ...|.........t..
-00004e50: 1f64 1ba1 0114 007d 0b74 12a0 2088 007c  .d.....}.t.. ..|
-00004e60: 0b64 1c9c 02a1 017d 0c7c 0c64 1d19 007c  .d.....}.|.d...|
-00004e70: 0c64 1e19 001b 007c 0c64 1f3c 007c 0c6a  .d.....|.d.<.|.j
-00004e80: 2164 1f64 2064 218d 02a0 2264 22a1 017d  !d.d d!..."d"..}
-00004e90: 0c7c 0c64 1f19 007c 0c64 1f19 00a0 23a1  .|.d...|.d....#.
-00004ea0: 001b 007c 0c64 233c 007c 0c64 2319 0088  ...|.d#<.|.d#...
-00004eb0: 0114 007c 0c64 243c 007c 0ca0 24a1 007d  ...|.d$<.|..$..}
-00004ec0: 0c7c 0c6a 2564 2564 2664 279c 0264 288d  .|.j%d%d&d'..d(.
-00004ed0: 017d 0c7c 0c64 2519 0044 005d 427d 0d74  .}.|.d%..D.]B}.t
-00004ee0: 176a 187c 0d64 1664 178d 027d 0e7c 0e64  .j.|.d.d...}.|.d
-00004ef0: 1819 006a 2664 2919 007c 0e64 1819 006a  ...j&d)..|.d...j
-00004f00: 2664 0f19 0018 007c 0e64 1819 006a 2664  &d.....|.d...j&d
-00004f10: 0f19 001b 0088 007c 0d3c 0090 0171 c487  .......|.<...q..
-00004f20: 0087 0166 0264 2a64 2b84 087c 0c64 2519  ...f.d*d+..|.d%.
-00004f30: 0044 0083 017d 0f7c 0fa0 27a1 007d 1074  .D...}.|..'..}.t
-00004f40: 287c 1083 017d 107c 107c 0c64 2c3c 007c  (|...}.|.|.d,<.|
-00004f50: 0c67 0064 2da2 0119 0053 0029 2e75 1a02  .g.d-....S.).u..
-00004f60: 0000 0a20 2020 2023 2320 5573 6162 696c  ...    ## Usabil
-00004f70: 6964 6164 650a 2020 2020 2d20 4675 6ec3  idade.    - Fun.
-00004f80: a7c3 a36f 2071 7565 2061 6e61 6c69 7361  ...o que analisa
-00004f90: 206f 7320 6174 6976 6f73 2064 6f20 4942   os ativos do IB
-00004fa0: 4f56 4553 5041 2071 7565 2063 6f6d 2062  OVESPA que com b
-00004fb0: 6173 6520 6e6f 2076 616c 6f72 2064 6520  ase no valor de 
-00004fc0: 696e 7665 7374 696d 656e 746f 2065 7363  investimento esc
-00004fd0: 6f6c 6869 646f 206d 6f73 7472 6120 7175  olhido mostra qu
-00004fe0: 6169 7320 706f 6465 6d20 7365 7220 7375  ais podem ser su
-00004ff0: 6173 2065 7363 6f6c 6861 732c 206f 2071  as escolhas, o q
-00005000: 7561 6e74 6f20 6972 6120 7465 7220 7175  uanto ira ter qu
-00005010: 6520 696e 7665 7374 6972 2070 6172 6120  e investir para 
-00005020: 6361 6461 2061 7469 766f 2065 206f 2072  cada ativo e o r
-00005030: 6574 6f72 6e6f 2061 7072 6f78 696d 6164  etorno aproximad
-00005040: 6f20 7061 7261 2063 6164 6120 756d 2064  o para cada um d
-00005050: 656c 6573 200a 0a20 2020 202d 2055 7361  eles ..    - Usa
-00005060: 6d6f 7320 636f 6d6f 206d 6574 6f64 6f20  mos como metodo 
-00005070: 6465 2063 c3a1 6c63 756c 6f20 6f20 6120  de c..lculo o a 
-00005080: 6d65 6469 6461 2053 6861 7270 6520 7175  medida Sharpe qu
-00005090: 6520 6e61 6461 206d 6169 7320 c3a9 2071  e nada mais .. q
-000050a0: 7565 2075 6d61 2020 6d65 6469 6461 2064  ue uma  medida d
-000050b0: 6520 6465 7365 6d70 656e 686f 2064 6520  e desempenho de 
-000050c0: 696e 7665 7374 696d 656e 746f 7320 7175  investimentos qu
-000050d0: 6520 6c65 7661 2065 6d20 636f 6e73 6964  e leva em consid
-000050e0: 6572 61c3 a7c3 a36f 206f 2072 6574 6f72  era....o o retor
-000050f0: 6e6f 206f 6274 6964 6f20 7065 6c6f 2069  no obtido pelo i
-00005100: 6e76 6573 7469 6d65 6e74 6f20 656d 2072  nvestimento em r
-00005110: 656c 61c3 a7c3 a36f 2061 6f20 7269 7363  ela....o ao risc
-00005120: 6f20 6173 7375 6d69 646f 0a20 2020 2023  o assumido.    #
-00005130: 2320 5061 72c3 a26d 6574 726f 730a 2020  # Par..metros.  
-00005140: 2020 0a20 2020 202d 2076 616c 6f72 202d    .    - valor -
-00005150: 3e20 5661 6c6f 7220 646f 2069 6e76 6573  > Valor do inves
-00005160: 7469 6d65 6e74 6f2c 2070 6f72 2070 6164  timento, por pad
-00005170: 72c3 a36f 2030 0a0a 2020 2020 fa0a 2d2d  r..o 0..    ..--
-00005180: 6865 6164 6c65 7373 a901 da07 6f70 7469  headless....opti
-00005190: 6f6e 737a 7c68 7474 7073 3a2f 2f77 7777  onsz|https://www
-000051a0: 2e62 332e 636f 6d2e 6272 2f70 745f 6272  .b3.com.br/pt_br
-000051b0: 2f6d 6172 6b65 742d 6461 7461 2d65 2d69  /market-data-e-i
-000051c0: 6e64 6963 6573 2f69 6e64 6963 6573 2f69  ndices/indices/i
-000051d0: 6e64 6963 6573 2d61 6d70 6c6f 732f 696e  ndices-amplos/in
-000051e0: 6469 6365 2d69 626f 7665 7370 612d 6962  dice-ibovespa-ib
-000051f0: 6f76 6573 7061 2d63 6f6d 706f 7369 6361  ovespa-composica
-00005200: 6f2d 6461 2d63 6172 7465 6972 612e 6874  o-da-carteira.ht
-00005210: 6d72 7400 0000 7a1b 6f6e 6574 7275 7374  mrt...z.onetrust
-00005220: 2d61 6363 6570 742d 6274 6e2d 6861 6e64  -accept-btn-hand
-00005230: 6c65 727a 162f 2f2a 5b40 6964 3d22 6276  lerz.//*[@id="bv
-00005240: 6d66 5f69 6672 616d 6522 5d7a 152f 2f2a  mf_iframe"]z.//*
-00005250: 5b40 6964 3d22 7365 6c65 6374 5061 6765  [@id="selectPage
-00005260: 225d 7a21 2373 656c 6563 7450 6167 6520  "]z!#selectPage 
-00005270: 3e20 6f70 7469 6f6e 3a6e 7468 2d63 6869  > option:nth-chi
-00005280: 6c64 2834 29e7 0000 0000 0000 f83f 7a6c  ld(4)........?zl
-00005290: 2364 6976 436f 6e74 6169 6e65 7249 6672  #divContainerIfr
-000052a0: 616d 6542 3320 3e20 6469 7620 3e20 6469  ameB3 > div > di
-000052b0: 762e 636f 6c2d 6c67 2d39 2e63 6f6c 2d31  v.col-lg-9.col-1
-000052c0: 322e 6f72 6465 722d 322e 6f72 6465 722d  2.order-2.order-
-000052d0: 6c67 2d31 203e 2066 6f72 6d20 3e20 6469  lg-1 > form > di
-000052e0: 763a 6e74 682d 6368 696c 6428 3429 203e  v:nth-child(4) >
-000052f0: 2064 6976 203e 2074 6162 6c65 da09 6f75   div > table..ou
-00005300: 7465 7248 544d 4c72 c000 0000 721a 0000  terHTMLr....r...
-00005310: 0072 c100 0000 7201 0000 0072 c300 0000  .r....r....r....
-00005320: 7506 0000 0041 c3a7 c3a3 6fe9 5800 0000  u....A....o.X...
-00005330: e959 0000 0063 0100 0000 0000 0000 0000  .Y...c..........
-00005340: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
-00005350: 0000 007c 0064 0117 0053 0072 a100 0000  ...|.d...S.r....
-00005360: 721f 0000 0072 a300 0000 721f 0000 0072  r....r....r....r
-00005370: 1f00 0000 7220 0000 0072 a500 0000 a303  ....r ...r......
-00005380: 0000 72a6 0000 007a 2362 6573 745f 6173  ..r....z#best_as
-00005390: 7365 7473 5f76 616c 7565 2e3c 6c6f 6361  sets_value.<loca
-000053a0: 6c73 3e2e 3c6c 616d 6264 613e 723a 0000  ls>.<lambda>r:..
-000053b0: 0072 3c00 0000 7248 0000 0072 1600 0000  .r<...rH...r....
-000053c0: a901 5a04 6178 6973 7265 0000 0029 0272  ..Z.axisre...).r
-000053d0: 9900 0000 729a 0000 0072 9900 0000 729a  ....r....r....r.
-000053e0: 0000 005a 0673 6861 7270 6546 2901 5a09  ...Z.sharpeF).Z.
-000053f0: 6173 6365 6e64 696e 67e9 0600 0000 5a08  ascending.....Z.
-00005400: 616c 6f63 6163 616f da05 7661 6c6f 72da  alocacao..valor.
-00005410: 0641 7469 766f 73fa 1351 7464 204e 6563  .Ativos..Qtd Nec
-00005420: 6573 7361 7269 6120 2852 2429 2902 7280  essaria (R$)).r.
-00005430: 0000 0072 d900 0000 72c9 0000 0072 2600  ...r....r....r&.
-00005440: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00005450: 0000 0005 0000 0013 0000 0073 1a00 0000  ...........s....
-00005460: 6900 7c00 5d12 7d01 7c01 8800 7c01 1900  i.|.].}.|...|...
-00005470: 8801 1400 9302 7104 5300 721f 0000 0072  ......q.S.r....r
-00005480: 1f00 0000 2902 da02 2e30 72ce 0000 00a9  ....)....0r.....
-00005490: 0272 9900 0000 72d9 0000 0072 1f00 0000  .r....r....r....
-000054a0: 7220 0000 00da 0a3c 6469 6374 636f 6d70  r .....<dictcomp
-000054b0: 3ec6 0300 0072 a600 0000 7a25 6265 7374  >....r....z%best
-000054c0: 5f61 7373 6574 735f 7661 6c75 652e 3c6c  _assets_value.<l
-000054d0: 6f63 616c 733e 2e3c 6469 6374 636f 6d70  ocals>.<dictcomp
-000054e0: 3efa 0e52 6574 6f72 6e6f 2041 7072 6f78  >..Retorno Aprox
-000054f0: 2e29 0372 da00 0000 72db 0000 0072 df00  .).r....r....r..
-00005500: 0000 2929 da1a 6368 726f 6d65 6472 6976  ..))..chromedriv
-00005510: 6572 5f61 7574 6f69 6e73 7461 6c6c 6572  er_autoinstaller
-00005520: da07 696e 7374 616c 6c72 0800 0000 da0c  ..installr......
-00005530: 6164 645f 6172 6775 6d65 6e74 7206 0000  add_argumentr...
-00005540: 00da 0643 6872 6f6d 6572 ae00 0000 da04  ...Chromer......
-00005550: 7469 6d65 da05 736c 6565 70da 0c66 696e  time..sleep..fin
-00005560: 645f 656c 656d 656e 7472 0900 0000 da02  d_elementr......
-00005570: 4944 da05 636c 6963 6b5a 0973 7769 7463  ID..clickZ.switc
-00005580: 685f 746f da05 6672 616d 655a 0558 5041  h_to..frameZ.XPA
-00005590: 5448 da0c 4353 535f 5345 4c45 4354 4f52  TH..CSS_SELECTOR
-000055a0: da0d 6765 745f 6174 7472 6962 7574 6572  ..get_attributer
-000055b0: 4300 0000 72b1 0000 0072 8200 0000 723f  C...r....r....r?
-000055c0: 0000 0072 b200 0000 722a 0000 0072 6600  ...r....r*...rf.
-000055d0: 0000 72cb 0000 0072 8d00 0000 726e 0000  ..r....r....rn..
-000055e0: 0072 5800 0000 7275 0000 0072 6700 0000  .rX...ru...rg...
-000055f0: 726a 0000 0072 4400 0000 5a0b 736f 7274  rj...rD...Z.sort
-00005600: 5f76 616c 7565 73da 0468 6561 6472 3100  _values..headr1.
-00005610: 0000 7246 0000 00da 0672 656e 616d 6572  ..rF.....renamer
-00005620: 3000 0000 da06 7661 6c75 6573 723e 0000  0.....valuesr>..
-00005630: 0029 1172 d900 0000 da0e 6368 726f 6d65  .).r......chrome
-00005640: 5f6f 7074 696f 6e73 da06 6472 6976 6572  _options..driver
-00005650: 72b4 0000 005a 0763 6f6f 6b69 6573 da06  r....Z.cookies..
-00005660: 7365 6c65 6374 da03 616c 6c72 9f00 0000  select..allr....
-00005670: da0a 7461 626c 655f 6874 6d6c 5a06 6174  ..table_htmlZ.at
-00005680: 6976 6f73 72c5 0000 0072 9a00 0000 5a09  ivosr....r....Z.
-00005690: 6174 6976 6f73 5f64 6672 ce00 0000 7286  ativos_dfr....r.
-000056a0: 0000 005a 1172 6574 6f72 6e6f 5f70 6f72  ...Z.retorno_por
-000056b0: 5f61 7469 766f 5a0c 4c69 7374 6152 6574  _ativoZ.ListaRet
-000056c0: 6f72 6e6f 721f 0000 0072 dd00 0000 7220  ornor....r....r 
-000056d0: 0000 00da 1162 6573 745f 6173 7365 7473  .....best_assets
-000056e0: 5f76 616c 7565 8003 0000 734c 0000 0000  _value....sL....
-000056f0: 0e08 0106 010a 010c 0204 010a 010a 0112  ................
-00005700: 0116 0112 0112 010a 020e 010a 0114 0108  ................
-00005710: 010c 010e 0216 031a 030c 0310 0116 0310  ................
-00005720: 0314 0314 0318 0310 0108 0212 020c 010e  ................
-00005730: 0132 0318 0108 0108 0208 0372 f400 0000  .2.........r....
-00005740: 7a16 2f6f 7074 696f 6e73 2f7b 7379 6d62  z./options/{symb
-00005750: 6f6c 7d2f 696e 666f 2904 7222 0000 00da  ol}/info).r"....
-00005760: 0463 616c 6cda 0370 7574 7223 0000 0063  .call..putr#...c
-00005770: 0300 0000 0000 0000 0000 0000 0b00 0000  ................
-00005780: 0500 0000 4300 0000 737a 0100 007c 00a0  ....C...sz...|..
-00005790: 0064 01a1 0172 187c 00a0 0164 0164 02a1  .d...r.|...d.d..
-000057a0: 027d 006e 0874 0264 0383 0101 0074 03a0  .}.n.t.d.....t..
-000057b0: 04a1 0001 0074 0583 007d 037c 03a0 0664  .....t...}.|...d
-000057c0: 04a1 0101 0074 076a 087c 0364 058d 017d  .....t.j.|.d...}
-000057d0: 0464 067c 009b 009d 027d 057c 04a0 097c  .d.|.....}.|...|
-000057e0: 05a1 0101 0074 0aa0 0b64 07a1 0101 007c  .....t...d.....|
-000057f0: 04a0 0c74 0d6a 0e64 08a1 027d 067c 06a0  ...t.j.d...}.|..
-00005800: 0f64 09a1 017d 0774 106a 1174 127c 0783  .d...}.t.j.t.|..
-00005810: 0164 0a64 0b64 0c8d 037d 087c 0864 0d19  .d.d.d...}.|.d..
-00005820: 007d 087c 0867 0064 0ea2 0119 007d 087c  .}.|.g.d.....}.|
-00005830: 0164 0f6b 0272 c07c 086a 137c 0864 1019  .d.k.r.|.j.|.d..
-00005840: 0064 116b 0219 007d 097c 0953 007c 0264  .d.k...}.|.S.|.d
-00005850: 0f6b 0272 de7c 086a 137c 0864 1019 0064  .k.r.|.j.|.d...d
-00005860: 126b 0219 007d 0a7c 0a53 007c 04a0 097c  .k...}.|.S.|...|
-00005870: 05a1 0101 0074 0aa0 0b64 07a1 0101 007c  .....t...d.....|
-00005880: 04a0 0c74 0d6a 0e64 08a1 027d 067c 06a0  ...t.j.d...}.|..
-00005890: 0f64 09a1 017d 0774 106a 1174 127c 0783  .d...}.t.j.t.|..
-000058a0: 0164 0a64 0b64 0c8d 037d 087c 0864 0d19  .d.d.d...}.|.d..
-000058b0: 007d 087c 0867 0064 0ea2 0119 007d 087c  .}.|.g.d.....}.|
-000058c0: 0164 0f6b 0290 0172 527c 086a 137c 0864  .d.k...rR|.j.|.d
-000058d0: 1019 0064 116b 0219 007d 097c 0953 007c  ...d.k...}.|.S.|
-000058e0: 0264 0f6b 0290 0172 727c 086a 137c 0864  .d.k...rr|.j.|.d
-000058f0: 1019 0064 126b 0219 007d 0a7c 0a53 007c  ...d.k...}.|.S.|
-00005900: 0853 0064 1353 0029 1475 c801 0000 0a20  .S.d.S.).u..... 
-00005910: 2020 2023 2320 5573 6162 696c 6964 6164     ## Usabilidad
-00005920: 650a 0a20 2020 202d 2046 756e c3a7 c3a3  e..    - Fun....
-00005930: 6f20 7175 6520 6170 7265 7365 6e74 6120  o que apresenta 
-00005940: 6173 2070 7269 6e63 6970 6169 7320 696e  as principais in
-00005950: 666f 726d 61c3 a7c3 b565 7320 6461 7320  forma....es das 
-00005960: 6f70 c3a7 c3b5 6573 2064 6f20 6174 6976  op....es do ativ
-00005970: 6f20 7365 6c65 6369 6f6e 6164 6f2c 2069  o selecionado, i
-00005980: 6e66 6f72 6d61 c3a7 c3b5 6573 2063 6f6d  nforma....es com
-00005990: 6f3a 2053 7472 696b 652c 2056 6172 2c20  o: Strike, Var, 
-000059a0: 4772 6567 6173 2c20 6465 6e74 7265 206f  Gregas, dentre o
-000059b0: 7574 7261 732e 0a0a 2020 2020 2323 2050  utras...    ## P
-000059c0: 6172 c3a2 6d65 7472 6f73 0a0a 2020 2020  ar..metros..    
-000059d0: 2d20 7379 6d62 6f6c 202d 3e20 4e6f 6d65  - symbol -> Nome
-000059e0: 2064 6f20 6174 6976 6f20 7061 7261 2062   do ativo para b
-000059f0: 7573 6361 7220 6173 206f 70c3 a7c3 b565  uscar as op....e
-00005a00: 7320 7265 6665 7265 6e74 6573 2061 2065  s referentes a e
-00005a10: 6c65 2e0a 2020 2020 2d20 6361 6c6c 202d  le..    - call -
-00005a20: 3e20 5265 6365 6265 2054 7275 6520 6f75  > Recebe True ou
-00005a30: 2046 616c 7365 2c20 7365 2054 7275 6520   False, se True 
-00005a40: 666f 7220 7365 6c65 6369 6f6e 6164 6f20  for selecionado 
-00005a50: 6120 6675 6ec3 a7c3 a36f 2069 7261 2066  a fun....o ira f
-00005a60: 696c 7472 6172 2073 6f20 6173 2043 414c  iltrar so as CAL
-00005a70: 4c2e 0a20 2020 202d 2070 7574 202d 3e20  L..    - put -> 
-00005a80: 5265 6365 6265 2054 7275 6520 6f75 2046  Recebe True ou F
-00005a90: 616c 7365 2c20 7365 2054 7275 6520 666f  alse, se True fo
-00005aa0: 7220 7365 6c65 6369 6f6e 6164 6f20 6120  r selecionado a 
-00005ab0: 6675 6ec3 a7c3 a36f 2069 7261 2066 696c  fun....o ira fil
-00005ac0: 7472 6172 2073 6f20 6173 2050 5554 2e0a  trar so as PUT..
-00005ad0: 0a0a 2020 2020 72a2 0000 0072 1800 0000  ..    r....r....
-00005ae0: f534 0000 0050 726f 6375 7261 6e64 6f20  .4...Procurando 
-00005af0: 6461 646f 7320 6465 206f 70c3 a7c3 b565  dados de op....e
-00005b00: 7320 646f 2061 7469 766f 2073 656c 6563  s do ativo selec
-00005b10: 696f 6e61 646f 2e2e 2e72 d000 0000 72d1  ionado...r....r.
-00005b20: 0000 007a 2568 7474 7073 3a2f 2f6f 7063  ...z%https://opc
-00005b30: 6f65 732e 6e65 742e 6272 2f6f 7063 6f65  oes.net.br/opcoe
-00005b40: 732f 626f 7665 7370 612f 72d3 0000 007a  s/bovespa/r....z
-00005b50: 0c23 7462 6c4c 6973 7461 4f70 6372 d400  .#tblListaOpcr..
-00005b60: 0000 72c0 0000 0072 1a00 0000 72c1 0000  ..r....r....r...
-00005b70: 0072 0100 0000 290d 722b 0000 00da 0454  .r....).r+.....T
-00005b80: 6970 6f5a 0653 7472 696b 657a 0741 2f49  ipoZ.Strikez.A/I
-00005b90: 2f4f 544d 7a13 4469 7374 2e20 2825 2920  /OTMz.Dist. (%) 
-00005ba0: 646f 2053 7472 696b 6575 0700 0000 c39a  do Strikeu......
-00005bb0: 6c74 696d 6f7a 0856 6172 2e20 2825 2975  ltimoz.Var. (%)u
-00005bc0: 0d00 0000 4ec3 ba6d 2e20 6465 204e 6567  ....N..m. de Neg
-00005bd0: 2e7a 0f56 6f6c 2e20 4669 6e61 6e63 6569  .z.Vol. Financei
-00005be0: 726f da05 4465 6c74 61da 0547 616d 6d61  ro..Delta..Gamma
-00005bf0: 7a09 5468 6574 6120 2824 295a 0456 6567  z.Theta ($)Z.Veg
-00005c00: 6154 72f8 0000 00da 0443 414c 4cda 0350  aTr......CALL..P
-00005c10: 5554 4e29 14da 0865 6e64 7377 6974 6872  UTN)...endswithr
-00005c20: 1b00 0000 722f 0000 0072 e000 0000 72e1  ....r/...r....r.
-00005c30: 0000 0072 0800 0000 72e2 0000 0072 0600  ...r....r....r..
-00005c40: 0000 72e3 0000 0072 ae00 0000 72e4 0000  ..r....r....r...
-00005c50: 0072 e500 0000 72e6 0000 0072 0900 0000  .r....r....r....
-00005c60: 72ea 0000 0072 eb00 0000 7243 0000 0072  r....r....rC...r
-00005c70: b100 0000 7282 0000 0072 b300 0000 290b  ....r....r....).
-00005c80: 7222 0000 0072 f500 0000 72f6 0000 0072  r"...r....r....r
-00005c90: ef00 0000 72f0 0000 0072 b400 0000 729f  ....r....r....r.
-00005ca0: 0000 0072 f300 0000 5a05 6466 4f50 435a  ...r....Z.dfOPCZ
-00005cb0: 0664 6643 616c 6c5a 0564 6650 7574 721f  .dfCallZ.dfPutr.
-00005cc0: 0000 0072 1f00 0000 7220 0000 00da 0767  ...r....r .....g
-00005cd0: 6574 5f6f 7063 d603 0000 7346 0000 0000  et_opc....sF....
-00005ce0: 110a 010e 0208 0208 0106 010a 010c 020a  ................
-00005cf0: 010a 010a 010e 010a 0114 0108 010c 0108  ................
-00005d00: 0112 0104 0108 0112 0104 020a 010a 020e  ................
-00005d10: 010a 0114 0108 040c 010a 0112 0104 010a  ................
-00005d20: 0112 0104 0272 fe00 0000 7a15 2f6f 7074  .....r....z./opt
-00005d30: 696f 6e73 2f62 6c61 636b 5363 686f 6c65  ions/blackSchole
-00005d40: 7329 0272 f500 0000 72f6 0000 0063 0500  s).r....r....c..
-00005d50: 0000 0000 0000 0000 0000 0c00 0000 0600  ................
-00005d60: 0000 4300 0000 73e8 0000 0074 007c 0174  ..C...s....t.|.t
-00005d70: 0174 0283 037d 057c 0564 0114 007d 0664  .t...}.|.d...}.d
-00005d80: 027d 0774 03a0 047c 027c 031b 00a1 017c  .}.t...|.|.....|
-00005d90: 077c 0664 0313 0064 031b 007c 0414 0017  .|.d...d...|....
-00005da0: 007c 0674 03a0 057c 04a1 0114 0014 0017  .|.t...|........
-00005db0: 007d 087c 0674 03a0 057c 04a1 0114 0004  .}.|.t...|......
-00005dc0: 007d 097d 087c 0064 046b 0272 9a74 0664  .}.}.|.d.k.r.t.d
-00005dd0: 0583 0101 007c 0274 07a0 087c 08a1 0114  .....|.t...|....
-00005de0: 007c 0374 03a0 097c 070b 007c 0414 00a1  .|.t...|...|....
-00005df0: 0114 0074 07a0 087c 09a1 0114 0018 007d  ...t...|.......}
-00005e00: 0a7c 0a53 007c 0064 066b 0272 dc74 0664  .|.S.|.d.k.r.t.d
-00005e10: 0783 0101 007c 0374 03a0 097c 070b 007c  .....|.t...|...|
-00005e20: 0414 00a1 0114 0074 07a0 087c 09a1 0114  .......t...|....
-00005e30: 007c 0274 07a0 087c 080b 00a1 0114 0018  .|.t...|........
-00005e40: 007d 0b7c 0b53 0074 0664 0883 0101 0064  .}.|.S.t.d.....d
-00005e50: 0953 0029 0a75 4a03 0000 0a20 2020 2023  .S.).uJ....    #
-00005e60: 2320 5573 6162 696c 6964 6164 650a 0a20  # Usabilidade.. 
-00005e70: 2020 202d 2046 756e c3a7 c3a3 6f20 7175     - Fun....o qu
-00005e80: 6520 7369 6d75 6c61 206f 2063 6163 756c  e simula o cacul
-00005e90: 6f20 646f 2062 6c61 636b 2d73 6368 6f6c  o do black-schol
-00005ea0: 6573 2c20 6d6f 6465 6c6f 206e 6f20 7175  es, modelo no qu
-00005eb0: 616c 20c3 a920 7574 696c 697a 6164 6f20  al .. utilizado 
-00005ec0: 7061 7261 2070 7265 6369 6669 6361 7220  para precificar 
-00005ed0: 6f70 c3a7 c3b5 6573 206e 6f20 6d65 7263  op....es no merc
-00005ee0: 6164 6f20 6465 2064 6572 6976 6174 6976  ado de derivativ
-00005ef0: 6f73 2e0a 2020 2020 2d20 506f 7220 7365  os..    - Por se
-00005f00: 2074 7261 7461 7220 6465 2075 6d61 2066   tratar de uma f
-00005f10: 756e c3a7 c3a3 6f20 656d 2064 6573 656e  un....o em desen
-00005f20: 766f 6c76 696d 656e 746f 206e c3a3 6f20  volvimento n..o 
-00005f30: 6c65 7661 7220 6f20 7265 7375 6c74 6164  levar o resultad
-00005f40: 6f20 636f 6d6f 2076 6572 6461 6465 2061  o como verdade a
-00005f50: 6273 6f6c 7574 612c 206d 6173 2075 6d20  bsoluta, mas um 
-00005f60: 7661 6c6f 7220 6120 7365 2062 6173 6561  valor a se basea
-00005f70: 722e 0a0a 2020 2020 2323 2050 6172 c3a2  r...    ## Par..
-00005f80: 6d65 7472 6f73 0a0a 2020 2020 2d20 4361  metros..    - Ca
-00005f90: 6c6c 5f6f 725f 5075 7420 2d3e 2052 6563  ll_or_Put -> Rec
-00005fa0: 6562 6520 6f73 2076 616c 6f72 6573 2022  ebe os valores "
-00005fb0: 6361 6c6c 2220 6520 2270 7574 222c 2070  call" e "put", p
-00005fc0: 6f72 2073 6572 656d 2063 616c 6375 6c6f  or serem calculo
-00005fd0: 7320 6469 6665 7265 6e74 6573 2070 6172  s diferentes par
-00005fe0: 6164 6120 6361 6461 2074 6970 6f2c 20c3  ada cada tipo, .
-00005ff0: a920 6e65 6365 7373 6172 696f 2061 2073  . necessario a s
-00006000: 656c 65c3 a7c3 a36f 0a20 2020 202d 2061  ele....o.    - a
-00006010: 7469 766f 202d 3e20 496e 7365 7269 7220  tivo -> Inserir 
-00006020: 6f20 6174 6976 6f20 636f 7272 6573 706f  o ativo correspo
-00006030: 6e64 656e 7465 2064 6120 6675 6ec3 a7c3  ndente da fun...
-00006040: a36f 2028 4578 656d 706c 6f3a 2027 5045  .o (Exemplo: 'PE
-00006050: 5452 342e 5341 2729 0a20 2020 202d 2070  TR4.SA').    - p
-00006060: 7265 636f 202d 3e20 696e 7365 7269 7220  reco -> inserir 
-00006070: 6f20 7072 65c3 a76f 2064 6f20 6174 6976  o pre..o do ativ
-00006080: 6f20 7365 6c65 6369 6f6e 6164 6f0a 2020  o selecionado.  
-00006090: 2020 2d20 7374 7269 6b65 202d 3e20 496e    - strike -> In
-000060a0: 7365 7269 7220 6f20 7374 7269 6b65 2064  serir o strike d
-000060b0: 6120 6f70 c3a7 c3a3 6f0a 2020 2020 2d20  a op....o.    - 
-000060c0: 6469 6173 5574 6569 7320 2d3e 2041 6469  diasUteis -> Adi
-000060d0: 6369 6f6e 6172 2061 2071 7561 6e74 6964  cionar a quantid
-000060e0: 6164 6520 6465 2064 6961 7320 c3ba 7465  ade de dias ..te
-000060f0: 6973 2061 7465 206f 2076 656e 6369 6d65  is ate o vencime
-00006100: 6e74 6f20 6461 206f 70c3 a7c3 a36f 2e0a  nto da op....o..
-00006110: 0a20 2020 2023 2320 4578 656d 706c 6f0a  .    ## Exemplo.
-00006120: 0a20 2020 2060 6060 0a20 2020 203e 3e3e  .    ```.    >>>
-00006130: 2062 622e 626c 6163 6b5f 7363 686f 6c65   bb.black_schole
-00006140: 7328 4361 6c6c 5f6f 725f 5075 743d 2027  s(Call_or_Put= '
-00006150: 6361 6c6c 272c 2061 7469 766f 3d20 2750  call', ativo= 'P
-00006160: 4554 5234 2e53 4127 2c20 7072 6563 6f3d  ETR4.SA', preco=
-00006170: 2032 362e 3235 2c20 7374 7269 6b65 3d20   26.25, strike= 
-00006180: 3236 2e32 352c 2064 6961 7355 7465 6973  26.25, diasUteis
-00006190: 3d20 3232 2029 0a20 2020 2060 6060 0a0a  = 22 ).    ```..
-000061a0: 2020 2020 6910 f800 0067 c1a8 a44e 40d3      i....g...N@.
-000061b0: 1540 7274 0000 0072 f500 0000 7a10 5365  .@rt...r....z.Se
-000061c0: 6c65 6369 6f6e 6164 6f20 4361 6c6c 72f6  lecionado Callr.
-000061d0: 0000 007a 0f53 656c 6563 696f 6e61 646f  ...z.Selecionado
-000061e0: 2050 7574 7530 0000 0041 7320 6f70 c3a7   Putu0...As op..
-000061f0: c3b5 6573 2076 616c 6964 6173 2073 616f  ..es validas sao
-00006200: 2073 6f6d 656e 7465 2061 7320 6465 2043   somente as de C
-00006210: 414c 4c20 6520 5055 544e 290a 726c 0000  ALL e PUTN).rl..
-00006220: 00da 0673 6576 656e 4472 cd00 0000 7267  ...sevenDr....rg
-00006230: 0000 0072 6800 0000 726a 0000 0072 2f00  ...rh...rj...r/.
-00006240: 0000 7202 0000 005a 0363 6466 da03 6578  ..r....Z.cdf..ex
-00006250: 7029 0c5a 0b43 616c 6c5f 6f72 5f50 7574  p).Z.Call_or_Put
-00006260: 72ce 0000 005a 0570 7265 636f da06 7374  r....Z.preco..st
-00006270: 7269 6b65 5a09 6469 6173 5574 6569 735a  rikeZ.diasUteisZ
-00006280: 0d76 6f6c 6174 696c 6964 6164 6544 5a0c  .volatilidadeDZ.
-00006290: 766f 6c61 7469 6c69 6461 6465 5a06 7461  volatilidadeZ.ta
-000062a0: 7861 4c52 da02 6431 da02 6432 da01 43da  xaLR..d1..d2..C.
-000062b0: 0150 721f 0000 0072 1f00 0000 7220 0000  .Pr....r....r ..
-000062c0: 00da 0d62 6c61 636b 5f73 6368 6f6c 6573  ...black_scholes
-000062d0: 1904 0000 731c 0000 0000 190c 0108 0104  ....s...........
-000062e0: 0230 0112 0208 0108 012c 0104 0108 0108  .0.......,......
-000062f0: 012e 0104 0272 0601 0000 6301 0000 0000  .....r....c.....
-00006300: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
-00006310: 0000 0073 2e00 0000 7400 a001 6401 a101  ...s....t...d...
-00006320: 7d01 7c01 a002 a100 7d02 6402 7d03 7403  }.|.....}.d.}.t.
-00006330: a004 7c03 7c01 a102 7d04 7c01 a005 a100  ..|.|...}.|.....
-00006340: 0100 6400 5300 2903 4e7a 3e51 3a5c 5269  ..d.S.).Nz>Q:\Ri
-00006350: 7363 6f5c 4e6f 766f 2052 6973 636f 5c70  sco\Novo Risco\p
-00006360: 7974 686f 6e72 6973 636f 5c42 4246 696e  ythonrisco\BBFin
-00006370: 616e 6365 5c42 616e 636f 5c44 6174 6143  ance\Banco\DataC
-00006380: 6c69 656e 7473 2e64 627a 1753 454c 4543  lients.dbz.SELEC
-00006390: 5420 2a20 4652 4f4d 2043 6172 7465 6972  T * FROM Carteir
-000063a0: 6173 2906 da07 7371 6c69 7465 33da 0763  as)...sqlite3..c
-000063b0: 6f6e 6e65 6374 da06 6375 7273 6f72 7243  onnect..cursorrC
-000063c0: 0000 005a 0e72 6561 645f 7371 6c5f 7175  ...Z.read_sql_qu
-000063d0: 6572 7972 8700 0000 2905 7285 0000 005a  eryr....).r....Z
-000063e0: 0763 6f6e 6578 616f 7209 0100 005a 0863  .conexaor....Z.c
-000063f0: 6f6e 7375 6c74 6172 1e00 0000 721f 0000  onsultar....r...
-00006400: 0072 1f00 0000 7220 0000 00da 0863 6172  .r....r .....car
-00006410: 7465 6972 614a 0400 0073 0a00 0000 0001  teiraJ...s......
-00006420: 0a01 0801 0402 0c01 720a 0100 0063 0100  ........r....c..
-00006430: 0000 0000 0000 0000 0000 0800 0000 0600  ................
-00006440: 0000 4300 0000 73e4 0000 007c 00a0 0064  ..C...s....|...d
-00006450: 01a1 0173 147c 0064 0117 007d 006e 0874  ...s.|.d...}.n.t
-00006460: 0164 0283 0101 0074 026a 037c 0064 0364  .d.....t.j.|.d.d
-00006470: 048d 027d 0174 0483 007d 0274 056a 067c  ...}.t...}.t.j.|
-00006480: 02a0 077c 01a1 017c 016a 0864 058d 027d  ...|...|.j.d...}
-00006490: 0174 0974 0a7c 0183 0164 0614 0083 017d  .t.t.|...d.....}
-000064a0: 037c 016a 0b64 007c 0385 0219 007d 047c  .|.j.d.|.....}.|
-000064b0: 016a 0b7c 0364 0085 0219 007d 0574 0c6a  .j.|.d.....}.t.j
-000064c0: 0da0 0e74 0c6a 0d6a 0f6a 1064 0764 0864  ...t.j.j.j.d.d.d
-000064d0: 098d 0274 0c6a 0d6a 0fa0 1064 0aa1 0167  ...t.j.j...d...g
-000064e0: 02a1 017d 067c 066a 1164 0b64 0c64 0d8d  ...}.|.j.d.d.d..
-000064f0: 0201 007c 066a 127c 046a 1364 0e67 0164  ...|.j.|.j.d.g.d
-00006500: 0a64 0f8d 027c 0464 0e19 0064 1064 1164  .d...|.d...d.d.d
-00006510: 128d 0401 007c 06a0 147c 056a 1364 0e67  .....|...|.j.d.g
-00006520: 0164 0a64 0f8d 02a1 017d 077c 0753 0029  .d.d.....}.|.S.)
-00006530: 134e 72a2 0000 0072 f700 0000 5a02 3764  .Nr....r....Z.7d
-00006540: 723c 0000 0072 c900 0000 679a 9999 9999  r<...r....g.....
-00006550: 99e9 3fe9 4000 0000 5a04 7265 6c75 2901  ..?.@...Z.relu).
-00006560: 5a0a 6163 7469 7661 7469 6f6e 7216 0000  Z.activationr...
-00006570: 005a 0461 6461 6d5a 126d 6561 6e5f 7371  .Z.adamZ.mean_sq
-00006580: 7561 7265 645f 6572 726f 7229 025a 096f  uared_error).Z.o
-00006590: 7074 696d 697a 6572 725c 0000 0072 4800  ptimizerr\...rH.
-000065a0: 0000 72d7 0000 0072 4f00 0000 e920 0000  ..r....rO.... ..
-000065b0: 0029 025a 0665 706f 6368 735a 0a62 6174  .).Z.epochsZ.bat
-000065c0: 6368 5f73 697a 6529 1572 fd00 0000 722f  ch_size).r....r/
-000065d0: 0000 0072 2a00 0000 7266 0000 0072 0500  ...r*...rf...r..
-000065e0: 0000 7243 0000 0072 4400 0000 5a0d 6669  ..rC...rD...Z.fi
-000065f0: 745f 7472 616e 7366 6f72 6d72 ca00 0000  t_transformr....
-00006600: da03 696e 7472 8300 0000 7230 0000 00da  ..intr....r0....
-00006610: 0274 665a 056b 6572 6173 5a0a 5365 7175  .tfZ.kerasZ.Sequ
-00006620: 656e 7469 616c 5a06 6c61 7965 7273 5a05  entialZ.layersZ.
-00006630: 4465 6e73 65da 0763 6f6d 7069 6c65 5a03  Dense..compileZ.
-00006640: 6669 7472 3f00 0000 5a07 7072 6564 6963  fitr?...Z.predic
-00006650: 7429 0872 2200 0000 721e 0000 005a 0673  t).r"...r....Z.s
-00006660: 6361 6c65 725a 0a74 7261 696e 5f73 697a  calerZ.train_siz
-00006670: 655a 0a74 7261 696e 5f64 6174 615a 0974  eZ.train_dataZ.t
-00006680: 6573 745f 6461 7461 da05 6d6f 6465 6c5a  est_data..modelZ
-00006690: 0b70 7265 6469 6374 696f 6e73 721f 0000  .predictionsr...
-000066a0: 0072 1f00 0000 7220 0000 00da 1370 7265  .r....r .....pre
-000066b0: 6469 6374 5f73 746f 636b 5f74 7265 6e64  dict_stock_trend
-000066c0: 5404 0000 7322 0000 0000 020a 010a 0208  T...s"..........
-000066d0: 050e 0306 0116 0310 010e 010e 0306 0110  ................
-000066e0: 010c fe06 040e 0322 0316 0272 1101 0000  ......."...r....
-000066f0: 2901 723a 0000 0029 0172 0100 0000 295a  ).r:...).r....)Z
-00006700: 5a08 7966 696e 616e 6365 722a 0000 005a  Z.yfinancer*...Z
-00006710: 0b73 6369 7079 2e73 7461 7473 7202 0000  .scipy.statsr...
-00006720: 005a 0e73 6369 7079 2e6f 7074 696d 697a  .Z.scipy.optimiz
-00006730: 6572 0300 0000 5a14 736b 6c65 6172 6e2e  er....Z.sklearn.
-00006740: 6c69 6e65 6172 5f6d 6f64 656c 7204 0000  linear_modelr...
-00006750: 00da 0a74 656e 736f 7266 6c6f 7772 0e01  ...tensorflowr..
-00006760: 0000 5a15 736b 6c65 6172 6e2e 7072 6570  ..Z.sklearn.prep
-00006770: 726f 6365 7373 696e 6772 0500 0000 5a08  rocessingr....Z.
-00006780: 7365 6c65 6e69 756d 7206 0000 005a 1e73  seleniumr....Z.s
-00006790: 656c 656e 6975 6d2e 7765 6264 7269 7665  elenium.webdrive
-000067a0: 722e 636f 6d6d 6f6e 2e6b 6579 7372 0700  r.common.keysr..
-000067b0: 0000 5a21 7365 6c65 6e69 756d 2e77 6562  ..Z!selenium.web
-000067c0: 6472 6976 6572 2e63 6872 6f6d 652e 6f70  driver.chrome.op
-000067d0: 7469 6f6e 7372 0800 0000 5a1c 7365 6c65  tionsr....Z.sele
-000067e0: 6e69 756d 2e77 6562 6472 6976 6572 2e63  nium.webdriver.c
-000067f0: 6f6d 6d6f 6e2e 6279 7209 0000 0072 e000  ommon.byr....r..
-00006800: 0000 72ad 0000 005a 0362 7334 720a 0000  ..r....Z.bs4r...
-00006810: 0072 e400 0000 5a07 6661 7374 6170 6972  .r....Z.fastapir
-00006820: 0b00 0000 720c 0000 0072 0d00 0000 5a11  ....r....r....Z.
-00006830: 6661 7374 6170 692e 7265 7370 6f6e 7365  fastapi.response
-00006840: 7372 0e00 0000 5a13 6661 7374 6170 692e  sr....Z.fastapi.
-00006850: 7374 6174 6963 6669 6c65 7372 0f00 0000  staticfilesr....
-00006860: 5a12 6661 7374 6170 692e 7465 6d70 6c61  Z.fastapi.templa
-00006870: 7469 6e67 7210 0000 00da 046a 736f 6e5a  tingr......jsonZ
-00006880: 0775 7669 636f 726e da06 7061 6e64 6173  .uvicorn..pandas
-00006890: 7243 0000 00da 056e 756d 7079 7267 0000  rC.....numpyrg..
-000068a0: 0072 1100 0000 7212 0000 00da 0674 7970  .r....r......typ
-000068b0: 696e 6772 1300 0000 7207 0100 00da 0877  ingr....r......w
-000068c0: 6172 6e69 6e67 73da 0e66 696c 7465 7277  arnings..filterw
-000068d0: 6172 6e69 6e67 735a 0c70 6472 5f6f 7665  arningsZ.pdr_ove
-000068e0: 7272 6964 65da 0574 6f64 6179 5a0c 6f6e  rride..todayZ.on
-000068f0: 655f 7965 6172 5f61 676f 5a0c 6f6e 655f  e_year_agoZ.one_
-00006900: 6461 7973 5f61 676f 5a0e 7365 7665 6e5f  days_agoZ.seven_
-00006910: 6461 7973 5f61 676f da08 7374 7266 7469  days_ago..strfti
-00006920: 6d65 72cc 0000 005a 046f 6e65 4472 ff00  mer....Z.oneDr..
-00006930: 0000 72cd 0000 00da 0361 7070 7221 0000  ..r......appr!..
-00006940: 0072 ae00 0000 7282 0000 0072 2e00 0000  .r....r....r....
-00006950: 7235 0000 00da 085f 5f6e 616d 655f 5fda  r5.....__name__.
-00006960: 0372 756e 72b5 0000 0072 4400 0000 7247  .runr....rD...rG
-00006970: 0000 005a 0f72 6573 706f 6e73 6548 6973  ...Z.responseHis
-00006980: 746f 7279 724d 0000 0072 5f00 0000 726c  toryrM...r_...rl
-00006990: 0000 0072 7000 0000 721d 0000 0072 0d01  ...rp...r....r..
-000069a0: 0000 7278 0000 0072 3e00 0000 7288 0000  ..rx...r>...r...
-000069b0: 0072 9c00 0000 72b9 0000 0072 bc00 0000  .r....r....r....
-000069c0: 72bf 0000 0072 cf00 0000 72f4 0000 00da  r....r....r.....
-000069d0: 0462 6f6f 6c72 fe00 0000 7206 0100 0072  .boolr....r....r
-000069e0: 0a01 0000 7211 0100 0072 1f00 0000 721f  ....r....r....r.
-000069f0: 0000 0072 1f00 0000 7220 0000 00da 083c  ...r....r .....<
-00006a00: 6d6f 6475 6c65 3e02 0000 0073 f000 0000  module>....s....
-00006a10: 0801 0c01 0c01 0c01 0801 0c04 0c01 0c01  ................
-00006a20: 0c01 0c01 0801 0801 0c01 0803 1401 0c01  ................
-00006a30: 0c01 0c01 0801 0803 0801 0801 1001 0c01  ................
-00006a40: 0803 0801 0a02 0802 0802 0e01 0e01 0e03  ................
-00006a50: 0a01 0a01 0a02 0a02 060c 0809 0c01 1226  ...............&
-00006a60: 0a01 1201 0a05 0c01 1826 0a01 1201 0a05  .........&......
-00006a70: 0c01 1220 0a01 1201 0a05 0c01 123a 0a01  ... .........:..
-00006a80: 1201 0a05 0c01 1618 0a01 1201 0a05 0c01  ................
-00006a90: 1232 0a01 1201 0a05 0c01 1623 0a01 1201  .2.........#....
-00006aa0: 0a05 0c01 2062 0a01 1201 0a05 0801 163a  .... b.........:
-00006ab0: 0a01 1201 0a05 0c01 1418 0a01 1201 0a05  ................
-00006ac0: 0c01 1642 0a01 1201 0a05 0c01 1a40 0a01  ...B.........@..
-00006ad0: 1201 0a05 0c01 167f 0007 0a01 1201 0a03  ................
-00006ae0: 0c01 1e4e 0a01 1201 0a05 0c01 1a3d 0a01  ...N.........=..
-00006af0: 1201 0a03 0c01 202a 0a01 1201 0a04 0c0a  ...... *........
+00000a40: 2020 0a20 2020 20fa 0f54 6963 6b65 7220    .    ..Ticker 
+00000a50: 496e 7661 6c69 646f 5a11 7265 6775 6c61  InvalidoZ.regula
+00000a60: 724d 6172 6b65 744f 7065 6e5a 086c 6f6e  rMarketOpenZ.lon
+00000a70: 674e 616d 65e9 ffff ffff 4e29 0472 2200  gName.....N).r".
+00000a80: 0000 da0d 6375 7272 656e 745f 7072 6963  ....current_pric
+00000a90: 65da 0c63 6f6d 7061 6e79 5f6e 616d 65da  e..company_name.
+00000aa0: 0964 6976 6964 656e 6473 2909 da02 7966  .dividends)...yf
+00000ab0: da06 5469 636b 6572 da04 696e 666f da04  ..Ticker..info..
+00000ac0: 7479 7065 da04 6469 6374 da05 7072 696e  type..dict..prin
+00000ad0: 7472 2800 0000 da04 696c 6f63 da03 7375  tr(.....iloc..su
+00000ae0: 6d29 0872 2200 0000 da05 7374 6f63 6b72  m).r".....stockr
+00000af0: 2b00 0000 da08 7469 706f 496e 666f 7226  +.....tipoInfor&
+00000b00: 0000 0072 2700 0000 5a08 6469 7669 6465  ...r'...Z.divide
+00000b10: 6e64 da09 6a73 6f6e 5f64 6174 6172 1f00  nd..json_datar..
+00000b20: 0000 721f 0000 0072 2000 0000 da08 6765  ..r....r .....ge
+00000b30: 745f 696e 666f 4b00 0000 7320 0000 0000  t_infoK...s ....
+00000b40: 110a 0106 0108 0108 0102 0208 020a 030a  ................
+00000b50: 0306 0112 0302 0102 0102 0102 fd06 0772  ...............r
+00000b60: 3400 0000 da08 5f5f 6d61 696e 5f5f 7a08  4.....__main__z.
+00000b70: 6d61 696e 3a61 7070 7a09 3132 372e 302e  main:appz.127.0.
+00000b80: 302e 3169 401f 0000 7a14 7374 6f63 6b73  0.1i@...z.stocks
+00000b90: 2f7b 7379 6d62 6f6c 7d2f 696e 666f 2903  /{symbol}/info).
+00000ba0: da04 686f 7374 da04 706f 7274 da07 6465  ..host..port..de
+00000bb0: 6661 756c 747a 1061 7070 6c69 6361 7469  faultz.applicati
+00000bc0: 6f6e 2f6a 736f 6e29 015a 0a6d 6564 6961  on/json).Z.media
+00000bd0: 5f74 7970 657a 182f 7374 6f63 6b73 2f7b  _typez./stocks/{
+00000be0: 7379 6d62 6f6c 7d2f 6869 7374 6f72 79da  symbol}/history.
+00000bf0: 0231 7929 0372 2200 0000 da06 7065 7269  .1y).r".....peri
+00000c00: 6f64 7223 0000 0063 0200 0000 0000 0000  odr#...c........
+00000c10: 0000 0000 0800 0000 0300 0000 4300 0000  ............C...
+00000c20: 7370 0000 0074 00a0 017c 00a1 017d 027c  sp...t...|...}.|
+00000c30: 026a 027d 0374 037c 0383 017d 047c 0474  .j.}.t.|...}.|.t
+00000c40: 046b 0272 226e 0874 0564 0183 0101 007c  .k.r"n.t.d.....|
+00000c50: 026a 067c 0164 028d 017d 057c 056a 0772  .j.|.d...}.|.j.r
+00000c60: 4864 0374 0564 0483 0169 0153 007c 056a  Hd.t.d...i.S.|.j
+00000c70: 0864 0564 068d 017d 0674 096a 0aa0 0b7c  .d.d...}.t.j...|
+00000c80: 06a1 016a 0c64 0764 088d 017d 077c 0753  ...j.d.d...}.|.S
+00000c90: 0064 0953 0029 0a75 ff00 0000 0a20 2020  .d.S.).u.....   
+00000ca0: 2023 2320 5573 6162 696c 6964 6164 6520   ## Usabilidade 
+00000cb0: 0a20 2020 202d 2055 7361 6461 2070 6172  .    - Usada par
+00000cc0: 6120 7665 7269 6669 6361 7220 6f20 6869  a verificar o hi
+00000cd0: 7374 c3b3 7269 636f 2064 6120 61c3 a761  st..rico da a..a
+00000ce0: 6f20 7365 6c65 6369 6f6e 6164 6120 6520  o selecionada e 
+00000cf0: 656d 2071 7561 6c20 7065 7269 6f64 6f20  em qual periodo 
+00000d00: 0a0a 2020 2020 0a20 2020 2023 2320 5061  ..    .    ## Pa
+00000d10: 72c3 a26d 6574 726f 730a 2020 2020 0a20  r..metros.    . 
+00000d20: 2020 202d 2073 796d 626f 6c20 2d3e 204e     - symbol -> N
+00000d30: 6f6d 6520 646f 2041 7469 766f 2070 6172  ome do Ativo par
+00000d40: 6120 6120 6275 7363 6120 0a0a 2020 2020  a a busca ..    
+00000d50: 2d20 7065 7269 6f64 202d 3e20 4461 7461  - period -> Data
+00000d60: 2065 6d20 414e 4f53 2070 6172 6120 6120   em ANOS para a 
+00000d70: 6275 7363 6120 6461 7320 696e 666f 726d  busca das inform
+00000d80: 61c3 a76f 6573 2064 6f20 4174 6976 6f20  a..oes do Ativo 
+00000d90: 0a0a 2020 2020 0a20 2020 2072 2400 0000  ..    .    r$...
+00000da0: a901 723a 0000 00da 0565 7272 6f72 7a0d  ..r:.....errorz.
+00000db0: 4e6f 2064 6174 6120 666f 756e 64da 046c  No data found..l
+00000dc0: 6973 7429 015a 066f 7269 656e 7446 2901  ist).Z.orientF).
+00000dd0: da04 6472 6f70 4e29 0d72 2900 0000 722a  ..dropN).r)...r*
+00000de0: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
+00000df0: 0000 722e 0000 00da 0768 6973 746f 7279  ..r......history
+00000e00: da05 656d 7074 79da 0774 6f5f 6469 6374  ..empty..to_dict
+00000e10: da02 7064 da09 4461 7461 4672 616d 65da  ..pd..DataFrame.
+00000e20: 0966 726f 6d5f 6469 6374 da0b 7265 7365  .from_dict..rese
+00000e30: 745f 696e 6465 7829 0872 2200 0000 723a  t_index).r"...r:
+00000e40: 0000 0072 3100 0000 722b 0000 0072 3200  ...r1...r+...r2.
+00000e50: 0000 723f 0000 005a 0c68 6973 746f 7279  ..r?...Z.history
+00000e60: 5f64 6963 745a 0a68 6973 746f 7279 5f64  _dictZ.history_d
+00000e70: 6672 1f00 0000 721f 0000 0072 2000 0000  fr....r....r ...
+00000e80: da11 6765 745f 7374 6f63 6b5f 6869 7374  ..get_stock_hist
+00000e90: 6f72 797e 0000 0073 1800 0000 000e 0a01  ory~...s........
+00000ea0: 0601 0801 0801 0202 0802 0c02 0601 0c02  ................
+00000eb0: 0c01 1402 7246 0000 007a 1773 746f 636b  ....rF...z.stock
+00000ec0: 732f 7b73 796d 626f 6c7d 2f68 6973 746f  s/{symbol}/histo
+00000ed0: 7279 7a15 2f73 746f 636b 2f7b 7379 6d62  ryz./stock/{symb
+00000ee0: 6f6c 7d2f 7472 656e 6463 0100 0000 0000  ol}/trendc......
+00000ef0: 0000 0000 0000 0800 0000 0300 0000 4300  ..............C.
+00000f00: 0000 7368 0000 0074 00a0 017c 00a1 017d  ..sh...t...|...}
+00000f10: 017c 016a 027d 0274 037c 0283 017d 037c  .|.j.}.t.|...}.|
+00000f20: 0374 046b 0272 226e 0874 0564 0183 0101  .t.k.r"n.t.d....
+00000f30: 007c 016a 0664 0264 038d 017d 047c 0464  .|.j.d.d...}.|.d
+00000f40: 0419 007d 057c 056a 0764 0519 007c 056a  ...}.|.j.d...|.j
+00000f50: 0764 0619 006b 0472 5664 076e 0264 087d  .d...k.rVd.n.d.}
+00000f60: 067c 007c 0664 099c 027d 077c 0753 0029  .|.|.d...}.|.S.)
+00000f70: 0a75 b900 0000 0a20 2020 2023 2320 5573  .u.....    ## Us
+00000f80: 6162 696c 6964 6164 6520 0a20 2020 202d  abilidade .    -
+00000f90: 2049 6465 6e74 6966 6963 6120 6120 7465   Identifica a te
+00000fa0: 6e64 656e 6369 6120 6465 2070 7265 c3a7  ndencia de pre..
+00000fb0: 6f20 6465 2075 6d61 2061 c3a7 616f 2c20  o de uma a..ao, 
+00000fc0: 7365 2069 7261 2073 6572 2064 6520 414c  se ira ser de AL
+00000fd0: 5441 206f 7520 4241 4958 410a 2020 2020  TA ou BAIXA.    
+00000fe0: 0a20 2020 2023 2320 5061 72c3 a26d 6574  .    ## Par..met
+00000ff0: 726f 730a 2020 2020 0a20 2020 202d 2073  ros.    .    - s
+00001000: 796d 626f 6c20 2d3e 204e 6f6d 6520 646f  ymbol -> Nome do
+00001010: 2041 7469 766f 2070 6172 6120 6120 6275   Ativo para a bu
+00001020: 7363 6120 0a0a 2020 2020 0a20 2020 2072  sca ..    .    r
+00001030: 2400 0000 5a02 3164 723b 0000 00da 0543  $...Z.1dr;.....C
+00001040: 6c6f 7365 7225 0000 0072 0100 0000 da02  loser%...r......
+00001050: 7570 da04 646f 776e 2902 7222 0000 00da  up..down).r"....
+00001060: 0574 7265 6e64 2908 7229 0000 0072 2a00  .trend).r)...r*.
+00001070: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+00001080: 0072 2e00 0000 723f 0000 0072 2f00 0000  .r....r?...r/...
+00001090: 2908 7222 0000 0072 3100 0000 722b 0000  ).r"...r1...r+..
+000010a0: 0072 3200 0000 723f 0000 00da 0c63 6c6f  .r2...r?.....clo
+000010b0: 7365 5f70 7269 6365 7372 4a00 0000 7233  se_pricesrJ...r3
+000010c0: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+000010d0: 0000 da0f 6765 745f 7374 6f63 6b5f 7472  ....get_stock_tr
+000010e0: 656e 64ac 0000 0073 1a00 0000 000d 0a01  end....s........
+000010f0: 0601 0801 0801 0202 0802 0c01 0801 1c02  ................
+00001100: 0201 02ff 0606 724c 0000 007a 1573 746f  ......rL...z.sto
+00001110: 636b 732f 7b73 796d 626f 6c7d 2f74 7265  cks/{symbol}/tre
+00001120: 6e64 7a19 2f73 746f 636b 2f7b 7379 6d62  ndz./stock/{symb
+00001130: 6f6c 7d2f 7465 6368 6e69 6361 6c63 0100  ol}/technicalc..
+00001140: 0000 0000 0000 0000 0000 1100 0000 0600  ................
+00001150: 0000 4300 0000 73f8 0000 0074 00a0 017c  ..C...s....t...|
+00001160: 00a1 017d 017c 016a 027d 0274 037c 0283  ...}.|.j.}.t.|..
+00001170: 017d 037c 0374 046b 0272 226e 0874 0564  .}.|.t.k.r"n.t.d
+00001180: 0183 0101 007c 016a 0664 0264 038d 017d  .....|.j.d.d...}
+00001190: 047c 0464 0419 007d 057c 056a 0764 0564  .|.d...}.|.j.d.d
+000011a0: 068d 01a0 08a1 006a 0964 0719 007d 067c  .......j.d...}.|
+000011b0: 056a 0764 0864 068d 01a0 08a1 006a 0964  .j.d.d.......j.d
+000011c0: 0719 007d 077c 05a0 0aa1 007d 087c 08a0  ...}.|.....}.|..
+000011d0: 0b7c 0864 096b 0464 09a1 027d 097c 08a0  .|.d.k.d...}.|..
+000011e0: 0b7c 0864 096b 0064 09a1 020b 007d 0a7c  .|.d.k.d.....}.|
+000011f0: 096a 0764 0a64 068d 01a0 08a1 007d 0b7c  .j.d.d.......}.|
+00001200: 0a6a 0764 0a64 068d 01a0 08a1 007d 0c7c  .j.d.d.......}.|
+00001210: 0b7c 0c1b 007d 0d64 0b64 0b64 0c7c 0d17  .|...}.d.d.d.|..
+00001220: 001b 006a 0964 0719 0018 007d 0e7c 0e64  ...j.d.....}.|.d
+00001230: 0d6b 0572 e064 0e7d 0f6e 0464 0f7d 0f7c  .k.r.d.}.n.d.}.|
+00001240: 007c 067c 077c 0e7c 0f64 109c 057d 107c  .|.|.|.|.d...}.|
+00001250: 1053 0029 1175 7902 0000 0a20 2020 2023  .S.).uy....    #
+00001260: 2320 5573 6162 696c 6964 6164 6520 0a20  # Usabilidade . 
+00001270: 2020 202d 2063 c3a1 6c63 756c 6f20 656e     - c..lculo en
+00001280: 766f 6c76 6520 6120 636f 6d70 6172 61c3  volve a compara.
+00001290: a7c3 a36f 2064 6120 6dc3 a964 6961 2064  ...o da m..dia d
+000012a0: 6520 6761 6e68 6f73 2065 6d20 756d 2070  e ganhos em um p
+000012b0: 6572 c3ad 6f64 6f20 6465 2074 656d 706f  er..odo de tempo
+000012c0: 2063 6f6d 2061 206d c3a9 6469 6120 6465   com a m..dia de
+000012d0: 2070 6572 6461 7320 656d 2075 6d20 7065   perdas em um pe
+000012e0: 72c3 ad6f 646f 2064 6520 7465 6d70 6f2e  r..odo de tempo.
+000012f0: 200a 0a20 2020 200a 2020 2020 2323 2043   ..    .    ## C
+00001300: 6f6d 6f20 696e 7465 7270 7265 7461 7220  omo interpretar 
+00001310: 0a20 2020 202d 2051 7561 6e64 6f20 6f20  .    - Quando o 
+00001320: 5253 4920 6573 74c3 a120 6163 696d 6120  RSI est.. acima 
+00001330: 6465 2037 302c 206f 2061 7469 766f 20c3  de 70, o ativo .
+00001340: a920 636f 6e73 6964 6572 6164 6f20 736f  . considerado so
+00001350: 6272 6563 6f6d 7072 6164 6f2c 206f 2071  brecomprado, o q
+00001360: 7565 2073 6967 6e69 6669 6361 2071 7565  ue significa que
+00001370: 2070 6f64 6520 6573 7461 7220 7072 6573   pode estar pres
+00001380: 7465 7320 6120 736f 6672 6572 2075 6d61  tes a sofrer uma
+00001390: 2063 6f72 7265 c3a7 c3a3 6f20 7061 7261   corre....o para
+000013a0: 2062 6169 786f 2e20 0a20 2020 2051 7561   baixo. .    Qua
+000013b0: 6e64 6f20 6f20 5253 4920 6573 74c3 a120  ndo o RSI est.. 
+000013c0: 6162 6169 786f 2064 6520 3330 2c20 6f20  abaixo de 30, o 
+000013d0: 6174 6976 6f20 c3a9 2063 6f6e 7369 6465  ativo .. conside
+000013e0: 7261 646f 2073 6f62 7265 7665 6e64 6964  rado sobrevendid
+000013f0: 6f2c 206f 2071 7565 2073 6967 6e69 6669  o, o que signifi
+00001400: 6361 2071 7565 2070 6f64 6520 6573 7461  ca que pode esta
+00001410: 7220 7072 6573 7465 7320 6120 7375 6269  r prestes a subi
+00001420: 7220 6e6f 7661 6d65 6e74 652e 200a 200a  r novamente. . .
+00001430: 2020 2020 2d20 736d 615f 3530 202d 3e20      - sma_50 -> 
+00001440: 4d65 6469 6120 6d6f 7665 6c20 646f 7320  Media movel dos 
+00001450: 3530 2070 6572 696f 646f 730a 2020 2020  50 periodos.    
+00001460: 2d20 736d 615f 3230 3020 2d3e 206d 6564  - sma_200 -> med
+00001470: 6961 206d 6f76 656c 2064 6f73 2032 3030  ia movel dos 200
+00001480: 2070 6572 6964 6f73 0a0a 2020 2020 2323   peridos..    ##
+00001490: 2050 6172 c3a2 6d65 7472 6f73 0a20 2020   Par..metros.   
+000014a0: 202d 2073 796d 626f 6c20 2d3e 204e 6f6d   - symbol -> Nom
+000014b0: 6520 646f 2041 7469 766f 2070 6172 6120  e do Ativo para 
+000014c0: 6120 6275 7363 6120 0a0a 2020 2020 0a20  a busca ..    . 
+000014d0: 2020 2072 2400 0000 da03 6d61 7872 3b00     r$.....maxr;.
+000014e0: 0000 7247 0000 00e9 3200 0000 2901 da06  ..rG....2...)...
+000014f0: 7769 6e64 6f77 7225 0000 00e9 c800 0000  windowr%........
+00001500: 7201 0000 00e9 0e00 0000 e964 0000 0072  r..........d...r
+00001510: 1600 0000 e946 0000 007a 1f41 2063 6861  .....F...z.A cha
+00001520: 6e63 6520 646f 2070 7265 636f 2064 6f20  nce do preco do 
+00001530: 6174 6976 6f20 4341 4952 7a20 4120 6368  ativo CAIRz A ch
+00001540: 616e 6365 2064 6f20 7072 6563 6f20 646f  ance do preco do
+00001550: 2061 7469 766f 2053 5542 4952 2905 7222   ativo SUBIR).r"
+00001560: 0000 00da 0673 6d61 5f35 30da 0773 6d61  .....sma_50..sma
+00001570: 5f32 3030 da03 7273 695a 0874 656e 6465  _200..rsiZ.tende
+00001580: 6e63 7929 0c72 2900 0000 722a 0000 0072  ncy).r)...r*...r
+00001590: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
+000015a0: 0000 0072 3f00 0000 5a07 726f 6c6c 696e  ...r?...Z.rollin
+000015b0: 67da 046d 6561 6e72 2f00 0000 da04 6469  g..meanr/.....di
+000015c0: 6666 da05 7768 6572 6529 1172 2200 0000  ff..where).r"...
+000015d0: 7231 0000 0072 2b00 0000 7232 0000 0072  r1...r+...r2...r
+000015e0: 3f00 0000 724b 0000 0072 5400 0000 7255  ?...rK...rT...rU
+000015f0: 0000 00da 0564 656c 7461 5a04 6761 696e  .....deltaZ.gain
+00001600: da04 6c6f 7373 5a08 6176 675f 6761 696e  ..lossZ.avg_gain
+00001610: 5a08 6176 675f 6c6f 7373 da02 7273 7256  Z.avg_loss..rsrV
+00001620: 0000 00da 0673 7461 7475 7372 3300 0000  .....statusr3...
+00001630: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+00001640: 1467 6574 5f73 746f 636b 5f74 6563 686e  .get_stock_techn
+00001650: 6963 616c 73d4 0000 0073 3600 0000 0012  icals....s6.....
+00001660: 0a01 0601 0801 0801 0202 0802 0c01 0803  ................
+00001670: 1601 1603 0801 1001 1201 1001 1001 0801  ................
+00001680: 1602 0801 0602 0403 0201 0201 0201 0201  ................
+00001690: 02fb 060a 725e 0000 007a 1973 746f 636b  ....r^...z.stock
+000016a0: 732f 7b73 796d 626f 6c7d 2f74 6563 686e  s/{symbol}/techn
+000016b0: 6963 616c 7a1a 7374 6f63 6b73 2f7b 7379  icalz.stocks/{sy
+000016c0: 6d62 6f6c 7d2f 766f 6c61 7469 6c69 7479  mbol}/volatility
+000016d0: 2904 7222 0000 00da 0a73 7461 7274 5f64  ).r".....start_d
+000016e0: 6174 65da 0865 6e64 5f64 6174 6572 2300  ate..end_dater#.
+000016f0: 0000 6303 0000 0000 0000 0000 0000 0006  ..c.............
+00001700: 0000 0006 0000 0043 0000 0073 6800 0000  .......C...sh...
+00001710: 7a28 7400 6a01 7c00 7c01 7c02 6401 8d03  z(t.j.|.|.|.d...
+00001720: 7d03 7c03 6a02 7226 6402 7403 6403 8301  }.|.j.r&d.t.d...
+00001730: 6901 5700 5300 5700 6e0c 0100 0100 0100  i.W.S.W.n.......
+00001740: 5900 6e02 3000 7404 a005 7c03 6404 1900  Y.n.0.t...|.d...
+00001750: 7c03 6404 1900 a006 6405 a101 1b00 a101  |.d.....d.......
+00001760: 7d04 7404 a007 6406 7c04 a008 a100 1400  }.t...d.|.......
+00001770: a101 7d05 7c05 5300 2907 756e 0100 000a  ..}.|.S.).un....
+00001780: 2020 2020 2323 2055 7361 6269 6c69 6461      ## Usabilida
+00001790: 6465 200a 2020 2020 2d20 4dc3 a974 6f64  de .    - M..tod
+000017a0: 6f20 7573 6164 6f20 7061 7261 2076 6572  o usado para ver
+000017b0: 6966 6963 6172 2061 2076 6f6c 6174 696c  ificar a volatil
+000017c0: 6964 6164 6520 6465 2075 6d20 6174 6976  idade de um ativ
+000017d0: 6f20 656d 2063 6f6d 7061 7261 6361 6f20  o em comparacao 
+000017e0: 616f 206d 6572 6361 646f 2065 6d20 7175  ao mercado em qu
+000017f0: 6520 6573 7461 2020 0a0a 2020 2020 0a20  e esta  ..    . 
+00001800: 2020 2023 2320 5061 72c3 a26d 6574 726f     ## Par..metro
+00001810: 730a 2020 2020 2d20 7379 6d62 6f6c 202d  s.    - symbol -
+00001820: 3e20 4e6f 6d65 2064 6f20 4174 6976 6f20  > Nome do Ativo 
+00001830: 7061 7261 2061 2062 7573 6361 200a 0a20  para a busca .. 
+00001840: 2020 202d 2073 7461 7274 5f64 6174 6520     - start_date 
+00001850: 2d3e 2044 6174 6120 6465 2049 6e69 6369  -> Data de Inici
+00001860: 6f20 6461 2062 7573 6361 2064 6173 2069  o da busca das i
+00001870: 6e66 6f73 2028 7072 6563 6f2c 2076 6f6c  nfos (preco, vol
+00001880: 756d 652c 2065 7463 2920 646f 2061 7469  ume, etc) do ati
+00001890: 766f 200a 0a20 2020 202d 2065 6e64 5f64  vo ..    - end_d
+000018a0: 6174 6520 2d3e 2044 6174 6120 4669 6e61  ate -> Data Fina
+000018b0: 6c20 7061 7261 2061 2062 7573 6361 2064  l para a busca d
+000018c0: 6173 2069 6e66 6f73 2028 7072 6563 6f2c  as infos (preco,
+000018d0: 2076 6f6c 756d 652c 2065 7463 2920 646f   volume, etc) do
+000018e0: 2061 7469 766f 200a 0a20 2020 20a9 02da   ativo ..    ...
+000018f0: 0573 7461 7274 da03 656e 6472 3c00 0000  .start..endr<...
+00001900: 7a38 4e61 6f20 666f 6920 656e 636f 6e74  z8Nao foi encont
+00001910: 7261 646f 206f 2068 6973 746f 7269 636f  rado o historico
+00001920: 206e 6573 7365 2070 6572 696f 646f 2c20   nesse periodo, 
+00001930: 7665 7269 6669 6361 722e 7247 0000 0072  verificar.rG...r
+00001940: 1600 0000 e9fc 0000 0029 0972 2900 0000  .........).r)...
+00001950: da08 646f 776e 6c6f 6164 7240 0000 0072  ..downloadr@...r
+00001960: 2e00 0000 da02 6e70 da03 6c6f 67da 0573  ......np..log..s
+00001970: 6869 6674 da04 7371 7274 da03 7661 7229  hift..sqrt..var)
+00001980: 0672 2200 0000 725f 0000 0072 6000 0000  .r"...r_...r`...
+00001990: 5a0a 7374 6f63 6b5f 6461 7461 5a0b 6c6f  Z.stock_dataZ.lo
+000019a0: 675f 7265 7475 726e 735a 0a76 6f6c 6174  g_returnsZ.volat
+000019b0: 696c 6974 7972 1f00 0000 721f 0000 0072  ilityr....r....r
+000019c0: 2000 0000 da0e 6765 745f 766f 6c61 7469   .....get_volati
+000019d0: 6c69 7479 1601 0000 7312 0000 0000 0d02  lity....s.......
+000019e0: 0110 0106 0112 0106 0106 021c 0112 0272  ...............r
+000019f0: 6b00 0000 7a14 7374 6f63 6b73 2f7b 7379  k...z.stocks/{sy
+00001a00: 6d62 6f6c 7d2f 6265 7461 6301 0000 0000  mbol}/betac.....
+00001a10: 0000 0000 0000 000f 0000 0003 0000 0043  ...............C
+00001a20: 0000 0073 be00 0000 7400 a001 7c00 a101  ...s....t...|...
+00001a30: 7d01 7400 a001 6401 a101 7d02 7c01 6a02  }.t...d...}.|.j.
+00001a40: 7d03 7c02 6a02 7d04 7403 7c03 8301 7d05  }.|.j.}.t.|...}.
+00001a50: 7c05 7404 6b02 7342 7c04 7404 6b02 723a  |.t.k.sB|.t.k.r:
+00001a60: 6e08 7405 6402 8301 0100 7c01 6a06 6403  n.t.d.....|.j.d.
+00001a70: 6404 8d01 7d06 7c02 6a06 6403 6404 8d01  d...}.|.j.d.d...
+00001a80: 7d07 7c06 6405 1900 a007 a100 7d08 7c07  }.|.d.......}.|.
+00001a90: 6405 1900 a007 a100 7d09 7c08 a008 7c09  d.......}.|...|.
+00001aa0: a101 7d0a 7c09 a009 a100 7d0b 7c0a 7c0b  ..}.|.....}.|.|.
+00001ab0: 1b00 7d0c 7c0c 6406 6b04 7298 6407 7d0d  ..}.|.d.k.r.d.}.
+00001ac0: 7c0c 6406 6b00 72a4 6408 7d0d 7c0c 6406  |.d.k.r.d.}.|.d.
+00001ad0: 6b02 72b0 6409 7d0d 7c0c 7c0d 640a 9c02  k.r.d.}.|.|.d...
+00001ae0: 7d0e 7c0e 5300 290b 7595 0100 000a 2020  }.|.S.).u.....  
+00001af0: 2020 2323 2055 7361 6269 6c69 6461 6465    ## Usabilidade
+00001b00: 200a 2020 2020 2d20 4f20 6265 7461 20c3   .    - O beta .
+00001b10: a920 756d 6120 6d65 6469 6461 2065 7374  . uma medida est
+00001b20: 6174 c3ad 7374 6963 6120 7175 6520 696e  at..stica que in
+00001b30: 6469 6361 2061 2072 656c 61c3 a7c3 a36f  dica a rela....o
+00001b40: 2065 6e74 7265 2061 2076 6f6c 6174 696c   entre a volatil
+00001b50: 6964 6164 6520 6465 2075 6d61 2061 c3a7  idade de uma a..
+00001b60: c3a3 6f20 6520 6120 766f 6c61 7469 6c69  ..o e a volatili
+00001b70: 6461 6465 2064 6f20 6d65 7263 6164 6f20  dade do mercado 
+00001b80: 636f 6d6f 2075 6d20 746f 646f 2e0a 2020  como um todo..  
+00001b90: 2020 4f20 7661 6c6f 7220 646f 2062 6574    O valor do bet
+00001ba0: 6120 c3a9 2075 7469 6c69 7a61 646f 2070  a .. utilizado p
+00001bb0: 6172 6120 6d65 6469 7220 6f20 7269 7363  ara medir o risc
+00001bc0: 6f20 6465 2075 6d61 2061 c3a7 c3a3 6f20  o de uma a....o 
+00001bd0: 656d 2072 656c 61c3 a7c3 a36f 2061 6f20  em rela....o ao 
+00001be0: 6d65 7263 6164 6f20 656d 2071 7565 2065  mercado em que e
+00001bf0: 6c61 20c3 a920 6e65 676f 6369 6164 612e  la .. negociada.
+00001c00: 200a 0a20 2020 200a 2020 2020 2323 2050   ..    .    ## P
+00001c10: 6172 c3a2 6d65 7472 6f73 0a20 2020 202d  ar..metros.    -
+00001c20: 2073 796d 626f 6c20 2d3e 204e 6f6d 6520   symbol -> Nome 
+00001c30: 646f 2041 7469 766f 2070 6172 6120 6120  do Ativo para a 
+00001c40: 6275 7363 6120 0a0a 2020 2020 2d20 6d61  busca ..    - ma
+00001c50: 726b 6574 202d 3e20 436f 6d6f 2070 6164  rket -> Como pad
+00001c60: 7261 6f2c 204d 6572 6361 646f 3a20 4942  rao, Mercado: IB
+00001c70: 4f56 4553 5041 202f 2042 5653 500a 2020  OVESPA / BVSP.  
+00001c80: 2020 7a05 5e42 5653 5072 2400 0000 724d    z.^BVSPr$...rM
+00001c90: 0000 0072 3b00 0000 7247 0000 0072 1600  ...r;...rG...r..
+00001ca0: 0000 7a28 4163 616f 206d 6169 7320 566f  ..z(Acao mais Vo
+00001cb0: 6c61 7469 6c20 7175 6520 6f20 6d65 7263  latil que o merc
+00001cc0: 6164 6f20 656d 2067 6572 616c 7a29 4163  ado em geralz)Ac
+00001cd0: 616f 206d 656e 6f73 2056 6f6c 6174 696c  ao menos Volatil
+00001ce0: 2071 7565 206f 206d 6572 6361 646f 2065   que o mercado e
+00001cf0: 6d20 6765 7261 6c7a 3441 6361 6f20 636f  m geralz4Acao co
+00001d00: 6d20 6120 6d65 736d 6120 566f 6c61 7469  m a mesma Volati
+00001d10: 6c69 6461 6465 2071 7565 206f 206d 6572  lidade que o mer
+00001d20: 6361 646f 2065 6d20 6765 7261 6c29 02da  cado em geral)..
+00001d30: 0462 6574 6172 5d00 0000 290a 7229 0000  .betar]...).r)..
+00001d40: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
+00001d50: 722d 0000 0072 2e00 0000 723f 0000 00da  r-...r....r?....
+00001d60: 0a70 6374 5f63 6861 6e67 65da 0363 6f76  .pct_change..cov
+00001d70: 726a 0000 0029 0f72 2200 0000 5a05 6173  rj...).r"...Z.as
+00001d80: 7365 745a 066d 6172 6b65 7472 2b00 0000  setZ.marketr+...
+00001d90: 5a0a 696e 666f 4d61 726b 6574 7232 0000  Z.infoMarketr2..
+00001da0: 005a 0d61 7373 6574 5f68 6973 746f 7279  .Z.asset_history
+00001db0: 5a0e 6d61 726b 6574 5f68 6973 746f 7279  Z.market_history
+00001dc0: 5a0d 6173 7365 745f 7265 7475 726e 735a  Z.asset_returnsZ
+00001dd0: 0e6d 6172 6b65 745f 7265 7475 726e 7372  .market_returnsr
+00001de0: 6e00 0000 726a 0000 0072 6c00 0000 725d  n...rj...rl...r]
+00001df0: 0000 0072 3300 0000 721f 0000 0072 1f00  ...r3...r....r..
+00001e00: 0000 7220 0000 00da 0867 6574 5f62 6574  ..r .....get_bet
+00001e10: 6136 0100 0073 3200 0000 000e 0a01 0a01  a6...s2.........
+00001e20: 0601 0601 0801 1001 0202 0802 0c01 0c03  ................
+00001e30: 0c01 0c03 0a01 0801 0802 0801 0401 0801  ................
+00001e40: 0401 0801 0403 0201 02ff 0605 726f 0000  ............ro..
+00001e50: 007a 1373 746f 636b 732f 7b73 796d 626f  .z.stocks/{symbo
+00001e60: 6c7d 2f56 6152 2904 7222 0000 00da 1063  l}/VaR).r".....c
+00001e70: 6f6e 6669 6465 6e63 655f 6c65 7665 6cda  onfidence_level.
+00001e80: 0f6c 6f6f 6b62 6163 6b5f 7065 7269 6f64  .lookback_period
+00001e90: 7223 0000 0063 0300 0000 0000 0000 0000  r#...c..........
+00001ea0: 0000 0b00 0000 0600 0000 4300 0000 739e  ..........C...s.
+00001eb0: 0000 0074 00a0 017c 00a1 017d 037c 036a  ...t...|...}.|.j
+00001ec0: 027d 0474 037c 0483 017d 057c 0574 046b  .}.t.|...}.|.t.k
+00001ed0: 0272 226e 0874 0564 0183 0101 007c 036a  .r"n.t.d.....|.j
+00001ee0: 067c 029b 0064 029d 0264 038d 0164 0419  .|...d...d...d..
+00001ef0: 007d 0674 07a0 087c 067c 06a0 0964 05a1  .}.t...|.|...d..
+00001f00: 011b 00a1 017d 077c 07a0 0aa1 007d 087c  .....}.|.....}.|
+00001f10: 0874 0ba0 0c64 057c 0118 00a1 0114 007d  .t...d.|.......}
+00001f20: 0974 0564 0674 0d7c 097c 0664 0719 0014  .t.d.t.|.|.d....
+00001f30: 0064 0883 0269 0183 0101 0074 0d7c 097c  .d...i.....t.|.|
+00001f40: 0664 0719 0014 0064 0883 027d 0a7c 0a53  .d.....d...}.|.S
+00001f50: 0029 0975 c801 0000 0a20 2020 2023 2320  .).u.....    ## 
+00001f60: 5573 6162 696c 6964 6164 6520 0a20 2020  Usabilidade .   
+00001f70: 202d 204f 2056 616c 7565 2061 7420 5269   - O Value at Ri
+00001f80: 736b 2028 5661 5229 20c3 a920 756d 6120  sk (VaR) .. uma 
+00001f90: 6d65 6469 6461 2064 6520 7269 7363 6f20  medida de risco 
+00001fa0: 7175 6520 696e 6469 6361 2061 2070 6572  que indica a per
+00001fb0: 6461 206d c3a1 7869 6d61 2065 7370 6572  da m..xima esper
+00001fc0: 6164 612c 2063 6f6d 2075 6d20 6465 7465  ada, com um dete
+00001fd0: 726d 696e 6164 6f20 6ec3 ad76 656c 2064  rminado n..vel d
+00001fe0: 6520 636f 6e66 6961 6ec3 a761 2c20 656d  e confian..a, em
+00001ff0: 2075 6d20 696e 7465 7276 616c 6f20 6465   um intervalo de
+00002000: 2074 656d 706f 2070 72c3 a92d 6465 7465   tempo pr..-dete
+00002010: 726d 696e 6164 6f2e 200a 0a20 2020 200a  rminado. ..    .
+00002020: 2020 2020 2323 2050 6172 c3a2 6d65 7472      ## Par..metr
+00002030: 6f73 0a20 2020 200a 2020 2020 2d20 7379  os.    .    - sy
+00002040: 6d62 6f6c 202d 3e20 4e6f 6d65 2064 6f20  mbol -> Nome do 
+00002050: 4174 6976 6f20 7061 7261 2066 617a 6572  Ativo para fazer
+00002060: 2061 2062 7573 6361 200a 0a20 2020 202d   a busca ..    -
+00002070: 2063 6f6e 6669 6465 6e63 655f 6c65 7665   confidence_leve
+00002080: 6c20 2d3e 204e 6976 656c 2064 6520 636f  l -> Nivel de co
+00002090: 6e66 6961 6ec3 a761 2070 6172 6120 6f20  nfian..a para o 
+000020a0: 5641 5220 2830 2061 2031 292c 206e 6f72  VAR (0 a 1), nor
+000020b0: 6d61 6c6d 656e 7465 2075 7361 646f 2065  malmente usado e
+000020c0: 6d20 302e 3935 200a 0a20 2020 202d 206c  m 0.95 ..    - l
+000020d0: 6f6f 6b62 6163 6b5f 7065 7269 6f64 202d  ookback_period -
+000020e0: 3e20 5065 7269 6f64 6f20 454d 2044 4941  > Periodo EM DIA
+000020f0: 5320 6120 7365 7220 636f 6e73 6964 6572  S a ser consider
+00002100: 6164 6f20 7061 7261 206f 2063 c3a1 6c63  ado para o c..lc
+00002110: 756c 6f20 646f 2056 6152 0a0a 2020 2020  ulo do VaR..    
+00002120: 7224 0000 00da 0164 723b 0000 0072 4700  r$.....dr;...rG.
+00002130: 0000 7216 0000 005a 0356 6152 7225 0000  ..r....Z.VaRr%..
+00002140: 00e9 0200 0000 290e 7229 0000 0072 2a00  ......).r)...r*.
+00002150: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+00002160: 0072 2e00 0000 723f 0000 0072 6600 0000  .r....r?...rf...
+00002170: 7267 0000 0072 6800 0000 da03 7374 6472  rg...rh.....stdr
+00002180: 0200 0000 5a03 7070 66da 0572 6f75 6e64  ....Z.ppf..round
+00002190: 290b 7222 0000 0072 7000 0000 7271 0000  ).r"...rp...rq..
+000021a0: 0072 3100 0000 722b 0000 0072 3200 0000  .r1...r+...r2...
+000021b0: 5a06 7072 6963 6573 da07 7265 7475 726e  Z.prices..return
+000021c0: 735a 0773 7464 5f64 6576 726a 0000 005a  sZ.std_devrj...Z
+000021d0: 0356 6172 721f 0000 0072 1f00 0000 7220  .Varr....r....r 
+000021e0: 0000 00da 0767 6574 5f76 6172 7001 0000  .....get_varp...
+000021f0: 731a 0000 0000 0f0a 0106 0108 0108 0102  s...............
+00002200: 0208 0316 0314 0308 0112 011a 0112 0172  ...............r
+00002210: 7700 0000 7a1c 7374 6f63 6b73 2f7b 7379  w...z.stocks/{sy
+00002220: 6d62 6f6c 7d2f 416e 6e75 616c 5265 7475  mbol}/AnnualRetu
+00002230: 726e 2904 da07 7379 6d62 6f6c 7372 5f00  rn)...symbolsr_.
+00002240: 0000 7260 0000 0072 2300 0000 6303 0000  ..r`...r#...c...
+00002250: 0000 0000 0000 0000 0011 0000 0007 0000  ................
+00002260: 0043 0000 0073 9201 0000 7400 7c00 7401  .C...s....t.|.t.
+00002270: 8302 72c8 7402 6401 7c00 9b00 9d02 8301  ..r.t.d.|.......
+00002280: 0100 7403 6a04 7c00 7c01 7c02 6402 6403  ..t.j.|.|.|.d.d.
+00002290: 8d04 7d03 7a86 7403 a005 7c00 a101 6a06  ..}.z.t...|...j.
+000022a0: 7d04 7c04 6404 1900 7d05 7c03 6405 1900  }.|.d...}.|.d...
+000022b0: 7d06 7c06 a007 a100 7d07 7c07 a008 a100  }.|.....}.|.....
+000022c0: 6406 1400 7d08 7c07 a009 a100 6407 1400  d...}.|.....d...
+000022d0: 7d09 7c06 6a0a 6408 1900 6409 1400 7d0a  }.|.j.d...d...}.
+000022e0: 7c06 6a0a 640a 1900 6409 1400 7d0b 7c0b  |.j.d...d...}.|.
+000022f0: 7c0a 1800 7c0a 1b00 7d0c 740b 6a0c 7c00  |...|...}.t.j.|.
+00002300: 7c05 7c08 7c09 7c0c 640b 9c05 640c 6701  |.|.|.|.d...d.g.
+00002310: 640d 8d02 7d0d 7c0d 5700 5300 0100 0100  d...}.|.W.S.....
+00002320: 0100 7402 640e 8301 0100 5900 6e02 3000  ..t.d.....Y.n.0.
+00002330: 6ec6 7400 7c00 740d 8302 9001 7286 740b  n.t.|.t.....r.t.
+00002340: a00c a100 7d0e 7402 640f 7c00 9b00 9d02  ....}.t.d.|.....
+00002350: 8301 0100 7c00 4400 5d92 7d0f 7403 6a04  ....|.D.].}.t.j.
+00002360: 7c0f 7c01 7c02 6402 6403 8d04 7d03 7c03  |.|.|.d.d...}.|.
+00002370: 6405 1900 7d06 7c06 a007 a100 7d07 7c07  d...}.|.....}.|.
+00002380: a008 a100 6406 1400 7d08 7c07 a009 a100  ....d...}.|.....
+00002390: 6407 1400 7d09 7c06 6a0a 6408 1900 6409  d...}.|.j.d...d.
+000023a0: 1400 7d0a 7c06 6a0a 640a 1900 6409 1400  ..}.|.j.d...d...
+000023b0: 7d0b 7c0b 7c0a 1800 7c0a 1b00 7d0c 740b  }.|.|...|...}.t.
+000023c0: 6a0c 7c0f 7c08 7c09 7c0c 6410 9c04 740e  j.|.|.|.|.d...t.
+000023d0: 7c00 8301 6701 640d 8d02 7d10 740b a00f  |...g.d...}.t...
+000023e0: 7c10 7c0e 6702 a101 7d0e 71ee 7c0e 5300  |.|.g...}.q.|.S.
+000023f0: 7402 6411 8301 0100 6412 5300 2913 759b  t.d.....d.S.).u.
+00002400: 0100 000a 2020 2020 2323 2055 7361 6269  ....    ## Usabi
+00002410: 6c69 6461 6465 0a20 2020 202d 2052 6563  lidade.    - Rec
+00002420: 6562 6520 756d 6120 6c69 7374 6120 6520  ebe uma lista e 
+00002430: 7265 746f 726e 6120 756d 2044 6174 6146  retorna um DataF
+00002440: 7261 6d65 2063 6f6d 2061 7320 696e 666f  rame com as info
+00002450: 726d 61c3 a7c3 b565 7320 646f 7320 6174  rma....es dos at
+00002460: 6976 6f73 2065 2061 6c67 756d 6173 2065  ivos e algumas e
+00002470: 7374 6174 c3ad 7374 6963 6173 2062 c3a1  stat..sticas b..
+00002480: 7369 6361 732e 200a 0a20 2020 200a 2020  sicas. ..    .  
+00002490: 2020 2323 2050 6172 c3a2 6d65 7472 6f73    ## Par..metros
+000024a0: 0a20 2020 202d 2073 796d 626f 6c73 202d  .    - symbols -
+000024b0: 3e20 5265 6365 6265 2075 6d61 206c 6973  > Recebe uma lis
+000024c0: 7461 206f 7520 756d 2075 6e69 636f 2061  ta ou um unico a
+000024d0: 7469 766f 2070 6172 6120 6275 7363 6172  tivo para buscar
+000024e0: 206e 6120 6261 7365 200a 0a20 2020 202d   na base ..    -
+000024f0: 2073 7461 7274 5f64 6174 6520 2d3e 2044   start_date -> D
+00002500: 6174 6120 6465 2049 6e69 6369 6f20 6461  ata de Inicio da
+00002510: 2062 7573 6361 2064 6173 2069 6e66 6f73   busca das infos
+00002520: 2028 7072 6563 6f2c 2076 6f6c 756d 652c   (preco, volume,
+00002530: 2065 7463 2920 646f 2061 7469 766f 200a   etc) do ativo .
+00002540: 0a20 2020 202d 2065 6e64 5f64 6174 6520  .    - end_date 
+00002550: 2d3e 2044 6174 6120 4669 6e61 6c20 7061  -> Data Final pa
+00002560: 7261 2061 2062 7573 6361 2064 6173 2069  ra a busca das i
+00002570: 6e66 6f73 2028 7072 6563 6f2c 2076 6f6c  nfos (preco, vol
+00002580: 756d 652c 2065 7463 2920 646f 2061 7469  ume, etc) do ati
+00002590: 766f 200a 0a20 2020 200a 2020 2020 751a  vo ..    .    u.
+000025a0: 0000 0056 6f63 c3aa 2064 6967 6974 6f75  ...Voc.. digitou
+000025b0: 2075 6d61 2073 7472 696e 673a 20da 0674   uma string: ..t
+000025c0: 6963 6b65 7229 045a 0774 6963 6b65 7273  icker).Z.tickers
+000025d0: 7262 0000 0072 6300 0000 5a08 6772 6f75  rb...rc...Z.grou
+000025e0: 705f 6279 5a12 7265 6775 6c61 724d 6172  p_byZ.regularMar
+000025f0: 6b65 7450 7269 6365 7247 0000 0072 6400  ketPricerG...rd.
+00002600: 0000 675f 75bc 7ebf bf2f 4072 0100 0000  ..g_u.~../@r....
+00002610: 7252 0000 0072 2500 0000 2905 da05 4174  rR...r%...)...At
+00002620: 6976 6f75 1000 0000 5072 65c3 a76f 2061  ivou....Pre..o a
+00002630: 204d 6572 6361 646f fa0d 5265 746f 726e   Mercado..Retorn
+00002640: 6f20 616e 7561 6cf5 1400 0000 4465 7376  o anual.....Desv
+00002650: 696f 2070 6164 72c3 a36f 2061 6e75 616c  io padr..o anual
+00002660: fa0d 5265 746f 726e 6f20 746f 7461 6c72  ..Retorno totalr
+00002670: 1600 0000 a901 da05 696e 6465 7875 1000  ........indexu..
+00002680: 0000 5469 636b 6572 2069 6e76 c3a1 6c69  ..Ticker inv..li
+00002690: 646f 7519 0000 0056 6f63 c3aa 2064 6967  dou....Voc.. dig
+000026a0: 6974 6f75 2075 6d61 206c 6973 7461 3a20  itou uma lista: 
+000026b0: 2904 727a 0000 0072 7b00 0000 727c 0000  ).rz...r{...r|..
+000026c0: 0072 7d00 0000 752f 0000 0054 6970 6f20  .r}...u/...Tipo 
+000026d0: 696e 76c3 a16c 6964 6f2e 2044 6967 6974  inv..lido. Digit
+000026e0: 6520 756d 6120 7374 7269 6e67 206f 7520  e uma string ou 
+000026f0: 756d 6120 6c69 7374 612e 4e29 10da 0a69  uma lista.N)...i
+00002700: 7369 6e73 7461 6e63 65da 0373 7472 722e  sinstance..strr.
+00002710: 0000 0072 2900 0000 7265 0000 0072 2a00  ...r)...re...r*.
+00002720: 0000 722b 0000 0072 6d00 0000 7257 0000  ..r+...rm...rW..
+00002730: 0072 7400 0000 722f 0000 0072 4200 0000  .rt...r/...rB...
+00002740: 7243 0000 0072 3d00 0000 da03 6c65 6eda  rC...r=.....len.
+00002750: 0663 6f6e 6361 7429 1172 7800 0000 725f  .concat).rx...r_
+00002760: 0000 0072 6000 0000 da05 6461 646f 73da  ...r`.....dados.
+00002770: 0464 6174 615a 0b76 616c 7565 4d61 726b  .dataZ.valueMark
+00002780: 6574 da05 636c 6f73 655a 0e72 6574 6f72  et..closeZ.retor
+00002790: 6e6f 5f64 6961 7269 6f5a 0d72 6574 6f72  no_diarioZ.retor
+000027a0: 6e6f 5f61 6e75 616c 5a13 6465 7376 696f  no_anualZ.desvio
+000027b0: 5f70 6164 7261 6f5f 616e 7561 6c5a 0f76  _padrao_anualZ.v
+000027c0: 616c 6f72 5f69 6e76 6573 7469 646f 5a0b  alor_investidoZ.
+000027d0: 7661 6c6f 725f 6174 7561 6c5a 0d72 6574  valor_atualZ.ret
+000027e0: 6f72 6e6f 5f74 6f74 616c 5a0c 7661 6c75  orno_totalZ.valu
+000027f0: 6553 796d 626f 6c73 5a07 7661 6c75 6544  eSymbolsZ.valueD
+00002800: 465a 0773 696d 626f 6c6f 5a0d 7265 7475  FZ.simboloZ.retu
+00002810: 726e 5379 6d62 6f6c 7372 1f00 0000 721f  rnSymbolsr....r.
+00002820: 0000 0072 2000 0000 da0f 6173 7365 745f  ...r .....asset_
+00002830: 706f 7274 666f 6c69 6f9b 0100 0073 6000  portfolio....s`.
+00002840: 0000 000e 0a01 0e01 1202 0202 0c01 0803  ................
+00002850: 0803 0803 0c03 0c03 0e03 0e03 0c03 0401  ................
+00002860: 0201 0201 0201 0201 02fb 0406 04fa 0608  ................
+00002870: 0602 0601 1002 0c01 0801 0e01 0801 1203  ................
+00002880: 0803 0803 0c03 0c03 0e03 0e03 0c03 0401  ................
+00002890: 0201 0201 0201 02fc 0405 08fb 0607 1002  ................
+000028a0: 0402 7287 0000 007a 2473 746f 636b 732f  ..r....z$stocks/
+000028b0: 7b73 796d 626f 6c7d 2f4d 6172 6b6f 7769  {symbol}/Markowi
+000028c0: 747a 416c 6c6f 6361 7469 6f6e 6e29 0472  tzAllocationn).r
+000028d0: 7800 0000 da09 7374 6172 5f64 6174 6572  x.....star_dater
+000028e0: 6000 0000 7223 0000 0063 0300 0000 0000  `...r#...c......
+000028f0: 0000 0000 0000 1100 0000 0900 0000 4300  ..............C.
+00002900: 0000 733a 0100 0074 006a 017c 007c 017c  ..s:...t.j.|.|.|
+00002910: 0264 018d 0364 0219 007d 037c 03a0 02a1  .d...d...}.|....
+00002920: 00a0 03a1 007d 047c 04a0 04a1 007d 0574  .....}.|.....}.t
+00002930: 05a0 0664 0374 077c 0083 011b 0067 0174  ...d.t.|.....g.t
+00002940: 077c 0083 0114 00a1 017d 0674 05a0 087c  .|.......}.t...|
+00002950: 04a0 09a1 007c 0614 00a1 0164 0414 007d  .....|.....d...}
+00002960: 0774 05a0 0a74 05a0 0b7c 066a 0c74 05a0  .t...t...|.j.t..
+00002970: 0b7c 057c 06a1 02a1 02a1 0174 05a0 0a64  .|.|.......t...d
+00002980: 04a1 0114 007d 0864 0574 05a0 0d7c 05a1  .....}.d.t...|..
+00002990: 0114 007d 0974 056a 0ea0 0f7c 057c 0974  ...}.t.j...|.|.t
+000029a0: 05a0 107c 056a 1164 0619 00a1 0114 0017  ...|.j.d........
+000029b0: 00a1 017d 0a74 05a0 1274 077c 0083 0164  ...}.t...t.|...d
+000029c0: 0366 02a1 017d 0b74 05a0 0b7c 0a7c 0ba1  .f...}.t...|.|..
+000029d0: 0274 05a0 0b74 05a0 0b7c 0b6a 0c7c 0aa1  .t...t...|.j.|..
+000029e0: 027c 0ba1 021b 007d 0c7c 0ca0 13a1 007d  .|.....}.|.....}
+000029f0: 0c67 007d 0d74 1474 077c 0083 0183 0144  .g.}.t.t.|.....D
+00002a00: 005d 2e7d 0e64 077c 007c 0e19 009b 0064  .].}.d.|.|.....d
+00002a10: 087c 0c7c 0e19 0064 0914 0064 0a9b 0464  .|.|...d...d...d
+00002a20: 0b9d 057d 0f7c 0da0 157c 0fa1 0101 0071  ...}.|...|.....q
+00002a30: fa7c 077c 087c 0d64 0c9c 037d 107c 1053  .|.|.|.d...}.|.S
+00002a40: 0029 0d75 2403 0000 0a20 2020 2023 2320  .).u$....    ## 
+00002a50: 5573 6162 696c 6964 6164 6573 200a 2020  Usabilidades .  
+00002a60: 2020 2d20 416c 6f63 61c3 a7c3 a36f 2064    - Aloca....o d
+00002a70: 6520 4d61 726b 6f77 6974 7a20 c3a9 2075  e Markowitz .. u
+00002a80: 6d61 2074 c3a9 636e 6963 6120 6465 206f  ma t..cnica de o
+00002a90: 7469 6d69 7a61 c3a7 c3a3 6f20 6465 2070  timiza....o de p
+00002aa0: 6f72 7466 c3b3 6c69 6f20 7175 6520 7669  ortf..lio que vi
+00002ab0: 7361 2065 6e63 6f6e 7472 6172 2061 2063  sa encontrar a c
+00002ac0: 6f6d 6269 6e61 c3a7 c3a3 6f20 6964 6561  ombina....o idea
+00002ad0: 6c20 6465 2061 7469 766f 7320 7061 7261  l de ativos para
+00002ae0: 206d 6178 696d 697a 6172 206f 2072 6574   maximizar o ret
+00002af0: 6f72 6e6f 2064 6f20 696e 7665 7374 696d  orno do investim
+00002b00: 656e 746f 2065 6e71 7561 6e74 6f20 6d69  ento enquanto mi
+00002b10: 6e69 6d69 7a61 206f 2072 6973 636f 2e20  nimiza o risco. 
+00002b20: 0a0a 0a20 2020 2023 2320 4f20 5265 746f  ...    ## O Reto
+00002b30: 726e 6f20 4573 7065 7261 646f 0a20 2020  rno Esperado.   
+00002b40: 202d 2072 6570 7265 7365 6e74 6120 6120   - representa a 
+00002b50: 7461 7861 2064 6520 7265 746f 726e 6f20  taxa de retorno 
+00002b60: 6dc3 a964 6961 2071 7565 2073 6520 6573  m..dia que se es
+00002b70: 7065 7261 206f 6274 6572 2064 6f20 706f  pera obter do po
+00002b80: 7274 66c3 b36c 696f 2064 6520 696e 7665  rtf..lio de inve
+00002b90: 7374 696d 656e 746f 7320 0a0a 2020 2020  stimentos ..    
+00002ba0: 2323 204f 2052 6973 636f 200a 2020 2020  ## O Risco .    
+00002bb0: 2d20 7265 7072 6573 656e 7461 2061 206d  - representa a m
+00002bc0: 6564 6964 6120 6465 2076 6f6c 6174 696c  edida de volatil
+00002bd0: 6964 6164 6520 646f 2070 6f72 7466 c3b3  idade do portf..
+00002be0: 6c69 6f2c 206f 7520 7365 6a61 2c20 0a20  lio, ou seja, . 
+00002bf0: 2020 2071 7561 6e74 6f20 6d61 6973 2069     quanto mais i
+00002c00: 6e73 74c3 a176 656c 2066 6f72 206f 2072  nst..vel for o r
+00002c10: 6574 6f72 6e6f 2064 6f73 2061 7469 766f  etorno dos ativo
+00002c20: 732c 206d 6169 6f72 2073 6572 c3a1 206f  s, maior ser.. o
+00002c30: 2072 6973 636f 2064 6f20 706f 7274 66c3   risco do portf.
+00002c40: b36c 696f 2063 6f6d 6f20 756d 2074 6f64  .lio como um tod
+00002c50: 6f20 0a0a 2020 2020 0a20 2020 200a 2020  o ..    .    .  
+00002c60: 2020 0a20 2020 2023 2320 5061 72c3 a26d    .    ## Par..m
+00002c70: 6574 726f 730a 2020 2020 0a20 2020 202d  etros.    .    -
+00002c80: 2073 796d 626f 6c73 202d 3e20 5265 6365   symbols -> Rece
+00002c90: 6265 2075 6d61 206c 6973 7461 2064 6520  be uma lista de 
+00002ca0: 6174 6976 6f73 2070 6172 6120 6275 7363  ativos para busc
+00002cb0: 6172 206e 6120 6261 7365 200a 0a20 2020  ar na base ..   
+00002cc0: 202d 2073 7461 7274 5f64 6174 6520 2d3e   - start_date ->
+00002cd0: 2044 6174 6120 6465 2049 6e69 6369 6f20   Data de Inicio 
+00002ce0: 6461 2062 7573 6361 2064 6173 2069 6e66  da busca das inf
+00002cf0: 6f73 2028 7072 6563 6f2c 2076 6f6c 756d  os (preco, volum
+00002d00: 652c 2065 7463 2920 646f 2061 7469 766f  e, etc) do ativo
+00002d10: 200a 0a20 2020 202d 2065 6e64 5f64 6174   ..    - end_dat
+00002d20: 6520 2d3e 2044 6174 6120 4669 6e61 6c20  e -> Data Final 
+00002d30: 7061 7261 2061 2062 7573 6361 2064 6173  para a busca das
+00002d40: 2069 6e66 6f73 2028 7072 6563 6f2c 2076   infos (preco, v
+00002d50: 6f6c 756d 652c 2065 7463 2920 646f 2061  olume, etc) do a
+00002d60: 7469 766f 200a 0a0a 2020 2020 7261 0000  tivo ...    ra..
+00002d70: 007a 0941 646a 2043 6c6f 7365 7216 0000  .z.Adj Closer...
+00002d80: 0072 6400 0000 679a 9999 9999 99b9 3f72  .rd...g.......?r
+00002d90: 0100 0000 7a08 4f20 6174 6976 6f20 7a15  ....z.O ativo z.
+00002da0: 2064 6576 6520 7365 7220 616c 6f63 6164   deve ser alocad
+00002db0: 6f20 656d 2072 5200 0000 7a03 2e32 667a  o em rR...z..2fz
+00002dc0: 0d25 2064 6120 6361 7274 6569 7261 2903  .% da carteira).
+00002dd0: fa10 5265 746f 726e 6f20 4573 7065 7261  ..Retorno Espera
+00002de0: 646f fa11 5269 7363 6f20 6461 2043 6172  do..Risco da Car
+00002df0: 7465 6972 61fa 1241 6c6f 6361 6361 6f20  teira..Alocacao 
+00002e00: 4d61 726b 6f77 6974 7a29 1672 2900 0000  Markowitz).r)...
+00002e10: 7265 0000 0072 6d00 0000 da06 6472 6f70  re...rm.....drop
+00002e20: 6e61 726e 0000 0072 6600 0000 da05 6172  narn...rf.....ar
+00002e30: 7261 7972 8200 0000 7230 0000 0072 5700  rayr....r0...rW.
+00002e40: 0000 7269 0000 00da 0364 6f74 da01 54da  ..ri.....dot..T.
+00002e50: 0574 7261 6365 5a06 6c69 6e61 6c67 da03  .traceZ.linalg..
+00002e60: 696e 76da 0365 7965 da05 7368 6170 65da  inv..eye..shape.
+00002e70: 046f 6e65 73da 0766 6c61 7474 656e da05  .ones..flatten..
+00002e80: 7261 6e67 65da 0661 7070 656e 6429 1172  range..append).r
+00002e90: 7800 0000 7288 0000 0072 6000 0000 7284  x...r....r`...r.
+00002ea0: 0000 005a 0872 6574 6f72 6e6f 735a 126d  ...Z.retornosZ.m
+00002eb0: 6174 7269 7a5f 636f 7661 7269 616e 6369  atriz_covarianci
+00002ec0: 615a 0570 6573 6f73 da10 7265 746f 726e  aZ.pesos..retorn
+00002ed0: 6f5f 6573 7065 7261 646f da05 7269 7363  o_esperado..risc
+00002ee0: 6f5a 076c 616d 6264 615f 5a07 636f 765f  oZ.lambda_Z.cov_
+00002ef0: 696e 765a 0976 6574 6f72 5f75 6e73 5a0b  invZ.vetor_unsZ.
+00002f00: 775f 6d61 726b 6f77 6974 7a5a 0d6d 6172  w_markowitzZ.mar
+00002f10: 6b6f 7769 747a 4c69 7374 da01 695a 0574  kowitzList..iZ.t
+00002f20: 6178 6173 7233 0000 0072 1f00 0000 721f  axasr3...r....r.
+00002f30: 0000 0072 2000 0000 da14 6d61 726b 6f77  ...r .....markow
+00002f40: 6974 7a5f 616c 6c6f 6361 7469 6f6e 0502  itz_allocation..
+00002f50: 0000 7328 0000 0000 1614 030c 0308 031c  ..s(............
+00002f60: 0316 0326 030e 0120 0112 0122 0108 0304  ...&... ..."....
+00002f70: 0110 0120 010c 0102 0102 0102 fe06 0672  ... ...........r
+00002f80: 9b00 0000 7a23 7374 6f63 6b73 2f7b 7379  ....z#stocks/{sy
+00002f90: 6d62 6f6c 7d2f 4d61 726b 6f77 6974 7a41  mbol}/MarkowitzA
+00002fa0: 6c6c 6f63 6174 696f 6e7a 0a2f 696e 666f  llocationz./info
+00002fb0: 4675 6e64 7363 0100 0000 0000 0000 0000  Fundsc..........
+00002fc0: 0000 0700 0000 0400 0000 4300 0000 7372  ..........C...sr
+00002fd0: 0000 0064 017d 0174 00a0 017c 01a1 017d  ...d.}.t...|...}
+00002fe0: 0274 027c 026a 0364 0283 027d 037c 03a0  .t.|.j.d...}.|..
+00002ff0: 0464 03a1 0164 0419 007d 0474 05a0 0674  .d...d...}.t...t
+00003000: 077c 0483 01a1 0164 0419 007d 057c 0564  .|.....d...}.|.d
+00003010: 0519 00a0 0864 0664 0784 00a1 017c 0564  .....d.d.....|.d
+00003020: 053c 007c 056a 097c 0564 0519 007c 006b  .<.|.j.|.d...|.k
+00003030: 0219 007d 067c 0667 0064 08a2 0119 007d  ...}.|.g.d.....}
+00003040: 067c 0653 0029 0975 ca00 0000 0a20 2020  .|.S.).u.....   
+00003050: 2023 2320 5573 6162 696c 6964 6164 650a   ## Usabilidade.
+00003060: 2020 2020 2d20 4675 6ec3 a761 6f20 7574      - Fun..ao ut
+00003070: 696c 697a 6164 6120 7061 7261 2061 6471  ilizada para adq
+00003080: 7569 7269 7220 6173 2070 7269 6e63 6970  uirir as princip
+00003090: 6169 7320 6361 7261 6374 6572 6973 7469  ais caracteristi
+000030a0: 6361 7320 6520 696e 666f 726d 61c3 a7c3  cas e informa...
+000030b0: b565 7320 646f 2066 756e 646f 2073 656c  .es do fundo sel
+000030c0: 6563 696f 6e61 646f 0a0a 2020 2020 2323  ecionado..    ##
+000030d0: 2050 6172 c3a2 6d65 7472 6f73 0a0a 2020   Par..metros..  
+000030e0: 2020 2d20 7379 6d62 6f6c 202d 3e20 4e6f    - symbol -> No
+000030f0: 6d65 2064 6f20 4675 6e64 6f20 7061 7261  me do Fundo para
+00003100: 2066 617a 6572 2061 2062 7573 6361 200a   fazer a busca .
+00003110: 0a0a 2020 2020 fa28 6874 7470 733a 2f2f  ..    .(https://
+00003120: 7777 772e 6675 6e64 7365 7870 6c6f 7265  www.fundsexplore
+00003130: 722e 636f 6d2e 6272 2f72 616e 6b69 6e67  r.com.br/ranking
+00003140: fa0b 6874 6d6c 2e70 6172 7365 72da 0574  ..html.parser..t
+00003150: 6162 6c65 7201 0000 00f5 1000 0000 43c3  abler.........C.
+00003160: b364 6967 6f20 646f 2066 756e 646f 6301  .digo do fundoc.
+00003170: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00003180: 0000 0053 0000 0073 0800 0000 7c00 6401  ...S...s....|.d.
+00003190: 1700 5300 a902 4efa 032e 5341 721f 0000  ..S...N...SAr...
+000031a0: 00a9 01da 0178 721f 0000 0072 1f00 0000  .....xr....r....
+000031b0: 7220 0000 00da 083c 6c61 6d62 6461 3e59  r .....<lambda>Y
+000031c0: 0200 00f3 0000 0000 7a1b 6765 745f 6675  ........z.get_fu
+000031d0: 6e64 732e 3c6c 6f63 616c 733e 2e3c 6c61  nds.<locals>.<la
+000031e0: 6d62 6461 3ea9 0672 9f00 0000 da05 5365  mbda>..r......Se
+000031f0: 746f 72f5 0c00 0000 5072 65c3 a76f 2041  tor.....Pre..o A
+00003200: 7475 616c da09 4469 7669 6465 6e64 6ff5  tual..Dividendo.
+00003210: 1100 0000 5661 7269 61c3 a7c3 a36f 2050  ....Varia....o P
+00003220: 7265 c3a7 6ff5 1000 0000 5265 6e74 6162  re..o.....Rentab
+00003230: 2e20 5065 72c3 ad6f 646f 290a da08 7265  . Per..odo)...re
+00003240: 7175 6573 7473 da03 6765 7472 0a00 0000  quests..getr....
+00003250: da07 636f 6e74 656e 74da 0866 696e 645f  ..content..find_
+00003260: 616c 6c72 4200 0000 da09 7265 6164 5f68  allrB.....read_h
+00003270: 746d 6c72 8100 0000 da05 6170 706c 79da  tmlr......apply.
+00003280: 036c 6f63 2907 7222 0000 00da 0375 726c  .loc).r".....url
+00003290: da08 7265 7370 6f6e 7365 da04 736f 7570  ..response..soup
+000032a0: 729e 0000 00da 0766 756e 6473 4446 da08  r......fundsDF..
+000032b0: 7661 6c75 6573 4649 721f 0000 0072 1f00  valuesFIr....r..
+000032c0: 0000 7220 0000 00da 0967 6574 5f66 756e  ..r .....get_fun
+000032d0: 6473 4702 0000 7312 0000 0000 0d04 010a  dsG...s.........
+000032e0: 010c 010e 0112 0116 0212 010c 0272 b800  .............r..
+000032f0: 0000 7a12 2f63 6f6d 7061 7265 5365 746f  ..z./compareSeto
+00003300: 7246 756e 6473 2902 da05 7365 746f 7272  rFunds)...setorr
+00003310: 2300 0000 6302 0000 0000 0000 0000 0000  #...c...........
+00003320: 000c 0000 0006 0000 0043 0000 0073 1e01  .........C...s..
+00003330: 0000 6401 7d02 7400 a001 7c02 a101 7d03  ..d.}.t...|...}.
+00003340: 7402 7c03 6a03 6402 8302 7d04 7c04 a004  t.|.j.d...}.|...
+00003350: 6403 a101 6404 1900 7d05 7405 a006 7407  d...d...}.t...t.
+00003360: 7c05 8301 a101 6404 1900 7d06 7408 7c06  |.....d...}.t.|.
+00003370: 6405 8302 0100 7c01 6406 1b00 7d01 7c06  d.....|.d...}.|.
+00003380: 6a09 7c06 6405 1900 6406 1b00 7c01 6b04  j.|.d...d...|.k.
+00003390: 1900 7d07 7c07 6700 6407 a201 1900 7d07  ..}.|.g.d.....}.
+000033a0: 7c07 a00a a100 7d07 7c07 6405 1900 a00b  |.....}.|.d.....
+000033b0: a100 7d08 7c00 6408 6b02 72aa 6409 7d00  ..}.|.d.k.r.d.}.
+000033c0: 7c07 6a09 7c07 640a 1900 7c00 6b02 1900  |.j.|.d...|.k...
+000033d0: 6405 1900 a00b a100 7d09 6e42 7c00 640b  d.......}.nB|.d.
+000033e0: 6b02 72d2 640c 7d00 7c07 6a09 7c07 640a  k.r.d.}.|.j.|.d.
+000033f0: 1900 7c00 6b02 1900 6405 1900 a00b a100  ..|.k...d.......
+00003400: 7d09 6e1a 7c07 6a09 7c07 640a 1900 7c00  }.n.|.j.|.d...|.
+00003410: 6b02 1900 6405 1900 a00b a100 7d09 7c07  k...d.......}.|.
+00003420: 6405 1900 a00c a100 7d0a 7405 a00d 7c08  d.......}.t...|.
+00003430: 6701 7c09 6701 7c0a 6701 640d 9c03 a101  g.|.g.|.g.d.....
+00003440: 7d0b 7c0b a00e 640e a101 7d0b 7c0b 5300  }.|...d...}.|.S.
+00003450: 290f 7506 0300 000a 2020 2020 2323 2055  ).u.....    ## U
+00003460: 7361 6269 6c69 6461 6465 0a20 2020 200a  sabilidade.    .
+00003470: 2020 2020 2d20 4675 6ec3 a761 6f20 7175      - Fun..ao qu
+00003480: 6520 7574 696c 697a 6120 6173 206d 6574  e utiliza as met
+00003490: 7269 6361 7320 6520 6d65 6469 6173 2064  ricas e medias d
+000034a0: 6f73 2066 756e 646f 2063 6f6d 2062 6173  os fundo com bas
+000034b0: 6520 6e6f 2073 6575 2053 6574 6f72 2070  e no seu Setor p
+000034c0: 6172 6120 756d 6120 616e 616c 6973 6520  ara uma analise 
+000034d0: 6d61 6973 2072 6573 7472 6974 610a 2020  mais restrita.  
+000034e0: 2020 0a20 2020 2023 2320 5061 72c3 a26d    .    ## Par..m
+000034f0: 6574 726f 730a 2020 2020 0a20 2020 202d  etros.    .    -
+00003500: 2072 656e 7461 6269 6c69 6461 6465 5f6d   rentabilidade_m
+00003510: 696e 202d 3e20 5661 6c6f 7220 656d 2025  in -> Valor em %
+00003520: 2070 6172 6120 6275 7363 6172 2061 2072   para buscar a r
+00003530: 656e 7461 6269 6c69 6461 6465 206d 696e  entabilidade min
+00003540: 696d 6120 646f 2066 756e 646f 2065 7363  ima do fundo esc
+00003550: 6f6c 6869 646f 0a20 2020 202d 2073 6574  olhido.    - set
+00003560: 6f72 202d 3e20 5365 746f 7265 7320 6465  or -> Setores de
+00003570: 2066 756e 646f 7320 7175 6520 706f 6465   fundos que pode
+00003580: 7261 6d20 7365 7220 6573 636f 6c68 6964  ram ser escolhid
+00003590: 6f73 2c20 7365 6775 6520 6120 6c69 7374  os, segue a list
+000035a0: 613a 0a20 2020 200a 2020 2020 6060 600a  a:.    .    ```.
+000035b0: 2020 2020 5469 706f 7353 6574 6f72 6573      TiposSetores
+000035c0: 3a0a 2020 2020 2d20 436f 7270 6f72 6174  :.    - Corporat
+000035d0: 6976 6173 203d 2022 4c61 6a65 7320 436f  ivas = "Lajes Co
+000035e0: 7270 6f72 6174 6976 6173 2220 0a20 2020  rporativas" .   
+000035f0: 202d 204d 6f62 696c 6961 7269 6f73 203d   - Mobiliarios =
+00003600: 2022 54c3 ad74 756c 6f73 2065 2056 616c   "T..tulos e Val
+00003610: 2e20 4d6f 622e 220a 2020 2020 2d20 5368  . Mob.".    - Sh
+00003620: 6f70 7069 6e67 7320 3d20 2253 686f 7070  oppings = "Shopp
+00003630: 696e 6773 220a 2020 2020 2d20 48c3 ad62  ings".    - H..b
+00003640: 7269 646f 203d 2027 48c3 ad62 7269 646f  rido = 'H..brido
+00003650: 270a 2020 2020 2d20 5265 6e64 6120 3d20  '.    - Renda = 
+00003660: 2752 656e 6461 270a 2020 2020 2d20 4c6f  'Renda'.    - Lo
+00003670: 67c3 ad73 7469 6361 203d 2027 4c6f 67c3  g..stica = 'Log.
+00003680: ad73 7469 6361 270a 2020 2020 2d20 486f  .stica'.    - Ho
+00003690: 7370 6974 616c 203d 2027 486f 7370 6974  spital = 'Hospit
+000036a0: 616c 270a 2020 2020 2d20 5265 7369 6465  al'.    - Reside
+000036b0: 6e63 6961 6c20 3d20 2752 6573 6964 656e  ncial = 'Residen
+000036c0: 6369 616c 270a 2020 2020 2d20 4f75 7472  cial'.    - Outr
+000036d0: 6f73 203d 2027 4f75 7472 6f73 270a 0a20  os = 'Outros'.. 
+000036e0: 2020 2060 6060 0a20 2020 2023 2320 4578     ```.    ## Ex
+000036f0: 656d 706c 6f3a 0a20 2020 200a 2020 2020  emplo:.    .    
+00003700: 6060 600a 2020 2020 3e3e 3e20 6262 2e63  ```.    >>> bb.c
+00003710: 6f6d 7061 7265 5f73 6574 6f72 5f66 756e  ompare_setor_fun
+00003720: 6473 2873 6574 6f72 3d27 436f 7270 6f72  ds(setor='Corpor
+00003730: 6174 6976 6173 272c 2072 656e 7461 6269  ativas', rentabi
+00003740: 6c69 6461 6465 5f6d 696e 203d 2033 290a  lidade_min = 3).
+00003750: 2020 2020 6060 600a 0a20 2020 2072 9c00      ```..    r..
+00003760: 0000 729d 0000 0072 9e00 0000 7201 0000  ..r....r....r...
+00003770: 0072 ab00 0000 7252 0000 0072 a600 0000  .r....rR...r....
+00003780: 5a0c 436f 7270 6f72 6174 6976 6173 7a12  Z.Corporativasz.
+00003790: 4c61 6a65 7320 436f 7270 6f72 6174 6976  Lajes Corporativ
+000037a0: 6173 72a7 0000 005a 0b4d 6f62 696c 6961  asr....Z.Mobilia
+000037b0: 7269 6f73 7514 0000 0054 c3ad 7475 6c6f  riosu....T..tulo
+000037c0: 7320 6520 5661 6c2e 204d 6f62 2e29 0375  s e Val. Mob.).u
+000037d0: 2a00 0000 5265 6e74 6162 696c 6964 6164  *...Rentabilidad
+000037e0: 6520 4dc3 a964 6961 2064 6f73 2046 4949  e M..dia dos FII
+000037f0: 7320 5365 6c65 6369 6f6e 6164 6f73 751f  s Selecionadosu.
+00003800: 0000 0052 656e 7461 6269 6c69 6461 6465  ...Rentabilidade
+00003810: 204d c3a9 6469 6120 646f 204d 6572 6361   M..dia do Merca
+00003820: 646f 7537 0000 0044 6573 7669 6f20 5061  dou7...Desvio Pa
+00003830: 6472 c3a3 6f20 6461 7320 5265 6e74 6162  dr..o das Rentab
+00003840: 696c 6964 6164 6573 2064 6f73 2046 4949  ilidades dos FII
+00003850: 7320 5365 6c65 6369 6f6e 6164 6f73 7a20  s Selecionadosz 
+00003860: 4f20 7365 746f 722f 7661 6c6f 7220 6e61  O setor/valor na
+00003870: 6f20 666f 6920 656e 636f 6e74 7261 646f  o foi encontrado
+00003880: 290f 72ac 0000 0072 ad00 0000 720a 0000  ).r....r....r...
+00003890: 0072 ae00 0000 72af 0000 0072 4200 0000  .r....r....rB...
+000038a0: 72b0 0000 0072 8100 0000 7221 0000 0072  r....r....r!...r
+000038b0: b200 0000 728c 0000 0072 5700 0000 7274  ....r....rW...rt
+000038c0: 0000 0072 4300 0000 5a06 6669 6c6c 6e61  ...rC...Z.fillna
+000038d0: 290c 72b9 0000 005a 1172 656e 7461 6269  ).r....Z.rentabi
+000038e0: 6c69 6461 6465 5f6d 696e 72b3 0000 0072  lidade_minr....r
+000038f0: b400 0000 72b5 0000 0072 9e00 0000 72b6  ....r....r....r.
+00003900: 0000 0072 b700 0000 5a13 7265 6e74 6162  ...r....Z.rentab
+00003910: 696c 6964 6164 655f 6d65 6469 615a 1572  ilidade_mediaZ.r
+00003920: 656e 7461 6269 6c69 6461 6465 5f6d 6572  entabilidade_mer
+00003930: 6361 646f da0d 6465 7376 696f 5f70 6164  cado..desvio_pad
+00003940: 7261 6f5a 0a72 6573 756c 7461 646f 7372  raoZ.resultadosr
+00003950: 1f00 0000 721f 0000 0072 2000 0000 da13  ....r....r .....
+00003960: 636f 6d70 6172 655f 7365 746f 725f 6675  compare_setor_fu
+00003970: 6e64 7367 0200 0073 3400 0000 0022 0401  ndsg...s4...."..
+00003980: 0a01 0c01 0e01 1202 0a01 0801 1601 0c01  ................
+00003990: 0801 0c01 0801 0401 1c01 0801 0401 1c02  ................
+000039a0: 1a02 0c02 0401 0401 0401 04fd 0806 0a02  ................
+000039b0: 72bb 0000 007a 0d2f 636f 6d70 6172 6546  r....z./compareF
+000039c0: 756e 6473 2901 7223 0000 0063 0300 0000  unds).r#...c....
+000039d0: 0000 0000 0000 0000 1200 0000 0400 0000  ................
+000039e0: 4300 0000 734a 0100 007c 0172 bc7c 0264  C...sJ...|.r.|.d
+000039f0: 016b 0372 bc64 027d 0374 00a0 017c 03a1  .k.r.d.}.t...|..
+00003a00: 017d 0474 027c 046a 0364 0383 027d 057c  .}.t.|.j.d...}.|
+00003a10: 05a0 0464 04a1 0164 0519 007d 0674 05a0  ...d...d...}.t..
+00003a20: 0674 077c 0683 01a1 0164 0519 007d 077c  .t.|.....d...}.|
+00003a30: 0764 0619 00a0 0864 0764 0884 00a1 017c  .d.....d.d.....|
+00003a40: 0764 063c 007c 0767 0064 09a2 0119 007d  .d.<.|.g.d.....}
+00003a50: 077c 076a 0964 0667 0164 0a8d 017d 077c  .|.j.d.g.d...}.|
+00003a60: 076a 0a7c 0764 0619 007c 016b 0219 007d  .j.|.d...|.k...}
+00003a70: 087c 076a 0a7c 0764 0619 007c 026b 0219  .|.j.|.d...|.k..
+00003a80: 007d 0974 05a0 0b7c 087c 0967 02a1 017d  .}.t...|.|.g...}
+00003a90: 0a7c 0a6a 0c72 b874 0d64 0b83 0101 006e  .|.j.r.t.d.....n
+00003aa0: 047c 0a53 007c 0064 0175 0072 ca67 007d  .|.S.|.d.u.r.g.}
+00003ab0: 006e 7c64 0c7d 0b64 0d7d 0c7c 0044 005d  .n|d.}.d.}.|.D.]
+00003ac0: 3a7d 0d74 0ea0 0f7c 0da1 017d 0e7c 0e6a  :}.t...|...}.|.j
+00003ad0: 1064 0e64 0f8d 017d 0f7c 0f64 1019 00a0  .d.d...}.|.d....
+00003ae0: 11a1 00a0 12a1 007d 107c 107c 0b6b 0472  .......}.|.|.k.r
+00003af0: d67c 107d 0b7c 0d7d 0c71 d674 056a 137c  .|.}.|.}.q.t.j.|
+00003b00: 0c7c 0b64 1114 0064 129c 0274 147c 0083  .|.d...d...t.|..
+00003b10: 0167 0164 138d 027d 117c 116a 0c90 0172  .g.d...}.|.j...r
+00003b20: 4274 0d64 1483 0101 006e 047c 1153 0064  Bt.d.....n.|.S.d
+00003b30: 0153 0029 1575 2403 0000 0a20 2020 2023  .S.).u$....    #
+00003b40: 2320 5573 6162 696c 6964 6164 650a 2020  # Usabilidade.  
+00003b50: 2020 0a20 2020 202d 2046 756e c3a7 616f    .    - Fun..ao
+00003b60: 2071 7565 2072 6561 6c69 7a61 2061 2063   que realiza a c
+00003b70: 6f6d 7061 7261 c3a7 616f 2065 6e74 7265  ompara..ao entre
+00003b80: 2064 6f69 7320 6675 6e64 6f73 2c20 7365   dois fundos, se
+00003b90: 6a61 2066 6569 7461 2061 2072 6571 7569  ja feita a requi
+00003ba0: 7369 c3a7 616f 2064 6f73 2066 756e 646f  si..ao dos fundo
+00003bb0: 7320 7669 6120 6c69 7374 6120 6f75 2075  s via lista ou u
+00003bc0: 6e69 636f 7320 0a20 2020 202d 2052 6571  nicos .    - Req
+00003bd0: 7569 7369 c3a7 616f 204c 6973 7461 733a  uisi..ao Listas:
+00003be0: 2052 6574 6f72 6e61 206f 2066 756e 646f   Retorna o fundo
+00003bf0: 2063 6f6d 206d 6169 6f72 2070 6f72 6365   com maior porce
+00003c00: 6e74 6167 656d 2064 6520 7269 7363 6f20  ntagem de risco 
+00003c10: 2861 2076 6172 6961 c3a7 c3a3 6f20 7065  (a varia....o pe
+00003c20: 7263 656e 7475 616c 2064 6f73 2070 7265  rcentual dos pre
+00003c30: c3a7 6f73 2064 6f73 2061 7469 766f 732c  ..os dos ativos,
+00003c40: 2063 616c 6375 6c6f 2072 6561 6c69 7a61   calculo realiza
+00003c50: 646f 2063 6f6d 2062 6173 6520 6e6f 2064  do com base no d
+00003c60: 6573 7669 6f20 7061 6472 c3a3 6f29 0a20  esvio padr..o). 
+00003c70: 2020 202d 2052 6571 7569 7369 c3a7 616f     - Requisi..ao
+00003c80: 2055 6e69 6361 3a20 5265 746f 726e 6120   Unica: Retorna 
+00003c90: 756d 2044 6174 6166 7261 6d65 2063 6f6d  um Dataframe com
+00003ca0: 2061 7320 7072 696e 6369 7061 6973 2069   as principais i
+00003cb0: 6e66 6f72 6d61 c3a7 6f65 7320 646f 7320  nforma..oes dos 
+00003cc0: 6675 6e64 6f73 2c20 6166 696d 2064 6520  fundos, afim de 
+00003cd0: 756d 6120 636f 6d70 6172 61c3 a761 6f20  uma compara..ao 
+00003ce0: 656e 7472 6520 7365 7573 2076 616c 6f72  entre seus valor
+00003cf0: 6573 200a 0a20 2020 200a 2020 2020 2323  es ..    .    ##
+00003d00: 2050 6172 c3a2 6d65 7472 6f73 0a20 2020   Par..metros.   
+00003d10: 200a 2020 2020 2d20 6c69 7374 6675 6e64   .    - listfund
+00003d20: 202d 3e20 4c69 7374 6120 646f 7320 6675   -> Lista dos fu
+00003d30: 6e64 6f73 2070 6172 6120 616e 616c 6973  ndos para analis
+00003d40: 6520 6465 2072 6973 636f 0a20 2020 202d  e de risco.    -
+00003d50: 2066 756e 645f 3120 2d3e 2050 7269 6d65   fund_1 -> Prime
+00003d60: 6972 6f20 6675 6e64 6f20 7061 7261 2061  iro fundo para a
+00003d70: 6e61 6c69 7365 2075 6e69 6361 0a20 2020  nalise unica.   
+00003d80: 202d 2066 756e 645f 3220 2d3e 2053 6567   - fund_2 -> Seg
+00003d90: 756e 646f 2066 756e 646f 2070 6172 6120  undo fundo para 
+00003da0: 616e 616c 6973 6520 756e 6963 610a 2020  analise unica.  
+00003db0: 2020 0a20 2020 2023 2320 4578 656d 706c    .    ## Exempl
+00003dc0: 6f73 3a0a 2020 2020 0a20 2020 2060 6060  os:.    .    ```
+00003dd0: 0a20 2020 203e 3e3e 2062 622e 636f 6d70  .    >>> bb.comp
+00003de0: 6172 655f 6675 6e64 7328 6c69 7374 6675  are_funds(listfu
+00003df0: 6e64 3d20 6c69 7374 2920 0a20 2020 2020  nd= list) .     
+00003e00: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00003e10: 750a 2020 2020 3e3e 3e20 6262 2e63 6f6d  u.    >>> bb.com
+00003e20: 7061 7265 5f66 756e 6473 2866 756e 645f  pare_funds(fund_
+00003e30: 313d 2027 6675 6e64 3127 2c20 6675 6e64  1= 'fund1', fund
+00003e40: 5f32 3d20 2766 756e 6432 2729 0a20 2020  _2= 'fund2').   
+00003e50: 2060 6060 0a20 2020 200a 2020 2020 4e72   ```.    .    Nr
+00003e60: 9c00 0000 729d 0000 0072 9e00 0000 7201  ....r....r....r.
+00003e70: 0000 0072 9f00 0000 6301 0000 0000 0000  ...r....c.......
+00003e80: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
+00003e90: 0073 0800 0000 7c00 6401 1700 5300 72a0  .s....|.d...S.r.
+00003ea0: 0000 0072 1f00 0000 72a2 0000 0072 1f00  ...r....r....r..
+00003eb0: 0000 721f 0000 0072 2000 0000 72a4 0000  ..r....r ...r...
+00003ec0: 00d0 0200 0072 a500 0000 7a1f 636f 6d70  .....r....z.comp
+00003ed0: 6172 655f 6675 6e64 732e 3c6c 6f63 616c  are_funds.<local
+00003ee0: 733e 2e3c 6c61 6d62 6461 3e29 0872 9f00  s>.<lambda>).r..
+00003ef0: 0000 72a7 0000 0072 a800 0000 72a9 0000  ..r....r....r...
+00003f00: 0072 aa00 0000 72ab 0000 007a 0e44 6976  .r....r....z.Div
+00003f10: 6964 656e 6420 5969 656c 647a 1144 5920  idend Yieldz.DY 
+00003f20: 2833 4d29 2041 6375 6d75 6c61 646f 2901  (3M) Acumulado).
+00003f30: 5a06 7375 6273 6574 753e 0000 004e 616f  Z.subsetu>...Nao
+00003f40: 2066 6f72 616d 2061 7072 6573 656e 7461   foram apresenta
+00003f50: 646f 2064 6164 6f73 2064 6f73 2066 756e  do dados dos fun
+00003f60: 646f 7320 7061 7261 2076 6572 6966 6963  dos para verific
+00003f70: 61c3 a761 6f20 756e 6963 6172 2500 0000  a..ao unicar%...
+00003f80: 7218 0000 0072 4d00 0000 723b 0000 0072  r....rM...r;...r
+00003f90: 4700 0000 7252 0000 0029 025a 0446 756e  G...rR...).Z.Fun
+00003fa0: 647a 0c4d 6178 2072 6973 6b20 2825 2972  dz.Max risk (%)r
+00003fb0: 7e00 0000 7542 0000 004e 616f 2066 6f72  ~...uB...Nao for
+00003fc0: 616d 2061 7072 6573 656e 7461 646f 2064  am apresentado d
+00003fd0: 6164 6f73 2064 6f73 2066 756e 646f 7320  ados dos fundos 
+00003fe0: 7061 7261 2076 6572 6966 6963 61c3 a761  para verifica..a
+00003ff0: 6f20 6dc3 ba6c 7469 706c 6129 1572 ac00  o m..ltipla).r..
+00004000: 0000 72ad 0000 0072 0a00 0000 72ae 0000  ..r....r....r...
+00004010: 0072 af00 0000 7242 0000 0072 b000 0000  .r....rB...r....
+00004020: 7281 0000 0072 b100 0000 da0f 6472 6f70  r....r......drop
+00004030: 5f64 7570 6c69 6361 7465 7372 b200 0000  _duplicatesr....
+00004040: 7283 0000 0072 4000 0000 722e 0000 0072  r....r@...r....r
+00004050: 2900 0000 722a 0000 0072 3f00 0000 726d  )...r*...r?...rm
+00004060: 0000 0072 7400 0000 7243 0000 0072 8200  ...rt...rC...r..
+00004070: 0000 2912 5a08 6c69 7374 6675 6e64 5a06  ..).Z.listfundZ.
+00004080: 6675 6e64 5f31 5a06 6675 6e64 5f32 72b3  fund_1Z.fund_2r.
+00004090: 0000 0072 b400 0000 72b5 0000 0072 9e00  ...r....r....r..
+000040a0: 0000 72b6 0000 005a 0566 756e 6431 5a05  ..r....Z.fund1Z.
+000040b0: 6675 6e64 32da 0475 6e69 745a 096d 6178  fund2..unitZ.max
+000040c0: 5f72 6973 636f 5a10 7469 636b 6572 5f6d  _riscoZ.ticker_m
+000040d0: 6178 5f72 6973 636f 7279 0000 005a 0566  ax_riscory...Z.f
+000040e0: 756e 646f 721e 0000 0072 ba00 0000 5a09  undor....r....Z.
+000040f0: 7661 6c75 6572 6973 6b72 1f00 0000 721f  valueriskr....r.
+00004100: 0000 0072 2000 0000 da0d 636f 6d70 6172  ...r .....compar
+00004110: 655f 6675 6e64 73b1 0200 0073 4400 0000  e_funds....sD...
+00004120: 0019 0c01 0401 0a01 0c01 0e01 1201 1601  ................
+00004130: 0c01 0e02 1201 1202 0e01 0601 0a02 0402  ................
+00004140: 0801 0602 0401 0401 0801 0a01 0c01 1001  ................
+00004150: 0801 0401 0602 0601 06ff 0401 08ff 0603  ................
+00004160: 0801 0a02 72be 0000 007a 0b2f 6265 7374  ....r....z./best
+00004170: 4173 7365 7473 6301 0000 0000 0000 0000  Assetsc.........
+00004180: 0000 0019 0000 0005 0000 0043 0000 0073  ...........C...s
+00004190: fa02 0000 6401 7d01 7400 a001 7c01 a101  ....d.}.t...|...
+000041a0: 7d02 7c02 6a02 6402 6b03 7224 7403 6403  }.|.j.d.k.r$t.d.
+000041b0: 8301 0100 9002 6ed2 7404 7c02 6a05 6404  ......n.t.|.j.d.
+000041c0: 8302 7d03 7c03 a006 6405 a101 6406 1900  ..}.|...d...d...
+000041d0: 7d04 7407 6a08 7409 7c04 8301 6407 6408  }.t.j.t.|...d.d.
+000041e0: 6409 8d03 6406 1900 7d05 7c05 640a 1900  d...d...}.|.d...
+000041f0: a00a 640b 640c 8400 a101 7c05 640a 3c00  ..d.d.....|.d.<.
+00004200: 7403 640d 8301 0100 740b 6a0c 7c05 640a  t.d.....t.j.|.d.
+00004210: 1900 a00d a100 640e 640f 8d02 6410 1900  ......d.d...d...
+00004220: 7d06 6411 6412 8400 7d07 6413 6414 8400  }.d.d...}.d.d...
+00004230: 7d08 6900 7d09 6900 7d0a 7c06 6a0e 4400  }.i.}.i.}.|.j.D.
+00004240: 5d24 7d0b 7c06 7c0b 1900 7d0c 7c07 7c0c  ]$}.|.|...}.|.|.
+00004250: 8301 7c09 7c0b 3c00 7c08 7c0c 8301 7c0a  ..|.|.<.|.|...|.
+00004260: 7c0b 3c00 71ac 7c00 6415 6b02 9001 7288  |.<.q.|.d.k...r.
+00004270: 6700 7d0d 7c06 6a0e 4400 5d26 7d0b 7c09  g.}.|.j.D.]&}.|.
+00004280: 7c0b 1900 6416 6b04 72e6 7c0a 7c0b 1900  |...d.k.r.|.|...
+00004290: 6417 6b04 72e6 7c0d a00f 7c0b a101 0100  d.k.r.|...|.....
+000042a0: 71e6 7407 6a10 7c0d 6418 6701 6419 8d02  q.t.j.|.d.g.d...
+000042b0: 7d0e 7403 641a 8301 0100 7411 7c0d 7412  }.t.d.....t.|.t.
+000042c0: 7413 641b 8d03 7d0f 7c0f 6701 7d0f 7407  t.d...}.|.g.}.t.
+000042d0: a010 7c0f a101 7d10 7c10 a014 641c a101  ..|...}.|...d...
+000042e0: 7d10 7c10 641d 1900 a015 a100 a016 a100  }.|.d...........
+000042f0: 7c10 641d 3c00 7c10 641e 1900 a015 a100  |.d.<.|.d.......
+00004300: a016 a100 7c10 641e 3c00 7c10 6a17 9001  ....|.d.<.|.j...
+00004310: 7280 6e04 7c10 5300 9001 6e6e 7c00 641f  r.n.|.S...nn|.d.
+00004320: 6b02 9002 7242 6700 7d11 7c06 6a0e 4400  k...rBg.}.|.j.D.
+00004330: 5d2c 7d0b 7c09 7c0b 1900 6420 6b04 9001  ],}.|.|...d k...
+00004340: 729c 7c0a 7c0b 1900 6421 6b00 9001 729c  r.|.|...d!k...r.
+00004350: 7c11 a00f 7c0b a101 0100 9001 719c 7407  |...|.......q.t.
+00004360: 6a10 7c11 6422 6701 6419 8d02 7d12 7403  j.|.d"g.d...}.t.
+00004370: 641a 8301 0100 7411 7c11 7412 7413 641b  d.....t.|.t.t.d.
+00004380: 8d03 7d13 7c13 6701 7d13 7407 a010 7c13  ..}.|.g.}.t...|.
+00004390: a101 7d14 7c14 a014 641c a101 7d14 7c14  ..}.|...d...}.|.
+000043a0: 641d 1900 a015 a100 a016 a100 7c14 641d  d...........|.d.
+000043b0: 3c00 7c14 641e 1900 a015 a100 a016 a100  <.|.d...........
+000043c0: 7c14 641e 3c00 7c14 6a17 9002 723c 6e04  |.d.<.|.j...r<n.
+000043d0: 7c14 5300 6eb4 7c00 6423 6b02 9002 72ee  |.S.n.|.d#k...r.
+000043e0: 6700 7d15 7c06 6a0e 4400 5d1e 7d0b 7c0a  g.}.|.j.D.].}.|.
+000043f0: 7c0b 1900 6417 6b00 9002 7256 7c15 a00f  |...d.k...rV|...
+00004400: 7c0b a101 0100 9002 7156 7407 6a10 7c15  |.......qVt.j.|.
+00004410: 6424 6701 6419 8d02 7d16 7403 641a 8301  d$g.d...}.t.d...
+00004420: 0100 7411 7c15 7412 7413 641b 8d03 7d17  ..t.|.t.t.d...}.
+00004430: 7c17 6701 7d17 7407 a010 7c17 a101 7d18  |.g.}.t...|...}.
+00004440: 7c18 a014 641c a101 7d18 7c18 641d 1900  |...d...}.|.d...
+00004450: a015 a100 a016 a100 7c18 641d 3c00 7c18  ........|.d.<.|.
+00004460: 641e 1900 a015 a100 a016 a100 7c18 641e  d...........|.d.
+00004470: 3c00 7c18 6a17 9002 72e8 6e04 7c18 5300  <.|.j...r.n.|.S.
+00004480: 6e08 7403 6425 8301 0100 6426 5300 2927  n.t.d%....d&S.)'
+00004490: 750c 0200 000a 2020 2020 2323 2055 7361  u.....    ## Usa
+000044a0: 6269 6c69 6461 6465 0a20 2020 202d 2046  bilidade.    - F
+000044b0: 756e c3a7 c3a3 6f20 7175 6520 616e 616c  un....o que anal
+000044c0: 6973 6120 6f73 2070 7269 6e63 6970 6169  isa os principai
+000044d0: 7320 6174 6976 6f73 206c 6973 7461 646f  s ativos listado
+000044e0: 7320 6e6f 206d 6572 6361 646f 2071 7565  s no mercado que
+000044f0: 2063 6f6d 2062 6173 6520 6e6f 2070 6572   com base no per
+00004500: 6669 6c20 6573 636f 6c68 6964 6f20 6d6f  fil escolhido mo
+00004510: 7374 7261 2071 7561 6973 2070 6f64 656d  stra quais podem
+00004520: 2073 6572 2073 7561 7320 6573 636f 6c68   ser suas escolh
+00004530: 6173 2065 2071 7561 6e74 6f73 2070 6f72  as e quantos por
+00004540: 6365 6e74 6f20 7365 2064 6576 6520 7465  cento se deve te
+00004550: 7220 6e61 2063 6172 7465 6972 610a 2020  r na carteira.  
+00004560: 2020 0a20 2020 2023 2320 5061 72c3 a26d    .    ## Par..m
+00004570: 6574 726f 730a 2020 2020 0a20 2020 202d  etros.    .    -
+00004580: 2070 6572 6669 6c20 2d3e 2050 6572 6669   perfil -> Perfi
+00004590: 7320 7175 6520 706f 6465 6d20 7365 7220  s que podem ser 
+000045a0: 6573 636f 6c68 6964 6f73 2070 6172 6120  escolhidos para 
+000045b0: 7265 616c 697a 6172 2061 2061 6ec3 a16c  realizar a an..l
+000045c0: 6973 652c 2073 6567 7565 2061 206c 6973  ise, segue a lis
+000045d0: 7461 3a20 0a0a 2020 2020 0a20 2020 2060  ta: ..    .    `
+000045e0: 6060 0a20 2020 2054 6970 6f50 6572 6669  ``.    TipoPerfi
+000045f0: 733a 0a20 2020 202a 2041 6772 6573 7369  s:.    * Agressi
+00004600: 766f 0a20 2020 202a 204d 6f64 6572 6164  vo.    * Moderad
+00004610: 6f0a 2020 2020 2a20 436f 6e73 6572 7661  o.    * Conserva
+00004620: 646f 720a 2020 2020 0a20 2020 2060 6060  dor.    .    ```
+00004630: 0a20 2020 200a 2020 2020 2323 2045 7865  .    .    ## Exe
+00004640: 6d70 6c6f 0a20 2020 200a 2020 2020 6060  mplo.    .    ``
+00004650: 600a 2020 2020 0a20 2020 203e 3e3e 2061  `.    .    >>> a
+00004660: 6c6f 6361 7469 6f6e 203d 2062 6573 745f  location = best_
+00004670: 6173 7365 7473 2870 6572 6669 6c3d 2741  assets(perfil='A
+00004680: 6772 6573 7369 766f 2729 0a20 2020 200a  gressivo').    .
+00004690: 2020 2020 6060 600a 2020 2020 0a20 2020      ```.    .   
+000046a0: 207a 2d68 7474 7073 3a2f 2f77 7777 2e64   z-https://www.d
+000046b0: 6164 6f73 6465 6d65 7263 6164 6f2e 636f  adosdemercado.co
+000046c0: 6d2e 6272 2f62 6f6c 7361 2f61 636f 6573  m.br/bolsa/acoes
+000046d0: 7250 0000 007a 3141 6365 7373 6f20 6e65  rP...z1Acesso ne
+000046e0: 6761 646f 2061 2062 6173 652c 2074 656e  gado a base, ten
+000046f0: 7465 206e 6f76 616d 656e 7465 206d 6169  te novamente mai
+00004700: 7320 7461 7264 652e 729d 0000 0072 9e00  s tarde.r....r..
+00004710: 0000 7201 0000 00fa 012c 721a 0000 00a9  ..r......,r.....
+00004720: 02da 0764 6563 696d 616c 5a09 7468 6f75  ...decimalZ.thou
+00004730: 7361 6e64 73f5 0700 0000 43c3 b364 6967  sands.....C..dig
+00004740: 6f63 0100 0000 0000 0000 0000 0000 0100  oc..............
+00004750: 0000 0200 0000 5300 0000 7308 0000 007c  ......S...s....|
+00004760: 0064 0117 0053 0072 a000 0000 721f 0000  .d...S.r....r...
+00004770: 0072 a200 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00004780: 7220 0000 0072 a400 0000 1f03 0000 72a5  r ...r........r.
+00004790: 0000 007a 1d62 6573 745f 6173 7365 7473  ...z.best_assets
+000047a0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+000047b0: 613e 7a13 4275 7363 616e 646f 2061 7469  a>z.Buscando ati
+000047c0: 766f 732e 2e2e 2e72 3900 0000 723b 0000  vos....r9...r;..
+000047d0: 0072 4700 0000 6301 0000 0000 0000 0000  .rG...c.........
+000047e0: 0000 0003 0000 0002 0000 0053 0000 0073  ...........S...s
+000047f0: 1400 0000 7c00 a000 a100 7d01 7c01 a001  ....|.....}.|...
+00004800: a100 7d02 7c02 5300 a901 4e29 0272 6d00  ..}.|.S...N).rm.
+00004810: 0000 7257 0000 0029 03da 0670 7265 636f  ..rW...)...preco
+00004820: 73da 0772 6574 6f72 6e6f 5a0d 7265 746f  s..retornoZ.reto
+00004830: 726e 6f5f 6d65 6469 6f72 1f00 0000 721f  rno_medior....r.
+00004840: 0000 0072 2000 0000 da10 6361 6c63 756c  ...r .....calcul
+00004850: 6172 5f72 6574 6f72 6e6f 2403 0000 7306  ar_retorno$...s.
+00004860: 0000 0000 0108 0108 017a 2562 6573 745f  .........z%best_
+00004870: 6173 7365 7473 2e3c 6c6f 6361 6c73 3e2e  assets.<locals>.
+00004880: 6361 6c63 756c 6172 5f72 6574 6f72 6e6f  calcular_retorno
+00004890: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+000048a0: 0002 0000 0053 0000 0073 1400 0000 7c00  .....S...s....|.
+000048b0: a000 a100 7d01 7c01 a001 a100 7d02 7c02  ....}.|.....}.|.
+000048c0: 5300 72c3 0000 0029 0272 6d00 0000 7274  S.r....).rm...rt
+000048d0: 0000 0029 0372 c400 0000 72c5 0000 0072  ...).r....r....r
+000048e0: 9900 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
+000048f0: 0000 00da 0e63 616c 6375 6c61 725f 7269  .....calcular_ri
+00004900: 7363 6f2a 0300 0073 0600 0000 0001 0801  sco*...s........
+00004910: 0801 7a23 6265 7374 5f61 7373 6574 732e  ..z#best_assets.
+00004920: 3c6c 6f63 616c 733e 2e63 616c 6375 6c61  <locals>.calcula
+00004930: 725f 7269 7363 6f5a 0941 6772 6573 7369  r_riscoZ.Agressi
+00004940: 766f 672d 431c ebe2 361a 3f67 7b14 ae47  vog-C...6.?g{..G
+00004950: e17a 843f 7a12 4174 6976 6f73 2050 2f41  .z.?z.Ativos P/A
+00004960: 6772 6573 7369 766f a901 da07 636f 6c75  gressivo....colu
+00004970: 6d6e 737a 3f52 6561 6c69 7a61 6e64 6f20  mnsz?Realizando 
+00004980: 6361 6c63 756c 6f73 2070 6172 6120 6120  calculos para a 
+00004990: 7375 6120 6361 7274 6569 7261 2063 6f6d  sua carteira com
+000049a0: 2062 6173 6520 6e6f 2073 6575 2070 6572   base no seu per
+000049b0: 6669 6c2e 2902 7288 0000 0072 6000 0000  fil.).r....r`...
+000049c0: 728b 0000 0072 8900 0000 728a 0000 005a  r....r....r....Z
+000049d0: 084d 6f64 6572 6164 6f67 6132 5530 2aa9  .Moderadoga2U0*.
+000049e0: 333f 67b8 1e85 eb51 b89e 3f7a 1141 7469  3?g....Q..?z.Ati
+000049f0: 766f 7320 502f 4d6f 6465 7261 646f 5a0b  vos P/ModeradoZ.
+00004a00: 436f 6e73 6572 7661 646f 727a 1441 7469  Conservadorz.Ati
+00004a10: 766f 7320 502f 436f 6e73 6572 7661 646f  vos P/Conservado
+00004a20: 7275 5a00 0000 5065 7266 696c 206e c3a3  ruZ...Perfil n..
+00004a30: 6f20 7265 636f 6e68 6563 6964 6f2c 206f  o reconhecido, o
+00004a40: 7320 7065 7266 6973 2064 6973 706f 6e69  s perfis disponi
+00004a50: 7665 6973 2065 7374 616f 2070 7265 7365  veis estao prese
+00004a60: 6e74 6573 206e 6120 6578 706c 6963 61c3  ntes na explica.
+00004a70: a7c3 a36f 2064 6120 6675 6ec3 a7c3 a36f  ...o da fun....o
+00004a80: 4e29 1872 ac00 0000 72ad 0000 005a 0b73  N).r....r....Z.s
+00004a90: 7461 7475 735f 636f 6465 722e 0000 0072  tatus_coder....r
+00004aa0: 0a00 0000 72ae 0000 0072 af00 0000 7242  ....r....r....rB
+00004ab0: 0000 0072 b000 0000 7281 0000 0072 b100  ...r....r....r..
+00004ac0: 0000 7229 0000 0072 6500 0000 da06 746f  ..r)...re.....to
+00004ad0: 6c69 7374 72c9 0000 0072 9700 0000 7243  listr....r....rC
+00004ae0: 0000 0072 9b00 0000 da04 6f6e 6559 da09  ...r......oneY..
+00004af0: 6375 7272 656e 746c 795a 0765 7870 6c6f  currentlyZ.explo
+00004b00: 6465 72bc 0000 0072 8c00 0000 7240 0000  der....r....r@..
+00004b10: 0029 195a 0670 6572 6669 6c72 b300 0000  .).Z.perfilr....
+00004b20: 72b4 0000 0072 b500 0000 729e 0000 0072  r....r....r....r
+00004b30: b600 0000 72c4 0000 0072 c600 0000 72c7  ....r....r....r.
+00004b40: 0000 0072 c500 0000 7299 0000 00da 0561  ...r....r......a
+00004b50: 7469 766f 5a0c 7072 6563 6f73 5f61 7469  tivoZ.precos_ati
+00004b60: 766f 5a09 6167 7265 7373 6976 6f5a 0b44  voZ.agressivoZ.D
+00004b70: 6641 6772 6573 7369 766f 5a13 616c 6f63  fAgressivoZ.aloc
+00004b80: 6174 696f 6e5f 4167 7265 7373 6976 655a  ation_AgressiveZ
+00004b90: 1764 6174 6141 6c6f 6361 7469 6f6e 5f41  .dataAlocation_A
+00004ba0: 6772 6573 7369 7665 5a08 6d6f 6465 7261  gressiveZ.modera
+00004bb0: 646f 5a0a 4466 4d6f 6465 7261 646f 5a12  doZ.DfModeradoZ.
+00004bc0: 616c 6f63 6174 696f 6e5f 4d6f 6465 7261  alocation_Modera
+00004bd0: 6465 5a16 6461 7461 416c 6f63 6174 696f  deZ.dataAlocatio
+00004be0: 6e5f 4d6f 6465 7261 6465 5a0b 636f 6e73  n_ModeradeZ.cons
+00004bf0: 6572 7661 646f 725a 0d44 6643 6f6e 7365  ervadorZ.DfConse
+00004c00: 7276 6164 6f72 5a16 616c 6f63 6174 696f  rvadorZ.alocatio
+00004c10: 6e5f 436f 6e73 6572 7661 7469 7665 5a1a  n_ConservativeZ.
+00004c20: 6461 7461 416c 6f63 6174 696f 6e5f 436f  dataAlocation_Co
+00004c30: 6e73 6572 7661 7469 7665 721f 0000 0072  nservativer....r
+00004c40: 1f00 0000 7220 0000 00da 0b62 6573 745f  ....r .....best_
+00004c50: 6173 7365 7473 f902 0000 7386 0000 0000  assets....s.....
+00004c60: 1e04 010a 010a 010c 020c 010e 0118 0116  ................
+00004c70: 0108 011a 0308 0608 0604 0104 010a 0108  ................
+00004c80: 010c 010e 030a 0104 010a 0118 010c 0210  ................
+00004c90: 0108 010e 0106 010a 010a 0414 0114 0208  ................
+00004ca0: 0102 0208 020a 0204 010a 011c 010e 0210  ................
+00004cb0: 0108 010e 0106 010a 010a 0414 0114 0208  ................
+00004cc0: 0102 0206 020a 0204 010a 010e 010e 0110  ................
+00004cd0: 0208 010e 0106 010a 010a 0314 0114 0208  ................
+00004ce0: 0102 0206 0272 ce00 0000 7a11 2f62 6573  .....r....z./bes
+00004cf0: 7441 7373 6574 7356 616c 7565 7363 0100  tAssetsValuesc..
+00004d00: 0000 0000 0000 0000 0000 1100 0000 0600  ................
+00004d10: 0000 0300 0000 7344 0200 0074 00a0 01a1  ......sD...t....
+00004d20: 0001 0074 0283 007d 017c 01a0 0364 01a1  ...t...}.|...d..
+00004d30: 0101 0074 046a 057c 0164 028d 017d 0264  ...t.j.|.d...}.d
+00004d40: 037d 037c 02a0 067c 03a1 0101 0074 07a0  .}.|...|.....t..
+00004d50: 0864 04a1 0101 007c 02a0 0974 0a6a 0b64  .d.....|...t.j.d
+00004d60: 05a1 02a0 0ca1 007d 047c 026a 0da0 0e7c  .......}.|.j...|
+00004d70: 02a0 0974 0a6a 0f64 06a1 02a1 0101 007c  ...t.j.d.......|
+00004d80: 02a0 0974 0a6a 0f64 07a1 02a0 0ca1 007d  ...t.j.d.......}
+00004d90: 057c 02a0 0974 0a6a 1064 08a1 02a0 0ca1  .|...t.j.d......
+00004da0: 007d 0674 07a0 0864 09a1 0101 007c 02a0  .}.t...d.....|..
+00004db0: 0974 0a6a 1064 0aa1 027d 077c 07a0 1164  .t.j.d...}.|...d
+00004dc0: 0ba1 017d 0874 126a 1374 147c 0883 0164  ...}.t.j.t.|...d
+00004dd0: 0c64 0d64 0e8d 037d 097c 0964 0f19 007d  .d.d...}.|.d...}
+00004de0: 097c 0964 1064 1167 0219 007d 097c 09a0  .|.d.d.g...}.|..
+00004df0: 1564 1264 1367 02a1 017d 097c 0964 1019  .d.d.g...}.|.d..
+00004e00: 00a0 1664 1464 1584 00a1 017c 0964 103c  ...d.d.....|.d.<
+00004e10: 0074 176a 187c 0964 1019 00a0 19a1 0064  .t.j.|.d.......d
+00004e20: 1664 178d 0264 1819 007d 0a7c 0a6a 1a64  .d...d...}.|.j.d
+00004e30: 1964 1a8d 017d 0a7c 0aa0 1ba1 00a0 1ca1  .d...}.|........
+00004e40: 0064 1b14 0089 007c 0aa0 1ba1 00a0 1da1  .d.....|........
+00004e50: 0074 1ea0 1f64 1ba1 0114 007d 0b74 12a0  .t...d.....}.t..
+00004e60: 2088 007c 0b64 1c9c 02a1 017d 0c7c 0c64   ..|.d.....}.|.d
+00004e70: 1d19 007c 0c64 1e19 001b 007c 0c64 1f3c  ...|.d.....|.d.<
+00004e80: 007c 0c6a 2164 1f64 2064 218d 02a0 2264  .|.j!d.d d!..."d
+00004e90: 22a1 017d 0c7c 0c64 1f19 007c 0c64 1f19  "..}.|.d...|.d..
+00004ea0: 00a0 23a1 001b 007c 0c64 233c 007c 0c64  ..#....|.d#<.|.d
+00004eb0: 2319 0088 0114 007c 0c64 243c 007c 0ca0  #......|.d$<.|..
+00004ec0: 24a1 007d 0c7c 0c6a 2564 2564 2664 279c  $..}.|.j%d%d&d'.
+00004ed0: 0264 288d 017d 0c7c 0c64 2519 0044 005d  .d(..}.|.d%..D.]
+00004ee0: 427d 0d74 176a 187c 0d64 1664 178d 027d  B}.t.j.|.d.d...}
+00004ef0: 0e7c 0e64 1819 006a 2664 2919 007c 0e64  .|.d...j&d)..|.d
+00004f00: 1819 006a 2664 0f19 0018 007c 0e64 1819  ...j&d.....|.d..
+00004f10: 006a 2664 0f19 001b 0088 007c 0d3c 0090  .j&d.......|.<..
+00004f20: 0171 c487 0087 0166 0264 2a64 2b84 087c  .q.....f.d*d+..|
+00004f30: 0c64 2519 0044 0083 017d 0f7c 0fa0 27a1  .d%..D...}.|..'.
+00004f40: 007d 1074 287c 1083 017d 107c 107c 0c64  .}.t(|...}.|.|.d
+00004f50: 2c3c 007c 0c67 0064 2da2 0119 0053 0029  ,<.|.g.d-....S.)
+00004f60: 2e75 1a02 0000 0a20 2020 2023 2320 5573  .u.....    ## Us
+00004f70: 6162 696c 6964 6164 650a 2020 2020 2d20  abilidade.    - 
+00004f80: 4675 6ec3 a7c3 a36f 2071 7565 2061 6e61  Fun....o que ana
+00004f90: 6c69 7361 206f 7320 6174 6976 6f73 2064  lisa os ativos d
+00004fa0: 6f20 4942 4f56 4553 5041 2071 7565 2063  o IBOVESPA que c
+00004fb0: 6f6d 2062 6173 6520 6e6f 2076 616c 6f72  om base no valor
+00004fc0: 2064 6520 696e 7665 7374 696d 656e 746f   de investimento
+00004fd0: 2065 7363 6f6c 6869 646f 206d 6f73 7472   escolhido mostr
+00004fe0: 6120 7175 6169 7320 706f 6465 6d20 7365  a quais podem se
+00004ff0: 7220 7375 6173 2065 7363 6f6c 6861 732c  r suas escolhas,
+00005000: 206f 2071 7561 6e74 6f20 6972 6120 7465   o quanto ira te
+00005010: 7220 7175 6520 696e 7665 7374 6972 2070  r que investir p
+00005020: 6172 6120 6361 6461 2061 7469 766f 2065  ara cada ativo e
+00005030: 206f 2072 6574 6f72 6e6f 2061 7072 6f78   o retorno aprox
+00005040: 696d 6164 6f20 7061 7261 2063 6164 6120  imado para cada 
+00005050: 756d 2064 656c 6573 200a 0a20 2020 202d  um deles ..    -
+00005060: 2055 7361 6d6f 7320 636f 6d6f 206d 6574   Usamos como met
+00005070: 6f64 6f20 6465 2063 c3a1 6c63 756c 6f20  odo de c..lculo 
+00005080: 6f20 6120 6d65 6469 6461 2053 6861 7270  o a medida Sharp
+00005090: 6520 7175 6520 6e61 6461 206d 6169 7320  e que nada mais 
+000050a0: c3a9 2071 7565 2075 6d61 2020 6d65 6469  .. que uma  medi
+000050b0: 6461 2064 6520 6465 7365 6d70 656e 686f  da de desempenho
+000050c0: 2064 6520 696e 7665 7374 696d 656e 746f   de investimento
+000050d0: 7320 7175 6520 6c65 7661 2065 6d20 636f  s que leva em co
+000050e0: 6e73 6964 6572 61c3 a7c3 a36f 206f 2072  nsidera....o o r
+000050f0: 6574 6f72 6e6f 206f 6274 6964 6f20 7065  etorno obtido pe
+00005100: 6c6f 2069 6e76 6573 7469 6d65 6e74 6f20  lo investimento 
+00005110: 656d 2072 656c 61c3 a7c3 a36f 2061 6f20  em rela....o ao 
+00005120: 7269 7363 6f20 6173 7375 6d69 646f 0a20  risco assumido. 
+00005130: 2020 2023 2320 5061 72c3 a26d 6574 726f     ## Par..metro
+00005140: 730a 2020 2020 0a20 2020 202d 2076 616c  s.    .    - val
+00005150: 6f72 202d 3e20 5661 6c6f 7220 646f 2069  or -> Valor do i
+00005160: 6e76 6573 7469 6d65 6e74 6f2c 2070 6f72  nvestimento, por
+00005170: 2070 6164 72c3 a36f 2030 0a0a 2020 2020   padr..o 0..    
+00005180: fa0a 2d2d 6865 6164 6c65 7373 a901 da07  ..--headless....
+00005190: 6f70 7469 6f6e 737a 7c68 7474 7073 3a2f  optionsz|https:/
+000051a0: 2f77 7777 2e62 332e 636f 6d2e 6272 2f70  /www.b3.com.br/p
+000051b0: 745f 6272 2f6d 6172 6b65 742d 6461 7461  t_br/market-data
+000051c0: 2d65 2d69 6e64 6963 6573 2f69 6e64 6963  -e-indices/indic
+000051d0: 6573 2f69 6e64 6963 6573 2d61 6d70 6c6f  es/indices-amplo
+000051e0: 732f 696e 6469 6365 2d69 626f 7665 7370  s/indice-ibovesp
+000051f0: 612d 6962 6f76 6573 7061 2d63 6f6d 706f  a-ibovespa-compo
+00005200: 7369 6361 6f2d 6461 2d63 6172 7465 6972  sicao-da-carteir
+00005210: 612e 6874 6d72 7300 0000 7a1b 6f6e 6574  a.htmrs...z.onet
+00005220: 7275 7374 2d61 6363 6570 742d 6274 6e2d  rust-accept-btn-
+00005230: 6861 6e64 6c65 727a 162f 2f2a 5b40 6964  handlerz.//*[@id
+00005240: 3d22 6276 6d66 5f69 6672 616d 6522 5d7a  ="bvmf_iframe"]z
+00005250: 152f 2f2a 5b40 6964 3d22 7365 6c65 6374  .//*[@id="select
+00005260: 5061 6765 225d 7a21 2373 656c 6563 7450  Page"]z!#selectP
+00005270: 6167 6520 3e20 6f70 7469 6f6e 3a6e 7468  age > option:nth
+00005280: 2d63 6869 6c64 2834 29e7 0000 0000 0000  -child(4).......
+00005290: f83f 7a6c 2364 6976 436f 6e74 6169 6e65  .?zl#divContaine
+000052a0: 7249 6672 616d 6542 3320 3e20 6469 7620  rIframeB3 > div 
+000052b0: 3e20 6469 762e 636f 6c2d 6c67 2d39 2e63  > div.col-lg-9.c
+000052c0: 6f6c 2d31 322e 6f72 6465 722d 322e 6f72  ol-12.order-2.or
+000052d0: 6465 722d 6c67 2d31 203e 2066 6f72 6d20  der-lg-1 > form 
+000052e0: 3e20 6469 763a 6e74 682d 6368 696c 6428  > div:nth-child(
+000052f0: 3429 203e 2064 6976 203e 2074 6162 6c65  4) > div > table
+00005300: da09 6f75 7465 7248 544d 4c72 bf00 0000  ..outerHTMLr....
+00005310: 721a 0000 0072 c000 0000 7201 0000 0072  r....r....r....r
+00005320: c200 0000 7506 0000 0041 c3a7 c3a3 6fe9  ....u....A....o.
+00005330: 5800 0000 e959 0000 0063 0100 0000 0000  X....Y...c......
+00005340: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
+00005350: 0000 7308 0000 007c 0064 0117 0053 0072  ..s....|.d...S.r
+00005360: a000 0000 721f 0000 0072 a200 0000 721f  ....r....r....r.
+00005370: 0000 0072 1f00 0000 7220 0000 0072 a400  ...r....r ...r..
+00005380: 0000 a803 0000 72a5 0000 007a 2362 6573  ......r....z#bes
+00005390: 745f 6173 7365 7473 5f76 616c 7565 2e3c  t_assets_value.<
+000053a0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+000053b0: 7239 0000 0072 3b00 0000 7247 0000 0072  r9...r;...rG...r
+000053c0: 1600 0000 a901 5a04 6178 6973 7264 0000  ......Z.axisrd..
+000053d0: 0029 0272 9800 0000 7299 0000 0072 9800  .).r....r....r..
+000053e0: 0000 7299 0000 005a 0673 6861 7270 6546  ..r....Z.sharpeF
+000053f0: 2901 5a09 6173 6365 6e64 696e 67e9 0600  ).Z.ascending...
+00005400: 0000 5a08 616c 6f63 6163 616f da05 7661  ..Z.alocacao..va
+00005410: 6c6f 72da 0641 7469 766f 73fa 1351 7464  lor..Ativos..Qtd
+00005420: 204e 6563 6573 7361 7269 6120 2852 2429   Necessaria (R$)
+00005430: 2902 727f 0000 0072 d800 0000 72c8 0000  ).r....r....r...
+00005440: 0072 2500 0000 6301 0000 0000 0000 0000  .r%...c.........
+00005450: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
+00005460: 1a00 0000 6900 7c00 5d12 7d01 7c01 8800  ....i.|.].}.|...
+00005470: 7c01 1900 8801 1400 9302 7104 5300 721f  |.........q.S.r.
+00005480: 0000 0072 1f00 0000 2902 da02 2e30 72cd  ...r....)....0r.
+00005490: 0000 00a9 0272 9800 0000 72d8 0000 0072  .....r....r....r
+000054a0: 1f00 0000 7220 0000 00da 0a3c 6469 6374  ....r .....<dict
+000054b0: 636f 6d70 3ecb 0300 0072 a500 0000 7a25  comp>....r....z%
+000054c0: 6265 7374 5f61 7373 6574 735f 7661 6c75  best_assets_valu
+000054d0: 652e 3c6c 6f63 616c 733e 2e3c 6469 6374  e.<locals>.<dict
+000054e0: 636f 6d70 3efa 0e52 6574 6f72 6e6f 2041  comp>..Retorno A
+000054f0: 7072 6f78 2e29 0372 d900 0000 72da 0000  prox.).r....r...
+00005500: 0072 de00 0000 2929 da1a 6368 726f 6d65  .r....))..chrome
+00005510: 6472 6976 6572 5f61 7574 6f69 6e73 7461  driver_autoinsta
+00005520: 6c6c 6572 da07 696e 7374 616c 6c72 0800  ller..installr..
+00005530: 0000 da0c 6164 645f 6172 6775 6d65 6e74  ....add_argument
+00005540: 7206 0000 00da 0643 6872 6f6d 6572 ad00  r......Chromer..
+00005550: 0000 da04 7469 6d65 da05 736c 6565 70da  ....time..sleep.
+00005560: 0c66 696e 645f 656c 656d 656e 7472 0900  .find_elementr..
+00005570: 0000 da02 4944 da05 636c 6963 6b5a 0973  ....ID..clickZ.s
+00005580: 7769 7463 685f 746f da05 6672 616d 655a  witch_to..frameZ
+00005590: 0558 5041 5448 da0c 4353 535f 5345 4c45  .XPATH..CSS_SELE
+000055a0: 4354 4f52 da0d 6765 745f 6174 7472 6962  CTOR..get_attrib
+000055b0: 7574 6572 4200 0000 72b0 0000 0072 8100  uterB...r....r..
+000055c0: 0000 723e 0000 0072 b100 0000 7229 0000  ..r>...r....r)..
+000055d0: 0072 6500 0000 72ca 0000 0072 8c00 0000  .re...r....r....
+000055e0: 726d 0000 0072 5700 0000 7274 0000 0072  rm...rW...rt...r
+000055f0: 6600 0000 7269 0000 0072 4300 0000 5a0b  f...ri...rC...Z.
+00005600: 736f 7274 5f76 616c 7565 73da 0468 6561  sort_values..hea
+00005610: 6472 3000 0000 7245 0000 00da 0672 656e  dr0...rE.....ren
+00005620: 616d 6572 2f00 0000 da06 7661 6c75 6573  amer/.....values
+00005630: 723d 0000 0029 1172 d800 0000 da0e 6368  r=...).r......ch
+00005640: 726f 6d65 5f6f 7074 696f 6e73 da06 6472  rome_options..dr
+00005650: 6976 6572 72b3 0000 005a 0763 6f6f 6b69  iverr....Z.cooki
+00005660: 6573 da06 7365 6c65 6374 da03 616c 6c72  es..select..allr
+00005670: 9e00 0000 da0a 7461 626c 655f 6874 6d6c  ......table_html
+00005680: 5a06 6174 6976 6f73 72c4 0000 0072 9900  Z.ativosr....r..
+00005690: 0000 5a09 6174 6976 6f73 5f64 6672 cd00  ..Z.ativos_dfr..
+000056a0: 0000 7285 0000 005a 1172 6574 6f72 6e6f  ..r....Z.retorno
+000056b0: 5f70 6f72 5f61 7469 766f 5a0c 4c69 7374  _por_ativoZ.List
+000056c0: 6152 6574 6f72 6e6f 721f 0000 0072 dc00  aRetornor....r..
+000056d0: 0000 7220 0000 00da 1162 6573 745f 6173  ..r .....best_as
+000056e0: 7365 7473 5f76 616c 7565 8503 0000 734c  sets_value....sL
+000056f0: 0000 0000 0e08 0106 010a 010c 0204 010a  ................
+00005700: 010a 0112 0116 0112 0112 010a 020e 010a  ................
+00005710: 0114 0108 010c 010e 0216 031a 030c 0310  ................
+00005720: 0116 0310 0314 0314 0318 0310 0108 0212  ................
+00005730: 020c 010e 0132 0318 0108 0108 0208 0372  .....2.........r
+00005740: f300 0000 7a16 2f6f 7074 696f 6e73 2f7b  ....z./options/{
+00005750: 7379 6d62 6f6c 7d2f 696e 666f 2904 7222  symbol}/info).r"
+00005760: 0000 00da 0463 616c 6cda 0370 7574 7223  .....call..putr#
+00005770: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00005780: 0b00 0000 0500 0000 4300 0000 737a 0100  ........C...sz..
+00005790: 007c 00a0 0064 01a1 0172 187c 00a0 0164  .|...d...r.|...d
+000057a0: 0164 02a1 027d 006e 0874 0264 0383 0101  .d...}.n.t.d....
+000057b0: 0074 03a0 04a1 0001 0074 0583 007d 037c  .t.......t...}.|
+000057c0: 03a0 0664 04a1 0101 0074 076a 087c 0364  ...d.....t.j.|.d
+000057d0: 058d 017d 0464 067c 009b 009d 027d 057c  ...}.d.|.....}.|
+000057e0: 04a0 097c 05a1 0101 0074 0aa0 0b64 07a1  ...|.....t...d..
+000057f0: 0101 007c 04a0 0c74 0d6a 0e64 08a1 027d  ...|...t.j.d...}
+00005800: 067c 06a0 0f64 09a1 017d 0774 106a 1174  .|...d...}.t.j.t
+00005810: 127c 0783 0164 0a64 0b64 0c8d 037d 087c  .|...d.d.d...}.|
+00005820: 0864 0d19 007d 087c 0867 0064 0ea2 0119  .d...}.|.g.d....
+00005830: 007d 087c 0164 0f6b 0272 c07c 086a 137c  .}.|.d.k.r.|.j.|
+00005840: 0864 1019 0064 116b 0219 007d 097c 0953  .d...d.k...}.|.S
+00005850: 007c 0264 0f6b 0272 de7c 086a 137c 0864  .|.d.k.r.|.j.|.d
+00005860: 1019 0064 126b 0219 007d 0a7c 0a53 007c  ...d.k...}.|.S.|
+00005870: 04a0 097c 05a1 0101 0074 0aa0 0b64 07a1  ...|.....t...d..
+00005880: 0101 007c 04a0 0c74 0d6a 0e64 08a1 027d  ...|...t.j.d...}
+00005890: 067c 06a0 0f64 09a1 017d 0774 106a 1174  .|...d...}.t.j.t
+000058a0: 127c 0783 0164 0a64 0b64 0c8d 037d 087c  .|...d.d.d...}.|
+000058b0: 0864 0d19 007d 087c 0867 0064 0ea2 0119  .d...}.|.g.d....
+000058c0: 007d 087c 0164 0f6b 0290 0172 527c 086a  .}.|.d.k...rR|.j
+000058d0: 137c 0864 1019 0064 116b 0219 007d 097c  .|.d...d.k...}.|
+000058e0: 0953 007c 0264 0f6b 0290 0172 727c 086a  .S.|.d.k...rr|.j
+000058f0: 137c 0864 1019 0064 126b 0219 007d 0a7c  .|.d...d.k...}.|
+00005900: 0a53 007c 0853 0064 1353 0029 1475 c801  .S.|.S.d.S.).u..
+00005910: 0000 0a20 2020 2023 2320 5573 6162 696c  ...    ## Usabil
+00005920: 6964 6164 650a 0a20 2020 202d 2046 756e  idade..    - Fun
+00005930: c3a7 c3a3 6f20 7175 6520 6170 7265 7365  ....o que aprese
+00005940: 6e74 6120 6173 2070 7269 6e63 6970 6169  nta as principai
+00005950: 7320 696e 666f 726d 61c3 a7c3 b565 7320  s informa....es 
+00005960: 6461 7320 6f70 c3a7 c3b5 6573 2064 6f20  das op....es do 
+00005970: 6174 6976 6f20 7365 6c65 6369 6f6e 6164  ativo selecionad
+00005980: 6f2c 2069 6e66 6f72 6d61 c3a7 c3b5 6573  o, informa....es
+00005990: 2063 6f6d 6f3a 2053 7472 696b 652c 2056   como: Strike, V
+000059a0: 6172 2c20 4772 6567 6173 2c20 6465 6e74  ar, Gregas, dent
+000059b0: 7265 206f 7574 7261 732e 0a0a 2020 2020  re outras...    
+000059c0: 2323 2050 6172 c3a2 6d65 7472 6f73 0a0a  ## Par..metros..
+000059d0: 2020 2020 2d20 7379 6d62 6f6c 202d 3e20      - symbol -> 
+000059e0: 4e6f 6d65 2064 6f20 6174 6976 6f20 7061  Nome do ativo pa
+000059f0: 7261 2062 7573 6361 7220 6173 206f 70c3  ra buscar as op.
+00005a00: a7c3 b565 7320 7265 6665 7265 6e74 6573  ...es referentes
+00005a10: 2061 2065 6c65 2e0a 2020 2020 2d20 6361   a ele..    - ca
+00005a20: 6c6c 202d 3e20 5265 6365 6265 2054 7275  ll -> Recebe Tru
+00005a30: 6520 6f75 2046 616c 7365 2c20 7365 2054  e ou False, se T
+00005a40: 7275 6520 666f 7220 7365 6c65 6369 6f6e  rue for selecion
+00005a50: 6164 6f20 6120 6675 6ec3 a7c3 a36f 2069  ado a fun....o i
+00005a60: 7261 2066 696c 7472 6172 2073 6f20 6173  ra filtrar so as
+00005a70: 2043 414c 4c2e 0a20 2020 202d 2070 7574   CALL..    - put
+00005a80: 202d 3e20 5265 6365 6265 2054 7275 6520   -> Recebe True 
+00005a90: 6f75 2046 616c 7365 2c20 7365 2054 7275  ou False, se Tru
+00005aa0: 6520 666f 7220 7365 6c65 6369 6f6e 6164  e for selecionad
+00005ab0: 6f20 6120 6675 6ec3 a7c3 a36f 2069 7261  o a fun....o ira
+00005ac0: 2066 696c 7472 6172 2073 6f20 6173 2050   filtrar so as P
+00005ad0: 5554 2e0a 0a0a 2020 2020 72a1 0000 0072  UT....    r....r
+00005ae0: 1800 0000 f534 0000 0050 726f 6375 7261  .....4...Procura
+00005af0: 6e64 6f20 6461 646f 7320 6465 206f 70c3  ndo dados de op.
+00005b00: a7c3 b565 7320 646f 2061 7469 766f 2073  ...es do ativo s
+00005b10: 656c 6563 696f 6e61 646f 2e2e 2e72 cf00  elecionado...r..
+00005b20: 0000 72d0 0000 007a 2568 7474 7073 3a2f  ..r....z%https:/
+00005b30: 2f6f 7063 6f65 732e 6e65 742e 6272 2f6f  /opcoes.net.br/o
+00005b40: 7063 6f65 732f 626f 7665 7370 612f 72d2  pcoes/bovespa/r.
+00005b50: 0000 007a 0c23 7462 6c4c 6973 7461 4f70  ...z.#tblListaOp
+00005b60: 6372 d300 0000 72bf 0000 0072 1a00 0000  cr....r....r....
+00005b70: 72c0 0000 0072 0100 0000 290d 722a 0000  r....r....).r*..
+00005b80: 00da 0454 6970 6f5a 0653 7472 696b 657a  ...TipoZ.Strikez
+00005b90: 0741 2f49 2f4f 544d 7a13 4469 7374 2e20  .A/I/OTMz.Dist. 
+00005ba0: 2825 2920 646f 2053 7472 696b 6575 0700  (%) do Strikeu..
+00005bb0: 0000 c39a 6c74 696d 6f7a 0856 6172 2e20  ....ltimoz.Var. 
+00005bc0: 2825 2975 0d00 0000 4ec3 ba6d 2e20 6465  (%)u....N..m. de
+00005bd0: 204e 6567 2e7a 0f56 6f6c 2e20 4669 6e61   Neg.z.Vol. Fina
+00005be0: 6e63 6569 726f da05 4465 6c74 61da 0547  nceiro..Delta..G
+00005bf0: 616d 6d61 7a09 5468 6574 6120 2824 295a  ammaz.Theta ($)Z
+00005c00: 0456 6567 6154 72f7 0000 00da 0443 414c  .VegaTr......CAL
+00005c10: 4cda 0350 5554 4e29 14da 0865 6e64 7377  L..PUTN)...endsw
+00005c20: 6974 6872 1b00 0000 722e 0000 0072 df00  ithr....r....r..
+00005c30: 0000 72e0 0000 0072 0800 0000 72e1 0000  ..r....r....r...
+00005c40: 0072 0600 0000 72e2 0000 0072 ad00 0000  .r....r....r....
+00005c50: 72e3 0000 0072 e400 0000 72e5 0000 0072  r....r....r....r
+00005c60: 0900 0000 72e9 0000 0072 ea00 0000 7242  ....r....r....rB
+00005c70: 0000 0072 b000 0000 7281 0000 0072 b200  ...r....r....r..
+00005c80: 0000 290b 7222 0000 0072 f400 0000 72f5  ..).r"...r....r.
+00005c90: 0000 0072 ee00 0000 72ef 0000 0072 b300  ...r....r....r..
+00005ca0: 0000 729e 0000 0072 f200 0000 5a05 6466  ..r....r....Z.df
+00005cb0: 4f50 435a 0664 6643 616c 6c5a 0564 6650  OPCZ.dfCallZ.dfP
+00005cc0: 7574 721f 0000 0072 1f00 0000 7220 0000  utr....r....r ..
+00005cd0: 00da 0767 6574 5f6f 7063 db03 0000 7346  ...get_opc....sF
+00005ce0: 0000 0000 110a 010e 0208 0208 0106 010a  ................
+00005cf0: 010c 020a 010a 010a 010e 010a 0114 0108  ................
+00005d00: 010c 0108 0112 0104 0108 0112 0104 020a  ................
+00005d10: 010a 020e 010a 0114 0108 040c 010a 0112  ................
+00005d20: 0104 010a 0112 0104 0272 fd00 0000 7a15  .........r....z.
+00005d30: 2f6f 7074 696f 6e73 2f62 6c61 636b 5363  /options/blackSc
+00005d40: 686f 6c65 7329 0272 f400 0000 72f5 0000  holes).r....r...
+00005d50: 0063 0500 0000 0000 0000 0000 0000 0c00  .c..............
+00005d60: 0000 0600 0000 4300 0000 73e8 0000 0074  ......C...s....t
+00005d70: 007c 0174 0174 0283 037d 057c 0564 0114  .|.t.t...}.|.d..
+00005d80: 007d 0664 027d 0774 03a0 047c 027c 031b  .}.d.}.t...|.|..
+00005d90: 00a1 017c 077c 0664 0313 0064 031b 007c  ...|.|.d...d...|
+00005da0: 0414 0017 007c 0674 03a0 057c 04a1 0114  .....|.t...|....
+00005db0: 0014 0017 007d 087c 0674 03a0 057c 04a1  .....}.|.t...|..
+00005dc0: 0114 0004 007d 097d 087c 0064 046b 0272  .....}.}.|.d.k.r
+00005dd0: 9a74 0664 0583 0101 007c 0274 07a0 087c  .t.d.....|.t...|
+00005de0: 08a1 0114 007c 0374 03a0 097c 070b 007c  .....|.t...|...|
+00005df0: 0414 00a1 0114 0074 07a0 087c 09a1 0114  .......t...|....
+00005e00: 0018 007d 0a7c 0a53 007c 0064 066b 0272  ...}.|.S.|.d.k.r
+00005e10: dc74 0664 0783 0101 007c 0374 03a0 097c  .t.d.....|.t...|
+00005e20: 070b 007c 0414 00a1 0114 0074 07a0 087c  ...|.......t...|
+00005e30: 09a1 0114 007c 0274 07a0 087c 080b 00a1  .....|.t...|....
+00005e40: 0114 0018 007d 0b7c 0b53 0074 0664 0883  .....}.|.S.t.d..
+00005e50: 0101 0064 0953 0029 0a75 4a03 0000 0a20  ...d.S.).uJ.... 
+00005e60: 2020 2023 2320 5573 6162 696c 6964 6164     ## Usabilidad
+00005e70: 650a 0a20 2020 202d 2046 756e c3a7 c3a3  e..    - Fun....
+00005e80: 6f20 7175 6520 7369 6d75 6c61 206f 2063  o que simula o c
+00005e90: 6163 756c 6f20 646f 2062 6c61 636b 2d73  aculo do black-s
+00005ea0: 6368 6f6c 6573 2c20 6d6f 6465 6c6f 206e  choles, modelo n
+00005eb0: 6f20 7175 616c 20c3 a920 7574 696c 697a  o qual .. utiliz
+00005ec0: 6164 6f20 7061 7261 2070 7265 6369 6669  ado para precifi
+00005ed0: 6361 7220 6f70 c3a7 c3b5 6573 206e 6f20  car op....es no 
+00005ee0: 6d65 7263 6164 6f20 6465 2064 6572 6976  mercado de deriv
+00005ef0: 6174 6976 6f73 2e0a 2020 2020 2d20 506f  ativos..    - Po
+00005f00: 7220 7365 2074 7261 7461 7220 6465 2075  r se tratar de u
+00005f10: 6d61 2066 756e c3a7 c3a3 6f20 656d 2064  ma fun....o em d
+00005f20: 6573 656e 766f 6c76 696d 656e 746f 206e  esenvolvimento n
+00005f30: c3a3 6f20 6c65 7661 7220 6f20 7265 7375  ..o levar o resu
+00005f40: 6c74 6164 6f20 636f 6d6f 2076 6572 6461  ltado como verda
+00005f50: 6465 2061 6273 6f6c 7574 612c 206d 6173  de absoluta, mas
+00005f60: 2075 6d20 7661 6c6f 7220 6120 7365 2062   um valor a se b
+00005f70: 6173 6561 722e 0a0a 2020 2020 2323 2050  asear...    ## P
+00005f80: 6172 c3a2 6d65 7472 6f73 0a0a 2020 2020  ar..metros..    
+00005f90: 2d20 4361 6c6c 5f6f 725f 5075 7420 2d3e  - Call_or_Put ->
+00005fa0: 2052 6563 6562 6520 6f73 2076 616c 6f72   Recebe os valor
+00005fb0: 6573 2022 6361 6c6c 2220 6520 2270 7574  es "call" e "put
+00005fc0: 222c 2070 6f72 2073 6572 656d 2063 616c  ", por serem cal
+00005fd0: 6375 6c6f 7320 6469 6665 7265 6e74 6573  culos diferentes
+00005fe0: 2070 6172 6164 6120 6361 6461 2074 6970   parada cada tip
+00005ff0: 6f2c 20c3 a920 6e65 6365 7373 6172 696f  o, .. necessario
+00006000: 2061 2073 656c 65c3 a7c3 a36f 0a20 2020   a sele....o.   
+00006010: 202d 2061 7469 766f 202d 3e20 496e 7365   - ativo -> Inse
+00006020: 7269 7220 6f20 6174 6976 6f20 636f 7272  rir o ativo corr
+00006030: 6573 706f 6e64 656e 7465 2064 6120 6675  espondente da fu
+00006040: 6ec3 a7c3 a36f 2028 4578 656d 706c 6f3a  n....o (Exemplo:
+00006050: 2027 5045 5452 342e 5341 2729 0a20 2020   'PETR4.SA').   
+00006060: 202d 2070 7265 636f 202d 3e20 696e 7365   - preco -> inse
+00006070: 7269 7220 6f20 7072 65c3 a76f 2064 6f20  rir o pre..o do 
+00006080: 6174 6976 6f20 7365 6c65 6369 6f6e 6164  ativo selecionad
+00006090: 6f0a 2020 2020 2d20 7374 7269 6b65 202d  o.    - strike -
+000060a0: 3e20 496e 7365 7269 7220 6f20 7374 7269  > Inserir o stri
+000060b0: 6b65 2064 6120 6f70 c3a7 c3a3 6f0a 2020  ke da op....o.  
+000060c0: 2020 2d20 6469 6173 5574 6569 7320 2d3e    - diasUteis ->
+000060d0: 2041 6469 6369 6f6e 6172 2061 2071 7561   Adicionar a qua
+000060e0: 6e74 6964 6164 6520 6465 2064 6961 7320  ntidade de dias 
+000060f0: c3ba 7465 6973 2061 7465 206f 2076 656e  ..teis ate o ven
+00006100: 6369 6d65 6e74 6f20 6461 206f 70c3 a7c3  cimento da op...
+00006110: a36f 2e0a 0a20 2020 2023 2320 4578 656d  .o...    ## Exem
+00006120: 706c 6f0a 0a20 2020 2060 6060 0a20 2020  plo..    ```.   
+00006130: 203e 3e3e 2062 622e 626c 6163 6b5f 7363   >>> bb.black_sc
+00006140: 686f 6c65 7328 4361 6c6c 5f6f 725f 5075  holes(Call_or_Pu
+00006150: 743d 2027 6361 6c6c 272c 2061 7469 766f  t= 'call', ativo
+00006160: 3d20 2750 4554 5234 2e53 4127 2c20 7072  = 'PETR4.SA', pr
+00006170: 6563 6f3d 2032 362e 3235 2c20 7374 7269  eco= 26.25, stri
+00006180: 6b65 3d20 3236 2e32 352c 2064 6961 7355  ke= 26.25, diasU
+00006190: 7465 6973 3d20 3232 2029 0a20 2020 2060  teis= 22 ).    `
+000061a0: 6060 0a0a 2020 2020 6910 f800 0067 c1a8  ``..    i....g..
+000061b0: a44e 40d3 1540 7273 0000 0072 f400 0000  .N@..@rs...r....
+000061c0: 7a10 5365 6c65 6369 6f6e 6164 6f20 4361  z.Selecionado Ca
+000061d0: 6c6c 72f5 0000 007a 0f53 656c 6563 696f  llr....z.Selecio
+000061e0: 6e61 646f 2050 7574 7530 0000 0041 7320  nado Putu0...As 
+000061f0: 6f70 c3a7 c3b5 6573 2076 616c 6964 6173  op....es validas
+00006200: 2073 616f 2073 6f6d 656e 7465 2061 7320   sao somente as 
+00006210: 6465 2043 414c 4c20 6520 5055 544e 290a  de CALL e PUTN).
+00006220: 726b 0000 00da 0673 6576 656e 4472 cc00  rk.....sevenDr..
+00006230: 0000 7266 0000 0072 6700 0000 7269 0000  ..rf...rg...ri..
+00006240: 0072 2e00 0000 7202 0000 005a 0363 6466  .r....r....Z.cdf
+00006250: da03 6578 7029 0c5a 0b43 616c 6c5f 6f72  ..exp).Z.Call_or
+00006260: 5f50 7574 72cd 0000 005a 0570 7265 636f  _Putr....Z.preco
+00006270: da06 7374 7269 6b65 5a09 6469 6173 5574  ..strikeZ.diasUt
+00006280: 6569 735a 0d76 6f6c 6174 696c 6964 6164  eisZ.volatilidad
+00006290: 6544 5a0c 766f 6c61 7469 6c69 6461 6465  eDZ.volatilidade
+000062a0: 5a06 7461 7861 4c52 da02 6431 da02 6432  Z.taxaLR..d1..d2
+000062b0: da01 43da 0150 721f 0000 0072 1f00 0000  ..C..Pr....r....
+000062c0: 7220 0000 00da 0d62 6c61 636b 5f73 6368  r .....black_sch
+000062d0: 6f6c 6573 1e04 0000 731c 0000 0000 190c  oles....s.......
+000062e0: 0108 0104 0230 0112 0208 0108 012c 0104  .....0.......,..
+000062f0: 0108 0108 012e 0104 0272 0501 0000 6301  .........r....c.
+00006300: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00006310: 0000 0043 0000 0073 2e00 0000 7400 a001  ...C...s....t...
+00006320: 6401 a101 7d01 7c01 a002 a100 7d02 6402  d...}.|.....}.d.
+00006330: 7d03 7403 a004 7c03 7c01 a102 7d04 7c01  }.t...|.|...}.|.
+00006340: a005 a100 0100 6400 5300 2903 4e7a 3e51  ......d.S.).Nz>Q
+00006350: 3a5c 5269 7363 6f5c 4e6f 766f 2052 6973  :\Risco\Novo Ris
+00006360: 636f 5c70 7974 686f 6e72 6973 636f 5c42  co\pythonrisco\B
+00006370: 4246 696e 616e 6365 5c42 616e 636f 5c44  BFinance\Banco\D
+00006380: 6174 6143 6c69 656e 7473 2e64 627a 1753  ataClients.dbz.S
+00006390: 454c 4543 5420 2a20 4652 4f4d 2043 6172  ELECT * FROM Car
+000063a0: 7465 6972 6173 2906 da07 7371 6c69 7465  teiras)...sqlite
+000063b0: 33da 0763 6f6e 6e65 6374 da06 6375 7273  3..connect..curs
+000063c0: 6f72 7242 0000 005a 0e72 6561 645f 7371  orrB...Z.read_sq
+000063d0: 6c5f 7175 6572 7972 8600 0000 2905 7284  l_queryr....).r.
+000063e0: 0000 005a 0763 6f6e 6578 616f 7208 0100  ...Z.conexaor...
+000063f0: 005a 0863 6f6e 7375 6c74 6172 1e00 0000  .Z.consultar....
+00006400: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+00006410: 0863 6172 7465 6972 614f 0400 0073 0a00  .carteiraO...s..
+00006420: 0000 0001 0a01 0801 0402 0c01 7209 0100  ............r...
+00006430: 0063 0100 0000 0000 0000 0000 0000 0800  .c..............
+00006440: 0000 0600 0000 4300 0000 73e4 0000 007c  ......C...s....|
+00006450: 00a0 0064 01a1 0173 147c 0064 0117 007d  ...d...s.|.d...}
+00006460: 006e 0874 0164 0283 0101 0074 026a 037c  .n.t.d.....t.j.|
+00006470: 0064 0364 048d 027d 0174 0483 007d 0274  .d.d...}.t...}.t
+00006480: 056a 067c 02a0 077c 01a1 017c 016a 0864  .j.|...|...|.j.d
+00006490: 058d 027d 0174 0974 0a7c 0183 0164 0614  ...}.t.t.|...d..
+000064a0: 0083 017d 037c 016a 0b64 007c 0385 0219  ...}.|.j.d.|....
+000064b0: 007d 047c 016a 0b7c 0364 0085 0219 007d  .}.|.j.|.d.....}
+000064c0: 0574 0c6a 0da0 0e74 0c6a 0d6a 0f6a 1064  .t.j...t.j.j.j.d
+000064d0: 0764 0864 098d 0274 0c6a 0d6a 0fa0 1064  .d.d...t.j.j...d
+000064e0: 0aa1 0167 02a1 017d 067c 066a 1164 0b64  ...g...}.|.j.d.d
+000064f0: 0c64 0d8d 0201 007c 066a 127c 046a 1364  .d.....|.j.|.j.d
+00006500: 0e67 0164 0a64 0f8d 027c 0464 0e19 0064  .g.d.d...|.d...d
+00006510: 1064 1164 128d 0401 007c 06a0 147c 056a  .d.d.....|...|.j
+00006520: 1364 0e67 0164 0a64 0f8d 02a1 017d 077c  .d.g.d.d.....}.|
+00006530: 0753 0029 134e 72a1 0000 0072 f600 0000  .S.).Nr....r....
+00006540: 5a02 3764 723b 0000 0072 c800 0000 679a  Z.7dr;...r....g.
+00006550: 9999 9999 99e9 3fe9 4000 0000 5a04 7265  ......?.@...Z.re
+00006560: 6c75 2901 5a0a 6163 7469 7661 7469 6f6e  lu).Z.activation
+00006570: 7216 0000 005a 0461 6461 6d5a 126d 6561  r....Z.adamZ.mea
+00006580: 6e5f 7371 7561 7265 645f 6572 726f 7229  n_squared_error)
+00006590: 025a 096f 7074 696d 697a 6572 725b 0000  .Z.optimizerr[..
+000065a0: 0072 4700 0000 72d6 0000 0072 4e00 0000  .rG...r....rN...
+000065b0: e920 0000 0029 025a 0665 706f 6368 735a  . ...).Z.epochsZ
+000065c0: 0a62 6174 6368 5f73 697a 6529 1572 fc00  .batch_size).r..
+000065d0: 0000 722e 0000 0072 2900 0000 7265 0000  ..r....r)...re..
+000065e0: 0072 0500 0000 7242 0000 0072 4300 0000  .r....rB...rC...
+000065f0: 5a0d 6669 745f 7472 616e 7366 6f72 6d72  Z.fit_transformr
+00006600: c900 0000 da03 696e 7472 8200 0000 722f  ......intr....r/
+00006610: 0000 00da 0274 665a 056b 6572 6173 5a0a  .....tfZ.kerasZ.
+00006620: 5365 7175 656e 7469 616c 5a06 6c61 7965  SequentialZ.laye
+00006630: 7273 5a05 4465 6e73 65da 0763 6f6d 7069  rsZ.Dense..compi
+00006640: 6c65 5a03 6669 7472 3e00 0000 5a07 7072  leZ.fitr>...Z.pr
+00006650: 6564 6963 7429 0872 2200 0000 721e 0000  edict).r"...r...
+00006660: 005a 0673 6361 6c65 725a 0a74 7261 696e  .Z.scalerZ.train
+00006670: 5f73 697a 655a 0a74 7261 696e 5f64 6174  _sizeZ.train_dat
+00006680: 615a 0974 6573 745f 6461 7461 da05 6d6f  aZ.test_data..mo
+00006690: 6465 6c5a 0b70 7265 6469 6374 696f 6e73  delZ.predictions
+000066a0: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+000066b0: 1370 7265 6469 6374 5f73 746f 636b 5f74  .predict_stock_t
+000066c0: 7265 6e64 5904 0000 7322 0000 0000 020a  rendY...s"......
+000066d0: 010a 0208 050e 0306 0116 0310 010e 010e  ................
+000066e0: 0306 0110 010c fe06 040e 0322 0316 0272  ..........."...r
+000066f0: 1001 0000 2901 7239 0000 0029 0172 0100  ....).r9...).r..
+00006700: 0000 295a 5a08 7966 696e 616e 6365 7229  ..)ZZ.yfinancer)
+00006710: 0000 005a 0b73 6369 7079 2e73 7461 7473  ...Z.scipy.stats
+00006720: 7202 0000 005a 0e73 6369 7079 2e6f 7074  r....Z.scipy.opt
+00006730: 696d 697a 6572 0300 0000 5a14 736b 6c65  imizer....Z.skle
+00006740: 6172 6e2e 6c69 6e65 6172 5f6d 6f64 656c  arn.linear_model
+00006750: 7204 0000 00da 0a74 656e 736f 7266 6c6f  r......tensorflo
+00006760: 7772 0d01 0000 5a15 736b 6c65 6172 6e2e  wr....Z.sklearn.
+00006770: 7072 6570 726f 6365 7373 696e 6772 0500  preprocessingr..
+00006780: 0000 5a08 7365 6c65 6e69 756d 7206 0000  ..Z.seleniumr...
+00006790: 005a 1e73 656c 656e 6975 6d2e 7765 6264  .Z.selenium.webd
+000067a0: 7269 7665 722e 636f 6d6d 6f6e 2e6b 6579  river.common.key
+000067b0: 7372 0700 0000 5a21 7365 6c65 6e69 756d  sr....Z!selenium
+000067c0: 2e77 6562 6472 6976 6572 2e63 6872 6f6d  .webdriver.chrom
+000067d0: 652e 6f70 7469 6f6e 7372 0800 0000 5a1c  e.optionsr....Z.
+000067e0: 7365 6c65 6e69 756d 2e77 6562 6472 6976  selenium.webdriv
+000067f0: 6572 2e63 6f6d 6d6f 6e2e 6279 7209 0000  er.common.byr...
+00006800: 0072 df00 0000 72ac 0000 005a 0362 7334  .r....r....Z.bs4
+00006810: 720a 0000 0072 e300 0000 5a07 6661 7374  r....r....Z.fast
+00006820: 6170 6972 0b00 0000 720c 0000 0072 0d00  apir....r....r..
+00006830: 0000 5a11 6661 7374 6170 692e 7265 7370  ..Z.fastapi.resp
+00006840: 6f6e 7365 7372 0e00 0000 5a13 6661 7374  onsesr....Z.fast
+00006850: 6170 692e 7374 6174 6963 6669 6c65 7372  api.staticfilesr
+00006860: 0f00 0000 5a12 6661 7374 6170 692e 7465  ....Z.fastapi.te
+00006870: 6d70 6c61 7469 6e67 7210 0000 00da 046a  mplatingr......j
+00006880: 736f 6e5a 0775 7669 636f 726e da06 7061  sonZ.uvicorn..pa
+00006890: 6e64 6173 7242 0000 00da 056e 756d 7079  ndasrB.....numpy
+000068a0: 7266 0000 0072 1100 0000 7212 0000 00da  rf...r....r.....
+000068b0: 0674 7970 696e 6772 1300 0000 7206 0100  .typingr....r...
+000068c0: 00da 0877 6172 6e69 6e67 73da 0e66 696c  ...warnings..fil
+000068d0: 7465 7277 6172 6e69 6e67 735a 0c70 6472  terwarningsZ.pdr
+000068e0: 5f6f 7665 7272 6964 65da 0574 6f64 6179  _override..today
+000068f0: 5a0c 6f6e 655f 7965 6172 5f61 676f 5a0c  Z.one_year_agoZ.
+00006900: 6f6e 655f 6461 7973 5f61 676f 5a0e 7365  one_days_agoZ.se
+00006910: 7665 6e5f 6461 7973 5f61 676f da08 7374  ven_days_ago..st
+00006920: 7266 7469 6d65 72cb 0000 005a 046f 6e65  rftimer....Z.one
+00006930: 4472 fe00 0000 72cc 0000 00da 0361 7070  Dr....r......app
+00006940: 7221 0000 0072 ad00 0000 7281 0000 0072  r!...r....r....r
+00006950: 2d00 0000 7234 0000 00da 085f 5f6e 616d  -...r4.....__nam
+00006960: 655f 5fda 0372 756e 72b4 0000 0072 4300  e__..runr....rC.
+00006970: 0000 7246 0000 005a 0f72 6573 706f 6e73  ..rF...Z.respons
+00006980: 6548 6973 746f 7279 724c 0000 0072 5e00  eHistoryrL...r^.
+00006990: 0000 726b 0000 0072 6f00 0000 721d 0000  ..rk...ro...r...
+000069a0: 0072 0c01 0000 7277 0000 0072 3d00 0000  .r....rw...r=...
+000069b0: 7287 0000 0072 9b00 0000 72b8 0000 0072  r....r....r....r
+000069c0: bb00 0000 72be 0000 0072 ce00 0000 72f3  ....r....r....r.
+000069d0: 0000 00da 0462 6f6f 6c72 fd00 0000 7205  .....boolr....r.
+000069e0: 0100 0072 0901 0000 7210 0100 0072 1f00  ...r....r....r..
+000069f0: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00006a00: 00da 083c 6d6f 6475 6c65 3e02 0000 0073  ...<module>....s
+00006a10: f000 0000 0801 0c01 0c01 0c01 0801 0c04  ................
+00006a20: 0c01 0c01 0c01 0c01 0801 0801 0c01 0803  ................
+00006a30: 1401 0c01 0c01 0c01 0801 0803 0801 0801  ................
+00006a40: 1001 0c01 0803 0801 0a02 0802 0802 0e01  ................
+00006a50: 0e01 0e03 0a01 0a01 0a02 0a02 060c 0809  ................
+00006a60: 0c01 122b 0a01 1201 0a05 0c01 1826 0a01  ...+.........&..
+00006a70: 1201 0a05 0c01 1220 0a01 1201 0a05 0c01  ....... ........
+00006a80: 123a 0a01 1201 0a05 0c01 1618 0a01 1201  .:..............
+00006a90: 0a05 0c01 1232 0a01 1201 0a05 0c01 1623  .....2.........#
+00006aa0: 0a01 1201 0a05 0c01 2062 0a01 1201 0a05  ........ b......
+00006ab0: 0801 163a 0a01 1201 0a05 0c01 1418 0a01  ...:............
+00006ac0: 1201 0a05 0c01 1642 0a01 1201 0a05 0c01  .......B........
+00006ad0: 1a40 0a01 1201 0a05 0c01 167f 0007 0a01  .@..............
+00006ae0: 1201 0a03 0c01 1e4e 0a01 1201 0a05 0c01  .......N........
+00006af0: 1a3d 0a01 1201 0a03 0c01 202a 0a01 1201  .=........ *....
+00006b00: 0a04 0c0a                                ....
```

### Comparing `BBFinance-1.5.1/BBFinance.egg-info/PKG-INFO` & `BBFinance-1.5.2/BBFinance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.5.1
+Version: 1.5.2
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rápida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.5.1/BBFinance.egg-info/SOURCES.txt` & `BBFinance-1.5.2/BBFinance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/Banco/DataClients.db` & `BBFinance-1.5.2/Banco/DataClients.db`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/LICENSE.txt` & `BBFinance-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/PKG-INFO` & `BBFinance-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.5.1
+Version: 1.5.2
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rápida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.5.1/README.md` & `BBFinance-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/__pycache__/main.cpython-39.pyc` & `BBFinance-1.5.2/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.5.1/requirements.txt` & `BBFinance-1.5.2/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 requests                      2.28.2
 bs4                           0.0.1
 beautifulsoup4                4.11.2
 pydantic                      1.10.7
 Unicode                       1.3.6
 typing_extensions             4.5.0
 scikit-image                  0.19.3
-scikit-learn                  1.2.2
+scikit-learn                  1.2.2
+tensorflow                    2.11.0
+chromedriver-autoinstaller    0.4.0
```

### Comparing `BBFinance-1.5.1/setup.py` & `BBFinance-1.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.5.1',
+    version='1.5.2',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rápida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
     license='GPLv3',
     packages=['BBFinance'],
     long_description= long_description,
@@ -26,15 +26,17 @@
         'requests>=2.28.2',
         'bs4>=0.0.1',
         'beautifulsoup4>=4.11.2',
         'pydantic>=1.10.7',
         'Unicode>=1.3.6',
         'typing_extensions>=4.5.0',
         'scikit-image>=0.19.3',
-        'scikit-learn>=1.2.2'
+        'scikit-learn>=1.2.2',
+        'tensorflow==2.11.0',
+        'chromedriver-autoinstaller==0.4.0'
         
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.9',
```

