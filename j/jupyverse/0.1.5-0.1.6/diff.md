# Comparing `tmp/jupyverse-0.1.5.tar.gz` & `tmp/jupyverse-0.1.6.tar.gz`

## Comparing `jupyverse-0.1.5.tar` & `jupyverse-0.1.6.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    61129 2020-02-02 00:00:00.000000 jupyverse-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.5/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.5/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.5/config.yaml
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.1.5/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.5/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.github/workflows/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.5/binder/environment.yml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.5/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.5/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.5/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/index.md
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/kernels.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/retrolab.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/yjs.md
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/usage/microservices.md
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/fps_retrolab/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/fps_retrolab/main.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/fps_retrolab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/README.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_contents.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_kernels.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_server.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/COPYING.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.5/README.md
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 jupyverse-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 jupyverse-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    61901 2020-02-02 00:00:00.000000 jupyverse-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.6/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.6/config.yaml
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.1.6/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.6/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.6/binder/environment.yml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.6/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.6/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.6/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/index.md
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/retrolab.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/fps_retrolab/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/fps_retrolab/main.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/fps_retrolab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/README.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/README.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_contents.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_kernels.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_server.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/COPYING.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.6/README.md
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 jupyverse-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jupyverse-0.1.6/PKG-INFO
```

### Comparing `jupyverse-0.1.5/.pre-commit-config.yaml` & `jupyverse-0.1.6/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.262
+    rev: v0.0.263
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyverse-0.1.5/CHANGELOG.md` & `jupyverse-0.1.6/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.6
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.5...442f12896cb390ef8346a2fc99e927fa3295421b))
+
+### Merged PRs
+
+- Update dependencies [#298](https://github.com/jupyter-server/jupyverse/pull/298) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-04-29&to=2023-05-05&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-04-29..2023-05-05&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-04-29..2023-05-05&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.5
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.4...bea8fa74efe86fa59ea6054f6e332ffd3d58b23f))
 
 ### Merged PRs
 
 - Update with FastAPI-Users v11 [#296](https://github.com/jupyter-server/jupyverse/pull/296) ([@davidbrochart](https://github.com/davidbrochart))
@@ -13,16 +29,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-04-18&to=2023-04-29&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-04-18..2023-04-29&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-04-18..2023-04-29&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.4
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.3...a42f7c4d0e951d620108afb4ca25e57da5bae2a1))
 
 ### Merged PRs
 
 - Move routes to jupyverse_api [#293](https://github.com/jupyter-server/jupyverse/pull/293) ([@davidbrochart](https://github.com/davidbrochart))
```

### Comparing `jupyverse-0.1.5/CONTRIBUTING.md` & `jupyverse-0.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/config.yaml` & `jupyverse-0.1.6/config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/mkdocs.yml` & `jupyverse-0.1.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/.devcontainer/devcontainer.json` & `jupyverse-0.1.6/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/.github/workflows/check-release.yml` & `jupyverse-0.1.6/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/.github/workflows/main.yml` & `jupyverse-0.1.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/binder/jupyter_notebook_config.py` & `jupyverse-0.1.6/binder/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/docs/index.md` & `jupyverse-0.1.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/docs/install.md` & `jupyverse-0.1.6/docs/install.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/docs/jupyter.svg` & `jupyverse-0.1.6/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/docs/plugins/auth.md` & `jupyverse-0.1.6/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/docs/usage/microservices.md` & `jupyverse-0.1.6/docs/usage/microservices.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/docs/usage/multi_user.md` & `jupyverse-0.1.6/docs/usage/multi_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/docs/usage/single_user.md` & `jupyverse-0.1.6/docs/usage/single_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/COPYING.md` & `jupyverse-0.1.6/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/pyproject.toml` & `jupyverse-0.1.6/jupyverse_api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel, Extra
 
 from .app import App
 
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/cli.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/contents/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/contents/models.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/jupyterlab/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/kernels/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/lab/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/nbconvert/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/resource_usage/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/retrolab/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/terminals/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/jupyverse_api/jupyverse_api/yjs/__init__.py` & `jupyverse-0.1.6/jupyverse_api/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth/COPYING.md` & `jupyverse-0.1.6/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth/pyproject.toml` & `jupyverse-0.1.6/plugins/auth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth/fps_auth/backends.py` & `jupyverse-0.1.6/plugins/auth/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth/fps_auth/config.py` & `jupyverse-0.1.6/plugins/auth/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth/fps_auth/db.py` & `jupyverse-0.1.6/plugins/auth/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth/fps_auth/main.py` & `jupyverse-0.1.6/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth/fps_auth/routes.py` & `jupyverse-0.1.6/plugins/auth/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth_fief/COPYING.md` & `jupyverse-0.1.6/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth_fief/pyproject.toml` & `jupyverse-0.1.6/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/contents/COPYING.md` & `jupyverse-0.1.6/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/contents/pyproject.toml` & `jupyverse-0.1.6/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.1.6/plugins/contents/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/contents/fps_contents/routes.py` & `jupyverse-0.1.6/plugins/contents/fps_contents/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/frontend/COPYING.md` & `jupyverse-0.1.6/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/frontend/pyproject.toml` & `jupyverse-0.1.6/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/jupyterlab/COPYING.md` & `jupyverse-0.1.6/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.1.6/plugins/jupyterlab/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "fps_jupyterlab"
 description = "An FPS plugin for the JupyterLab API"
 keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
-  "jupyterlab >=4.0.0b0,<5",
+  "jupyterlab >=4.0.0rc0,<5",
   "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```

### Comparing `jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/COPYING.md` & `jupyverse-0.1.6/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/pyproject.toml` & `jupyverse-0.1.6/plugins/kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.1.6/plugins/kernels/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.1.6/plugins/kernels/fps_kernels/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/lab/COPYING.md` & `jupyverse-0.1.6/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/lab/pyproject.toml` & `jupyverse-0.1.6/plugins/lab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/lab/fps_lab/main.py` & `jupyverse-0.1.6/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/lab/fps_lab/routes.py` & `jupyverse-0.1.6/plugins/lab/fps_lab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/lab/fps_lab/static/favicon.ico` & `jupyverse-0.1.6/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/COPYING.md` & `jupyverse-0.1.6/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/pyproject.toml` & `jupyverse-0.1.6/plugins/login/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/routes.py` & `jupyverse-0.1.6/plugins/login/fps_login/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/index.html` & `jupyverse-0.1.6/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.1.6/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.1.6/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.1.6/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/nbconvert/COPYING.md` & `jupyverse-0.1.6/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/nbconvert/pyproject.toml` & `jupyverse-0.1.6/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.1.6/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/noauth/COPYING.md` & `jupyverse-0.1.6/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/noauth/pyproject.toml` & `jupyverse-0.1.6/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.1.6/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/resource_usage/COPYING.md` & `jupyverse-0.1.6/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/resource_usage/pyproject.toml` & `jupyverse-0.1.6/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/retrolab/COPYING.md` & `jupyverse-0.1.6/plugins/retrolab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/retrolab/pyproject.toml` & `jupyverse-0.1.6/plugins/retrolab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/retrolab/fps_retrolab/main.py` & `jupyverse-0.1.6/plugins/retrolab/fps_retrolab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/retrolab/fps_retrolab/routes.py` & `jupyverse-0.1.6/plugins/retrolab/fps_retrolab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/terminals/COPYING.md` & `jupyverse-0.1.6/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/terminals/pyproject.toml` & `jupyverse-0.1.6/plugins/terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.1.6/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/terminals/fps_terminals/routes.py` & `jupyverse-0.1.6/plugins/terminals/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/terminals/fps_terminals/server.py` & `jupyverse-0.1.6/plugins/terminals/fps_terminals/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.1.6/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/yjs/COPYING.md` & `jupyverse-0.1.6/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/yjs/pyproject.toml` & `jupyverse-0.1.6/plugins/yjs/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "fps_yjs"
 description = "An FPS plugin for the Yjs API"
 keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
-    "jupyter_ydoc >=0.3.4,<0.4.0",
+    "jupyter_ydoc >=1,<2",
     "ypy-websocket >=0.8.2,<1",
     "y-py >=0.6.0,<0.7.0",
     "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
```

### Comparing `jupyverse-0.1.5/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.1.6/plugins/yjs/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.1.6/plugins/yjs/fps_yjs/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/tests/conftest.py` & `jupyverse-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/tests/test_auth.py` & `jupyverse-0.1.6/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/tests/test_contents.py` & `jupyverse-0.1.6/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/tests/test_kernels.py` & `jupyverse-0.1.6/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/tests/test_server.py` & `jupyverse-0.1.6/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/tests/test_settings.py` & `jupyverse-0.1.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/tests/utils.py` & `jupyverse-0.1.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/tests/data/notebook0.ipynb` & `jupyverse-0.1.6/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/.gitignore` & `jupyverse-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/COPYING.md` & `jupyverse-0.1.6/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/README.md` & `jupyverse-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.5/pyproject.toml` & `jupyverse-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 [project.urls]
 Homepage = "https://jupyter.org"
 
 [project.optional-dependencies]
 jupyterlab = ["fps-jupyterlab >=0.1.2,<1"]
 retrolab = ["fps-retrolab >=0.1.2,<1"]
-auth = ["fps-auth >=0.1.2,<1"]
+auth = ["fps-auth >=0.1.2,<1", "fps-login >=0.1.2,<1"]
 auth-fief = ["fps-auth-fief >=0.1.2,<1"]
 noauth = ["fps-noauth >=0.1.2,<1"]
 test = [
     "mypy",
     "types-setuptools",
     "pytest",
     "pytest-asyncio",
```

### Comparing `jupyverse-0.1.5/PKG-INFO` & `jupyverse-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse
-Version: 0.1.5
+Version: 0.1.6
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
@@ -14,14 +14,15 @@
 Requires-Dist: fps-lab<1,>=0.1.2
 Requires-Dist: fps-nbconvert<1,>=0.1.2
 Requires-Dist: fps-terminals<1,>=0.1.2
 Requires-Dist: fps-yjs<1,>=0.1.2
 Requires-Dist: jupyverse-api<1,>=0.1.2
 Provides-Extra: auth
 Requires-Dist: fps-auth<1,>=0.1.2; extra == 'auth'
+Requires-Dist: fps-login<1,>=0.1.2; extra == 'auth'
 Provides-Extra: auth-fief
 Requires-Dist: fps-auth-fief<1,>=0.1.2; extra == 'auth-fief'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Provides-Extra: jupyterlab
 Requires-Dist: fps-jupyterlab<1,>=0.1.2; extra == 'jupyterlab'
```

