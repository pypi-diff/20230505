# Comparing `tmp/pop-create-idem-3.3.1.tar.gz` & `tmp/pop-create-idem-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-3.3.1.tar", last modified: Tue May  2 15:33:51 2023, max compression
+gzip compressed data, was "pop-create-idem-3.4.0.tar", last modified: Fri May  5 13:31:18 2023, max compression
```

## Comparing `pop-create-idem-3.3.1.tar` & `pop-create-idem-3.4.0.tar`

### file list

```diff
@@ -1,111 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.871142 pop-create-idem-3.3.1/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8796 2023-05-02 15:33:51.871142 pop-create-idem-3.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7947 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.864141 pop-create-idem-3.3.1/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8546 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.864141 pop-create-idem-3.3.1/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.865141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.866141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     2533 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.866141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/tool.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.866141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     2154 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3477 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      209 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     2091 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1266 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2509 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.862141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.862141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      960 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.862141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      763 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     2649 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.869141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/
--rw-r--r--   0 root         (0) root         (0)     3840 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.869141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)      366 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     6081 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     4931 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/params.py
--rw-r--r--   0 root         (0) root         (0)     6475 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/schemas.py
--rw-r--r--   0 root         (0) root         (0)    15090 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.869141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1740 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      708 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.865141 pop-create-idem-3.3.1/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8796 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4373 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-02 15:33:51.871142 pop-create-idem-3.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3004 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.816471 pop-create-idem-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-05-05 13:31:18.816471 pop-create-idem-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.809137 pop-create-idem-3.4.0/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8546 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.809137 pop-create-idem-3.4.0/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810054 pop-create-idem-3.4.0/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810054 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/templates.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3477 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      822 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      209 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     5076 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     4964 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/params.py
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.814637 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.814637 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
+-rw-r--r--   0 root         (0) root         (0)      969 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
+-rw-r--r--   0 root         (0) root         (0)      700 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.814637 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.814637 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810054 pop-create-idem-3.4.0/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5938 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-05 13:31:18.816471 pop-create-idem-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/setup.py
```

### Comparing `pop-create-idem-3.3.1/LICENSE` & `pop-create-idem-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/PKG-INFO` & `pop-create-idem-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.3.1
+Version: 3.4.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.3.1/README.rst` & `pop-create-idem-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/cloudspec/__init__.py` & `pop-create-idem-3.4.0/cloudspec/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/cloudspec/conf.py` & `pop-create-idem-3.4.0/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,28 @@
+import os.path
 import pathlib
 
 import tqdm
 
 from cloudspec import CloudSpec
 
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
     cloud_spec = CloudSpec(**ctx.cloud_spec)
     exec_dir = root_directory / ctx.clean_name / "exec" / ctx.service_name
+    template_dir = (
+        root_directory
+        / ctx.clean_name
+        / "autogen"
+        / ctx.service_name
+        / "templates"
+        / "exec"
+    )
 
     for ref, plugin in cloud_spec.plugins.items():
         mod_file = hub.cloudspec.parse.plugin.touch(exec_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
 
         plugin["func_alias"] = {"list_": "list"}
         plugin["contracts"] = ["auto_state", "soft_fail"]
@@ -42,15 +51,25 @@
                 ["get", "list", "create", "update", "delete"],
                 desc=f"{ref} auto_state functions",
             ):
                 if func_data.get(function_name):
                     base_template = hub.cloudspec.template.auto_state[
                         function_name.upper()
                     ]
-                    template_str = f"{base_template}\n    {cloud_spec.request_format[function_name]}\n\n\n"
+
+                    request_format_template_file = (
+                        f"{template_dir}/{function_name}.jinja2"
+                    )
+                    if os.path.isfile(request_format_template_file):
+                        with open(f"{template_dir}/{function_name}.jinja2", "rb+") as f:
+                            request_format = f.read().decode()
+                    else:
+                        request_format = cloud_spec.request_format.get(function_name)
+
+                    template_str = f"{base_template}\n    {request_format}\n\n\n"
                     template = hub.tool.jinja.template(template_str)
 
                     to_write += template.render(
                         service_name=cloud_spec.service_name,
                         function=dict(
                             ref=ref,
                             exec_ref=f"exec.{exec_ref}",
```

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+import os
 import pathlib
 
 from cloudspec import CloudSpec
 
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
     cloud_spec = CloudSpec(**ctx.cloud_spec)
     exec_dir = root_directory / ctx.clean_name / "exec" / ctx.service_name
+    template_dir = (
+        root_directory
+        / ctx.clean_name
+        / "autogen"
+        / ctx.service_name
+        / "templates"
+        / "exec"
+    )
 
     for ref, plugin in cloud_spec.plugins.items():
         mod_file = hub.cloudspec.parse.plugin.touch(exec_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
         cli_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
 
         plugin["func_alias"] = {"list_": "list"}
@@ -20,16 +29,23 @@
 
         for function_name, function_data in plugin.functions.items():
 
             if function_name in ["present", "absent", "describe"]:
                 # If plugin comes in with all methods, let's not create for state_modules functions
                 continue
 
+            request_format_template_file = f"{template_dir}/{function_name}.jinja2"
+            if os.path.isfile(request_format_template_file):
+                with open(f"{template_dir}/{function_name}.jinja2", "rb+") as f:
+                    request_format = f.read().decode()
+            else:
+                request_format = cloud_spec.request_format.get(function_name)
+
             template = hub.tool.jinja.template(
-                f"{hub.cloudspec.template.exec.FUNCTION}\n    {cloud_spec.request_format[function_name]}\n\n\n"
+                f"{hub.cloudspec.template.exec.FUNCTION}\n    {request_format}\n\n\n"
             )
 
             function_alias = plugin.func_alias.get(function_name, function_name)
 
             to_write += template.render(
                 function=dict(
                     name=function_name,
```

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+import os
 import pathlib
 
 from cloudspec import CloudSpec
 
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
     cloud_spec = CloudSpec(**ctx.cloud_spec)
     states_dir = root_directory / ctx.clean_name / "states" / ctx.service_name
+    template_dir = (
+        root_directory
+        / ctx.clean_name
+        / "autogen"
+        / ctx.service_name
+        / "templates"
+        / "state"
+    )
 
     for ref, plugin in cloud_spec.plugins.items():
         mod_file = hub.cloudspec.parse.plugin.touch(states_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
         state_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
 
         plugin["contracts"] = ["resource"]
@@ -44,16 +53,23 @@
             (
                 hub.cloudspec.template.state.PRESENT_FUNCTION,
                 hub.cloudspec.template.state.ABSENT_FUNCTION,
                 hub.cloudspec.template.state.DESCRIBE_FUNCTION,
             ),
         ):
             if func_data.get(function_name):
+                request_format_template_file = f"{template_dir}/{function_name}.jinja2"
+                if os.path.isfile(request_format_template_file):
+                    with open(f"{template_dir}/{function_name}.jinja2", "rb+") as f:
+                        request_format = f.read().decode()
+                else:
+                    request_format = cloud_spec.request_format.get(function_name)
+
                 template = hub.tool.jinja.template(
-                    f"{TEMPLATE}\n    {cloud_spec.request_format[function_name]}\n\n\n"
+                    f"{TEMPLATE}\n    {request_format}\n\n\n"
                 )
 
                 to_write += template.render(
                     service_name=cloud_spec.service_name,
                     function=dict(
                         ref=ref,
                         state_ref=f"states.{state_ref}",
```

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/tests.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/tests.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/init.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/function.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/param.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/exec.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/conf.py` & `pop-create-idem-3.4.0/pop_create_idem/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,19 @@
     },
     "specification": {
         "options": ["--spec", "--file", "--url"],
         "nargs": "+",
         "subcommands": ["openapi3", "swagger", "idem-cloud"],
         "dyne": "pop_create",
     },
+    "templates_dir": {
+        "options": ["--td"],
+        "subcommands": ["_global_"],
+        "dyne": "pop_create",
+    },
 }
 CONFIG = {
     "create_plugin": {
         "default": "state_modules",
         "dyne": "pop_create",
         "help": "The `create` plugin to use for resource modules. The other options are 'auto_states', 'exec_modules'.",
     },
@@ -33,14 +38,19 @@
         "dyne": "pop_create",
     },
     "specification": {
         "default": None,
         "help": "The url or file path to a spec",
         "dyne": "pop_create",
     },
+    "templates_dir": {
+        "default": None,
+        "help": "The full absolute path of directory where jinja templates are saved",
+        "dyne": "pop_create",
+    },
 }
 SUBCOMMANDS = {
     # https://openapi.tools/#converters
     "idem-cloud": {"help": "Boostrap an idem cloud project", "dyne": "pop_create"},
     "openapi3": {
         "help": "Create idem_cloud modules based off of an openapi3 spec",
         "dyne": "pop_create",
```

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,33 +30,24 @@
     elif ctx.create_plugin == "state_modules":
         # For now restrict only CRUDs for exec modules, auto_state already does that
         hub.cloudspec.init.run(
             ctx,
             root_directory,
             create_plugins=["auto_state", "tool", "state_modules", "tests", "docs"],
         )
-    else:
-        # TODO: State module or anything else
+    elif ctx.create_plugin == "templates":
         hub.cloudspec.init.run(
             ctx,
             root_directory,
-            create_plugins=["tests", "docs"],
+            create_plugins=["templates", "tests", "docs"],
         )
+    else:
+        raise ValueError(f"Invalid input '{ctx.create_plugin}' for --create-plugin.")
 
     # Sanitize based on other arguments
     if ctx.has_acct_plugin:
         hub.tool.path.rmtree(root_directory / ctx.clean_name / "acct")
-        hub.tool.path.rmtree(root_directory / ctx.clean_name / "tool")
-
-    if ctx.specification:
-        # sample files don't matter when creating from a specification
-        hub.tool.path.delete(
-            root_directory / ctx.clean_name / "exec" / ctx.service_name / "sample.py"
-        )
-        hub.tool.path.delete(
-            root_directory / ctx.clean_name / "states" / ctx.service_name / "sample.py"
-        )
 
     # End with the cicd template
     hub.pop_create.init.run(directory=root_directory, subparsers=["cicd"], **ctx)
 
     # TODO Run sphinx on the docstrings to make sure it all works
```

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import pathlib
+import shutil
 
 import pop.hub
 from dict_tools.data import NamespaceDict
 
 if __name__ == "__main__":
     root_directory = pathlib.Path.cwd()
 
     hub = pop.hub.Hub()
     hub.pop.sub.add(dyne_name="pop_create")
     hub.pop.sub.add(dyne_name="config")
     hub.config.integrate.load(["pop_create"], "pop_create", parse_cli=False, logs=False)
     ctx = NamespaceDict({{cookiecutter}})
 
-    idem_dynes = ["exec", "states"]
+    idem_dynes = ["exec", "states", "tool"]
     if not ctx.has_acct_plugin:
-        idem_dynes.append("tool")
         idem_dynes.append("acct")
 
     dyne_list = set(idem_dynes + list(ctx.short_dyne_list))
     # FIXME generating tests is problematic for some reason
     # pop_create_core = ["seed", "tests", "docs"]
     pop_create_core = ["seed", "docs"]
     seed_ctx = NamespaceDict(vertical=True, dyne_list=dyne_list)
 
     if "cloud_spec" not in ctx:
         # The openapi3/swagger plugin might call this with their own spec
         ctx.cloud_spec = {}
 
+    if ctx.get("templates_dir", None):
+        target = (
+            root_directory / ctx.clean_name / "autogen" / ctx.service_name / "templates"
+        )
+        shutil.copytree(ctx.get("templates_dir"), target, dirs_exist_ok=True)
+
     # Bring in the full context, but don't override any of our overrides
     for k in ctx:
         if k not in seed_ctx:
             seed_ctx[k] = ctx[k]
 
     # Run a traditional pop seed on the directory with common idem states
     hub.pop_create.init.run(
```

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 
 def __init__(hub):
     hub.pop.sub.add(dyne_name="cloudspec")
 
 
 def context(hub, ctx, directory: pathlib.Path):
+    # all template files are copied without render
+    ctx["_copy_without_render"] = ["*.jinja2"]
+
     # non openapi/swagger based would not have cloud_spec here
     if "cloud_spec" not in ctx or not ctx.cloud_spec:
         # If an acct plugin was passed in then we don't need to create auth plugins
         if ctx.get("simple_service_name"):
             ctx.service_name = ctx.simple_service_name
         elif not ctx.get("service_name"):
             ctx.service_name = (
```

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/function.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/init.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pathlib
 from typing import Dict
 
 import openapi3.object_base
 import requests
 import yaml
 from dict_tools.data import NamespaceDict
@@ -16,14 +17,25 @@
         )
 
     ctx.has_acct_plugin = bool(ctx.acct_plugin)
     if not ctx.has_acct_plugin:
         # Create auth plugins
         ctx.acct_plugin = ctx.service_name
 
+    # Add extra templates provided by openapi3
+    if not ctx.get("templates_dir"):
+        # Use default templates
+        ctx["templates_dir"] = (
+            os.path.dirname(os.path.realpath(__file__))
+            + "/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/"
+        )
+
+    # all template files are copied without render
+    ctx["_copy_without_render"] = ["*.jinja2"]
+
     # FIXME: Not an optimal way, it could take longer as for each spec we go through post generation hooks
     for specification in ctx.specification:
         # Read the spec from URL or local file (Yaml)
         spec = hub.pop_create.openapi3.init.read(source=specification)
         api = openapi3.OpenAPI(spec, validate=True)
         errors = api.errors()
         if errors:
@@ -55,22 +67,19 @@
 
         # Get function plugins
         plugins = hub.pop_create.openapi3.parse.plugins(ctx, api)
 
         # Add any missing function which is required for idem resource modules
         plugins = hub.pop_create.openapi3.init.add_missing_known_functions(ctx, plugins)
 
-        # Create request formats for function
-        request_formats = hub.pop_create.openapi3.init.get_requests_formats(plugins)
-
         cloud_spec = NamespaceDict(
             api_version=ctx.cloud_api_version,
             project_name=ctx.project_name,
             service_name=ctx.service_name,
-            request_format=request_formats,
+            request_format={},
             plugins=plugins,
         )
         ctx.cloud_spec = cloud_spec
 
         hub.pop_create.init.run(directory=directory, subparsers=["idem_cloud"], **ctx)
 
     return ctx
@@ -92,47 +101,14 @@
     else:
         request = requests.get(source, headers={"Content-Type": "application/json"})
         ret = request.json()
 
     return ret
 
 
-def get_requests_formats(hub, plugins):
-    request_formats = {}
-
-    request_formats["get"] = hub.pop_create.openapi3.template.GET_REQUEST_FORMAT
-    request_formats["list"] = hub.pop_create.openapi3.template.LIST_REQUEST_FORMAT
-    request_formats["create"] = hub.pop_create.openapi3.template.CREATE_REQUEST_FORMAT
-    request_formats["update"] = hub.pop_create.openapi3.template.UPDATE_REQUEST_FORMAT
-    request_formats["delete"] = hub.pop_create.openapi3.template.DELETE_REQUEST_FORMAT
-    request_formats["present"] = hub.pop_create.openapi3.template.PRESENT_REQUEST_FORMAT
-    request_formats["absent"] = hub.pop_create.openapi3.template.ABSENT_REQUEST_FORMAT
-    request_formats[
-        "describe"
-    ] = hub.pop_create.openapi3.template.DESCRIBE_REQUEST_FORMAT
-
-    for ref, func in plugins.items():
-        for func_name, func_data in func["functions"].items():
-            if func_name not in [
-                "get",
-                "list",
-                "create",
-                "update",
-                "delete",
-                "present",
-                "absent",
-                "describe",
-            ]:
-                request_formats[
-                    func_name
-                ] = hub.pop_create.openapi3.template.OTHER_FUNCTION_REQUEST_FORMAT
-
-    return request_formats
-
-
 def add_missing_known_functions(hub, ctx, plugins):
     # This is to make sure we still create standard skeletons for CRUD operations in exec
     # This way the only missing part would be API call in those modules
     for ref in list(plugins):
         for idem_func_name in ["get", "list", "create", "update", "delete"]:
             if not plugins[ref].get("functions", {}).get(idem_func_name):
                 plugins[ref]["functions"][idem_func_name] = {
```

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/params.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         for p in parameters:
             if "actual_name" in p and p.get("actual_name"):
                 ret += (
                     '        "'
                     + p.get("actual_name")
                     + '"'
                     + ": "
-                    + p.get("idem_name").strip('"')
+                    + hub.tool.format.keyword.unclash(p.get("idem_name").strip('"'))
                     + ",\n    "
                 )
 
     ret += "}"
     return ret
```

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/schemas.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/schemas.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/tool/format/case.py` & `pop-create-idem-3.4.0/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-3.4.0/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem/tool/gradle.py` & `pop-create-idem-3.4.0/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.1/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-3.4.0/pop_create_idem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.3.1
+Version: 3.4.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.3.1/setup.py` & `pop-create-idem-3.4.0/setup.py`

 * *Files identical despite different names*

