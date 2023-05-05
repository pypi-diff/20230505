# Comparing `tmp/idpyoidc-1.4.0.tar.gz` & `tmp/idpyoidc-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idpyoidc-1.4.0.tar", last modified: Thu Jan 19 14:35:11 2023, max compression
+gzip compressed data, was "idpyoidc-2.0.0.tar", last modified: Fri May  5 07:55:18 2023, max compression
```

## Comparing `idpyoidc-1.4.0.tar` & `idpyoidc-2.0.0.tar`

### file list

```diff
@@ -1,178 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.687196 idpyoidc-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-01-19 14:35:11.687196 idpyoidc-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 14:35:11.687196 idpyoidc-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.659195 idpyoidc-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.667195 idpyoidc-1.4.0/src/idpyoidc/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.667195 idpyoidc-1.4.0/src/idpyoidc/actor/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/actor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.667195 idpyoidc-1.4.0/src/idpyoidc/actor/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/actor/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.667195 idpyoidc-1.4.0/src/idpyoidc/actor/client/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/actor/client/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/actor/client/oidc/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.667195 idpyoidc-1.4.0/src/idpyoidc/actor/server/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/actor/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.667195 idpyoidc-1.4.0/src/idpyoidc/actor/server/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/actor/server/oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.671195 idpyoidc-1.4.0/src/idpyoidc/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22053 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/client_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/configure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12100 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/entity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.671195 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10679 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.671195 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/dpop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/pkce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/pushed_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/status_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.671195 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/client_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/client_credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/client_credentials/cc_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/client_credentials/cc_refresh_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/refresh_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/server_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oauth2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.675196 idpyoidc-1.4.0/src/idpyoidc/client/oidc/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5687 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.675196 idpyoidc-1.4.0/src/idpyoidc/client/oidc/add_on/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/backchannel_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/check_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/check_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/end_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/provider_info_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/read_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/refresh_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/oidc/webfinger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.675196 idpyoidc-1.4.0/src/idpyoidc/client/provider/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/provider/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/provider/linkedin.py
--rw-r--r--   0 runner    (1001) docker     (123)    38229 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/rp_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.675196 idpyoidc-1.4.0/src/idpyoidc/client/specification/
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/specification/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/specification/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/state_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9392 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/client/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/impexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.675196 idpyoidc-1.4.0/src/idpyoidc/message/
--rw-r--r--   0 runner    (1001) docker     (123)    32969 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.675196 idpyoidc-1.4.0/src/idpyoidc/message/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/message/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/message/oauth2/device_authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.675196 idpyoidc-1.4.0/src/idpyoidc/message/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    41229 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/message/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/message/oidc/backchannel_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/message/oidc/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.679196 idpyoidc-1.4.0/src/idpyoidc/server/
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/authn_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.679196 idpyoidc-1.4.0/src/idpyoidc/server/authz/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3974 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/authz/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18577 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/client_authn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/client_configure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18215 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/construct.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10319 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/cookie_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15425 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11711 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/endpoint_context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1845 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/login_hint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.679196 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.679196 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/add_on/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/add_on/dpop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/add_on/extra_args.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43973 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/pushed_authorization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/server_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6245 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29875 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oauth2/token_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.683196 idpyoidc-1.4.0/src/idpyoidc/server/oidc/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.683196 idpyoidc-1.4.0/src/idpyoidc/server/oidc/add_on/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/add_on/pkce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3698 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/backchannel_authentication.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1161 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/discovery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/provider_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/read_registration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18900 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/session.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1476 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14027 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/token_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6723 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/oidc/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.683196 idpyoidc-1.4.0/src/idpyoidc/server/session/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/session/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10433 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/session/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/session/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/session/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/session/grant_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/session/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/session/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/session/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/template_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.683196 idpyoidc-1.4.0/src/idpyoidc/server/token/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/token/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5373 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/token/handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10764 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/token/id_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/token/jwt_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.683196 idpyoidc-1.4.0/src/idpyoidc/server/user_authn/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/user_authn/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5622 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/user_authn/authn_context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10754 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/user_authn/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.683196 idpyoidc-1.4.0/src/idpyoidc/server/user_info/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/user_info/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/server/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/ssl_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.687196 idpyoidc-1.4.0/src/idpyoidc/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/storage/abfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/time_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-01-19 14:34:58.000000 idpyoidc-1.4.0/src/idpyoidc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 14:35:11.667195 idpyoidc-1.4.0/src/idpyoidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-01-19 14:35:11.000000 idpyoidc-1.4.0/src/idpyoidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-01-19 14:35:11.000000 idpyoidc-1.4.0/src/idpyoidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 14:35:11.000000 idpyoidc-1.4.0/src/idpyoidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 14:35:11.000000 idpyoidc-1.4.0/src/idpyoidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-19 14:35:11.000000 idpyoidc-1.4.0/src/idpyoidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-19 14:35:11.000000 idpyoidc-1.4.0/src/idpyoidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.642208 idpyoidc-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-05 07:55:18.642208 idpyoidc-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:55:18.642208 idpyoidc-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.602207 idpyoidc-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.610207 idpyoidc-2.0.0/src/idpyoidc/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/claims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.610207 idpyoidc-2.0.0/src/idpyoidc/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.614207 idpyoidc-2.0.0/src/idpyoidc/client/claims/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/claims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/claims/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/claims/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/claims/transform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22760 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/client_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4369 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/configure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12100 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/entity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.614207 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11485 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.614207 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/dpop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/pkce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/pushed_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/status_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/refresh_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/resource_owner_password_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/server_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/client/oidc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6312 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/client/oidc/add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/backchannel_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/check_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/check_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/end_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/provider_info_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/refresh_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/webfinger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/client/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/provider/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/provider/linkedin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37660 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/rp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25118 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/service_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/state_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9655 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/impexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1166 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/message/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)    20695 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oauth2/device_authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/message/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    41092 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oidc/backchannel_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oidc/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/authn_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/server/authz/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4191 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/authz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/claims/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/claims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/claims/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/claims/oidc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18698 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/client_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/client_configure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18238 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/construct.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10319 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/cookie_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17179 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15939 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/endpoint_context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1845 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/login_hint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/dpop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/extra_args.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43800 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/pushed_authorization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/server_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7650 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7566 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/access_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2854 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5239 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3657 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12739 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_revocation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/oidc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/pkce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/backchannel_authentication.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/provider_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7742 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/access_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6452 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/token_exchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8215 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/session/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10348 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/grant_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/template_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/token/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4168 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5430 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10787 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/id_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/jwt_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/user_authn/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/user_authn/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5569 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/user_authn/authn_context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11410 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/user_authn/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/user_info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/user_info/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4330 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/ssl_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/storage/abfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.610207 idpyoidc-2.0.0/src/idpyoidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.642208 idpyoidc-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_01_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_03_time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_04_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_05_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55382 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_06_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_07_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21649 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_08_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_09_work_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_11_impexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_12_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_13_dump_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_20_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_21_abfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_22_backchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_00_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_01_service_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_02_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_02b_entity_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_03_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_04_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_05_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21456 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_06_client_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_10_entity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20658 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_12_client_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_14_service_context_impexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_15_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_16_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_17_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_18_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_19_webfinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_20_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_21_oidc_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8912 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_22_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_23_pkce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_24_oic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_25_oauth2_cc_ropc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_26_read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_27_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40243 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_28_rp_handler_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_29_pushed_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_30_rph_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_31_oauth2_persistent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5164 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_32_oidc_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_40_dpop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_41_rp_handler_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_50_ciba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_51_identity_assurance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_55_token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_00_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_00a_client_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_01_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_01_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_02_session_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_03_authz_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_04_session_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_05_token_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_06_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_07_sess_mngm_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23551 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_08_id_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_09_authn_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26303 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_10_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_11_session_manager_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_12_session_life.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_13_user_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_14_userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_15_login_hint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9101 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_16_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_16_endpoint_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_17_client_authn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5537 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20a_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20b_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20c_authz_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25356 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20d_client_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20e_jwt_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20f_userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20g_cookie_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_21_oidc_discovery_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3834 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_22_oidc_provider_config_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14660 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_23_oidc_registration_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28098 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oauth2_authorization_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7926 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oauth2_authorization_endpoint_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24593 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oauth2_resource_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39291 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oauth2_token_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55966 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oidc_authorization_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_25_oauth2_cc_ropc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26880 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_26_oidc_userinfo_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26745 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_30_oidc_end_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_31_oauth2_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_32_oidc_read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_33_oauth2_pkce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9960 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_34_oidc_sso.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45234 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_35_oidc_token_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61543 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_36_oauth2_token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_38_oauth2_revocation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_40_oauth2_pushed_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_50_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_60_dpop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_61_add_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_tandem_08_oauth2_cc_ropc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25517 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_tandem_10_oauth2_token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_y_actor_01.py
```

### Comparing `idpyoidc-1.4.0/LICENSE` & `idpyoidc-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/PKG-INFO` & `idpyoidc-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: idpyoidc
-Version: 1.4.0
+Version: 2.0.0
 Summary: Python implementation of everything OAuth2 and OpenID Connect
 Home-page: https://github.com/IdentityPython/idpy-oidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # idpyoidc
 
 ![CI build](https://github.com/IdentityPython/idpy-oidc/workflows/idpy-oidc/badge.svg)
```

### Comparing `idpyoidc-1.4.0/README.md` & `idpyoidc-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/pyproject.toml` & `idpyoidc-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "idpyoidc"
-version = "1.4.0"
+version = "2.0.0"
 author = "Roland Hedberg"
 author_email = "roland@catalogix.se"
 description = "Everything OAuth2 and OIDC"
 long_description = "file: README.md"
 long_description_content_type = "text/markdown"
 url = "https://github.com/IdentityPython/oidc-op"
 license = "Apache-2.0"
```

### Comparing `idpyoidc-1.4.0/setup.py` & `idpyoidc-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules"],
     install_requires=[
         "cryptojwt>=1.8.1",
         "pyOpenSSL",
         "filelock>=3.0.12",
         'pyyaml>=5.1.2',
         "jinja2>=2.11.3",
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 __author__ = "Roland Hedberg"
-__version__ = "1.4.0"
-
-import os
-from typing import Dict
+__version__ = "2.0.0"
 
 VERIFIED_CLAIM_PREFIX = "__verified"
 
 
 def verified_claim_name(claim):
     return "{}_{}".format(VERIFIED_CLAIM_PREFIX, claim)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/actor/client/oidc/registration.py` & `idpyoidc-2.0.0/src/idpyoidc/client/entity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-import hashlib
 import logging
+from typing import Callable
 from typing import Optional
+from typing import Union
 
-from cryptojwt.utils import as_bytes
-
-from idpyoidc.client.service import Service
-from idpyoidc.message import oidc
-from idpyoidc.message.oauth2 import ResponseMessage
-
-__author__ = "Roland Hedberg"
+from cryptojwt import KeyBundle
+from cryptojwt import KeyJar
+from cryptojwt.jwk.rsa import RSAKey
+from cryptojwt.jwk.rsa import import_private_rsa_key_from_file
+from cryptojwt.key_jar import init_key_jar
+
+from idpyoidc.client.client_auth import client_auth_setup
+from idpyoidc.client.client_auth import method_to_item
+from idpyoidc.client.configure import Configuration
+from idpyoidc.client.defaults import DEFAULT_OAUTH2_SERVICES
+from idpyoidc.client.defaults import DEFAULT_OIDC_SERVICES
+from idpyoidc.client.service import init_services
+from idpyoidc.client.service_context import ServiceContext
+from idpyoidc.context import OidcContext
+from idpyoidc.node import Unit
 
 logger = logging.getLogger(__name__)
 
-rt2gt = {
+RESPONSE_TYPES2GRANT_TYPES = {
     "code": ["authorization_code"],
     "id_token": ["implicit"],
     "id_token token": ["implicit"],
     "code id_token": ["authorization_code", "implicit"],
     "code token": ["authorization_code", "implicit"],
     "code id_token token": ["authorization_code", "implicit"],
 }
@@ -25,193 +34,174 @@
 def response_types_to_grant_types(response_types):
     _res = set()
 
     for response_type in response_types:
         _rt = response_type.split(" ")
         _rt.sort()
         try:
-            _gt = rt2gt[" ".join(_rt)]
+            _gt = RESPONSE_TYPES2GRANT_TYPES[" ".join(_rt)]
         except KeyError:
             logger.warning("No such response type combination: {}".format(response_types))
         else:
             _res.update(set(_gt))
 
     return list(_res)
 
 
-def create_callbacks(
-        issuer: str,
-        hash_seed: str,
-        base_url: str,
-        code: Optional[bool] = False,
-        implicit: Optional[bool] = False,
-        form_post: Optional[bool] = False,
-        request_uris: Optional[bool] = False,
-        backchannel_logout_uri: Optional[bool] = False,
-        frontchannel_logout_uri: Optional[bool] = False,
-):
-    """
-    To mitigate some security issues the redirect_uris should be OP/AS
-    specific. This method creates a set of redirect_uris unique to the
-    OP/AS.
-
-    :param frontchannel_logout_uri: Whether a front-channel logout uri should be constructed
-    :param backchannel_logout_uri: Whether a back-channel logout uri should be constructed
-    :param request_uri: Whether a request_uri should be constructed
-    :param issuer: Issuer ID
-    :return: A set of redirect_uris
-    """
-    _hash = hashlib.sha256()
-    _hash.update(hash_seed)
-    _hash.update(as_bytes(issuer))
-    _hex = _hash.hexdigest()
-
-    res = {"__hex": _hex}
-
-    if code:
-        res["code"] = f"{base_url}/authz_cb/{_hex}"
-
-    if implicit:
-        res["implicit"] = f"{base_url}/authz_im_cb/{_hex}"
-
-    if form_post:
-        res["form_post"] = f"{base_url}/authz_fp_cb/{_hex}"
-
-    if request_uris:
-        res["request_uris"] = f"{base_url}/req_uri/{_hex}"
-
-    if backchannel_logout_uri or frontchannel_logout_uri:
-        res["post_logout_redirect_uris"] = [f"{base_url}/session_logout/{_hex}"]
+def _set_jwks(service_context, config: Configuration, keyjar: Optional[KeyJar]):
+    _key_conf = config.get("key_conf") or config.conf.get('key_conf')
+
+    if _key_conf:
+        keys_args = {k: v for k, v in _key_conf.items() if k != "uri_path"}
+        _keyjar = init_key_jar(**keys_args)
+        service_context.set_preference("jwks", _keyjar.export_jwks())
+    elif keyjar:
+        service_context.set_preference("jwks", keyjar.export_jwks())
 
-    if backchannel_logout_uri:
-        res["backchannel_logout_uri"] = f"{base_url}/bc_logout/{_hex}"
 
-    if frontchannel_logout_uri:
-        res["frontchannel_logout_uri"] = f"{base_url}/fc_logout/{_hex}"
+def set_jwks_uri_or_jwks(service_context, config, jwks_uri, keyjar):
+    # lots of different ways to configure the RP's keys
+    if jwks_uri:
+        service_context.set_preference("jwks_uri", jwks_uri)
+    else:
+        if config.get("jwks_uri"):
+            service_context.set_preference("jwks_uri", jwks_uri)
+        else:
+            _set_jwks(service_context, config, keyjar)
+
 
-    logger.debug(f"Created callback URIs: {res}")
+def redirect_uris_from_callback_uris(callback_uris):
+    res = []
+    for k, v in callback_uris['redirect_uris'].items():
+        res.extend(v)
     return res
 
 
-def _cmp(a, b):
-    if b is None:  # Don't care about the value as long as there is one
-        return True
-    elif isinstance(a, str) and a == b:
-        return True
-    elif isinstance(a, list) and b in a:
-        return True
-
-    return a == b
-
-
-def check(entity, attribute, expected):
-    try:
-        _usable = entity.get_metadata_attribute(attribute)
-    except KeyError:
-        pass
-    else:
-        if _usable is expected:
-            return True
-    return False
+class Entity(Unit):  # This is a Client. What type is undefined here.
+    parameter = {
+        'entity_id': None,
+        'jwks_uri': None,
+        'httpc_params': None,
+        'key_conf': None,
+        'keyjar': KeyJar,
+        'context': None
+    }
+
+    def __init__(
+            self,
+            keyjar: Optional[KeyJar] = None,
+            config: Optional[Union[dict, Configuration]] = None,
+            services: Optional[dict] = None,
+            jwks_uri: Optional[str] = "",
+            httpc: Optional[Callable] = None,
+            httpc_params: Optional[dict] = None,
+            client_type: Optional[str] = "oauth2",
+            context: Optional[OidcContext] = None,
+            upstream_get: Optional[Callable] = None,
+            key_conf: Optional[dict] = None,
+            entity_id: Optional[str] = ''
+    ):
+        if config is None:
+            config = {}
+
+        _id = config.get('client_id')
+        self.client_id = self.entity_id = entity_id or config.get('entity_id', _id)
+
+        Unit.__init__(self, upstream_get=upstream_get, keyjar=keyjar, httpc=httpc,
+                      httpc_params=httpc_params, config=config, key_conf=key_conf,
+                      client_id=self.client_id)
+
+        if services:
+            _srvs = services
+        elif config:
+            _srvs = config.get("services")
+        else:
+            _srvs = None
 
+        if not _srvs:
+            if client_type == 'oauth2':
+                _srvs = DEFAULT_OAUTH2_SERVICES
+            else:
+                _srvs = DEFAULT_OIDC_SERVICES
 
-def add_jwks_uri_or_jwks(request_args=None, service=None, **kwargs):
-    if "jwks_uri" in request_args:
-        if "jwks" in request_args:
-            del request_args["jwks"]  # only one of jwks_uri and jwks allowed
-        return request_args, {}
-    elif "jwks" in request_args:
-        return request_args, {}
+        self._service = init_services(service_definitions=_srvs, upstream_get=self.unit_get)
 
-    for attr in ["jwks_uri", "jwks"]:
-        _val = getattr(service.client_get("service_context"), attr, 0)
-        if _val:
-            request_args[attr] = _val
-            break
+        if context:
+            self.context = context
         else:
-            try:
-                _val = service.client_get("service_context").config[attr]
-            except KeyError:
-                pass
-            else:
-                request_args[attr] = _val
-                break
+            self.context = ServiceContext(config=config, jwks_uri=jwks_uri, keyjar=self.keyjar,
+                                          upstream_get=self.unit_get, client_type=client_type)
 
-    return request_args, {}
+        self.setup_client_authn_methods(config)
 
+        self.upstream_get = upstream_get
 
-class Registration(Service):
-    msg_type = oidc.RegistrationRequest
-    response_cls = oidc.RegistrationResponse
-    error_msg = ResponseMessage
-    endpoint_name = "registration_endpoint"
-    synchronous = True
-    service_name = "registration"
-    request_body_type = "json"
-    http_method = "POST"
-
-    def __init__(self, client_get, conf=None):
-        Service.__init__(self, client_get, conf=conf)
-        self.pre_construct = [
-            self.add_client_behaviour_preference,
-            # add_redirect_uris,
-            # add_callback_uris,
-            add_jwks_uri_or_jwks,
-        ]
-        self.post_construct = [self.oidc_post_construct]
-
-    def add_client_behaviour_preference(self, request_args=None, **kwargs):
-        _context = self.client_get("service_context")
-        for prop in self.msg_type.c_param.keys():
-            if prop in request_args:
-                continue
-
-            try:
-                request_args[prop] = _context.specs.behaviour[prop]
-            except KeyError:
-                try:
-                    request_args[prop] = _context.client_preferences[prop]
-                except KeyError:
-                    pass
-        return request_args, {}
+    def get_services(self, *arg):
+        return self._service
 
-    def oidc_post_construct(self, request_args=None, **kwargs):
-        try:
-            request_args["grant_types"] = response_types_to_grant_types(
-                request_args["response_types"]
-            )
-        except KeyError:
-            pass
+    def get_service_context(self, *arg):  # Want to get rid of this
+        return self.context
 
-        # If a Client can use jwks_uri, it MUST NOT use jwks.
-        if "jwks_uri" in request_args and "jwks" in request_args:
-            del request_args["jwks"]
-
-        return request_args
-
-    def update_service_context(self, resp, key="", **kwargs):
-        if "token_endpoint_auth_method" not in resp:
-            resp["token_endpoint_auth_method"] = "client_secret_basic"
-
-        _context = self.client_get("service_context")
-        _context.registration_response = resp
-        _client_id = resp.get("client_id")
-        if _client_id:
-            _context.set_metadata("client_id", _client_id)
-            if _client_id not in _context.keyjar:
-                _context.keyjar.import_jwks(
-                    _context.keyjar.export_jwks(True, ""), issuer_id=_client_id
-                )
-            _client_secret = resp.get("client_secret")
-            if _client_secret:
-                _context.client_secret = _client_secret
-                _context.keyjar.add_symmetric("", _client_secret)
-                _context.keyjar.add_symmetric(_client_id, _client_secret)
-                try:
-                    _context.client_secret_expires_at = resp["client_secret_expires_at"]
-                except KeyError:
-                    pass
+    def get_context(self, *arg):
+        return self.context
 
+    def get_service(self, service_name, *arg):
         try:
-            _context.registration_access_token = resp["registration_access_token"]
+            return self._service[service_name]
         except KeyError:
-            pass
+            return None
+
+    def get_service_by_endpoint_name(self, endpoint_name, *arg):
+        for service in self._service.values():
+            if service.endpoint_name == endpoint_name:
+                return service
+
+        return None
+
+    def get_entity(self):
+        return self
+
+    def get_client_id(self):
+        _val = self.context.claims.get_usage('client_id')
+        if _val:
+            return _val
+        else:
+            return self.context.claims.get_preference('client_id')
+
+    def setup_client_authn_methods(self, config):
+        if config and "client_authn_methods" in config:
+            _methods = config.get("client_authn_methods")
+            self.context.client_authn_methods = client_auth_setup(method_to_item(_methods))
+        else:
+            self.context.client_authn_methods = {}
+
+    def import_keys(self, keyspec):
+        """
+        The client needs its own set of keys. It can either dynamically
+        create them or load them from local storage.
+        This method can also fetch other entities keys provided the
+        URL points to a JWKS.
+
+        :param keyspec:
+        """
+        _keyjar = self.get_attribute('keyjar')
+        if _keyjar is None:
+            _keyjar = KeyJar()
+
+        for where, spec in keyspec.items():
+            if where == "file":
+                for typ, files in spec.items():
+                    if typ == "rsa":
+                        for fil in files:
+                            _key = RSAKey(priv_key=import_private_rsa_key_from_file(fil),
+                                          use="sig")
+                            _bundle = KeyBundle()
+                            _bundle.append(_key)
+                            _keyjar.add_kb("", _bundle)
+            elif where == "url":
+                for iss, url in spec.items():
+                    _bundle = KeyBundle(source=url)
+                    _keyjar.add_kb(iss, _bundle)
+        return _keyjar
+
+    def get_callback_uris(self):
+        return self.context.claims.callback_uri
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/client_auth.py` & `idpyoidc-2.0.0/src/idpyoidc/client/client_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Implementation of a number of client authentication methods."""
 import base64
 import logging
-from urllib.parse import quote_plus
+from typing import Optional
+from typing import Union
 
 from cryptojwt.exception import MissingKey
 from cryptojwt.exception import UnsupportedAlgorithm
 from cryptojwt.jws.jws import SIGNER_ALGS
 from cryptojwt.jws.utils import alg2keytype
 from cryptojwt.utils import importer
 
 from idpyoidc.defaults import DEF_SIGN_ALG
 from idpyoidc.defaults import JWT_BEARER
-from idpyoidc.message.oauth2 import SINGLE_OPTIONAL_STRING
 from idpyoidc.message.oauth2 import AccessTokenRequest
+from idpyoidc.message.oauth2 import SINGLE_OPTIONAL_STRING
 from idpyoidc.message.oidc import AuthnToken
 from idpyoidc.time_util import utc_time_sans_frac
 from idpyoidc.util import rndstr
-
-from ..message import VREQUIRED
 from .util import sanitize
+from ..message import VREQUIRED
+from ..util import instantiate
 
 # from idpyoidc.oidc.backchannel_authentication import ClientNotificationAuthn
 
 
 LOGGER = logging.getLogger(__name__)
 
 __author__ = "roland hedberg"
@@ -93,23 +94,23 @@
     def _get_passwd(request, service, **kwargs):
         try:
             passwd = kwargs["password"]
         except KeyError:
             try:
                 passwd = request["client_secret"]
             except KeyError:
-                passwd = service.client_get("service_context").client_secret
+                passwd = service.upstream_get("context").get_usage('client_secret')
         return passwd
 
     @staticmethod
     def _get_user(service, **kwargs):
         try:
             user = kwargs["user"]
         except KeyError:
-            user = service.client_get("service_context").get_client_id()
+            user = service.upstream_get("context").get_client_id()
         return user
 
     def _get_authentication_token(self, request, service, **kwargs):
         """
         Return authentication Token.
 
         The credential is username and password concatenated with a ':'
@@ -131,20 +132,20 @@
 
         If we're doing an access token request with an authorization code
         then we should add client_id to the request if it's not already there.
         :param request: A request
         :param service: A :py:class:`idpyoidc.client.service.Service` instance
         """
         if (
-            isinstance(request, AccessTokenRequest)
-            and request["grant_type"] == "authorization_code"
+                isinstance(request, AccessTokenRequest)
+                and request["grant_type"] == "authorization_code"
         ):
             if "client_id" not in request:
                 try:
-                    request["client_id"] = service.client_get("service_context").get_client_id()
+                    request["client_id"] = service.upstream_get("context").get_client_id()
                 except AttributeError:
                     pass
         else:
             # remove client_id if not required by the request definition
             try:
                 _req = request.c_param["client_id"][VREQUIRED]
             except (KeyError, AttributeError):
@@ -213,22 +214,21 @@
         I MUST have a client_secret, there are 3 possible places
         where I can find it. In the request, as an argument in http_args
         or among the client information.
 
         :param request: The request
         :param service: The service that is using this authentication method
         """
-        _context = service.client_get("service_context")
+        _context = service.upstream_get("context")
         if "client_secret" not in request:
             try:
                 request["client_secret"] = kwargs["client_secret"]
             except (KeyError, TypeError):
-                if _context.client_secret:
-                    request["client_secret"] = _context.client_secret
-                else:
+                request["client_secret"] = _context.get_usage('client_secret')
+                if not request["client_secret"]:
                     raise AuthnFailure("Missing client secret")
 
         # Set the client_id in the the request
         request["client_id"] = _context.get_client_id()
 
     def construct(self, request, service=None, http_args=None, **kwargs):
         """
@@ -269,36 +269,30 @@
             # Required under certain circumstances :-) not under other
             request.c_param[token_type] = SINGLE_OPTIONAL_STRING
             return _token
 
     try:
         return kwargs["access_token"]
     except KeyError:
-        # I should pick the latest acquired token, this should be the right
-        # order for that.
+        # Get the latest acquired token.
         _state = kwargs.get("state", kwargs.get("key"))
-        _arg = service.client_get("service_context").state.multiple_extend_request_args(
-            {},
-            _state,
-            ["access_token"],
-            ["auth_response", "token_response", "refresh_token_response"],
-        )
+        _arg = service.upstream_get("context").cstate.get_set(_state, claim=[token_type])
         return _arg.get("access_token")
 
 
 class BearerHeader(ClientAuthnMethod):
     """The bearer header authentication method."""
 
     def construct(self, request=None, service=None, http_args=None, **kwargs):
         """
         Constructing the Authorization header. The value of
         the Authorization header is "Bearer <access_token>".
 
         :param request: Request class instance
-        :param service: Service
+        :param service: The service this authentication method applies to.
         :param http_args: HTTP header arguments
         :param kwargs: extra keyword arguments
         :return:
         """
 
         if service.service_name == "refresh_token":
             _acc_token = find_token(request, "refresh_token", service, **kwargs)
@@ -404,120 +398,119 @@
             # different contexts uses different signing algorithms
             algorithm = DEF_SIGN_ALG[context]
         if not algorithm:
             raise AuthnFailure("Missing algorithm specification")
         return algorithm
 
     @staticmethod
-    def get_signing_key_from_keyjar(algorithm, service_context):
+    def get_signing_key_from_keyjar(algorithm, keyjar):
         """
         Pick signing key based on signing algorithm to be used
 
         :param algorithm: Signing algorithm
-        :param service_context: A :py:class:`idpyoidc.client.service_context.ServiceContext` instance
+        :param service_context: A :py:class:`idpyoidc.client.service_context.ServiceContext`
+        instance
         :return: A key
         """
-        return service_context.keyjar.get_signing_key(alg2keytype(algorithm), alg=algorithm)
+        return keyjar.get_signing_key(alg2keytype(algorithm), alg=algorithm)
 
     @staticmethod
-    def _get_key_by_kid(kid, algorithm, service_context):
+    def _get_key_by_kid(kid, algorithm, keyjar):
         """
         Pick a key that matches a given key ID and signing algorithm.
 
         :param kid: Key ID
         :param algorithm: Signing algorithm
         :param service_context: A
             :py:class:`idpyoidc.client.service_context.ServiceContext` instance
         :return: A matching key
         """
         # signing so using my keys
-        for _key in service_context.keyjar.get_issuer_keys(""):
+        for _key in keyjar.get_issuer_keys(""):
             if kid == _key.kid:
                 ktype = alg2keytype(algorithm)
                 if _key.kty != ktype:
                     raise MissingKey("Wrong key type")
 
                 return _key
 
         raise MissingKey("No key with kid:%s" % kid)
 
-    def _get_signing_key(self, algorithm, context, kid=None):
+    def _get_signing_key(self, algorithm, keyjar, key_types, kid=None):
         ktype = alg2keytype(algorithm)
         try:
             if kid:
-                signing_key = [self._get_key_by_kid(kid, algorithm, context)]
-            elif ktype in context.kid["sig"]:
+                signing_key = [self._get_key_by_kid(kid, algorithm, keyjar)]
+            elif ktype in key_types:
                 try:
                     signing_key = [
-                        self._get_key_by_kid(context.kid["sig"][ktype], algorithm, context)
+                        self._get_key_by_kid(key_types[ktype], algorithm, keyjar)
                     ]
                 except KeyError:
-                    signing_key = self.get_signing_key_from_keyjar(algorithm, context)
+                    signing_key = self.get_signing_key_from_keyjar(algorithm, keyjar)
             else:
-                signing_key = self.get_signing_key_from_keyjar(algorithm, context)
+                signing_key = self.get_signing_key_from_keyjar(algorithm, keyjar)
         except (MissingKey,) as err:
             LOGGER.error("%s", sanitize(err))
             raise
 
         return signing_key
 
-    def _get_audience_and_algorithm(self, context, entity, **kwargs):
+    def _get_audience_and_algorithm(self, context, keyjar, **kwargs):
         algorithm = None
 
         # audience for the signed JWT depends on which endpoint
         # we're talking to.
         if "authn_endpoint" in kwargs and kwargs["authn_endpoint"] in ["token_endpoint"]:
-            _alg = context.registration_response.get("token_endpoint_auth_signing_alg")
-            if _alg :
-                algorithm = _alg
-            else:
-                algorithm = entity.get_metadata_value("token_endpoint_auth_signing_alg")
-                if algorithm is None:
-                    _pi = context.provider_info
-                    try:
-                        algs = _pi["token_endpoint_auth_signing_alg_values_supported"]
-                    except KeyError:
-                        algorithm = "RS256"  # default
-                    else:
-                        for alg in algs:  # pick the first one I support and have keys for
-                            if alg in SIGNER_ALGS and self.get_signing_key_from_keyjar(
-                                alg, context
-                            ):
-                                algorithm = alg
-                                break
+            algorithm = context.get_usage("token_endpoint_auth_signing_alg")
+            if algorithm is None:
+                _pi = context.provider_info
+                try:
+                    algs = _pi["token_endpoint_auth_signing_alg_values_supported"]
+                except KeyError:
+                    algorithm = "RS256"  # default
+                else:
+                    for alg in algs:  # pick the first one I support and have keys for
+                        if alg in SIGNER_ALGS and self.get_signing_key_from_keyjar(
+                                alg, keyjar
+                        ):
+                            algorithm = alg
+                            break
 
-            audience = context.provider_info["token_endpoint"]
+            audience = context.provider_info.get("token_endpoint")
         else:
             audience = context.provider_info["issuer"]
 
         if not algorithm:
             algorithm = self.choose_algorithm(**kwargs)
         return audience, algorithm
 
     def _construct_client_assertion(self, service, **kwargs):
-        _context = service.client_get("service_context")
-        _entity = service.client_get("entity")
-        audience, algorithm = self._get_audience_and_algorithm(_context, _entity, **kwargs)
+        _context = service.upstream_get("context")
+        _entity = service.upstream_get("entity")
+        _keyjar = service.upstream_get('attribute', 'keyjar')
+        audience, algorithm = self._get_audience_and_algorithm(_context, _keyjar, **kwargs)
 
         if "kid" in kwargs:
-            signing_key = self._get_signing_key(algorithm, _context, kid=kwargs["kid"])
+            signing_key = self._get_signing_key(algorithm, _keyjar, _context.kid["sig"],
+                                                kid=kwargs["kid"])
         else:
-            signing_key = self._get_signing_key(algorithm, _context)
+            signing_key = self._get_signing_key(algorithm, _keyjar, _context.kid["sig"])
 
         if not signing_key:
             raise UnsupportedAlgorithm(algorithm)
 
         try:
             _args = {"lifetime": kwargs["lifetime"]}
         except KeyError:
             _args = {}
 
         # construct the signed JWT with the assertions and add
         # it as value to the 'client_assertion' claim of the request
-        return assertion_jwt(_entity.get_client_id(), signing_key, audience, algorithm, **_args)
+        return assertion_jwt(_entity.client_id, signing_key, audience, algorithm, **_args)
 
     def modify_request(self, request, service, **kwargs):
         """
         Modify the request if necessary.
 
         :param request: The request
         :param service: The service using this authentication method.
@@ -572,28 +565,28 @@
     The HMAC (Hash-based Message Authentication Code) is calculated using the
     bytes of the UTF-8 representation of the client_secret as the shared key.
     """
 
     def choose_algorithm(self, context="client_secret_jwt", **kwargs):
         return JWSAuthnMethod.choose_algorithm(context, **kwargs)
 
-    def get_signing_key_from_keyjar(self, algorithm, service_context):
-        return service_context.keyjar.get_signing_key(alg2keytype(algorithm), alg=algorithm)
+    def get_signing_key_from_keyjar(self, algorithm, keyjar):
+        return keyjar.get_signing_key(alg2keytype(algorithm), alg=algorithm)
 
 
 class PrivateKeyJWT(JWSAuthnMethod):
     """
     Clients that have registered a public key can sign a JWT using that key.
     """
 
     def choose_algorithm(self, context="private_key_jwt", **kwargs):
         return JWSAuthnMethod.choose_algorithm(context, **kwargs)
 
-    def get_signing_key_from_keyjar(self, algorithm, service_context=None):
-        return service_context.keyjar.get_signing_key(alg2keytype(algorithm), "", alg=algorithm)
+    def get_signing_key_from_keyjar(self, algorithm, keyjar):
+        return keyjar.get_signing_key(alg2keytype(algorithm), "", alg=algorithm)
 
 
 # Map from client authentication identifiers to corresponding class
 CLIENT_AUTHN_METHOD = {
     "client_secret_basic": ClientSecretBasic,
     "client_secret_post": ClientSecretPost,
     "bearer_header": BearerHeader,
@@ -618,19 +611,58 @@
     eta = service_context.client_secret_expires_at
     now = when or utc_time_sans_frac()
     if eta != 0 and eta < now:
         return False
     return True
 
 
-def client_auth_setup(auth_set=None):
+def get_client_authn_class(name):
+    try:
+        return CLIENT_AUTHN_METHOD[name]
+    except KeyError:
+        return None
+
+
+def get_client_authn_methods():
+    return list(CLIENT_AUTHN_METHOD.keys())
+
+
+def method_to_item(methods):
+    if isinstance(methods, list):
+        return {k: get_client_authn_class(k) for k in methods if get_client_authn_class(k)}
+    elif isinstance(methods, dict):
+        return methods
+    elif not methods:
+        return {}
+
+
+def single_authn_setup(name, spec):
+    if isinstance(spec, dict):  # class and kwargs
+        if spec:
+            return instantiate(spec["class"], **spec["kwargs"])
+        else:
+            cls = get_client_authn_class(name)
+            return cls()
+    else:
+        if spec is None:
+            cls = get_client_authn_class(name)
+        elif isinstance(spec, str):
+            cls = importer(spec)
+        else:
+            cls = spec
+        return cls()
+
+
+def client_auth_setup(auth_set: Optional[Union[list, dict]] = None):
     if auth_set is None:
         auth_set = CLIENT_AUTHN_METHOD
-    else:
-        auth_set.update(CLIENT_AUTHN_METHOD)
+
     res = {}
 
-    for name, cls in auth_set.items():
-        if isinstance(cls, str):
-            cls = importer(cls)
-        res[name] = cls()
+    if isinstance(auth_set, list):  # From the known set
+        for name in auth_set:
+            res[name] = single_authn_setup(name, None)
+    else:
+        for name, spec in auth_set.items():
+            res[name] = single_authn_setup(name, spec)
+
     return res
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/configure.py` & `idpyoidc-2.0.0/src/idpyoidc/client/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from idpyoidc.configure import Base
 from idpyoidc.logging import configure_logging
-from idpyoidc.message.oidc import RegistrationResponse
 from .util import lower_or_upper
 
 try:
     from secrets import token_urlsafe as rnd_token
 except ImportError:
     from cryptojwt import rndstr as rnd_token
 
@@ -22,14 +21,15 @@
     "backchannel_logout_uri",
     "issuer",
     "base_url",
 ]
 
 
 class RPHConfiguration(Base):
+
     def __init__(
             self,
             conf: Dict,
             base_path: Optional[str] = "",
             entity_conf: Optional[List[dict]] = None,
             domain: Optional[str] = "127.0.0.1",
             port: Optional[int] = 80,
@@ -59,23 +59,23 @@
         self.hash_seed = hash_seed
 
         self.base_url = lower_or_upper(conf, "base_url")
         self.httpc_params = lower_or_upper(conf, "httpc_params", {"verify": True})
 
         self.default = lower_or_upper(conf, "default", {})
 
-        for param in ["services", "metadata", "add_ons", "usage"]:
+        for param in ["services", "claims", "add_ons", "usage"]:
             _val = lower_or_upper(conf, param, {})
             if _val and param not in self.default:
                 self.default[param] = _val
 
         self.clients = lower_or_upper(conf, "clients")
         if self.clients:
             for id, client in self.clients.items():
-                for param in ["services", "usage", "add_ons", 'metadata']:
+                for param in ["services", "usage", "add_ons", 'claims']:
                     if param not in client:
                         if param in self.default:
                             client[param] = self.default[param]
 
         if entity_conf:
             self.extend(
                 entity_conf=entity_conf,
@@ -108,15 +108,15 @@
             dir_attributes=dir_attributes,
         )
 
         _del_key = []
         for attr, val in self.conf.items():
             if attr in ["issuer", "key_conf"]:
                 setattr(self, attr, val)
-                _del_key.append(attr)
+                # _del_key.append(attr)
 
         for _key in _del_key:
             del self.conf[_key]
 
         log_conf = conf.get("logging")
         if log_conf:
             self.logger = configure_logging(config=log_conf).getChild(__name__)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/cookie.py` & `idpyoidc-2.0.0/src/idpyoidc/client/cookie.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/defaults.py` & `idpyoidc-2.0.0/src/idpyoidc/client/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,37 +22,37 @@
     "authorization": {"class": "idpyoidc.client.oauth2.authorization.Authorization"},
     "access_token": {"class": "idpyoidc.client.oauth2.access_token.AccessToken"},
     "refresh_access_token": {
         "class": "idpyoidc.client.oauth2.refresh_access_token.RefreshAccessToken"
     },
 }
 
-DEFAULT_CLIENT_METADATA = {
+DEFAULT_CLIENT_PREFERENCES = {
     "application_type": "web",
     "response_types": [
         "code",
         "id_token",
         "id_token token",
         "code id_token",
         "code id_token token",
         "code token",
     ],
     "token_endpoint_auth_method": "client_secret_basic",
+    "scopes_supported": ["openid"],
 }
 
 DEFAULT_USAGE = {
     "jwks_uri": True,
     "scope": ["openid"],
 }
 
 # Using PKCE is default
 DEFAULT_CLIENT_CONFIGS = {
     "": {
-        "metadata": DEFAULT_CLIENT_METADATA,
-        "usage": DEFAULT_USAGE,
+        "preference": DEFAULT_CLIENT_PREFERENCES,
         "add_ons": {
             "pkce": {
                 "function": "idpyoidc.client.oauth2.add_on.pkce.add_support",
                 "kwargs": {"code_challenge_length": 64, "code_challenge_method": "S256"},
             }
         },
     }
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/exception.py` & `idpyoidc-2.0.0/src/idpyoidc/client/exception.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/http.py` & `idpyoidc-2.0.0/src/idpyoidc/client/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import logging
 from http.cookiejar import FileCookieJar
 from http.cookies import CookieError
 from http.cookies import SimpleCookie
 
-import requests
+from requests import request
 from idpyoidc.client.exception import NonFatalException
 from idpyoidc.client.util import sanitize
 from idpyoidc.client.util import set_cookie
 
 __author__ = "roland"
 
 logger = logging.getLogger(__name__)
@@ -63,15 +63,15 @@
             logger.debug("RECEIVED COOKIE")
             try:
                 # add received cookies to the cookie jar
                 set_cookie(self.cookiejar, SimpleCookie(_cookie))
             except CookieError as err:
                 logger.error(err)
                 raise NonFatalException(response, "{}".format(err))
-        except (AttributeError, KeyError) as err:
+        except (AttributeError, KeyError):
             pass
 
     def __call__(self, url, method="GET", **kwargs):
         """
         Send a HTTP request to a URL using a specified method
 
         :param url: The URL to access
@@ -90,15 +90,15 @@
 
         # If I want to modify the request arguments based on URL, method
         # and current arguments I can use this call back function.
         self.run_req_callback(url, method, kwargs)
 
         try:
             # Do the request
-            r = requests.request(method, url, **_kwargs)
+            r = request(method, url, **_kwargs)
         except Exception as err:
             logger.error(
                 "http_request failed: %s, url: %s, htargs: %s, method: %s"
                 % (err, url, sanitize(_kwargs), method)
             )
             raise
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-import logging
 from json import JSONDecodeError
+import logging
+from typing import Callable
 from typing import Optional
+from typing import Union
+
+from cryptojwt.key_jar import KeyJar
+from requests import request
 
 from idpyoidc.client.entity import Entity
 from idpyoidc.client.exception import ConfigurationError
 from idpyoidc.client.exception import OidcServiceError
 from idpyoidc.client.exception import ParseError
-from idpyoidc.client.http import HTTPLib
 from idpyoidc.client.service import REQUEST_INFO
 from idpyoidc.client.service import SUCCESSFUL
 from idpyoidc.client.service import Service
 from idpyoidc.client.util import do_add_ons
 from idpyoidc.client.util import get_deserialization_method
 from idpyoidc.configure import Configuration
+from idpyoidc.context import OidcContext
 from idpyoidc.exception import FormatError
 from idpyoidc.message import Message
 from idpyoidc.message.oauth2 import is_error_message
 
 __author__ = "Roland Hedberg"
 
 logger = logging.getLogger(__name__)
@@ -28,146 +33,161 @@
     pass
 
 
 # =============================================================================
 
 
 class Client(Entity):
+    client_type = 'oauth2'
     def __init__(
-        self,
-        keyjar=None,
-        verify_ssl=True,
-        config=None,
-        httplib=None,
-        services=None,
-        jwks_uri="",
-        httpc_params=None,
-        client_type: Optional[str] = ""
+            self,
+            keyjar: Optional[KeyJar] = None,
+            config: Optional[Union[dict, Configuration]] = None,
+            services: Optional[dict] = None,
+            httpc: Optional[Callable] = None,
+            httpc_params: Optional[dict] = None,
+            context: Optional[OidcContext] = None,
+            upstream_get: Optional[Callable] = None,
+            key_conf: Optional[dict] = None,
+            entity_id: Optional[str] = '',
+            verify_ssl: Optional[bool] = True,
+            jwks_uri: Optional[str] = "",
+            client_type: Optional[str] = "",
+            **kwargs
     ):
         """
 
         :type client_type: str
         :param client_type: What kind of client this is. Presently 'oauth2' or 'oidc'
         :param keyjar: A py:class:`idpyoidc.key_jar.KeyJar` instance
         :param config: Configuration information passed on to the
             :py:class:`idpyoidc.client.service_context.ServiceContext`
             initialization
-        :param httplib: A HTTP client to use
+        :param httpc: A HTTP client to use
+        :param httpc_params: HTTP request arguments
         :param services: A list of service definitions
         :param jwks_uri: A jwks_uri
-        :param httpc_params: HTTP request arguments
         :return: Client instance
         """
 
         if not client_type:
-            client_type = "oauth2"
+            client_type = self.client_type
+
+        if verify_ssl is False:
+            # just ignore verify_ssl until it goes away
+            if httpc_params:
+                httpc_params['verify'] = False
+            else:
+                httpc_params = {'verify': False}
 
         Entity.__init__(
             self,
             keyjar=keyjar,
             config=config,
             services=services,
             jwks_uri=jwks_uri,
+            httpc=httpc,
             httpc_params=httpc_params,
-            client_type=client_type
+            client_type=client_type,
+            context=context,
+            upstream_get=upstream_get,
+            key_conf=key_conf,
+            entity_id=entity_id
         )
 
-        self.http = httplib or HTTPLib(httpc_params)
+        self.httpc = httpc or request
 
         if isinstance(config, Configuration):
             _add_ons = config.conf.get("add_ons")
         else:
             _add_ons = config.get("add_ons")
 
         if _add_ons:
             do_add_ons(_add_ons, self._service)
 
-        # just ignore verify_ssl until it goes away
-        self.verify_ssl = self.httpc_params.get("verify", True)
-
     def do_request(
-        self,
-        request_type: str,
-        response_body_type: Optional[str] = "",
-        request_args: Optional[dict] = None,
-        behaviour_args: Optional[dict] = None,
-        **kwargs
+            self,
+            request_type: str,
+            response_body_type: Optional[str] = "",
+            request_args: Optional[dict] = None,
+            behaviour_args: Optional[dict] = None,
+            **kwargs
     ):
         _srv = self._service[request_type]
 
         _info = _srv.get_request_parameters(request_args=request_args, **kwargs)
 
         if not response_body_type:
             response_body_type = _srv.response_body_type
 
         logger.debug("do_request info: {}".format(_info))
 
         try:
             _state = kwargs["state"]
-        except:
+        except Exception:
             _state = ""
         return self.service_request(
             _srv, response_body_type=response_body_type, state=_state, **_info
         )
 
     def set_client_id(self, client_id):
-        self._service_context.set("client_id", client_id)
+        self.get_context().set("client_id", client_id)
 
     def get_response(
-        self,
-        service: Service,
-        url: str,
-        method: Optional[str] = "GET",
-        body: Optional[dict] = None,
-        response_body_type: Optional[str] = "",
-        headers: Optional[dict] = None,
-        **kwargs
+            self,
+            service: Service,
+            url: str,
+            method: Optional[str] = "GET",
+            body: Optional[dict] = None,
+            response_body_type: Optional[str] = "",
+            headers: Optional[dict] = None,
+            **kwargs
     ):
         """
 
         :param url:
         :param method:
         :param body:
         :param response_body_type:
         :param headers:
         :param kwargs:
         :return:
         """
         try:
-            resp = self.http(url, method, data=body, headers=headers)
+            resp = self.httpc(method, url, data=body, headers=headers, **self.httpc_params)
         except Exception as err:
             logger.error("Exception on request: {}".format(err))
             raise
 
         if 300 <= resp.status_code < 400:
             return {"http_response": resp}
 
         if resp.status_code < 300:
             if "keyjar" not in kwargs:
-                kwargs["keyjar"] = service.client_get("service_context").keyjar
+                kwargs["keyjar"] = self.get_attribute('keyjar')
             if not response_body_type:
                 response_body_type = service.response_body_type
 
             if response_body_type == "html":
                 return resp.text
 
             if body:
                 kwargs["request_body"] = body
 
         return self.parse_request_response(service, resp, response_body_type, **kwargs)
 
     def service_request(
-        self,
-        service: Service,
-        url: str,
-        method: Optional[str] = "GET",
-        body: Optional[dict] = None,
-        response_body_type: Optional[str] = "",
-        headers: Optional[dict] = None,
-        **kwargs
+            self,
+            service: Service,
+            url: str,
+            method: Optional[str] = "GET",
+            body: Optional[dict] = None,
+            response_body_type: Optional[str] = "",
+            headers: Optional[dict] = None,
+            **kwargs
     ) -> Message:
         """
         The method that sends the request and handles the response returned.
         This assumes that the response arrives in the HTTP response.
 
         :param service: The Service instance
         :param url: The URL to which the request should be sent
@@ -193,25 +213,20 @@
             response = self.get_response(
                 service, url, method, body, response_body_type, headers, **kwargs
             )
 
         if "error" in response:
             pass
         else:
-            try:
-                kwargs["key"] = kwargs["state"]
-            except KeyError:
-                pass
-
-            service.update_service_context(response, **kwargs)
+            service.update_service_context(response, key=kwargs.get('state'), **kwargs)
         return response
 
     def parse_request_response(self, service, reqresp, response_body_type="", state="", **kwargs):
         """
-        Deal with a self.http response. The response are expected to
+        Deal with a self.httpc response. The response are expected to
         follow a special pattern, having the attributes:
 
             - headers (list of tuples with headers attributes and their values)
             - status_code (integer)
             - text (The text version of the response)
             - url (The calling URL)
 
@@ -297,15 +312,15 @@
     :param client: A :py:class:`idpyoidc.client.oidc.Client` instance
     """
     try:
         client.get_service("provider_info")
     except KeyError:
         raise ConfigurationError("Can not do dynamic provider info discovery")
     else:
-        _context = client.client_get("service_context")
+        _context = client.get_context()
         try:
             _context.set("issuer", _context.config["srv_discovery_url"])
         except KeyError:
             pass
 
         response = client.do_request("provider_info", behaviour_args=behaviour_args)
         if is_error_message(response):
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/access_token.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/access_token.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Implements the service that talks to the Access Token endpoint."""
 import logging
+from typing import Optional
 
+from idpyoidc.client.client_auth import get_client_authn_methods
 from idpyoidc.client.oauth2.utils import get_state_parameter
 from idpyoidc.client.service import Service
 from idpyoidc.message import oauth2
 from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.time_util import time_sans_frac
+from idpyoidc.claims import get_signing_algs
 
 LOGGER = logging.getLogger(__name__)
 
 
 class AccessToken(Service):
     """The access token service."""
 
@@ -20,50 +23,43 @@
     synchronous = True
     service_name = "accesstoken"
     default_authn_method = "client_secret_basic"
     http_method = "POST"
     request_body_type = "urlencoded"
     response_body_type = "json"
 
-    metadata_attributes = {
-        "token_endpoint_auth_method": "client_secret_basic",
-        "token_endpoint_auth_signing_alg": "RS256"
-    }
+    _include = {"grant_types_supported": ['authorization_code']}
 
-    usage_rules = {
-        "token_endpoint_auth_methods": None
+    _supports = {
+        "token_endpoint_auth_methods_supported": get_client_authn_methods,
+        "token_endpoint_auth_signing_alg": get_signing_algs,
     }
 
-    def __init__(self, client_get, conf=None):
-        Service.__init__(self, client_get, conf=conf)
+    def __init__(self, upstream_get, conf=None):
+        Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct.append(self.oauth_pre_construct)
 
-    def update_service_context(self, resp, key="", **kwargs):
+    def update_service_context(self, resp, key: Optional[str] = '', **kwargs):
         if "expires_in" in resp:
             resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
-        self.client_get("service_context").state.store_item(resp, "token_response", key)
+        if key:
+            self.upstream_get("context").cstate.update(key, resp)
 
     def oauth_pre_construct(self, request_args=None, post_args=None, **kwargs):
         """
 
         :param request_args: Initial set of request arguments
         :param kwargs: Extra keyword arguments
         :return: Request arguments
         """
         _state = get_state_parameter(request_args, kwargs)
         parameters = list(self.msg_type.c_param.keys())
 
-        _context = self.client_get("service_context")
-        _args = _context.state.extend_request_args(
-            {}, oauth2.AuthorizationRequest, "auth_request", _state, parameters
-        )
-
-        _args = _context.state.extend_request_args(
-            _args, oauth2.AuthorizationResponse, "auth_response", _state, parameters
-        )
+        _context = self.upstream_get("context")
+        _args = _context.cstate.get_set(_state, claim=parameters)
 
         if "grant_type" not in _args:
             _args["grant_type"] = "authorization_code"
 
         if request_args is None:
             request_args = _args
         else:
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/dpop.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/dpop.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,28 +140,28 @@
         headers = {"dpop": jws}
     else:
         headers["dpop"] = jws
 
     return headers
 
 
-def add_support(services, signing_algorithms):
+def add_support(services, dpop_signing_alg_values_supported):
     """
     Add the necessary pieces to make pushed authorization happen.
 
     :param services: A dictionary with all the services the client has access to.
     :param signing_algorithms: Allowed signing algorithms, there is no default algorithms
     """
 
     # Access token request should use DPoP header
     _service = services["accesstoken"]
-    _context = _service.client_get("service_context")
+    _context = _service.upstream_get("context")
     _context.add_on["dpop"] = {
         # "key": key_by_alg(signing_algorithm),
-        "sign_algs": signing_algorithms
+        "sign_algs": dpop_signing_alg_values_supported
     }
     _service.construct_extra_headers.append(dpop_header)
 
     # The same for userinfo requests
     _userinfo_service = services.get("userinfo")
     if _userinfo_service:
         _userinfo_service.construct_extra_headers.append(dpop_header)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,18 @@
             else:
                 _resp[json.dumps(vr["verification"])] = vr["claims"]
 
     return _resp
 
 
 def identity_assurance_process(response, service_context, state):
-    auth_request = service_context.state.get_item(AuthorizationRequest, "auth_request", state)
+    auth_request = service_context.cstate.get_set(state,
+                                                  message=AuthorizationRequest)
     claims_request = auth_request.get("claims")
-    if "userinfo" in claims_request:
+    if claims_request and "userinfo" in claims_request:
         vc = VerifiedClaims(**response["verified_claims"])
 
         # find the claims request in the authorization request
         verified_response = match_verified_claims(vc, claims_request["userinfo"]["verified_claims"])
         _response_format = service_context.add_on["identity_assurance"]["response_format"]
         response = format_response(_response_format, response, verified_response)
     return response
@@ -68,15 +69,15 @@
     :param claims_in_verified_claims_supported:
     :param verified_claims_request:
     :param response_format: One of 'claims', 'per_claim', 'per_verification'
     """
 
     # Access token request should use DPoP header
     _service = services["userinfo"]
-    _context = _service.client_get("service_context")
+    _context = _service.upstream_get("context")
     _context.add_on["identity_assurance"] = {
         "verified_claims_supported": True,
         "trust_frameworks_supported": trust_frameworks_supported,
         "evidence_supported": evidence_supported,
         "id_documents_supported": id_documents_supported,
         "id_documents_verification_methods_supported": id_documents_verification_methods_supported,
         "claims_in_verified_claims_supported": claims_in_verified_claims_supported,
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/pkce.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/pkce.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     :py:class:`idpyoidc.client.oidc.service.Authorization` instance
 
     :param service: The service that uses this function
     :param request_args: Set of request arguments
     :param kwargs: Extra set of keyword arguments
     :return: Updated set of request arguments
     """
-    _context = service.client_get("service_context")
+    _context = service.upstream_get("context")
     _kwargs = _context.add_on["pkce"]
 
     try:
         cv_len = _kwargs["code_challenge_length"]
     except KeyError:
         cv_len = 64  # Use default
 
@@ -46,15 +46,15 @@
         _hv = _hash_method(_cv).digest()
         # base64 encode the hash value
         code_challenge = b64e(_hv).decode("ascii")
     except KeyError:
         raise Unsupported("PKCE Transformation method:{}".format(_method))
 
     _item = Message(code_verifier=code_verifier, code_challenge_method=_method)
-    _context.state.store_item(_item, "pkce", request_args["state"])
+    _context.cstate.update(request_args["state"], _item)
 
     request_args.update({"code_challenge": code_challenge, "code_challenge_method": _method})
     return request_args, {}
 
 
 def add_code_verifier(request_args, service, **kwargs):
     """
@@ -65,16 +65,16 @@
     :param service: The service that uses this function
     :param request_args: Set of request arguments
     :return: updated set of request arguments
     """
     _state = request_args.get("state")
     if _state is None:
         _state = kwargs.get("state")
-    _item = service.client_get("service_context").state.get_item(Message, "pkce", _state)
-    request_args.update({"code_verifier": _item["code_verifier"]})
+    _item = service.upstream_get("context").cstate.get_set(_state, claim=['code_verifier'])
+    request_args.update(_item)
     return request_args
 
 
 def put_state_in_post_args(request_args, **kwargs):
     state = get_state_parameter(request_args, kwargs)
     return request_args, {"state": state}
 
@@ -87,15 +87,15 @@
     :param service: Dictionary of services
     :param code_challenge_length:
     :param code_challenge_method:
     :return:
     """
     if "authorization" in service and "accesstoken" in service:
         _service = service["authorization"]
-        _context = _service.client_get("service_context")
+        _context = _service.upstream_get("context")
         _context.add_on["pkce"] = {
             "code_challenge_length": code_challenge_length,
             "code_challenge_method": code_challenge_method,
         }
 
         _service.pre_construct.append(add_code_challenge)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/pushed_authorization.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/pushed_authorization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,83 @@
 import logging
 
 from cryptojwt import JWT
+from requests import request
 
-import requests
 from idpyoidc.message import Message
 from idpyoidc.message.oauth2 import JWTSecuredAuthorizationRequest
 
 logger = logging.getLogger(__name__)
 
 
 def push_authorization(request_args, service, **kwargs):
     """
     :param request_args: All the request arguments as a AuthorizationRequest instance
     :param service: The service to which this post construct method is applied.
     :param kwargs: Extra keyword arguments.
     """
 
-    _context = service.client_get("service_context")
+    _context = service.upstream_get("context")
     method_args = _context.add_on["pushed_authorization"]
+    if method_args['apply'] is False:
+        return request_args
 
     # construct the message body
     if method_args["body_format"] == "urlencoded":
         _body = request_args.to_urlencoded()
     else:
-        _jwt = JWT(key_jar=_context.keyjar, iss=_context.base_url)
+        _jwt = JWT(key_jar=service.upstream_get('attribute', 'keyjar'),
+                   iss=_context.base_url)
         _jws = _jwt.pack(request_args.to_dict())
 
         _msg = Message(request=_jws)
         if method_args["merge_rule"] == "lax":
             for param in request_args.required_parameters():
                 _msg[param] = request_args.get(param)
 
         _body = _msg.to_urlencoded()
 
     # Send it to the Pushed Authorization Request Endpoint
-    resp = method_args["http_client"].get(
-        _context.provider_info["pushed_authorization_request_endpoint"], data=_body
+    resp = method_args["http_client"](
+        method="GET",
+        url=_context.provider_info["pushed_authorization_request_endpoint"],
+        data=_body
     )
 
     if resp.status_code == 200:
         _resp = Message().from_json(resp.text)
         _req = JWTSecuredAuthorizationRequest(request_uri=_resp["request_uri"])
         if method_args["merge_rule"] == "lax":
             for param in request_args.required_parameters():
                 _req[param] = request_args.get(param)
         request_args = _req
 
     return request_args
 
 
 def add_support(
-    services, body_format="jws", signing_algorithm="RS256", http_client=None, merge_rule="strict"
+        services, body_format="jws", signing_algorithm="RS256", http_client=None,
+        merge_rule="strict"
 ):
     """
     Add the necessary pieces to make Demonstration of proof of possession (DPOP).
 
     :param merge_rule:
     :param http_client:
     :param signing_algorithm:
     :param services: A dictionary with all the services the client has access to.
     :param body_format: jws or urlencoded
     """
 
     if http_client is None:
-        http_client = requests
+        http_client = request
 
     _service = services["authorization"]
-    _service.client_get("service_context").add_on["pushed_authorization"] = {
+    _service.upstream_get("context").add_on["pushed_authorization"] = {
         "body_format": body_format,
         "signing_algorithm": signing_algorithm,
         "http_client": http_client,
         "merge_rule": merge_rule,
+        'apply': True
     }
 
     _service.post_construct.append(push_authorization)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/add_on/status_check.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/status_check.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/client_credentials/cc_access_token.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oidc/check_session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+import logging
+
 from idpyoidc.client.service import Service
-from idpyoidc.message import oauth2
+from idpyoidc.message.oauth2 import Message
 from idpyoidc.message.oauth2 import ResponseMessage
-from idpyoidc.time_util import time_sans_frac
+from idpyoidc.message.oidc import session
+
+__author__ = "Roland Hedberg"
+
+logger = logging.getLogger(__name__)
 
 
-class CCAccessToken(Service):
-    msg_type = oauth2.CCAccessTokenRequest
-    response_cls = oauth2.AccessTokenResponse
+class CheckSession(Service):
+    msg_type = session.CheckSessionRequest
+    response_cls = Message
     error_msg = ResponseMessage
-    endpoint_name = "token_endpoint"
+    endpoint_name = ""
     synchronous = True
-    service_name = "accesstoken"
-    default_authn_method = "client_secret_basic"
-    http_method = "POST"
-    request_body_type = "urlencoded"
-    response_body_type = "json"
-
-    def __init__(self, client_get, conf=None):
-        Service.__init__(self, client_get, conf=conf)
-
-    def update_service_context(self, resp, key="cc", **kwargs):
-        if "expires_in" in resp:
-            resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
-        self.client_get("service_context").state.store_item(resp, "token_response", key)
+    service_name = "check_session"
+
+    def __init__(self, upstream_get, conf=None):
+        Service.__init__(self, upstream_get, conf=conf)
+        self.pre_construct = [self.oidc_pre_construct]
+
+    def oidc_pre_construct(self, request_args=None, **kwargs):
+        _args = self.upstream_get("context").cstate.get_set(kwargs["state"],
+                                                            claim=["id_token"])
+        if request_args:
+            request_args.update(_args)
+        else:
+            request_args = _args
+
+        return request_args, {}
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/client_credentials/cc_refresh_access_token.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/refresh_access_token.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,51 @@
+"""The service that talks to the OAuth2 refresh access token endpoint."""
+import logging
+from typing import Optional
+
+from idpyoidc.client.oauth2.utils import get_state_parameter
 from idpyoidc.client.service import Service
 from idpyoidc.message import oauth2
 from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.time_util import time_sans_frac
 
+LOGGER = logging.getLogger(__name__)
+
+
+class RefreshAccessToken(Service):
+    """The service that talks to the OAuth2 refresh access token endpoint."""
 
-class CCRefreshAccessToken(Service):
     msg_type = oauth2.RefreshAccessTokenRequest
     response_cls = oauth2.AccessTokenResponse
     error_msg = ResponseMessage
     endpoint_name = "token_endpoint"
     synchronous = True
     service_name = "refresh_token"
     default_authn_method = "bearer_header"
     http_method = "POST"
 
-    def __init__(self, client_get, conf=None):
-        Service.__init__(self, client_get, conf=conf)
-        self.pre_construct.append(self.cc_pre_construct)
-        self.post_construct.append(self.cc_post_construct)
-
-    def cc_pre_construct(self, request_args=None, **kwargs):
-        _state_id = kwargs.get("state", "cc")
-        parameters = ["refresh_token"]
-        _state_interface = self.client_get("service_context").state
-        _args = _state_interface.extend_request_args(
-            {}, oauth2.AccessTokenResponse, "token_response", _state_id, parameters
-        )
-
-        _args = _state_interface.extend_request_args(
-            _args, oauth2.AccessTokenResponse, "refresh_token_response", _state_id, parameters
-        )
+    _include = {"grant_types_supported": ['refresh_token']}
+
+    def __init__(self, upstream_get, conf=None):
+        Service.__init__(self, upstream_get, conf=conf)
+        self.pre_construct.append(self.oauth_pre_construct)
+
+    def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
+        if "expires_in" in resp:
+            resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
+        self.upstream_get("context").cstate.update(key, resp)
+
+    def oauth_pre_construct(self, request_args=None, **kwargs):
+        """Preconstructor of request arguments"""
+        _state = get_state_parameter(request_args, kwargs)
+        parameters = list(self.msg_type.c_param.keys())
+
+        _current = self.upstream_get("context").cstate
+        _args = _current.get_set(_state, claim=parameters)
 
         if request_args is None:
             request_args = _args
         else:
             _args.update(request_args)
             request_args = _args
 
         return request_args, {}
-
-    def cc_post_construct(self, request_args, **kwargs):
-        for attr in ["client_id", "client_secret"]:
-            try:
-                del request_args[attr]
-            except KeyError:
-                pass
-
-        return request_args
-
-    def update_service_context(self, resp, key="cc", **kwargs):
-        if "expires_in" in resp:
-            resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
-        self.client_get("service_context").state.store_item(resp, "token_response", key)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/refresh_access_token.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/token_exchange.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,68 @@
-"""The service that talks to the OAuth2 refresh access token endpoint."""
+"""Implements the service that can exchange one token for another."""
 import logging
+from typing import Optional
 
 from idpyoidc.client.oauth2.utils import get_state_parameter
 from idpyoidc.client.service import Service
+from idpyoidc.exception import MissingParameter
+from idpyoidc.exception import MissingRequiredAttribute
 from idpyoidc.message import oauth2
 from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.time_util import time_sans_frac
 
 LOGGER = logging.getLogger(__name__)
 
 
-class RefreshAccessToken(Service):
-    """The service that talks to the OAuth2 refresh access token endpoint."""
+class TokenExchange(Service):
+    """The token exchange service."""
 
-    msg_type = oauth2.RefreshAccessTokenRequest
-    response_cls = oauth2.AccessTokenResponse
+    msg_type = oauth2.TokenExchangeRequest
+    response_cls = oauth2.TokenExchangeResponse
     error_msg = ResponseMessage
     endpoint_name = "token_endpoint"
     synchronous = True
-    service_name = "refresh_token"
-    default_authn_method = "bearer_header"
+    service_name = "token_exchange"
+    default_authn_method = "client_secret_basic"
     http_method = "POST"
+    request_body_type = "urlencoded"
+    response_body_type = "json"
 
-    def __init__(self, client_get, conf=None):
-        Service.__init__(self, client_get, conf=conf)
+    _include = {'grant_types_supported': ['urn:ietf:params:oauth:grant-type:token-exchange']}
+
+    def __init__(self, upstream_get, conf=None):
+        Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct.append(self.oauth_pre_construct)
 
-    def update_service_context(self, resp, key="", **kwargs):
+    def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
         if "expires_in" in resp:
             resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
-        self.client_get("service_context").state.store_item(resp, "token_response", key)
+        self.upstream_get("service_context").cstate.update(key, resp)
 
-    def oauth_pre_construct(self, request_args=None, **kwargs):
-        """Preconstructor of request arguments"""
-        _state = get_state_parameter(request_args, kwargs)
-        parameters = list(self.msg_type.c_param.keys())
-
-        _si = self.client_get("service_context").state
-        _args = _si.extend_request_args(
-            {}, oauth2.AccessTokenResponse, "token_response", _state, parameters
-        )
-
-        _args = _si.extend_request_args(
-            _args, oauth2.AccessTokenResponse, "refresh_token_response", _state, parameters
-        )
+    def oauth_pre_construct(self, request_args=None, post_args=None, **kwargs):
+        """
 
+        :param request_args: Initial set of request arguments
+        :param kwargs: Extra keyword arguments
+        :return: Request arguments
+        """
         if request_args is None:
-            request_args = _args
-        else:
-            _args.update(request_args)
-            request_args = _args
+            request_args = {}
+
+        if 'subject_token' not in request_args:
+            try:
+                _key = get_state_parameter(request_args, kwargs)
+            except MissingParameter:
+                raise MissingRequiredAttribute("subject_token")
+
+            parameters = {'access_token', 'scope'}
+
+            _current = self.upstream_get("service_context").cstate
+
+            _args = _current.get_set(_key, claim=parameters)
+
+            request_args["subject_token"] = _args["access_token"]
+            request_args["subject_token_type"] = 'urn:ietf:params:oauth:token-type:access_token'
+            if 'scope' not in request_args and "scope" in _args:
+                request_args["scope"] = _args["scope"]
 
-        return request_args, {}
+        return request_args, post_args
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/server_metadata.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/server_metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """The service that talks to the OAuth2 provider info discovery endpoint."""
 import logging
+from typing import Optional
 
 from cryptojwt.key_jar import KeyJar
 
 from idpyoidc.client.defaults import OIDCONF_PATTERN
 from idpyoidc.client.exception import OidcServiceError
 from idpyoidc.client.service import Service
+from idpyoidc.message import Message
 from idpyoidc.message import oauth2
 from idpyoidc.message.oauth2 import ResponseMessage
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ServerMetadata(Service):
-    """The service that talks to the OAuth2 server metadata endpoint."""
+    """The service that talks to the OAuth2 server claims endpoint."""
 
     msg_type = oauth2.Message
     response_cls = oauth2.ASConfigurationResponse
     error_msg = ResponseMessage
     synchronous = True
     service_name = "server_metadata"
     http_method = "GET"
 
-    metadata_attributes = {}
+    _supports = {}
 
-    def __init__(self, client_get, conf=None):
-        Service.__init__(self, client_get, conf=conf)
+    def __init__(self, upstream_get, conf=None):
+        Service.__init__(self, upstream_get, conf=conf)
 
     def get_endpoint(self):
         """
         Find the issuer ID and from it construct the service endpoint
 
         :return: Service endpoint
         """
         try:
-            _iss = self.client_get("service_context").issuer
+            _iss = self.upstream_get("context").issuer
         except AttributeError:
             _iss = self.endpoint
 
         if _iss.endswith("/"):
             return OIDCONF_PATTERN.format(_iss[:-1])
 
         return OIDCONF_PATTERN.format(_iss)
@@ -65,15 +67,15 @@
                 _issuer = issuer[:-1]
             else:
                 _issuer = issuer
 
         # In some cases we can live with the two URLs not being
         # the same. But this is an excepted that has to be explicit
         try:
-            self.client_get("service_context").allow["issuer_mismatch"]
+            self.upstream_get("context").allow["issuer_mismatch"]
         except KeyError:
             if _issuer != _pcr_issuer:
                 raise OidcServiceError(
                     "provider info issuer mismatch '%s' != '%s'" % (_issuer, _pcr_issuer)
                 )
         return _issuer
 
@@ -82,51 +84,58 @@
         If there are services defined set the service endpoint to be
         the URLs specified in the provider information."""
         for key, val in resp.items():
             # All service endpoint parameters in the provider info has
             # a name ending in '_endpoint' so I can look specifically
             # for those
             if key.endswith("_endpoint"):
-                _srv = self.client_get("service_by_endpoint_name", key)
+                _srv = self.upstream_get("service_by_endpoint_name", key)
                 if _srv:
                     _srv.endpoint = val
 
     def _update_service_context(self, resp):
         """
         Deal with Provider Config Response. Based on the provider info
         response a set of parameters in different places needs to be set.
 
         :param resp: The provider info response
         :param service_context: Information collected/used by services
         """
 
-        _context = self.client_get("service_context")
+        _context = self.upstream_get("context")
         # Verify that the issuer value received is the same as the
         # url that was used as service endpoint (without the .well-known part)
         if "issuer" in resp:
             _pcr_issuer = self._verify_issuer(resp, _context.issuer)
         else:  # No prior knowledge
             _pcr_issuer = _context.issuer
 
         _context.issuer = _pcr_issuer
         _context.provider_info = resp
 
         self._set_endpoints(resp)
 
         # If I already have a Key Jar then I'll add then provider keys to
-        # that. Otherwise a new Key Jar is minted
+        # that. Otherwise, a new Key Jar is minted
         try:
-            _keyjar = _context.keyjar
+            _keyjar = self.upstream_get('attribute', 'keyjar')
+            if _keyjar is None:
+                _keyjar = KeyJar()
         except KeyError:
             _keyjar = KeyJar()
 
         # Load the keys. Note that this only means that the key specification
         # is loaded not necessarily that any keys are fetched.
         if "jwks_uri" in resp:
             _keyjar.load_keys(_pcr_issuer, jwks_uri=resp["jwks_uri"])
         elif "jwks" in resp:
             _keyjar.load_keys(_pcr_issuer, jwks=resp["jwks"])
 
-        _context.keyjar = _keyjar
+        # Combine what I prefer/supports with what the Provider supports
+        if isinstance(resp, Message):
+            _info = resp.to_dict()
+        else:
+            _info = resp
+        _context.map_supported_to_preferred(_info)
 
-    def update_service_context(self, resp, **kwargs):
+    def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
         return self._update_service_context(resp)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oauth2/utils.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import List
 from typing import Optional
 from typing import Union
 
 from idpyoidc.client.service import Service
 from idpyoidc.exception import MissingParameter
 from idpyoidc.exception import MissingRequiredAttribute
 from idpyoidc.message import Message
@@ -22,61 +21,69 @@
             raise MissingParameter("state")
 
     return _state
 
 
 def pick_redirect_uri(
         context,
-        entity,
         request_args: Optional[Union[Message, dict]] = None,
         response_type: Optional[str] = "",
 ):
     if request_args is None:
         request_args = {}
 
     if "redirect_uri" in request_args:
         return request_args["redirect_uri"]
 
-    if context.specs.callback:
+    _callback_uris = context.get_preference("callback_uris")
+    if _callback_uris:
+        _callback_uris = _callback_uris.get("redirect_uris")
+
+    if _callback_uris:
         if not response_type:
-            _conf_resp_types = context.specs.behaviour.get("response_types", [])
+            _conf_resp_types = context.get_usage("response_types", [])
             response_type = request_args.get("response_type")
             if not response_type and _conf_resp_types:
                 response_type = _conf_resp_types[0]
 
         _response_mode = request_args.get("response_mode")
 
-        if _response_mode == "form_post" or response_type == ["form_post"]:
-            redirect_uri = context.specs.callback["form_post"]
-        elif response_type == "code" or response_type == ["code"]:
-            redirect_uri = context.specs.callback["code"]
+        if _response_mode:
+            if _response_mode == "form_post":
+                redirect_uri = _callback_uris["form_post"][0]
+            elif response_type == "code" or response_type == ["code"]:
+                redirect_uri = _callback_uris["code"][0]
+            else:
+                redirect_uri = _callback_uris["implicit"][0]
         else:
-            redirect_uri = context.specs.callback["implicit"]
+            if 'code' == response_type:
+                redirect_uri = _callback_uris["code"][0]
+            else:
+                redirect_uri = _callback_uris["implicit"][0]
 
         logger.debug(
             f"pick_redirect_uris: response_type={response_type}, response_mode={_response_mode}, "
             f"redirect_uri={redirect_uri}"
         )
     else:
-        redirect_uris = entity.get_metadata_value("redirect_uris", [])
+        redirect_uris = context.get_usage("redirect_uris", [])
         if redirect_uris:
             redirect_uri = redirect_uris[0]
         else:
             logger.error("No redirect_uri")
             raise MissingRequiredAttribute("redirect_uri")
 
     return redirect_uri
 
 
 def pre_construct_pick_redirect_uri(
         request_args: Optional[Union[Message, dict]] = None, service: Optional[Service] = None,
         **kwargs
 ):
-    request_args["redirect_uri"] = pick_redirect_uri(service.client_get("service_context"),
-                                                     entity=service.client_get("entity"),
+    request_args["redirect_uri"] = pick_redirect_uri(service.upstream_get("context"),
                                                      request_args=request_args)
     return request_args, {}
 
 
 def set_state_parameter(request_args=None, **kwargs):
     """Assigned a state value."""
     request_args["state"] = get_state_parameter(request_args, kwargs)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oidc/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import json
 import logging
+from typing import Callable
+from typing import Optional
+from typing import Union
+
+from cryptojwt.key_jar import KeyJar
 
 from idpyoidc.client import oauth2
 from idpyoidc.client.client_auth import BearerHeader
 from idpyoidc.client.defaults import DEFAULT_OIDC_SERVICES
 from idpyoidc.configure import Configuration
 
 try:
@@ -68,43 +73,55 @@
 
 
 class FetchException(Exception):
     pass
 
 
 class RP(oauth2.Client):
+    client_type = 'oidc'
+
     def __init__(
-        self,
-        keyjar=None,
-        verify_ssl=True,
-        config=None,
-        httplib=None,
-        services=None,
-        httpc_params=None,
+            self,
+            keyjar: Optional[KeyJar] = None,
+            config: Optional[Union[dict, Configuration]] = None,
+            services: Optional[dict] = None,
+            httpc: Optional[Callable] = None,
+            httpc_params: Optional[dict] = None,
+            upstream_get: Optional[Callable] = None,
+            key_conf: Optional[dict] = None,
+            entity_id: Optional[str] = '',
+            verify_ssl: Optional[bool] = True,
+            jwks_uri: Optional[str] = "",
+            **kwargs
     ):
-
-        if isinstance(config, Configuration):
-            _srvs = services or config.conf.get("services", DEFAULT_OIDC_SERVICES)
+        self.upstream_get = upstream_get
+        if services:
+            _srvs = services
         else:
-            _srvs = services or config.get("services", DEFAULT_OIDC_SERVICES)
+            _srvs = config.get("services", DEFAULT_OIDC_SERVICES)
 
         oauth2.Client.__init__(
             self,
             keyjar=keyjar,
-            verify_ssl=verify_ssl,
             config=config,
-            httplib=httplib,
             services=_srvs,
+            httpc=httpc,
             httpc_params=httpc_params,
-            client_type="oidc"
+            upstream_get=upstream_get,
+            key_conf=key_conf,
+            entity_id=entity_id,
+            verify_ssl=verify_ssl,
+            jwks_uri=jwks_uri,
+            client_type='oidc',
+            **kwargs
         )
 
         _context = self.get_service_context()
-        if _context.callback is None:
-            _context.callback = {}
+        if _context.get_preference('callback_uris') is None:
+            _context.set_preference('callback_uris', {})
 
     def fetch_distributed_claims(self, userinfo, callback=None):
         """
 
         :param userinfo: A :py:class:`idpyoidc.message.Message` sub class
             instance
         :param callback: A function that can be used to fetch things
@@ -116,28 +133,28 @@
             pass
         else:
             for csrc, spec in _csrc.items():
                 if "endpoint" in spec:
                     if "access_token" in spec:
                         cauth = BearerHeader()
                         httpc_params = cauth.construct(
-                            service=self.client_get("service", "userinfo"),
+                            service=self.get_service("userinfo"),
                             access_token=spec["access_token"],
                         )
-                        _resp = self.http.send(spec["endpoint"], "GET", **httpc_params)
+                        _resp = self.httpc("GET", spec["endpoint"], **httpc_params)
                     else:
                         if callback:
                             token = callback(spec["endpoint"])
                             cauth = BearerHeader()
                             httpc_params = cauth.construct(
-                                service=self.client_get("service", "userinfo"), access_token=token
+                                service=self.get_service("userinfo"), access_token=token
                             )
-                            _resp = self.http.send(spec["endpoint"], "GET", **httpc_params)
+                            _resp = self.httpc("GET", spec["endpoint"], **httpc_params)
                         else:
-                            _resp = self.http.send(spec["endpoint"], "GET")
+                            _resp = self.httpc("GET", spec["endpoint"])
 
                     if _resp.status_code == 200:
                         _uinfo = json.loads(_resp.text)
                     else:  # There shouldn't be any redirect
                         raise FetchException(
                             "HTTP error {}: {}".format(_resp.status_code, _resp.reason)
                         )
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/access_token.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,81 @@
 import logging
 from typing import Optional
 from typing import Union
 
-from idpyoidc.client.exception import ParameterError
-from idpyoidc.client.oauth2 import access_token
-from idpyoidc.client.oidc import IDT2REG
 from idpyoidc.message import Message
-from idpyoidc.message import oidc
-from idpyoidc.message.oidc import verified_claim_name
-from idpyoidc.time_util import time_sans_frac
+from idpyoidc.message.oauth2 import CCAccessTokenRequest
+from idpyoidc.time_util import utc_time_sans_frac
+from idpyoidc.util import sanitize
+from . import TokenEndpointHelper
 
-__author__ = "Roland Hedberg"
+logger = logging.getLogger(__name__)
 
-LOGGER = logging.getLogger(__name__)
 
+class ClientCredentials(TokenEndpointHelper):
 
-class AccessToken(access_token.AccessToken):
-    msg_type = oidc.AccessTokenRequest
-    response_cls = oidc.AccessTokenResponse
-    error_msg = oidc.ResponseMessage
+    def __init__(self, endpoint, config=None):
+        TokenEndpointHelper.__init__(self, endpoint, config)
 
-    def __init__(self, client_get, conf: Optional[dict] = None):
-        access_token.AccessToken.__init__(self, client_get, conf=conf)
+    def process_request(self, req: Union[Message, dict], **kwargs):
+        _context = self.endpoint.upstream_get("context")
+        _mngr = _context.session_manager
+        logger.debug("Client credentials flow")
 
-    def gather_verify_arguments(
-        self, response: Optional[Union[dict, Message]] = None, behaviour_args: Optional[dict] = None
-    ):
-        """
-        Need to add some information before running verify()
+        # verify the client and the user
 
-        :return: dictionary with arguments to the verify call
-        """
-        _context = self.client_get("service_context")
-        _entity = self.client_get("entity")
-
-        kwargs = {
-            "client_id": _entity.get_client_id(),
-            "iss": _context.issuer,
-            "keyjar": _context.keyjar,
-            "verify": True,
-            "skew": _context.clock_skew,
-        }
+        client_id = req['client_id']
+        _authenticated = req.get("authenticated", False)
+        if not _authenticated:
+            if _context.cdb[client_id] != req['client_secret']:
+                logger.warning("Client authentication failed")
+                return self.error_cls(error="invalid_request", error_description="Wrong client")
 
-        _reg_resp = _context.registration_response
-        if _reg_resp:
-            for attr, param in IDT2REG.items():
-                try:
-                    kwargs[attr] = _reg_resp[param]
-                except KeyError:
-                    pass
+        _grant_types_supported = _context.cdb[client_id].get('grant_types_supported')
+        if _grant_types_supported and 'client_credentials' not in _grant_types_supported:
+            return self.error_cls(error="invalid_request",
+                                  error_description="Unsupported grant type")
 
+        # Is there a previous session ?
         try:
-            kwargs["allow_missing_kid"] = _context.allow["missing_kid"]
+            _session_info = _mngr.get(['client_credentials', client_id])
+            _grant = _session_info["grant"]
         except KeyError:
-            pass
-
-        _verify_args = _context.specs.behaviour.get("verify_args")
-        if _verify_args:
-            if _verify_args:
-                kwargs.update(_verify_args)
-
-        return kwargs
-
-    def update_service_context(self, resp, key="", **kwargs):
-        _state_interface = self.client_get("service_context").state
-        try:
-            _idt = resp[verified_claim_name("id_token")]
-        except KeyError:
-            pass
-        else:
-            try:
-                if _state_interface.get_state_by_nonce(_idt["nonce"]) != key:
-                    raise ParameterError('Someone has messed with "nonce"')
-            except KeyError:
-                raise ValueError("Invalid nonce value")
-
-            _state_interface.store_sub2state(_idt["sub"], key)
+            logger.debug('No previous session')
+            branch_id = _mngr.add_grant(['client_credentials', client_id])
+            _session_info = _mngr.get_session_info(branch_id)
+
+        _grant = _session_info["grant"]
+
+        token_type = "Bearer"
+
+        _allowed = _context.cdb[client_id].get('allowed_scopes', [])
+        access_token = self._mint_token(
+            token_class="access_token",
+            grant=_grant,
+            session_id=_session_info["branch_id"],
+            client_id=_session_info["client_id"],
+            based_on=None,
+            scope=_allowed,
+            token_type=token_type,
+        )
+
+        _resp = {
+            "access_token": access_token.value,
+            "token_type": access_token.token_class,
+            "scope": _allowed,
+        }
 
-        if "expires_in" in resp:
-            resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
+        if access_token.expires_at:
+            _resp["expires_in"] = access_token.expires_at - utc_time_sans_frac()
 
-        _state_interface.store_item(resp, "token_response", key)
+        return _resp
 
-    def get_authn_method(self):
-        _specs = self.client_get("service_context").specs
-        try:
-            return _specs.behaviour["token_endpoint_auth_method"]
-        except KeyError:
-            return self.default_authn_method
+    def post_parse_request(
+            self,
+            request: Union[Message, dict],
+            client_id: Optional[str] = "",
+            **kwargs
+    ):
+        request = CCAccessTokenRequest(**request.to_dict())
+        logger.debug("%s: %s" % (request.__class__.__name__, sanitize(request)))
+        return request
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/authorization.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,320 +1,310 @@
 import logging
-from typing import Optional
-from typing import Union
 
-from idpyoidc.client.oauth2 import authorization
-from idpyoidc.client.oauth2.utils import pre_construct_pick_redirect_uri
-from idpyoidc.client.oidc import IDT2REG
-from idpyoidc.client.oidc.utils import construct_request_uri
-from idpyoidc.client.oidc.utils import request_object_encryption
+from cryptojwt import BadSyntax
+from cryptojwt.exception import JWKESTException
+
+from idpyoidc.exception import ImproperlyConfigured
 from idpyoidc.exception import MissingRequiredAttribute
-from idpyoidc.message import Message
-from idpyoidc.message import oauth2
-from idpyoidc.message import oidc
-from idpyoidc.message.oidc import make_openid_request
-from idpyoidc.message.oidc import verified_claim_name
-from idpyoidc.time_util import time_sans_frac
+from idpyoidc.exception import MissingRequiredValue
+from idpyoidc.message.oauth2 import TokenExchangeRequest
+from idpyoidc.message.oauth2 import TokenExchangeResponse
+from idpyoidc.message.oidc import TokenErrorResponse
+from idpyoidc.server.constant import DEFAULT_REQUESTED_TOKEN_TYPE
+from idpyoidc.server.exception import ToOld
+from idpyoidc.server.exception import UnAuthorizedClientScope
+from idpyoidc.server.oauth2.authorization import check_unknown_scopes_policy
+from idpyoidc.server.session.token import MintingNotAllowed
+from idpyoidc.server.session.token import TOKEN_TYPES_MAPPING
+from idpyoidc.server.token.exception import UnknownToken
 from idpyoidc.time_util import utc_time_sans_frac
-from idpyoidc.util import rndstr
-
-__author__ = "Roland Hedberg"
+from idpyoidc.util import importer
+from . import TokenEndpointHelper
+from . import validate_token_exchange_policy
 
-LOGGER = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
-class Authorization(authorization.Authorization):
-    msg_type = oidc.AuthorizationRequest
-    response_cls = oidc.AuthorizationResponse
-    error_msg = oidc.ResponseMessage
+class TokenExchangeHelper(TokenEndpointHelper):
+    """Implements Token Exchange a.k.a. RFC8693"""
 
-    usage_rules = {
+    token_types_mapping = {
+        "urn:ietf:params:oauth:token-type:access_token": "access_token",
+        "urn:ietf:params:oauth:token-type:refresh_token": "refresh_token",
     }
 
-    def __init__(self, client_get, conf=None):
-        authorization.Authorization.__init__(self, client_get, conf=conf)
-        self.default_request_args.update({"scope": ["openid"]})
-        self.pre_construct = [
-            self.set_state,
-            pre_construct_pick_redirect_uri,
-            self.oidc_pre_construct,
-        ]
-        self.post_construct = [self.oidc_post_construct]
+    def __init__(self, endpoint, config=None):
+        TokenEndpointHelper.__init__(self, endpoint=endpoint, config=config)
+        if config is None:
+            self.config = {
+                "requested_token_types_supported": [
+                    "urn:ietf:params:oauth:token-type:access_token",
+                    "urn:ietf:params:oauth:token-type:refresh_token",
+                ],
+                "default_requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
+                "policy": {"": {"function": validate_token_exchange_policy}},
+            }
+        else:
+            self.config = config
 
-    def set_state(self, request_args, **kwargs):
-        try:
-            _state = kwargs["state"]
-        except KeyError:
-            try:
-                _state = request_args["state"]
-            except KeyError:
-                _state = ""
-
-        _context = self.client_get("service_context")
-        request_args["state"] = _context.state.create_state(_context.issuer, _state)
-        return request_args, {}
-
-    def update_service_context(self, resp, key="", **kwargs):
-        _context = self.client_get("service_context")
-
-        if "expires_in" in resp:
-            resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
-        _context.state.store_item(resp.to_json(), "auth_response", key)
-
-    def get_request_from_response(self, response):
-        _context = self.client_get("service_context")
-        return _context.state.get_item(
-            oauth2.AuthorizationRequest, "auth_request", response["state"]
-        )
+    def post_parse_request(self, request, client_id="", **kwargs):
+        request = TokenExchangeRequest(**request.to_dict())
 
-    def post_parse_response(self, response, **kwargs):
-        response = authorization.Authorization.post_parse_response(self, response, **kwargs)
+        _context = self.endpoint.upstream_get("context")
+        if "token_exchange" in _context.cdb[request["client_id"]]:
+            config = _context.cdb[request["client_id"]]["token_exchange"]
+        else:
+            config = self.config
 
-        _idt = response.get(verified_claim_name("id_token"))
-        if _idt:
-            # If there is a verified ID Token then we have to do nonce
-            # verification.
-            _request = self.get_request_from_response(response)
-            _req_nonce = _request.get("nonce")
-            if _req_nonce:
-                _id_token_nonce = _idt.get("nonce")
-                if not _id_token_nonce:
-                    raise MissingRequiredAttribute("nonce")
-                elif _req_nonce != _id_token_nonce:
-                    raise ValueError("Invalid nonce")
-        return response
-
-    def oidc_pre_construct(self, request_args=None, post_args=None, **kwargs):
-        _context = self.client_get("service_context")
-        _entity = self.client_get("entity")
+        try:
+            request.verify(
+                keyjar=self.endpoint.upstream_get('attribute', 'keyjar'),
+                opponent_id=client_id
+            )
+        except (
+                MissingRequiredAttribute,
+                ValueError,
+                MissingRequiredValue,
+                JWKESTException,
+        ) as err:
+            return self.endpoint.error_cls(error="invalid_request", error_description="%s" % err)
 
-        if request_args is None:
-            request_args = {}
+        self._validate_configuration(config)
 
+        _mngr = _context.session_manager
         try:
-            _response_types = [request_args["response_type"]]
-        except KeyError:
-            _response_types = _context.specs.behaviour.get("response_types")
-            if _response_types:
-                request_args["response_type"] = _response_types[0]
-            else:
-                request_args["response_type"] = "code"
-
-        # For OIDC 'openid' is required in scope
-        if "scope" not in request_args:
-            _scope = self.client_get("entity").get_usage_value("scope")
-            if _scope:
-                request_args["scope"] = _scope
-            else:
-                request_args["scope"] = "openid"
-        elif "openid" not in request_args["scope"]:
-            request_args["scope"].append("openid")
-
-        # 'code' and/or 'id_token' in response_type means an ID Roken
-        # will eventually be returnedm, hence the need for a nonce
-        if "code" in _response_types or "id_token" in _response_types:
-            if "nonce" not in request_args:
-                request_args["nonce"] = rndstr(32)
+            # token exchange is about minting one token based on another
+            _handler_key = self.token_types_mapping[request["subject_token_type"]]
+            _session_info = _mngr.get_session_info_by_token(
+                request["subject_token"], grant=True, handler_key=_handler_key
+            )
+        except (KeyError, UnknownToken, BadSyntax) as err:
+            logger.error(f"Subject token invalid ({err}).")
+            return self.error_cls(
+                error="invalid_request", error_description="Subject token invalid"
+            )
+
+        # Find the token instance based on the token value
+        token = _mngr.find_token(_session_info["branch_id"], request["subject_token"])
+        if token.is_active() is False:
+            return self.error_cls(
+                error="invalid_request", error_description="Subject token inactive"
+            )
+
+        resp = self._enforce_policy(request, token, config)
+        if isinstance(resp, TokenErrorResponse):
+            return resp
+
+        scopes = resp.get("scope", [])
+        scopes = _context.scopes_handler.filter_scopes(scopes, client_id=resp["client_id"])
+
+        if not scopes:
+            logger.error("All requested scopes have been filtered out.")
+            return self.error_cls(
+                error="invalid_scope", error_description="Invalid requested scopes"
+            )
+
+        _requested_token_type = resp.get(
+            "requested_token_type", "urn:ietf:params:oauth:token-type:access_token"
+        )
+        _token_class = self.token_types_mapping[_requested_token_type]
+        if _token_class == "refresh_token" and "offline_access" not in scopes:
+            return TokenErrorResponse(
+                error="invalid_request",
+                error_description="Exchanging this subject token to refresh token forbidden",
+            )
+
+        return resp
+
+    def _enforce_policy(self, request, token, config):
+        _context = self.endpoint.upstream_get("context")
+        subject_token_types_supported = config.get(
+            "subject_token_types_supported", self.token_types_mapping.keys()
+        )
+        subject_token_type = request["subject_token_type"]
+        if subject_token_type not in subject_token_types_supported:
+            return TokenErrorResponse(
+                error="invalid_request",
+                error_description="Unsupported subject token type",
+            )
+        if self.token_types_mapping[subject_token_type] != token.token_class:
+            return TokenErrorResponse(
+                error="invalid_request",
+                error_description="Wrong token type",
+            )
+
+        if (
+                "requested_token_type" in request
+                and request["requested_token_type"] not in config["requested_token_types_supported"]
+        ):
+            return TokenErrorResponse(
+                error="invalid_request",
+                error_description="Unsupported requested token type",
+            )
 
-        if post_args is None:
-            post_args = {}
+        request_info = dict(scope=request.get("scope", token.scope))
+        try:
+            check_unknown_scopes_policy(request_info, request["client_id"], _context)
+        except UnAuthorizedClientScope:
+            return self.error_cls(
+                error="invalid_grant",
+                error_description="Unauthorized scope requested",
+            )
+
+        if subject_token_type not in config["policy"]:
+            subject_token_type = ""
+
+        policy = config["policy"][subject_token_type]
+        function = policy["function"]
+        kwargs = policy.get("kwargs", {})
 
-        for attr in ["request_object_signing_alg", "algorithm", "sig_kid"]:
+        if isinstance(function, str):
             try:
-                post_args[attr] = kwargs[attr]
-            except KeyError:
-                pass
-            else:
-                del kwargs[attr]
-
-        if "request_method" in kwargs:
-            if kwargs["request_method"] == "reference":
-                post_args["request_param"] = "request_uri"
-            else:
-                post_args["request_param"] = "request"
-            del kwargs["request_method"]
+                fn = importer(function)
+            except Exception:
+                raise ImproperlyConfigured(f"Error importing {function} policy function")
         else:
-            if _entity.get_usage_value("request_uri"):
-                post_args["request_param"] = "request_uri"
-            elif _entity.get_usage_value("request_parameter"):
-                post_args["request_param"] = "request"
-
-        return request_args, post_args
-
-    def get_request_object_signing_alg(self, **kwargs):
-        alg = ""
-        for arg in ["request_object_signing_alg", "algorithm"]:
-            try:  # Trumps everything
-                alg = kwargs[arg]
-            except KeyError:
-                pass
-            else:
-                break
+            fn = function
 
-        if not alg:
-            _context = self.client_get("service_context")
-            try:
-                alg = _context.specs.behaviour["request_object_signing_alg"]
-            except KeyError:  # Use default
-                alg = "RS256"
-        return alg
-
-    def store_request_on_file(self, req, **kwargs):
-        """
-        Stores the request parameter in a file.
-        :param req: The request
-        :param kwargs: Extra keyword arguments
-        :return: The URL the OP should use to access the file
-        """
-        _context = self.client_get("service_context")
         try:
-            _webname = _context.registration_response["request_uris"][0]
-            filename = _context.filename_from_webname(_webname)
-        except KeyError:
-            filename, _webname = construct_request_uri(**kwargs)
-
-        fid = open(filename, mode="w")
-        fid.write(req)
-        fid.close()
-        return _webname
-
-    def construct_request_parameter(
-            self, req, request_param, audience=None, expires_in=0, **kwargs
-    ):
-        """Construct a request parameter"""
-        alg = self.get_request_object_signing_alg(**kwargs)
-        kwargs["request_object_signing_alg"] = alg
-
-        _context = self.client_get("service_context")
-        if "keys" not in kwargs and alg and alg != "none":
-            kwargs["keys"] = _context.keyjar
-
-        if alg == "none":
-            kwargs["keys"] = []
-
-        _srv_cntx = _context
-
-        # This is the issuer of the JWT, that is me !
-        _issuer = kwargs.get("issuer")
-        if _issuer is None:
-            kwargs["issuer"] = _srv_cntx.get_client_id()
+            return fn(request, context=_context, subject_token=token, **kwargs)
+        except Exception as e:
+            logger.error(f"Error while executing the {fn} policy function: {e}")
+            return self.error_cls(error="server_error", error_description="Internal server error")
+
+    def token_exchange_response(self, token, issued_token_type):
+        response_args = {}
+        response_args["access_token"] = token.value
+        response_args["scope"] = token.scope
+        response_args["issued_token_type"] = issued_token_type
+
+        if token.expires_at:
+            response_args["expires_in"] = token.expires_at - utc_time_sans_frac()
+        if hasattr(token, "token_type"):
+            response_args["token_type"] = token.token_type
+        else:
+            response_args["token_type"] = "N_A"
 
-        if kwargs.get("recv") is None:
-            try:
-                kwargs["recv"] = _srv_cntx.provider_info["issuer"]
-            except KeyError:
-                kwargs["recv"] = _srv_cntx.issuer
+        return TokenExchangeResponse(**response_args)
 
+    def process_request(self, request, **kwargs):
+        _context = self.endpoint.upstream_get("context")
+        _mngr = _context.session_manager
         try:
-            del kwargs["service"]
-        except KeyError:
-            pass
-
-        if expires_in:
-            req["exp"] = utc_time_sans_frac() + int(expires_in)
-
-        _mor_args = {
-            k: kwargs[k]
-            for k in [
-                "keys",
-                "issuer",
-                "request_object_signing_alg",
-                "recv",
-                "with_jti",
-                "lifetime",
-            ]
-            if k in kwargs
-        }
-
-        _req = make_openid_request(req, **_mor_args)
-
-        # Should the request be encrypted
-        return request_object_encryption(_req, _context, **kwargs)
-
-    def oidc_post_construct(self, req, **kwargs):
-        """
-        Modify the request arguments.
-
-        :param req: The request
-        :param kwargs: Extra keyword arguments
-        :return: A possibly modified request.
-        """
-        _context = self.client_get("service_context")
-        if "openid" in req["scope"]:
-            _response_type = req["response_type"][0]
-            if "id_token" in _response_type or "code" in _response_type:
-                _context.state.store_nonce2state(req["nonce"], req["state"])
-
-        if "offline_access" in req["scope"]:
-            if "prompt" not in req:
-                req["prompt"] = "consent"
-
-        _context.state.store_item(req, "auth_request", req["state"])
-
-        # Overrides what's in the configuration
-        _request_param = kwargs.get("request_param")
-        if _request_param:
-            del kwargs["request_param"]
+            _handler_key = self.token_types_mapping[request["subject_token_type"]]
+            _session_info = _mngr.get_session_info_by_token(
+                request["subject_token"], grant=True, handler_key=_handler_key
+            )
+        except ToOld:
+            logger.error("Subject token has expired.")
+            return self.error_cls(
+                error="invalid_request", error_description="Subject token has expired"
+            )
+        except (KeyError, UnknownToken):
+            logger.error("Subject token invalid.")
+            return self.error_cls(
+                error="invalid_request", error_description="Subject token invalid"
+            )
+
+        grant = _session_info["grant"]
+        token = _mngr.find_token(_session_info["branch_id"], request["subject_token"])
+        _requested_token_type = request.get(
+            "requested_token_type", "urn:ietf:params:oauth:token-type:access_token"
+        )
+
+        _token_class = self.token_types_mapping[_requested_token_type]
+
+        sid = _session_info["branch_id"]
+
+        _token_type = "Bearer"
+        # Is DPOP supported
+        if "dpop_signing_alg_values_supported" in _context.provider_info:
+            if request.get("dpop_jkt"):
+                _token_type = "DPoP"
+        scopes = request.get("scope", [])
+
+        if request["client_id"] != _session_info["client_id"]:
+            _token_usage_rules = _context.authz.usage_rules(request["client_id"])
+
+            sid = _mngr.create_exchange_session(
+                exchange_request=request,
+                original_grant=grant,
+                original_session_id=sid,
+                user_id=_session_info["user_id"],
+                client_id=request["client_id"],
+                token_usage_rules=_token_usage_rules,
+                scopes=scopes,
+            )
+
+            try:
+                _session_info = _mngr.get_session_info(session_id=sid, grant=True)
+            except Exception:
+                logger.error("Error retrieving token exchange session information")
+                return self.error_cls(
+                    error="server_error", error_description="Internal server error"
+                )
+
+        resources = request.get("resource")
+        if resources and request.get("audience"):
+            resources = list(set(resources + request.get("audience")))
         else:
-            if _context.specs.get_usage("request_uri"):
-                _request_param = "request_uri"
-            elif _context.specs.get_usage("request_parameter"):
-                _request_param = "request"
-
-        _req = None  # just a flag
-        if _request_param == "request_uri":
-            kwargs["base_path"] = _context.get("base_url") + "/" + "requests"
-            kwargs["local_dir"] = _context.specs.get("requests_dir", "./requests")
-            _req = self.construct_request_parameter(req, _request_param, **kwargs)
-            req["request_uri"] = self.store_request_on_file(_req, **kwargs)
-        elif _request_param == "request":
-            _req = self.construct_request_parameter(req, _request_param)
-            req["request"] = _req
-
-        if _req:
-            _leave = ["request", "request_uri"]
-            _leave.extend(req.required_parameters())
-            _keys = [k for k in req.keys() if k not in _leave]
-            for k in _keys:
-                del req[k]
-
-        return req
-
-    def gather_verify_arguments(
-            self, response: Optional[Union[dict, Message]] = None,
-            behaviour_args: Optional[dict] = None
-    ):
-        """
-        Need to add some information before running verify()
-
-        :return: dictionary with arguments to the verify call
-        """
-        _context = self.client_get("service_context")
-        kwargs = {
-            "iss": _context.issuer,
-            "keyjar": _context.keyjar,
-            "verify": True,
-            "skew": _context.clock_skew,
-        }
-
-        _client_id = _context.get_client_id()
-        if _client_id:
-            kwargs["client_id"] = _client_id
-
-        _reg_res = _context.registration_response
-        if _reg_res:
-            for attr, param in IDT2REG.items():
-                try:
-                    kwargs[attr] = _reg_res[param]
-                except KeyError:
-                    pass
+            resources = request.get("audience")
+
+        _token_args = None
+        if resources:
+            _token_args = {"resources": resources}
 
         try:
-            kwargs["allow_missing_kid"] = _context.allow["missing_kid"]
-        except KeyError:
-            pass
-
-        _verify_args = _context.specs.behaviour.get("verify_args")
-        if _verify_args:
-            kwargs.update(_verify_args)
+            new_token = self._mint_token(
+                token_class=_token_class,
+                grant=_session_info["grant"],
+                session_id=sid,
+                client_id=request["client_id"],
+                based_on=token,
+                scope=scopes,
+                token_args=_token_args,
+                token_type=_token_type,
+            )
+            new_token.expires_at = token.expires_at
+        except MintingNotAllowed:
+            logger.error(f"Minting not allowed for {_token_class}")
+            return self.error_cls(
+                error="invalid_grant",
+                error_description="Token Exchange not allowed with that token",
+            )
+
+        return self.token_exchange_response(new_token, _requested_token_type)
+
+    def _validate_configuration(self, config):
+        if "requested_token_types_supported" not in config:
+            raise ImproperlyConfigured(
+                "Missing 'requested_token_types_supported' from Token Exchange configuration"
+            )
+        if "policy" not in config:
+            raise ImproperlyConfigured("Missing 'policy' from Token Exchange configuration")
+        if "" not in config["policy"]:
+            raise ImproperlyConfigured(
+                "Default Token Exchange policy configuration is not defined"
+            )
+        if "function" not in config["policy"][""]:
+            raise ImproperlyConfigured(
+                "Missing 'function' from default Token Exchange policy configuration"
+            )
+
+        _default_requested_token_type = config.get("default_requested_token_type",
+                                                   DEFAULT_REQUESTED_TOKEN_TYPE)
+        if _default_requested_token_type not in config["requested_token_types_supported"]:
+            raise ImproperlyConfigured(
+                f"Unsupported default requested_token_type {_default_requested_token_type}"
+            )
+
+    def get_handler_key(self, request, endpoint_context):
+        client_info = endpoint_context.cdb.get(request["client_id"], {})
+
+        default_requested_token_type = (
+                client_info.get("token_exchange", {}).get("default_requested_token_type", None)
+                or
+                self.config.get("default_requested_token_type", DEFAULT_REQUESTED_TOKEN_TYPE)
+        )
 
-        return kwargs
+        requested_token_type = request.get("requested_token_type", default_requested_token_type)
+        return TOKEN_TYPES_MAPPING[requested_token_type]
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/backchannel_authentication.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oidc/backchannel_authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     response_cls = AuthenticationResponse
     error_msg = ResponseMessage
     endpoint_name = "backchannel_authentication_endpoint"
     synchronous = True
     service_name = "backchannel_authentication"
     response_body_type = "json"
 
-    def __init__(self, client_get, conf=None, **kwargs):
-        Service.__init__(self, client_get=client_get, conf=conf, **kwargs)
+    def __init__(self, upstream_get, conf=None, **kwargs):
+        Service.__init__(self, upstream_get=upstream_get, conf=conf, **kwargs)
         self.default_request_args = {"scope": ["openid"]}
         self.pre_construct = []
         self.post_construct = []
 
 
 class ClientNotification(Service):
     """The service that talks to the Client Notification endpoint."""
@@ -33,16 +33,16 @@
     endpoint_name = "client_notification_endpoint"
     synchronous = True
     request_body_type = "json"
     service_name = "client_notification"
     response_body_type = ""
     http_method = "POST"
 
-    def __init__(self, client_get, conf=None, **kwargs):
-        Service.__init__(self, client_get=client_get, conf=conf, **kwargs)
+    def __init__(self, upstream_get, conf=None, **kwargs):
+        Service.__init__(self, upstream_get=upstream_get, conf=conf, **kwargs)
         self.pre_construct = []
         self.post_construct = []
 
 
 class ClientNotificationAuthn(ClientAuthnMethod):
     """The bearer header authentication method."""
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/check_id.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oidc/check_id.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from typing import Optional
 
 from idpyoidc.client.service import Service
 from idpyoidc.message.oauth2 import Message
 from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.message.oidc import session
 
 __author__ = "Roland Hedberg"
@@ -14,19 +15,22 @@
     msg_type = session.CheckIDRequest
     response_cls = Message
     error_msg = ResponseMessage
     endpoint_name = ""
     synchronous = True
     service_name = "check_id"
 
-    def __init__(self, client_get, conf=None):
-        Service.__init__(self, client_get, conf=conf)
+    def __init__(self, upstream_get, conf=None):
+        Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct = [self.oidc_pre_construct]
 
-    def oidc_pre_construct(self, request_args=None, **kwargs):
-        request_args = self.client_get("service_context").state.multiple_extend_request_args(
-            request_args,
+    def oidc_pre_construct(self, request_args: Optional[dict] = None, **kwargs):
+        _args = self.upstream_get("context").cstate.get_set(
             kwargs["state"],
-            ["id_token"],
-            ["auth_response", "token_response", "refresh_token_response"],
+            claim=["id_token"]
         )
+        if request_args:
+            request_args.update()
+        else:
+            request_args = _args
+
         return request_args, {}
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/check_session.py` & `idpyoidc-2.0.0/src/idpyoidc/client/provider/github.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-import logging
-
-from idpyoidc.client.service import Service
-from idpyoidc.message.oauth2 import Message
+from idpyoidc.client.client_auth import get_client_authn_methods
+from idpyoidc.client.oauth2 import access_token
+from idpyoidc.client.oidc import userinfo
+from idpyoidc.message import Message
+from idpyoidc.message import SINGLE_OPTIONAL_STRING
+from idpyoidc.message import SINGLE_REQUIRED_STRING
+from idpyoidc.message import oauth2
 from idpyoidc.message.oauth2 import ResponseMessage
-from idpyoidc.message.oidc import session
+from idpyoidc.claims import get_signing_algs
+
+
+class AccessTokenResponse(Message):
+    """
+    Access token response
+    """
+
+    c_param = {
+        "access_token": SINGLE_REQUIRED_STRING,
+        "token_type": SINGLE_REQUIRED_STRING,
+        "scope": SINGLE_OPTIONAL_STRING,
+    }
+
 
-__author__ = "Roland Hedberg"
+class AccessToken(access_token.AccessToken):
+    msg_type = oauth2.AccessTokenRequest
+    response_cls = AccessTokenResponse
+    error_msg = oauth2.TokenErrorResponse
+    response_body_type = "urlencoded"
 
-logger = logging.getLogger(__name__)
+    _supports = {
+        "token_endpoint_auth_methods_supported": get_client_authn_methods,
+        "token_endpoint_auth_signing_alg_values_supported": get_signing_algs
+    }
 
 
-class CheckSession(Service):
-    msg_type = session.CheckSessionRequest
+class UserInfo(userinfo.UserInfo):
     response_cls = Message
     error_msg = ResponseMessage
-    endpoint_name = ""
-    synchronous = True
-    service_name = "check_session"
-
-    def __init__(self, client_get, conf=None):
-        Service.__init__(self, client_get, conf=conf)
-        self.pre_construct = [self.oidc_pre_construct]
-
-    def oidc_pre_construct(self, request_args=None, **kwargs):
-        request_args = self.client_get("service_context").state.multiple_extend_request_args(
-            request_args,
-            kwargs["state"],
-            ["id_token"],
-            ["auth_response", "token_response", "refresh_token_response"],
-        )
-        return request_args, {}
+    default_authn_method = ""
+    http_method = "GET"
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/end_session.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oidc/end_session.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,93 +16,65 @@
     response_cls = Message
     error_msg = ResponseMessage
     endpoint_name = "end_session_endpoint"
     synchronous = True
     service_name = "end_session"
     response_body_type = "html"
 
-    metadata_attributes = {
+    _supports = {
         "post_logout_redirect_uris": None,
+        'frontchannel_logout_supported': None,
         "frontchannel_logout_uri": None,
         "frontchannel_logout_session_required": None,
+        'backchannel_logout_supported': None,
         "backchannel_logout_uri": None,
         "backchannel_logout_session_required": None
     }
 
-    usage_rules = {
-        "frontchannel_logout": None,
-        "backchannel_logout": None,
-        "post_logout_redirects": None
-    }
-
-    callback_path = {
+    _callback_path = {
         "frontchannel_logout_uri": "fc_logout",
         "backchannel_logout_uri": "bc_logout",
-        "post_logout_redirect_uris": "session_logout"
-    }
-
-    usage_to_uri_map = {
-        "frontchannel_logout": "frontchannel_logout_uri",
-        "backchannel_logout": "backchannel_logout_uri",
-        "post_logout_redirect": "post_logout_redirect_uris"
+        "post_logout_redirect_uris": ["session_logout"]
     }
 
-    callback_uris = [
-        "frontchannel_logout_uri",
-        "backchannel_logout_uri",
-        "post_logout_redirect_uris"
-    ]
-
-    def __init__(self, client_get, conf=None):
-        Service.__init__(self, client_get, conf=conf)
+    def __init__(self, upstream_get, conf=None):
+        Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct = [
             self.get_id_token_hint,
             self.add_post_logout_redirect_uri,
             self.add_state,
         ]
 
     def get_id_token_hint(self, request_args=None, **kwargs):
         """
         Add id_token_hint to request
 
         :param request_args:
         :param kwargs:
         :return:
         """
-        request_args = self.client_get("service_context").state.multiple_extend_request_args(
-            request_args,
-            kwargs["state"],
-            ["id_token"],
-            ["auth_response", "token_response", "refresh_token_response"],
-            orig=True,
-        )
-
-        try:
-            request_args["id_token_hint"] = request_args["id_token"]
-        except KeyError:
-            pass
-        else:
-            del request_args["id_token"]
+
+        _id_token = self.upstream_get("context").cstate.get_claim(kwargs["state"], claim='id_token')
+        if _id_token:
+            request_args["id_token_hint"] = _id_token
 
         return request_args, {}
 
     def add_post_logout_redirect_uri(self, request_args=None, **kwargs):
         if "post_logout_redirect_uri" not in request_args:
-            _uri = self.metadata.get("post_logout_redirect_uris", '')
+            _uri = self.upstream_get("context").get_usage("post_logout_redirect_uris")
             if _uri:
                 if isinstance(_uri, str):
                     request_args["post_logout_redirect_uri"] = _uri
                 else:  # assume list
                     request_args["post_logout_redirect_uri"] = _uri[0]
 
         return request_args, {}
 
     def add_state(self, request_args=None, **kwargs):
         if "state" not in request_args:
             request_args["state"] = rndstr(32)
 
         # As a side effect bind logout state to session state
-        self.client_get("service_context").state.store_logout_state2state(
-            request_args["state"], kwargs["state"]
-        )
+        self.upstream_get("context").cstate.bind_key(request_args["state"], kwargs["state"])
 
         return request_args, {}
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/provider_info_discovery.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/access_token.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,174 +1,206 @@
 import logging
+from typing import Optional
+from typing import Union
 
-from idpyoidc.client.exception import ConfigurationError
-from idpyoidc.client.oauth2 import server_metadata
-from idpyoidc.message import oidc
-from idpyoidc.message.oauth2 import ResponseMessage
+from cryptojwt.jwt import utc_time_sans_frac
+from cryptojwt.utils import importer
 
-__author__ = "Roland Hedberg"
+from idpyoidc.exception import ImproperlyConfigured
+from idpyoidc.message import Message
+from idpyoidc.message.oauth2 import TokenErrorResponse
+from idpyoidc.util import sanitize
+from . import TokenEndpointHelper
+from . import validate_resource_indicators_policy
+from ...session import MintingNotAllowed
+from ...session.token import AuthorizationCode
+from ...token import UnknownToken
 
 logger = logging.getLogger(__name__)
 
-PREFERENCE2PROVIDER = {
-    # "require_signed_request_object": "request_object_algs_supported",
-    "request_object_signing_alg": "request_object_signing_alg_values_supported",
-    "request_object_encryption_alg": "request_object_encryption_alg_values_supported",
-    "request_object_encryption_enc": "request_object_encryption_enc_values_supported",
-    "userinfo_signed_response_alg": "userinfo_signing_alg_values_supported",
-    "userinfo_encrypted_response_alg": "userinfo_encryption_alg_values_supported",
-    "userinfo_encrypted_response_enc": "userinfo_encryption_enc_values_supported",
-    "id_token_signed_response_alg": "id_token_signing_alg_values_supported",
-    "id_token_encrypted_response_alg": "id_token_encryption_alg_values_supported",
-    "id_token_encrypted_response_enc": "id_token_encryption_enc_values_supported",
-    "default_acr_values": "acr_values_supported",
-    "subject_type": "subject_types_supported",
-    "token_endpoint_auth_method": "token_endpoint_auth_methods_supported",
-    "token_endpoint_auth_signing_alg": "token_endpoint_auth_signing_alg_values_supported",
-    "response_types": "response_types_supported",
-    "grant_types": "grant_types_supported",
-    "scope": "scopes_supported",
-}
-
-PROVIDER2PREFERENCE = dict([(v, k) for k, v in PREFERENCE2PROVIDER.items()])
-
-PROVIDER_DEFAULT = {
-    "token_endpoint_auth_method": "client_secret_basic",
-    "id_token_signed_response_alg": "RS256",
-}
-
-
-def add_redirect_uris(request_args, service=None, **kwargs):
-    """
-    Add redirect_uris to the request arguments.
-
-    :param request_args: Incomming request arguments
-    :param service: A link to the service
-    :param kwargs: Possible extra keyword arguments
-    :return: A possibly augmented set of request arguments.
-    """
-    _context = service.client_get("service_context")
-    if "redirect_uris" not in request_args:
-        # Callbacks is a dictionary with callback type 'code', 'implicit',
-        # 'form_post' as keys.
-        _cbs = _context.callback
-        if _cbs:
-            # Filter out local additions.
-            _uris = [v for k, v in _cbs.items() if not k.startswith("__")]
-            request_args["redirect_uris"] = _uris
+
+class AccessTokenHelper(TokenEndpointHelper):
+
+    def process_request(self, req: Union[Message, dict], **kwargs):
+        """
+
+        :param req:
+        :param kwargs:
+        :return:
+        """
+        _context = self.endpoint.upstream_get("context")
+        _mngr = _context.session_manager
+        logger.debug("Access Token")
+
+        if req["grant_type"] != "authorization_code":
+            return self.error_cls(error="invalid_request", error_description="Unknown grant_type")
+
+        try:
+            _access_code = req["code"].replace(" ", "+")
+        except KeyError:  # Missing code parameter - absolutely fatal
+            return self.error_cls(error="invalid_request", error_description="Missing code")
+
+        _session_info = _mngr.get_session_info_by_token(
+            _access_code, grant=True, handler_key="authorization_code"
+        )
+        client_id = _session_info["client_id"]
+        if client_id != req["client_id"]:
+            logger.debug("{} owner of token".format(client_id))
+            logger.warning("Client using token it was not given")
+            return self.error_cls(error="invalid_grant", error_description="Wrong client")
+
+        _cinfo = self.endpoint.upstream_get("context").cdb.get(client_id)
+
+        if ("resource_indicators" in _cinfo
+                and "access_token" in _cinfo["resource_indicators"]):
+            resource_indicators_config = _cinfo["resource_indicators"]["access_token"]
         else:
-            request_args["redirect_uris"] = _context.metadata["redirect_uris"]
+            resource_indicators_config = self.endpoint.kwargs.get("resource_indicators", None)
 
-    return request_args, {}
+        if resource_indicators_config is not None:
+            if "policy" not in resource_indicators_config:
+                policy = {"policy": {"function": validate_resource_indicators_policy}}
+                resource_indicators_config.update(policy)
 
+            req = self._enforce_resource_indicators_policy(req, resource_indicators_config)
 
-class ProviderInfoDiscovery(server_metadata.ServerMetadata):
-    msg_type = oidc.Message
-    response_cls = oidc.ProviderConfigurationResponse
-    error_msg = ResponseMessage
-    service_name = "provider_info"
+            if isinstance(req, TokenErrorResponse):
+                return req
 
-    metadata_attributes = {}
+        # if "grant_types_supported" in _context.cdb[client_id]:
+        #     grant_types_supported = _context.cdb[client_id].get("grant_types_supported")
+        # else:
+        #     grant_types_supported = _context.provider_info["grant_types_supported"]
 
-    def __init__(self, client_get, conf=None):
-        server_metadata.ServerMetadata.__init__(self, client_get, conf=conf)
+        grant = _session_info["grant"]
 
-    def update_service_context(self, resp, **kwargs):
-        _context = self.client_get("service_context")
-        self._update_service_context(resp)
-        self.match_preferences(resp, _context.issuer)
-        if "pre_load_keys" in self.conf and self.conf["pre_load_keys"]:
-            _jwks = _context.keyjar.export_jwks_as_json(issuer=resp["issuer"])
-            logger.info("Preloaded keys for {}: {}".format(resp["issuer"], _jwks))
+        _based_on = grant.get_token(_access_code)
+        _supports_minting = _based_on.usage_rules.get("supports_minting", [])
 
-    def match_preferences(self, pcr=None, issuer=None):
-        """
-        Match the clients preferences against what the provider can do.
-        This is to prepare for later client registration and or what
-        functionality the client actually will use.
-        In the client configuration the client preferences are expressed.
-        These are then compared with the Provider Configuration information.
-        If the Provider has left some claims out, defaults specified in the
-        standard will be used.
+        _authn_req = grant.authorization_request
 
-        :param pcr: Provider configuration response if available
-        :param issuer: The issuer identifier
-        """
-        _context = self.client_get("service_context")
-        _entity = self.client_get("entity")
+        # If redirect_uri was in the initial authorization request
+        # verify that the one given here is the correct one.
+        if "redirect_uri" in _authn_req:
+            if req["redirect_uri"] != _authn_req["redirect_uri"]:
+                return self.error_cls(
+                    error="invalid_request", error_description="redirect_uri mismatch"
+                )
 
-        if not pcr:
-            pcr = _context.provider_info
+        logger.debug("All checks OK")
 
-        regreq = oidc.RegistrationRequest
+        issue_refresh = kwargs.get("issue_refresh", False)
 
-        _behaviour = _context.specs.behaviour
+        if resource_indicators_config is not None:
+            scope = req["scope"]
+        else:
+            scope = grant.scope
 
-        for _pref, _prov in PREFERENCE2PROVIDER.items():
-            if _pref in ["scope"]:
-                vals = _entity.get_usage_value(_pref)
+        _response = {
+            "token_type": "Bearer",
+            "scope": scope,
+        }
+
+        if "access_token" in _supports_minting:
+
+            resources = req.get("resource", None)
+            if resources:
+                token_args = {"resources": resources}
             else:
-                try:
-                    vals = _entity.get_metadata_value(_pref)
-                except KeyError:
-                    continue
-
-            if not vals:
-                continue
+                token_args = None
 
             try:
-                _pvals = pcr[_prov]
-            except KeyError:
-                try:
-                    # If the provider have not specified use what the
-                    # standard says is mandatory if at all.
-                    _pvals = PROVIDER_DEFAULT[_pref]
-                except KeyError:
-                    logger.info("No info from provider on {} and no default".format(_pref))
-                    _pvals = vals
-
-            if isinstance(vals, str):
-                if vals in _pvals:
-                    _behaviour[_pref] = vals
+                token = self._mint_token(
+                    token_class="access_token",
+                    grant=grant,
+                    session_id=_session_info["branch_id"],
+                    client_id=_session_info["client_id"],
+                    based_on=_based_on,
+                    token_args=token_args
+                )
+            except MintingNotAllowed as err:
+                logger.warning(err)
             else:
-                try:
-                    vtyp = regreq.c_param[_pref]
-                except KeyError:
-                    # Allow non standard claims
-                    if isinstance(vals, list):
-                        _behaviour[_pref] = [v for v in vals if v in _pvals]
-                    elif vals in _pvals:
-                        _behaviour[_pref] = vals
-                else:
-                    if isinstance(vtyp[0], list):
-                        _behaviour[_pref] = []
-                        for val in vals:
-                            if val in _pvals:
-                                _behaviour[_pref].append(val)
-                    else:
-                        for val in vals:
-                            if val in _pvals:
-                                _behaviour[_pref] = val
-                                break
-
-            if _pref not in _behaviour:
-                raise ConfigurationError("OP couldn't match preference:%s" % _pref, pcr)
-
-        for key, val in _entity.collect_metadata().items():
-            if key in _behaviour:
-                continue
-            if key in ["jwks", "jwks_uri"]:
-                continue
+                _response["access_token"] = token.value
+                if token.expires_at:
+                    _response["expires_in"] = token.expires_at - utc_time_sans_frac()
+
+        if (
+                issue_refresh
+                and "refresh_token" in _supports_minting
+        ):
+            try:
+                refresh_token = self._mint_token(
+                    token_class="refresh_token",
+                    grant=grant,
+                    session_id=_session_info["branch_id"],
+                    client_id=_session_info["client_id"],
+                    based_on=_based_on,
+                )
+            except MintingNotAllowed as err:
+                logger.warning(err)
+            else:
+                _response["refresh_token"] = refresh_token.value
+
+        # since the grant content has changed. Make sure it's stored
+        _mngr[_session_info["branch_id"]] = grant
 
+        _based_on.register_usage()
+
+        return _response
+
+    def _enforce_resource_indicators_policy(self, request, config):
+        _context = self.endpoint.upstream_get('context')
+
+        policy = config["policy"]
+        function = policy["function"]
+        kwargs = policy.get("kwargs", {})
+
+        if isinstance(function, str):
             try:
-                vtyp = regreq.c_param[key]
-                if isinstance(vtyp[0], list):
-                    pass
-                elif isinstance(val, list) and not isinstance(val, str):
-                    val = val[0]
-            except KeyError:
-                pass
-            if key not in PREFERENCE2PROVIDER:
-                _behaviour[key] = val
+                fn = importer(function)
+            except Exception:
+                raise ImproperlyConfigured(f"Error importing {function} policy function")
+        else:
+            fn = function
+        try:
+            return fn(request, context=_context, **kwargs)
+        except Exception as e:
+            logger.error(f"Error while executing the {fn} policy function: {e}")
+            return self.error_cls(error="server_error", error_description="Internal server error")
+
+    def post_parse_request(
+            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+    ):
+        """
+        This is where clients come to get their access tokens
+
+        :param request: The request
+        :param client_id: Client identifier
+        :returns:
+        """
+
+        _mngr = self.endpoint.upstream_get("context").session_manager
+        try:
+            _session_info = _mngr.get_session_info_by_token(
+                request["code"], grant=True, handler_key="authorization_code"
+            )
+        except (KeyError, UnknownToken):
+            logger.error("Access Code invalid")
+            return self.error_cls(error="invalid_grant", error_description="Unknown code")
+
+        grant = _session_info["grant"]
+        code = grant.get_token(request["code"])
+        if not isinstance(code, AuthorizationCode):
+            return self.error_cls(error="invalid_request", error_description="Wrong token type")
+
+        if code.is_active() is False:
+            return self.error_cls(error="invalid_request", error_description="Code inactive")
+
+        _auth_req = grant.authorization_request
+
+        if "client_id" not in request:  # Optional for access token request
+            request["client_id"] = _auth_req["client_id"]
+
+        logger.debug("%s: %s" % (request.__class__.__name__, sanitize(request)))
 
-        _context.specs.behaviour = _behaviour
-        logger.debug("service_context behaviour: {}".format(_behaviour))
+        return request
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/read_registration.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oidc/read_registration.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     synchronous = True
     service_name = "registration_read"
     http_method = "GET"
     default_authn_method = "client_secret_basic"
 
     def get_endpoint(self):
         try:
-            return self.client_get("service_context").registration_response[
+            return self.upstream_get("context").registration_response[
                 "registration_client_uri"
             ]
         except KeyError:
             return ""
 
     def get_authn_header(self, request, authn_method, **kwargs):
         """
@@ -36,13 +36,13 @@
         :return: A set of keyword arguments to be sent in the HTTP header.
         """
         headers = {}
 
         if authn_method == "client_secret_basic":
             LOGGER.debug("Client authn method: %s", authn_method)
             headers["Authorization"] = "Bearer {}".format(
-                self.client_get("service_context").registration_response[
+                self.upstream_get("context").registration_response[
                     "registration_access_token"
                 ]
             )
 
         return headers
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/utils.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oidc/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,61 +3,62 @@
 from cryptojwt.jwe.jwe import JWE
 from cryptojwt.jwe.utils import alg2keytype
 
 from idpyoidc.exception import MissingRequiredAttribute
 from idpyoidc.util import rndstr
 
 
-def request_object_encryption(msg, service_context, **kwargs):
+def request_object_encryption(msg, service_context, keyjar, **kwargs):
     """
     Created an encrypted JSON Web token with *msg* as body.
 
     :param msg: The mesaqg
     :param service_context:
     :param kwargs:
     :return:
     """
     try:
         encalg = kwargs["request_object_encryption_alg"]
     except KeyError:
         try:
-            encalg = service_context.specs.behaviour["request_object_encryption_alg"]
+            encalg = service_context.get_usage("request_object_encryption_alg")
         except KeyError:
             return msg
 
     if not encalg:
         return msg
 
     try:
         encenc = kwargs["request_object_encryption_enc"]
     except KeyError:
         try:
-            encenc = service_context.specs.behaviour["request_object_encryption_enc"]
+            encenc = service_context.get_usage("request_object_encryption_enc")
         except KeyError:
             raise MissingRequiredAttribute("No request_object_encryption_enc specified")
 
     if not encenc:
         raise MissingRequiredAttribute("No request_object_encryption_enc specified")
 
     _jwe = JWE(msg, alg=encalg, enc=encenc)
     _kty = alg2keytype(encalg)
 
     try:
         _kid = kwargs["enc_kid"]
     except KeyError:
         _kid = ""
 
-    if "target" not in kwargs:
+    _target = kwargs.get('target', kwargs.get('recv', None))
+    if _target is None:
         raise MissingRequiredAttribute("No target specified")
 
     if _kid:
-        _keys = service_context.keyjar.get_encrypt_key(_kty, issuer_id=kwargs["target"], kid=_kid)
+        _keys = keyjar.get_encrypt_key(_kty, issuer_id=_target, kid=_kid)
         _jwe["kid"] = _kid
     else:
-        _keys = service_context.keyjar.get_encrypt_key(_kty, issuer_id=kwargs["target"])
+        _keys = keyjar.get_encrypt_key(_kty, issuer_id=_target)
 
     return _jwe.encrypt(_keys)
 
 
 def construct_request_uri(local_dir, base_path, **kwargs):
     """
     Constructs a special redirect_uri to be used when communicating with
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/oidc/webfinger.py` & `idpyoidc-2.0.0/src/idpyoidc/client/oidc/webfinger.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,37 +31,35 @@
     response_cls = JRD
     error_msg = ResponseMessage
     synchronous = True
     service_name = "webfinger"
     http_method = "GET"
     response_body_type = "json"
 
-    def __init__(self, client_get, conf=None, rel="", **kwargs):
-        Service.__init__(self, client_get, conf=conf, **kwargs)
+    def __init__(self, upstream_get, conf=None, rel="", **kwargs):
+        Service.__init__(self, upstream_get, conf=conf, **kwargs)
 
         self.rel = rel or OIC_ISSUER
 
     def update_service_context(self, resp, key="", **kwargs):
         try:
             links = resp["links"]
         except KeyError:
             raise MissingRequiredAttribute("links")
         else:
             for link in links:
                 if link["rel"] == self.rel:
                     _href = link["href"]
-                    try:
-                        _http_allowed = self.get_conf_attr("allow", default={})["http_links"]
-                    except KeyError:
-                        _http_allowed = False
+                    _context = self.upstream_get('service_context')
+                    _http_allowed = 'http_links' in _context.get("allow", default={})
 
                     if _href.startswith("http://") and not _http_allowed:
                         raise ValueError("http link not allowed ({})".format(_href))
 
-                    self.client_get("service_context").issuer = link["href"]
+                    self.upstream_get("context").issuer = link["href"]
                     break
         return resp
 
     @staticmethod
     def create_url(part, ignore):
         res = []
         for a in range(0, 5):
@@ -148,12 +146,12 @@
         try:
             _resource = request_args["resource"]
         except KeyError:
             try:
                 _resource = kwargs["resource"]
             except KeyError:
                 try:
-                    _resource = self.client_get("service_context").config["resource"]
+                    _resource = self.upstream_get("context").config["resource"]
                 except KeyError:
                     raise MissingRequiredAttribute("resource")
 
         return {"url": self.query(_resource), "method": "GET"}
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/rp_handler.py` & `idpyoidc-2.0.0/src/idpyoidc/client/rp_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 import logging
 import sys
 import traceback
 from typing import Optional
 
 from cryptojwt import as_unicode
+from cryptojwt import KeyJar
 from cryptojwt.key_bundle import keybundle_from_local_file
 from cryptojwt.key_jar import init_key_jar
 from cryptojwt.utils import as_bytes
 
 from idpyoidc import verified_claim_name
 from idpyoidc.client.defaults import DEFAULT_CLIENT_CONFIGS
 from idpyoidc.client.defaults import DEFAULT_OIDC_SERVICES
 from idpyoidc.client.defaults import DEFAULT_RP_KEY_DEFS
 from idpyoidc.client.exception import ConfigurationError
 from idpyoidc.client.exception import OidcServiceError
 from idpyoidc.exception import MessageException
 from idpyoidc.exception import MissingRequiredAttribute
 from idpyoidc.exception import NotForMe
-from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.message.oauth2 import is_error_message
-from idpyoidc.message.oidc import AccessTokenResponse
 from idpyoidc.message.oidc import AuthorizationRequest
 from idpyoidc.message.oidc import AuthorizationResponse
 from idpyoidc.message.oidc import Claims
 from idpyoidc.message.oidc import OpenIDSchema
 from idpyoidc.message.oidc import RegistrationRequest
 from idpyoidc.message.oidc.session import BackChannelLogoutRequest
 from idpyoidc.time_util import utc_time_sans_frac
 from idpyoidc.util import add_path
 from idpyoidc.util import rndstr
-
 from . import oidc
 from .oauth2 import Client
 from .oauth2 import dynamic_provider_info_discovery
 from .oauth2.utils import pick_redirect_uri
+from ..message.oauth2 import ResponseMessage
 
 logger = logging.getLogger(__name__)
 
 
 class RPHandler(object):
+
     def __init__(
-        self,
-        base_url: Optional[str] = "",
-        client_configs=None,
-        services=None,
-        keyjar=None,
-        hash_seed="",
-        verify_ssl=True,
-        client_cls=None,
-        state_db=None,
-        http_lib=None,
-        httpc_params=None,
-        config=None,
-        **kwargs,
+            self,
+            base_url: Optional[str] = "",
+            client_configs=None,
+            services=None,
+            keyjar=None,
+            hash_seed="",
+            verify_ssl=True,
+            client_cls=None,
+            state_db=None,
+            httpc=None,
+            httpc_params=None,
+            config=None,
+            **kwargs,
     ):
         self.base_url = base_url
         _jwks_path = kwargs.get("jwks_path")
 
         if config:
             if not hash_seed:
                 self.hash_seed = config.hash_seed
@@ -104,15 +104,15 @@
             self.services = DEFAULT_OIDC_SERVICES
         else:
             self.services = services
 
         # keep track on which RP instance that serves which OP
         self.issuer2rp = {}
         self.hash2issuer = {}
-        self.httplib = http_lib
+        self.httpc = httpc
 
         if not httpc_params:
             self.httpc_params = {"verify": verify_ssl}
         else:
             self.httpc_params = httpc_params
 
         if not self.keyjar.httpc_params:
@@ -124,21 +124,18 @@
         was used against.
         Will raise a KeyError if the state is unknown.
 
         :param state: The state value
         :return: An Issuer ID
         """
         for _rp in self.issuer2rp.values():
-            try:
-                _iss = _rp.client_get("service_context").state.get_iss(state)
-            except KeyError:
-                continue
-            else:
-                if _iss:
-                    return _iss
+            _iss = _rp.get_context().cstate.get_set(
+                state, claim=['iss']).get('iss')
+            if _iss:
+                return _iss
         return None
 
     def pick_config(self, issuer):
         """
         From the set of client configurations pick one based on the issuer ID.
         Will raise a KeyError if issuer is unknown.
 
@@ -147,23 +144,23 @@
         """
         return self.client_configs[issuer]
 
     def get_session_information(self, key, client=None):
         """
         This is the second of the methods users of this class should know about.
         It will return the complete session information as an
-        :py:class:`idpyoidc.client.state_interface.State` instance.
+        :py:class:`idpyoidc.client.current.Current` instance.
 
         :param key: The session key (state)
         :return: A State instance
         """
         if not client:
             client = self.get_client_from_session_key(key)
 
-        return client.client_get("service_context").state.get_state(key)
+        return client.get_context().cstate.get(key)
 
     def init_client(self, issuer):
         """
         Initiate a Client instance. Specifically which Client class is used
         is decided by configuration.
 
         :param issuer: An issuer ID
@@ -179,43 +176,57 @@
             _cnf["issuer"] = issuer
 
         try:
             _services = _cnf["services"]
         except KeyError:
             _services = self.services
 
+        if 'base_url' not in _cnf:
+            _cnf['base_url'] = self.base_url
+
+        if self.jwks_uri:
+            _cnf['jwks_uri'] = self.jwks_uri
+
         try:
             client = self.client_cls(
                 services=_services,
                 config=_cnf,
-                httplib=self.httplib,
+                httpc=self.httpc,
                 httpc_params=self.httpc_params,
             )
         except Exception as err:
             logger.error("Failed initiating client: {}".format(err))
             message = traceback.format_exception(*sys.exc_info())
             logger.error(message)
             raise
 
-        _context = client.client_get("service_context")
+        _context = client.get_context()
         if _context.iss_hash:
             self.hash2issuer[_context.iss_hash] = issuer
         # If non persistent
-        _context.keyjar.load(self.keyjar.dump())
+        _keyjar = client.keyjar
+        if not _keyjar:
+            _keyjar = KeyJar()
+            _keyjar.httpc_params.update(self.httpc_params)
+
+        for iss in self.keyjar.owners():
+            _keyjar.import_jwks(self.keyjar.export_jwks(issuer_id=iss, private=True), iss)
+
+        client.keyjar = _keyjar
         # If persistent nothing has to be copied
 
         _context.base_url = self.base_url
         _context.jwks_uri = self.jwks_uri
         return client
 
     def do_provider_info(
-        self,
-        client: Optional[Client] = None,
-        state: Optional[str] = "",
-        behaviour_args: Optional[dict] = None,
+            self,
+            client: Optional[Client] = None,
+            state: Optional[str] = "",
+            behaviour_args: Optional[dict] = None,
     ) -> str:
         """
         Either get the provider info from configuration or through dynamic
         discovery.
 
         :param behaviour_args:
         :param client: A Client instance
@@ -227,59 +238,62 @@
 
         if not client:
             if state:
                 client = self.get_client_from_session_key(state)
             else:
                 raise ValueError("Missing state/session key")
 
-        _context = client.client_get("service_context")
+        _context = client.get_context()
         if not _context.get("provider_info"):
             dynamic_provider_info_discovery(client, behaviour_args=behaviour_args)
             return _context.get("provider_info")["issuer"]
         else:
             _pi = _context.get("provider_info")
             for key, val in _pi.items():
                 # All service endpoint parameters in the provider info has
                 # a name ending in '_endpoint' so I can look specifically
                 # for those
                 if key.endswith("_endpoint"):
-                    for _srv in client.client_get("services").values():
+                    for _srv in client.get_services().values():
                         # Every service has an endpoint_name assigned
                         # when initiated. This name *MUST* match the
                         # endpoint names used in the provider info
                         if _srv.endpoint_name == key:
                             _srv.endpoint = val
 
             if "keys" in _pi:
-                _kj = _context.keyjar
+                _kj = client.get_attribute('keyjar')
                 for typ, _spec in _pi["keys"].items():
                     if typ == "url":
                         for _iss, _url in _spec.items():
                             _kj.add_url(_iss, _url)
                     elif typ == "file":
                         for kty, _name in _spec.items():
                             if kty == "jwks":
                                 _kj.import_jwks_from_file(_name, _context.get("issuer"))
                             elif kty == "rsa":  # PEM file
                                 _kb = keybundle_from_local_file(_name, "der", ["sig"])
                                 _kj.add_kb(_context.get("issuer"), _kb)
                     else:
                         raise ValueError("Unknown provider JWKS type: {}".format(typ))
+
+            _context.map_supported_to_preferred(info=_pi)
+
             try:
                 return _context.get("provider_info")["issuer"]
             except KeyError:
                 return _context.get("issuer")
 
     def do_client_registration(
-        self,
-        client=None,
-        iss_id: Optional[str] = "",
-        state: Optional[str] = "",
-        request_args: Optional[dict] = None,
-        behaviour_args: Optional[dict] = None,
+            self,
+            client=None,
+            iss_id: Optional[str] = "",
+            state: Optional[str] = "",
+            request_args: Optional[dict] = None,
+            behaviour_args: Optional[dict] = None,
     ):
         """
         Prepare for and do client registration if configured to do so
 
         :param iss_id: Issuer ID
         :param behaviour_args: To fine tune behaviour
         :param client: A Client instance
@@ -291,15 +305,15 @@
 
         if not client:
             if state:
                 client = self.get_client_from_session_key(state)
             else:
                 raise ValueError("Missing state/session key")
 
-        _context = client.client_get("service_context")
+        _context = client.get_context()
         _iss = _context.get("issuer")
         self.hash2issuer[iss_id] = _iss
 
         # This should only be interesting if the client supports Single Log Out
         # if _context.callback.get("post_logout_redirect_uri") is None:
         #     _context.callback["post_logout_redirect_uri"] = [self.base_url]
 
@@ -308,14 +322,16 @@
                 request_args = {}
 
             if behaviour_args:
                 _params = RegistrationRequest().parameters()
                 request_args.update({k: v for k, v in behaviour_args.items() if k in _params})
 
             load_registration_response(client, request_args=request_args)
+        else:
+            _context.map_preferred_to_registered()
 
     def do_webfinger(self, user: str) -> Client:
         """
         Does OpenID Provider Issuer discovery using webfinger.
 
         :param user: Identifier for the target End-User that is the subject of the discovery
             request.
@@ -325,18 +341,18 @@
         logger.debug(20 * "*" + " do_webfinger " + 20 * "*")
 
         temporary_client = self.init_client("")
         temporary_client.do_request("webfinger", resource=user)
         return temporary_client
 
     def client_setup(
-        self,
-        iss_id: Optional[str] = "",
-        user: Optional[str] = "",
-        behaviour_args: Optional[dict] = None,
+            self,
+            iss_id: Optional[str] = "",
+            user: Optional[str] = "",
+            behaviour_args: Optional[dict] = None,
     ) -> Client:
         """
         First if no issuer ID is given then the identifier for the user is
         used by the webfinger service to try to find the issuer ID.
         Once the method has an issuer ID if no client is bound to this issuer
         one is created and initiated with
         the necessary information for the client to be able to communicate
@@ -379,24 +395,25 @@
         self.do_client_registration(client, iss_id, behaviour_args=behaviour_args)
 
         self.issuer2rp[issuer] = client
         return client
 
     def _get_response_type(self, context, req_args: Optional[dict] = None):
         if req_args:
-            return req_args.get("response_type", context.specs.behaviour["response_types"][0])
+            return req_args.get("response_type",
+                                context.claims.get_usage("response_types")[0])
         else:
-            return context.specs.behaviour["response_types"][0]
+            return context.claims.get_usage("response_types")[0]
 
     def init_authorization(
-        self,
-        client: Optional[Client] = None,
-        state: Optional[str] = "",
-        req_args: Optional[dict] = None,
-        behaviour_args: Optional[dict] = None,
+            self,
+            client: Optional[Client] = None,
+            state: Optional[str] = "",
+            req_args: Optional[dict] = None,
+            behaviour_args: Optional[dict] = None,
     ) -> dict:
         """
         Constructs the URL that will redirect the user to the authorization
         endpoint of the OP/AS.
 
         :param behaviour_args:
         :param state:
@@ -410,40 +427,45 @@
         logger.debug(20 * "*" + " init_authorization " + 20 * "*")
         if not client:
             if state:
                 client = self.get_client_from_session_key(state)
             else:
                 raise ValueError("Missing state/session key")
 
-        _context = client.client_get("service_context")
-        _entity = client.client_get("entity")
+        _context = client.get_context()
+        # _entity = client.upstream_get("entity")
         _nonce = rndstr(24)
         _response_type = self._get_response_type(_context, req_args)
         request_args = {
             "redirect_uri": pick_redirect_uri(
-                _context, _entity, request_args=req_args, response_type=_response_type
+                _context, request_args=req_args, response_type=_response_type
             ),
-            "scope": _context.specs.behaviour["scope"],
             "response_type": _response_type,
             "nonce": _nonce,
         }
 
+        _scope = _context.claims.get_usage("scope")
+        if _scope:
+            request_args['scope'] = _scope
+
         _req_args = _context.config.get("request_args")
         if _req_args:
             if "claims" in _req_args:
                 _req_args["claims"] = Claims(**_req_args["claims"])
             request_args.update(_req_args)
 
         if req_args is not None:
             request_args.update(req_args)
 
         # Need a new state for a new authorization request
-        _state = _context.state.create_state(_context.get("issuer"))
+        _current = _context.cstate
+        _state = _current.create_key()
         request_args["state"] = _state
-        _context.state.store_nonce2state(_nonce, _state)
+        _current.bind_key(_nonce, _state)
+        _current.set(_state, {'iss': _context.get("issuer")})
 
         logger.debug("Authorization request args: {}".format(request_args))
 
         # if behaviour_args and "request_param" not in behaviour_args:
         #     _pi = _context.get("provider_info")
 
         _srv = client.get_service("authorization")
@@ -492,32 +514,29 @@
     def get_response_type(client):
         """
         Return the response_type a specific client wants to use.
 
         :param client: A Client instance
         :return: The response_type
         """
-        return client.service_context.get("behaviour")["response_types"][0]
+        return client.service_context.claims.get_usage("response_types")[0]
 
     @staticmethod
     def get_client_authn_method(client, endpoint):
         """
         Return the client authentication method a client wants to use a
         specific endpoint
 
         :param client: A Client instance
         :param endpoint: The endpoint at which the client has to authenticate
         :return: The client authentication method
         """
         if endpoint == "token_endpoint":
-            try:
-                am = client.client_get("service_context").get("behaviour")[
-                    "token_endpoint_auth_method"
-                ]
-            except KeyError:
+            am = client.get_context().get_usage("token_endpoint_auth_method")
+            if not am:
                 return ""
             else:
                 if isinstance(am, str):
                     return am
                 else:  # a list
                     return am[0]
 
@@ -532,37 +551,34 @@
             :py:class:`idpyoidc.message.oauth2.AuthorizationResponse`
         """
         logger.debug(20 * "*" + " get_tokens " + 20 * "*")
 
         if client is None:
             client = self.get_client_from_session_key(state)
 
-        _context = client.client_get("service_context")
-        authorization_response = _context.state.get_item(
-            AuthorizationResponse, "auth_response", state
-        )
-        authorization_request = _context.state.get_item(AuthorizationRequest, "auth_request", state)
+        _context = client.get_context()
+        _claims = _context.cstate.get_set(state, claim=['code', 'redirect_uri'])
 
         req_args = {
-            "code": authorization_response["code"],
+            "code": _claims["code"],
             "state": state,
-            "redirect_uri": authorization_request["redirect_uri"],
+            "redirect_uri": _claims["redirect_uri"],
             "grant_type": "authorization_code",
             "client_id": client.get_client_id(),
             "client_secret": _context.get("client_secret"),
         }
         logger.debug("request_args: {}".format(req_args))
         try:
             tokenresp = client.do_request(
                 "accesstoken",
                 request_args=req_args,
                 authn_method=self.get_client_authn_method(client, "token_endpoint"),
                 state=state,
             )
-        except Exception as err:
+        except Exception:
             message = traceback.format_exception(*sys.exc_info())
             logger.error(message)
             raise
         else:
             if is_error_message(tokenresp):
                 raise OidcServiceError(tokenresp["error"])
 
@@ -593,15 +609,15 @@
         try:
             tokenresp = client.do_request(
                 "refresh_token",
                 authn_method=self.get_client_authn_method(client, "token_endpoint"),
                 state=state,
                 request_args=req_args,
             )
-        except Exception as err:
+        except Exception:
             message = traceback.format_exception(*sys.exc_info())
             logger.error(message)
             raise
         else:
             if is_error_message(tokenresp):
                 raise OidcServiceError(tokenresp["error"])
 
@@ -621,20 +637,16 @@
 
         logger.debug(20 * "*" + " get_user_info " + 20 * "*")
 
         if client is None:
             client = self.get_client_from_session_key(state)
 
         if not access_token:
-            _arg = client.client_get("service_context").state.multiple_extend_request_args(
-                {},
-                state,
-                ["access_token"],
-                ["auth_response", "token_response", "refresh_token_response"],
-            )
+            _arg = client.get_context().cstate.get_set(state, claim=["access_token"])
+            access_token = _arg["access_token"]
 
         request_args = {"access_token": access_token}
 
         resp = client.do_request("userinfo", state=state, request_args=request_args, **kwargs)
         if is_error_message(resp):
             raise OidcServiceError(resp["error"])
 
@@ -650,15 +662,15 @@
         :return: A dictionary with user information
         """
         res = dict([(k, id_token[k]) for k in OpenIDSchema.c_param.keys() if k in id_token])
         res.update(id_token.extra())
         return res
 
     def finalize_auth(
-        self, client, issuer: str, response: dict, behaviour_args: Optional[dict] = None
+            self, client, issuer: str, response: dict, behaviour_args: Optional[dict] = None
     ):
         """
         Given the response returned to the redirect_uri, parse and verify it.
 
         :param behaviour_args: For fine tuning behaviour
         :param client: A Client instance
         :param issuer: An Issuer ID
@@ -681,37 +693,35 @@
             raise
         else:
             logger.debug("Authz response: {}".format(authorization_response.to_dict()))
 
         if is_error_message(authorization_response):
             return authorization_response
 
-        _context = client.client_get("service_context")
+        _context = client.get_context()
         try:
-            _iss = _context.state.get_iss(authorization_response["state"])
+            _iss = _context.cstate.get_set(
+                authorization_response["state"], claim=['iss']).get('iss')
         except KeyError:
             raise KeyError("Unknown state value")
 
         if _iss != issuer:
             logger.error("Issuer problem: {} != {}".format(_iss, issuer))
             # got it from the wrong bloke
             raise ValueError("Impersonator {}".format(issuer))
 
         _srv.update_service_context(authorization_response, key=authorization_response["state"])
-        _context.state.store_item(
-            authorization_response, "auth_response", authorization_response["state"]
-        )
         return authorization_response
 
     def get_access_and_id_token(
-        self,
-        authorization_response=None,
-        state: Optional[str] = "",
-        client: Optional[object] = None,
-        behaviour_args: Optional[dict] = None,
+            self,
+            authorization_response=None,
+            state: Optional[str] = "",
+            client: Optional[object] = None,
+            behaviour_args: Optional[dict] = None,
     ):
         """
         There are a number of services where access tokens and ID tokens can
         occur in the response. This method goes through the possible places
         based on the response_type the client uses.
 
         :param behaviour_args: For fine tuning behaviour
@@ -724,29 +734,26 @@
         """
 
         logger.debug(20 * "*" + " get_access_and_id_token " + 20 * "*")
 
         if client is None:
             client = self.get_client_from_session_key(state)
 
-        _context = client.client_get("service_context")
+        _context = client.get_context()
 
-        if authorization_response is None:
-            if state:
-                authorization_response = _context.state.get_item(
-                    AuthorizationResponse, "auth_response", state
-                )
-            else:
-                raise ValueError("One of authorization_response or state must be provided")
+        resp_attr = authorization_response or _context.cstate.get_set(state,
+                                                                      message=AuthorizationResponse)
+        if resp_attr is None:
+            raise ValueError("One of authorization_response or state must be provided")
 
         if not state:
             state = authorization_response["state"]
 
-        authreq = _context.state.get_item(AuthorizationRequest, "auth_request", state)
-        _resp_type = set(authreq["response_type"])
+        _req_attr = _context.cstate.get_set(state, AuthorizationRequest)
+        _resp_type = set(_req_attr["response_type"].split(' '))
 
         access_token = None
         id_token = None
         if _resp_type in [{"id_token"}, {"id_token", "token"}, {"code", "id_token", "token"}]:
             id_token = authorization_response["__verified_id_token"]
 
         if _resp_type in [
@@ -782,17 +789,17 @@
     # noinspection PyUnusedLocal
     def finalize(self, issuer, response, behaviour_args: Optional[dict] = None):
         """
         The third of the high level methods that a user of this Class should
         know about.
         Once the consumer has redirected the user back to the
         callback URL there might be a number of services that the client should
-        use. Which one those are are defined by the client configuration.
+        use. Which one those are defined by the client configuration.
 
-        :param behaviour_args: For fine tuning
+        :param behaviour_args: For finetuning
         :param issuer: Who sent the response
         :param response: The Authorization response as a dictionary
         :returns: A dictionary with two claims:
             **state** The key under which the session information is
             stored in the data store and
             **error** and encountered error or
             **userinfo** The collected user information
@@ -813,15 +820,15 @@
         _state = authorization_response["state"]
         token = self.get_access_and_id_token(
             authorization_response, state=_state, client=client, behaviour_args=behaviour_args
         )
         _id_token = token.get("id_token")
         logger.debug(f"ID Token: {_id_token}")
 
-        if client.client_get("service", "userinfo") and token["access_token"]:
+        if client.get_service("userinfo") and token["access_token"]:
             inforesp = self.get_user_info(
                 state=authorization_response["state"],
                 client=client,
                 access_token=token["access_token"],
             )
 
             if isinstance(inforesp, ResponseMessage) and "error" in inforesp:
@@ -830,37 +837,37 @@
         elif _id_token:  # look for it in the ID Token
             inforesp = self.userinfo_in_id_token(_id_token)
         else:
             inforesp = {}
 
         logger.debug("UserInfo: %s", inforesp)
 
-        _context = client.client_get("service_context")
+        _context = client.get_context()
         try:
             _sid_support = _context.get("provider_info")["backchannel_logout_session_required"]
         except KeyError:
             try:
                 _sid_support = _context.get("provider_info")[
                     "frontchannel_logout_session_required"
                 ]
-            except:
+            except Exception:
                 _sid_support = False
 
         if _sid_support and _id_token:
             try:
                 sid = _id_token["sid"]
             except KeyError:
                 pass
             else:
-                _context.state.store_sid2state(sid, _state)
+                _context.cstate.bind_key(sid, _state)
 
         if _id_token:
-            _context.state.store_sub2state(_id_token["sub"], _state)
+            _context.cstate.bind_key(_id_token["sub"], _state)
         else:
-            _context.state.store_sub2state(inforesp["sub"], _state)
+            _context.cstate.bind_key(inforesp["sub"], _state)
 
         return {
             "userinfo": inforesp,
             "state": authorization_response["state"],
             "token": token["access_token"],
             "id_token": _id_token,
             "session_state": authorization_response.get("session_state", ""),
@@ -872,21 +879,17 @@
 
         :param state:
         :return: True/False
         """
 
         client = self.get_client_from_session_key(state)
 
-        # Look for Id Token in all the places where it can be
-        _arg = client.client_get("service_context").state.multiple_extend_request_args(
-            {},
-            state,
-            ["__verified_id_token"],
-            ["auth_response", "token_response", "refresh_token_response"],
-        )
+        # Look for an IdToken
+        _arg = client.get_context().cstate.get_set(state,
+                                                   claim=["__verified_id_token"])
 
         if _arg:
             _now = utc_time_sans_frac()
             exp = _arg["__verified_id_token"]["exp"]
             return _now < exp
         else:
             return False
@@ -896,89 +899,78 @@
         Find a valid access token.
 
         :param state:
         :return: An access token if a valid one exists and when it
             expires. Otherwise raise exception.
         """
 
-        exp = 0
         token = None
         indefinite = []
         now = utc_time_sans_frac()
 
         client = self.get_client_from_session_key(state)
-        _context = client.client_get("service_context")
-        for cls, typ in [
-            (AccessTokenResponse, "refresh_token_response"),
-            (AccessTokenResponse, "token_response"),
-            (AuthorizationResponse, "auth_response"),
-        ]:
-            try:
-                response = _context.state.get_item(cls, typ, state)
-            except KeyError:
-                pass
+        _context = client.get_context()
+        _args = _context.cstate.get_set(state, claim=["access_token", "__expires_at"])
+        if "access_token" in _args:
+            access_token = _args["access_token"]
+            _exp = _args.get("__expires_at", 0)
+            if not _exp:  # No expiry date, lives for ever
+                indefinite.append((access_token, 0))
             else:
-                if "access_token" in response:
-                    access_token = response["access_token"]
-                    try:
-                        _exp = response["__expires_at"]
-                    except KeyError:  # No expiry date, lives for ever
-                        indefinite.append((access_token, 0))
-                    else:
-                        if _exp > now and _exp > exp:  # expires sometime in the future
-                            exp = _exp
-                            token = (access_token, _exp)
+                if _exp > now:  # expires sometime in the future
+                    token = (access_token, _exp)
 
         if indefinite:
             return indefinite[0]
         else:
             if token:
                 return token
             else:
                 raise OidcServiceError("No valid access token")
 
     def logout(
-        self,
-        state: str,
-        client: Optional[Client] = None,
-        post_logout_redirect_uri: Optional[str] = "",
+            self,
+            state: str,
+            client: Optional[Client] = None,
+            post_logout_redirect_uri: Optional[str] = "",
     ) -> dict:
         """
-        Does a RP initiated logout from an OP. After logout the user will be
-        redirect by the OP to a URL of choice (post_logout_redirect_uri).
+        Does an RP initiated logout from an OP. After logout the user will be
+        redirected by the OP to a URL of choice (post_logout_redirect_uri).
 
         :param state: Key to an active session
         :param client: Which client to use
         :param post_logout_redirect_uri: If a special post_logout_redirect_uri
             should be used
-        :return: A US
+        :return: Request arguments
         """
 
         logger.debug(20 * "*" + " logout " + 20 * "*")
 
         if client is None:
             client = self.get_client_from_session_key(state)
 
         try:
-            srv = client.client_get("service", "end_session")
+            srv = client.get_service("end_session")
         except KeyError:
             raise OidcServiceError("Does not know how to logout")
 
         if post_logout_redirect_uri:
             request_args = {"post_logout_redirect_uri": post_logout_redirect_uri}
         else:
             request_args = {}
 
         resp = srv.get_request_parameters(state=state, request_args=request_args)
 
         logger.debug(f"EndSession Request: {resp}")
         return resp
 
     def close(
-        self, state: str, issuer: Optional[str] = "", post_logout_redirect_uri: Optional[str] = ""
+            self, state: str, issuer: Optional[str] = "",
+            post_logout_redirect_uri: Optional[str] = ""
     ) -> dict:
 
         logger.debug(20 * "*" + " close " + 20 * "*")
 
         if issuer:
             client = self.issuer2rp[issuer]
         else:
@@ -986,15 +978,15 @@
 
         return self.logout(
             state=state, client=client, post_logout_redirect_uri=post_logout_redirect_uri
         )
 
     def clear_session(self, state):
         client = self.get_client_from_session_key(state)
-        client.client_get("service_context").state.remove_state(state)
+        client.get_context().cstate.remove_state(state)
 
 
 def backchannel_logout(client, request="", request_args=None):
     """
 
     :param request: URL encoded logout request
     :return:
@@ -1002,19 +994,19 @@
     if request:
         req = BackChannelLogoutRequest().from_urlencoded(as_unicode(request))
     elif request_args:
         req = BackChannelLogoutRequest(**request_args)
     else:
         raise MissingRequiredAttribute("logout_token")
 
-    _context = client.client_get("service_context")
+    _context = client.get_context()
     kwargs = {
         "aud": client.get_client_id(),
         "iss": _context.get("issuer"),
-        "keyjar": _context.keyjar,
+        "keyjar": client.get_attribute('keyjar'),
         "allowed_sign_alg": _context.get("registration_response").get(
             "id_token_signed_response_alg", "RS256"
         ),
     }
 
     logger.debug(f"(backchannel_logout) Verifying request using: {kwargs}")
     try:
@@ -1029,32 +1021,32 @@
     sid = None
     if not sub:
         sid = req[verified_claim_name("logout_token")].get("sid")
 
     if not sub and not sid:
         raise MessageException('Neither "sid" nor "sub"')
     elif sub:
-        _state = _context.state.get_state_by_sub(sub)
+        _state = _context.cstate.get_base_key(sub)
     elif sid:
-        _state = _context.state.get_state_by_sid(sid)
+        _state = _context.cstate.get_base_key(sid)
     else:
         _state = None
 
     return _state
 
 
 def load_registration_response(client, request_args=None):
     """
     If the client has been statically registered that information
     must be provided during the configuration. If expected to be
     done dynamically this method will do dynamic client registration.
 
     :param client: A :py:class:`idpyoidc.client.oidc.Client` instance
     """
-    if not client.client_get("service_context").get_client_id():
+    if not client.get_context().get_client_id():
         try:
             response = client.do_request("registration", request_args=request_args)
         except KeyError:
             raise ConfigurationError("No registration info")
         except Exception as err:
             logger.error(err)
             raise
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/service.py` & `idpyoidc-2.0.0/src/idpyoidc/client/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 """ The basic Service class upon which all the specific services are built. """
+import copy
 import json
 import logging
 from typing import Callable
+from typing import List
 from typing import Optional
 from typing import Union
 from urllib.parse import urlparse
 
 from cryptojwt.jwt import JWT
-from cryptojwt.utils import qualified_name
 
 from idpyoidc.client.exception import Unsupported
 from idpyoidc.impexp import ImpExp
 from idpyoidc.item import DLDict
 from idpyoidc.message import Message
-from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.message.oauth2 import is_error_message
+from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.util import importer
+from .client_auth import client_auth_setup
+from .client_auth import method_to_item
+from .client_auth import single_authn_setup
 from .configure import Configuration
 from .exception import ResponseError
 from .util import get_http_body
 from .util import get_http_url
 from ..constant import JOSE_ENCODED
 from ..constant import JSON_ENCODED
 from ..constant import URL_ENCODED
 
 __author__ = "Roland Hedberg"
 
+from ..context import OidcContext
+
 LOGGER = logging.getLogger(__name__)
 
 SUCCESSFUL = [200, 201, 202, 203, 204, 205, 206]
 
 SPECIAL_ARGS = ["authn_endpoint", "algs"]
 
 REQUEST_INFO = "Doing request with: URL:{}, method:{}, data:{}, https_args:{}"
@@ -57,73 +63,65 @@
         "http_method": None,
         "msg_type": object,
         "request_body_type": None,
         "response_body_type": None,
         "response_cls": object,
     }
 
-    init_args = ["client_get"]
+    init_args = ["upstream_get"]
 
-    metadata_attributes = {}
-    usage_rules = {}
-    usage_to_uri_map = {}
-    callback_path = {}
-    callback_uris = []
+    _include = {}
+    _supports = {}
+    _callback_path = {}
 
     def __init__(
             self,
-            client_get: Callable,
+            upstream_get: Callable,
             conf: Optional[Union[dict, Configuration]] = None,
             **kwargs
     ):
         ImpExp.__init__(self)
 
-        self.client_get = client_get
+        self.upstream_get = upstream_get
         self.default_request_args = {}
-        self.metadata = {}
-        self.usage = {}
-        self.callback_uri = {}
+        self.client_authn_methods = {}
 
         if conf:
             self.conf = conf
             for param in [
                 "msg_type",
                 "response_cls",
                 "error_msg",
-                "default_authn_method",
                 "http_method",
                 "request_body_type",
                 "response_body_type",
+                "default_authn_method"
             ]:
                 if param in conf:
                     setattr(self, param, conf[param])
 
-            md_conf = conf.get("metadata", {})
-            if md_conf:
-                for param, def_val in self.metadata_attributes.items():
-                    if param in md_conf:
-                        self.metadata[param] = md_conf[param]
-                    elif def_val is not None:
-                        self.metadata[param] = def_val
-
-            usage_conf = conf.get("usage", {})
-            if usage_conf:
-                for param, def_val in self.usage_rules.items():
-                    if param in usage_conf:
-                        self.usage[param] = usage_conf[param]
-                    elif def_val is not None:
-                        self.usage[param] = def_val
-
             _default_request_args = conf.get("request_args", {})
             if _default_request_args:
                 self.default_request_args = _default_request_args
                 del conf["request_args"]
 
+            _client_authn_methods = conf.get("client_authn_methods", None)
+            if _client_authn_methods:
+                self.client_authn_methods = client_auth_setup(method_to_item(_client_authn_methods))
+
+            if self.default_authn_method:
+                if self.default_authn_method not in self.client_authn_methods:
+                    self.client_authn_methods[self.default_authn_method] = single_authn_setup(
+                        self.default_authn_method, None)
+
         else:
             self.conf = {}
+            if self.default_authn_method:
+                self.client_authn_methods[self.default_authn_method] = single_authn_setup(
+                    self.default_authn_method, None)
 
         # pull in all the modifiers
         self.pre_construct = []
         self.post_construct = []
         self.construct_extra_headers = []
         self.post_parse_process = []
 
@@ -134,42 +132,38 @@
         when there are default values.
 
         :param kwargs: Initial set of attributes.
         :return: Possibly augmented set of attributes
         """
         ar_args = kwargs.copy()
 
-        _entity = self.client_get("entity")
-        md = _entity.collect_metadata()
+        _context = self.upstream_get("context")
+        _use = _context.collect_usage()
+        if not _use:
+            _use = _context.map_preferred_to_registered()
+
+        if "request_args" in self.conf:
+            ar_args.update(self.conf["request_args"])
 
-        _context = self.client_get("service_context")
         # Go through the list of claims defined for the message class.
         # There are a couple of places where information can be found.
         # Access them in the order of priority
         # 1. A keyword argument
         # 2. configured set of default attribute values
         # 3. default attribute values defined in the OIDC standard document
         for prop in self.msg_type.c_param:
             if prop in ar_args:
                 continue
 
-            if prop != "state":
-                val = _context.get(prop)
-            else:
-                val = ""
-
+            val = _use.get(prop)
             if not val:
-                if "request_args" in self.conf:
-                    val = self.conf["request_args"].get(prop)
-                if not val:
-                    val = self.default_request_args.get(prop)
-                    if not val:
-                        val = _context.specs.behaviour.get(prop)
-                        if not val:
-                            val = md.get(prop)
+                # val = request_claim(_context, prop)
+                # if not val:
+                val = self.default_request_args.get(prop)
+
             if val:
                 ar_args[prop] = val
 
         for key, val in self.default_request_args.items():
             if key not in ar_args:
                 ar_args[key] = val
 
@@ -223,25 +217,25 @@
         _args = self.method_args("post_construct", **kwargs)
 
         for meth in self.post_construct:
             request_args = meth(request_args, service=self, **_args)
 
         return request_args
 
-    def update_service_context(self, resp, key="", **kwargs):
+    def update_service_context(self, resp: Message, key: Optional[str] = '', **kwargs):
         """
         A method run after the response has been parsed and verified.
 
         :param resp: The response as a :py:class:`idpyoidc.Message` instance
         :param key: The key under which the response should be stored
         :param kwargs: Extra key word arguments
         """
         pass
 
-    def construct(self, request_args=None, **kwargs):
+    def construct(self, request_args: Optional[dict] = None, **kwargs):
         """
         Instantiate the request as a message class instance with
         attribute values gathered in a pre_construct method or in the
         gather_request_args method.
 
         :param request_args:
         :param kwargs: extra keyword arguments
@@ -289,20 +283,23 @@
         :return: Extended set of HTTP header arguments
         """
         if http_args is None:
             http_args = {}
 
         if authn_method:
             LOGGER.debug("Client authn method: %s", authn_method)
-            _context = self.client_get("service_context")
-            try:
-                _func = _context.client_authn_method[authn_method]
-            except KeyError:  # not one of the common
-                LOGGER.error(f"Unknown client authentication method: {authn_method}")
-                raise Unsupported(f"Unknown client authentication method: {authn_method}")
+            if self.client_authn_methods and authn_method in self.client_authn_methods:
+                _func = self.client_authn_methods[authn_method]
+            else:
+                _context = self.upstream_get("context")
+                try:
+                    _func = _context.client_authn_methods[authn_method]
+                except KeyError:  # not one of the common
+                    LOGGER.error(f"Unknown client authentication method: {authn_method}")
+                    raise Unsupported(f"Unknown client authentication method: {authn_method}")
 
             return _func.construct(request, self, http_args=http_args, **kwargs)
 
         return http_args
 
     def construct_request(self, request_args=None, **kwargs):
         """
@@ -325,15 +322,15 @@
         Find the service endpoint
 
         :return: The service endpoint (a URL)
         """
         if self.endpoint:
             return self.endpoint
 
-        return self.client_get("service_context").provider_info[self.endpoint_name]
+        return self.upstream_get("context").provider_info[self.endpoint_name]
 
     def get_authn_header(
             self, request: Union[dict, Message], authn_method: Optional[str] = "", **kwargs
     ) -> dict:
         """
         Construct an authorization specification to be sent in the
         HTTP header.
@@ -382,15 +379,15 @@
 
         _headers = self.get_authn_header(
             request, authn_method=authn_method, authn_endpoint=self.endpoint_name, **kwargs
         )
 
         for meth in self.construct_extra_headers:
             _headers = meth(
-                self.client_get("service_context"),
+                self.upstream_get("context"),
                 headers=_headers,
                 request=request,
                 authn_method=authn_method,
                 service_endpoint=self.endpoint_name,
                 http_method=http_method,
                 **kwargs,
             )
@@ -429,15 +426,15 @@
 
         request = self.construct_request(request_args=request_args, **kwargs)
 
         LOGGER.debug("Request: %s", request)
         _info = {"method": method, "request": request}
 
         _args = kwargs.copy()
-        _context = self.client_get("service_context")
+        _context = self.upstream_get("context")
         if _context.issuer:
             _args["iss"] = _context.issuer
 
         # Client authentication by usage of the Authorization HTTP header
         # or by modifying the request object
         _headers = self.get_headers(request, http_method=method, authn_method=authn_method, **_args)
 
@@ -505,44 +502,46 @@
     ):
         """
         Need to add some information before running verify()
 
         :return: dictionary with arguments to the verify call
         """
 
-        _context = self.client_get("service_context")
+        _context = self.upstream_get("context")
         kwargs = {
             "iss": _context.issuer,
-            "keyjar": _context.keyjar,
+            "keyjar": self.upstream_get('attribute', 'keyjar'),
             "verify": True,
             "client_id": _context.get_client_id(),
         }
 
         if self.service_name == "provider_info":
             if _context.issuer.startswith("http://"):
                 kwargs["allow_http"] = True
 
         return kwargs
 
     def _do_jwt(self, info):
-        _context = self.client_get("service_context")
+        _context = self.upstream_get("context")
         args = {"allowed_sign_algs": _context.get_sign_alg(self.service_name)}
         enc_algs = _context.get_enc_alg_enc(self.service_name)
         args["allowed_enc_algs"] = enc_algs["alg"]
         args["allowed_enc_encs"] = enc_algs["enc"]
-        _jwt = JWT(key_jar=_context.keyjar, **args)
+
+        _jwt = JWT(key_jar=self.upstream_get('attribute', 'keyjar'), **args)
         _jwt.iss = _context.get_client_id()
         return _jwt.unpack(info)
 
     def _do_response(self, info, sformat, **kwargs):
-        _context = self.client_get("service_context")
+        _context = self.upstream_get("context")
 
         try:
             resp = self.response_cls().deserialize(info, sformat, iss=_context.issuer, **kwargs)
         except Exception as err:
+            LOGGER.error("Error while deserializing: %s (1 pass)", err)
             resp = None
             if sformat == "json":
                 # Could be JWS or JWE but wrongly tagged
                 # Adding issuer is just a fail-safe. If one thing was wrong then two can be.
                 try:
                     resp = self.response_cls().deserialize(
                         info, "jwt", iss=_context.issuer, **kwargs
@@ -575,44 +574,53 @@
               an error response.
 
         :param behaviour_args:
         :param info: The response, can be either in a JSON or an urlencoded format
         :param sformat: Which serialization that was used
         :param state: The state
         :param kwargs: Extra key word arguments
-        :return: The parsed and to some extend verified response
+        :return: The parsed and to some extent verified response
         """
 
         if not sformat:
             sformat = self.response_body_type
 
         LOGGER.debug("response format: %s", sformat)
 
-        if sformat in ["jose", "jws", "jwe"]:
-            resp = self.post_parse_response(info, state=state)
-
-            if not resp:
-                LOGGER.error("Missing or faulty response")
-                raise ResponseError("Missing or faulty response")
-
-            return resp
+        resp = None
+        if sformat == "jose":
+            try:
+                self._do_jwt(info)
+                sformat = "dict"
+            except Exception:
+                _keyjar = self.upstream_get("attribute", 'keyjar')
+                resp = self.response_cls().from_jwe(info, keys=_keyjar)
+        elif sformat == "jwe":
+            _keyjar = self.upstream_get("attribute", 'keyjar')
+            _client_id = self.upstream_get("attribute", 'client_id')
+            resp = self.response_cls().from_jwe(info, keys=_keyjar.get_issuer_keys(_client_id))
         # If format is urlencoded 'info' may be a URL
         # in which case I have to get at the query/fragment part
         elif sformat == "urlencoded":
             info = self.get_urlinfo(info)
-        elif sformat == "jwt":
+        elif sformat in ["jwt", "jws"]:
             info = self._do_jwt(info)
             sformat = "dict"
         elif sformat == "json":
             info = json.loads(info)
             sformat = "dict"
 
         LOGGER.debug("response_cls: %s", self.response_cls.__name__)
 
-        resp = self._do_response(info, sformat, **kwargs)
+        if resp is None:
+            if not info:
+                LOGGER.error("Missing or faulty response")
+                raise ResponseError("Missing or faulty response")
+
+            resp = self._do_response(info, sformat, **kwargs)
 
         LOGGER.debug('Initial response parsing => "%s"', resp.to_dict())
 
         # is this an error message
         if is_error_message(resp):
             LOGGER.debug("Error response: %s", resp)
         else:
@@ -629,87 +637,90 @@
 
         if not resp:
             LOGGER.error("Missing or faulty response")
             raise ResponseError("Missing or faulty response")
 
         return resp
 
-    def get_conf_attr(self, attr, default=None):
-        """
-        Get the value of a attribute in the configuration
-
-        :param attr: The attribute
-        :param default: If the attribute doesn't appear in the configuration
-            return this value
-        :return: The value of attribute in the configuration or the default
-            value
-        """
-        if attr in self.conf:
-            return self.conf[attr]
-
-        return default
+    def supports(self):
+        res = {}
+        for key, val in self._supports.items():
+            if isinstance(val, Callable):
+                res[key] = val()
+            else:
+                res[key] = val
+        return res
 
-    def usage_to_uri(self, usage):
-        return self.usage_to_uri_map.get(usage)
+    def extends(self, info):
+        for claim, val in self._include.items():
+            if claim in info:
+                info[claim].extend(val)
+            else:
+                info[claim] = copy.copy(val)
+        return info
 
     def get_callback_path(self, callback):
-        return self.callback_path.get(callback)
+        return self._callback_path.get(callback)
 
     @staticmethod
     def get_uri(base_url, path, hex):
         return f"{base_url}/{path}/{hex}"
 
-    def construct_uris(self, base_url, hex):
-        for usage in self.usage_rules.keys():
-            if usage in self.usage:
-                uri = self.usage_to_uri_map.get(usage)
-                if uri and uri not in self.metadata:
-                    self.metadata[uri] = self.get_uri(base_url, self.callback_path[uri],
-                                                      hex)
+    def construct_uris(self,
+                       base_url: str,
+                       hex: bytes,
+                       context: OidcContext,
+                       targets: Optional[List[str]] = None,
+                       response_types: Optional[list] = None):
+        if not targets:
+            targets = self._callback_path.keys()
+
+        if not targets:
+            return {}
+
+        _callback_uris = context.get_preference('callback_uris', {})
+        for uri in targets:
+            if uri in _callback_uris:
+                pass
+            else:
+                _path = self._callback_path.get(uri)
+                if isinstance(_path, str):
+                    _callback_uris[uri] = self.get_uri(base_url, _path, hex)
+                else:
+                    _callback_uris[uri] = [self.get_uri(base_url, _var, hex) for _var in _path]
+
+        return _callback_uris
 
-    def get_metadata(self, attribute, default=None):
-        try:
-            return self.metadata[attribute]
-        except KeyError:
-            return default
+    def supported(self, claim):
+        return claim in self._supports
 
-    def set_metadata(self, key, value):
-        self.metadata[key] = value
+    def callback_uris(self):
+        return list(self._callback_path.keys())
 
 
-def init_services(service_definitions, client_get, metadata, usage):
+def init_services(service_definitions, upstream_get):
     """
     Initiates a set of services
 
     :param service_definitions: A dictionary containing service definitions
-    :param client_get: A function that returns different things from the base entity.
+    :param upstream_get: A function that returns different things from the base entity.
     :return: A dictionary, with service name as key and the service instance as
         value.
     """
     service = DLDict()
     for service_name, service_configuration in service_definitions.items():
         try:
             kwargs = {"conf": service_configuration["kwargs"]}
         except KeyError:
             kwargs = {}
 
-        kwargs.update({"client_get": client_get})
+        kwargs.update({"upstream_get": upstream_get})
 
         if isinstance(service_configuration["class"], str):
-            _value_cls = service_configuration["class"]
             _cls = importer(service_configuration["class"])
             _srv = _cls(**kwargs)
         else:
-            _value_cls = qualified_name(service_configuration["class"])
             _srv = service_configuration["class"](**kwargs)
 
-        for key, val in metadata.items():
-            if key in _srv.metadata_attributes and key not in _srv.metadata:
-                _srv.metadata[key] = val
-
-        for key, val in usage.items():
-            if key in _srv.usage_rules and key not in _srv.usage:
-                _srv.usage[key] = val
-
         service[_srv.service_name] = _srv
 
     return service
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/service_context.py` & `idpyoidc-2.0.0/src/idpyoidc/client/service_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 """
 Implements a service context. A Service context is used to keep information that are
 common between all the services that are used by OAuth2 client or OpenID Connect Relying Party.
 """
-import copy
+import hashlib
+import logging
+from typing import Callable
 from typing import Optional
 from typing import Union
 
 from cryptojwt.jwk.rsa import RSAKey
 from cryptojwt.jwk.rsa import import_private_rsa_key_from_file
 from cryptojwt.key_bundle import KeyBundle
 from cryptojwt.key_jar import KeyJar
 from cryptojwt.utils import as_bytes
 
+from idpyoidc.claims import Claims
+from idpyoidc.claims import claims_dump
+from idpyoidc.claims import claims_load
+from idpyoidc.client.claims.oauth2 import Claims as OAUTH2_Specs
+from idpyoidc.client.claims.oidc import Claims as OIDC_Specs
 from idpyoidc.client.configure import Configuration
-from idpyoidc.client.specification.oauth2 import Specification as OAUTH2_Specs
-from idpyoidc.client.specification.oidc import Specification as OIDC_Specs
-from idpyoidc.context import OidcContext
 from idpyoidc.util import rndstr
+from .claims.transform import preferred_to_registered
+from .claims.transform import supported_to_preferred
 from .configure import get_configuration
-from .specification import Specification
-from .specification import specification_dump
-from .specification import specification_load
-from .state_interface import StateInterface
+from .current import Current
+from ..impexp import ImpExp
+
+logger = logging.getLogger(__name__)
 
 CLI_REG_MAP = {
     "userinfo": {
         "sign": "userinfo_signed_response_alg",
         "alg": "userinfo_encrypted_response_alg",
         "enc": "userinfo_encrypted_response_enc",
     },
@@ -61,109 +67,95 @@
 }
 
 DEFAULT_VALUE = {
     "client_secret": "",
     "client_id": "",
     "redirect_uris": [],
     "provider_info": {},
-    "behaviour": {},
     "callback": {},
     "issuer": ""
 }
 
 
-class ServiceContext(OidcContext):
+class ServiceContext(ImpExp):
     """
     This class keeps information that a client needs to be able to talk
     to a server. Some of this information comes from configuration and some
     from dynamic provider info discovery or client registration.
     But information is also picked up during the conversation with a server.
     """
 
-    parameter = OidcContext.parameter.copy()
-    parameter.update(
-        {
-            "add_on": None,
-            "allow": None,
-            "args": None,
-            "base_url": None,
-            "behaviour": None,
-            "callback": None,
-            "client_secret": None,
-            "client_secret_expires_at": 0,
-            "clock_skew": None,
-            "config": None,
-            "hash_seed": b"",
-            "httpc_params": None,
-            "iss_hash": None,
-            "issuer": None,
-            "specs": Specification,
-            "provider_info": None,
-            "requests_dir": None,
-            "registration_response": None,
-            "state": StateInterface,
-            'usage': None,
-            "verify_args": None,
-        }
-    )
+    parameter = {
+        "add_on": None,
+        "allow": None,
+        "args": None,
+        "base_url": None,
+        # "behaviour": None,
+        # "client_secret_expires_at": 0,
+        "clock_skew": None,
+        "config": None,
+        "hash_seed": b"",
+        "httpc_params": None,
+        "iss_hash": None,
+        "issuer": None,
+        'keyjar': KeyJar,
+        "claims": Claims,
+        "provider_info": None,
+        "requests_dir": None,
+        "registration_response": None,
+        "cstate": Current,
+        # 'usage': None,
+        "verify_args": None,
+    }
 
     special_load_dump = {
-        "specs": {"load": specification_load, "dump": specification_dump},
+        "specs": {"load": claims_load, "dump": claims_dump},
     }
 
+    init_args = ['upstream_get']
 
     def __init__(self,
+                 upstream_get: Optional[Callable] = None,
                  base_url: Optional[str] = "",
                  keyjar: Optional[KeyJar] = None,
                  config: Optional[Union[dict, Configuration]] = None,
-                 state: Optional[StateInterface] = None,
-                 client_type: Optional[str] = None,
+                 cstate: Optional[Current] = None,
+                 client_type: Optional[str] = 'oauth2',
                  **kwargs):
+        ImpExp.__init__(self)
         config = get_configuration(config)
         self.config = config
+        self.upstream_get = upstream_get
+
         if not client_type or client_type == "oidc":
-            self.specs = OIDC_Specs()
+            self.claims = OIDC_Specs()
         elif client_type == "oauth2":
-            self.specs = OAUTH2_Specs()
+            self.claims = OAUTH2_Specs()
         else:
             raise ValueError(f"Unknown client type: {client_type}")
 
-        OidcContext.__init__(self, config, keyjar, entity_id=config.conf.get("client_id", ""))
-        self.state = state or StateInterface()
+        self.entity_id = config.conf.get("client_id", "")
+        self.cstate = cstate or Current()
 
         self.kid = {"sig": {}, "enc": {}}
 
-        self.base_url = base_url or config.get("base_url") or config.conf.get('base_url', '')
+        self.allow = config.conf.get('allow', {})
+        self.base_url = base_url or config.conf.get("base_url", "")
+        self.provider_info = config.conf.get("provider_info", {})
+
         # Below so my IDE won't complain
-        self.allow = {}
         self.args = {}
         self.add_on = {}
         self.iss_hash = ""
         self.issuer = ""
         self.httpc_params = {}
-        self.callback = {}
-        self.client_secret = ""
         self.client_secret_expires_at = 0
-        self.provider_info = {}
-        # self.post_logout_redirect_uri = ""
-        # self.redirect_uris = []
         self.registration_response = {}
-        self.requests_dir = ""
 
-        _def_value = copy.deepcopy(DEFAULT_VALUE)
-
-        for param in [
-            "client_secret",
-            "provider_info",
-            "behaviour"
-        ]:
-            _val = config.conf.get(param, _def_value[param])
-            self.set(param, _val)
-            if param == "client_secret" and _val:
-                self.keyjar.add_symmetric("", _val)
+        # _def_value = copy.deepcopy(DEFAULT_VALUE)
 
         _issuer = config.get("issuer")
         if _issuer:
             self.issuer = _issuer
         else:
             self.issuer = self.provider_info.get("issuer", "")
 
@@ -171,15 +163,22 @@
 
         _seed = config.get("hash_seed", rndstr(32))
         self.hash_seed = as_bytes(_seed)
 
         for key, val in kwargs.items():
             setattr(self, key, val)
 
-        self.specs.load_conf(config.conf)
+        self.keyjar = self.claims.load_conf(config.conf, supports=self.supports(),
+                                            keyjar=keyjar)
+
+        _response_types = self.get_preference(
+            'response_types_supported',
+            self.supports().get('response_types_supported', []))
+
+        self.construct_uris(response_types=_response_types)
 
     def __setitem__(self, key, value):
         setattr(self, key, value)
 
     def filename_from_webname(self, webname):
         """
         A 1<->1 map is maintained between a URL pointing to a file and
@@ -207,67 +206,168 @@
         The client needs its own set of keys. It can either dynamically
         create them or load them from local storage.
         This method can also fetch other entities keys provided the
         URL points to a JWKS.
 
         :param keyspec:
         """
+        _keyjar = self.upstream_get('attribute', 'keyjar')
+        if _keyjar is None:
+            _keyjar = KeyJar()
+            new = True
+        else:
+            new = False
+
         for where, spec in keyspec.items():
             if where == "file":
                 for typ, files in spec.items():
                     if typ == "rsa":
                         for fil in files:
                             _key = RSAKey(priv_key=import_private_rsa_key_from_file(fil), use="sig")
                             _bundle = KeyBundle()
                             _bundle.append(_key)
-                            self.keyjar.add_kb("", _bundle)
+                            _keyjar.add_kb("", _bundle)
             elif where == "url":
                 for iss, url in spec.items():
                     _bundle = KeyBundle(source=url)
-                    self.keyjar.add_kb(iss, _bundle)
+                    _keyjar.add_kb(iss, _bundle)
+
+        if new:
+            _unit = self.upstream_get('unit')
+            _unit.setattribute('keyjar', _keyjar)
+
+    def _get_crypt(self, typ, attr):
+        _item_typ = CLI_REG_MAP.get(typ)
+        _alg = ''
+        if _item_typ:
+            _alg = self.claims.get_usage(_item_typ[attr])
+            if not _alg:
+                _alg = self.claims.get_preference(_item_typ[attr])
+
+        if not _alg:
+            _item_typ = PROVIDER_INFO_MAP.get(typ)
+            if _item_typ:
+                _alg = self.provider_info.get(_item_typ[attr])
+
+        return _alg
 
     def get_sign_alg(self, typ):
         """
 
         :param typ: ['id_token', 'userinfo', 'request_object']
-        :return:
+        :return: signing algorithm
         """
-
-        try:
-            return self.specs.behaviour[CLI_REG_MAP[typ]["sign"]]
-        except KeyError:
-            try:
-                return self.provider_info[PROVIDER_INFO_MAP[typ]["sign"]]
-            except (KeyError, TypeError):
-                pass
-
-        return None
+        return self._get_crypt(typ, 'sign')
 
     def get_enc_alg_enc(self, typ):
         """
 
         :param typ:
         :return:
         """
 
         res = {}
         for attr in ["enc", "alg"]:
-            try:
-                _alg = self.specs.behaviour[CLI_REG_MAP[typ][attr]]
-            except KeyError:
-                try:
-                    _alg = self.provider_info[PROVIDER_INFO_MAP[typ][attr]]
-                except KeyError:
-                    _alg = None
-
-            res[attr] = _alg
+            res[attr] = self._get_crypt(typ, attr)
 
         return res
 
     def get(self, key, default=None):
         return getattr(self, key, default)
 
     def set(self, key, value):
         setattr(self, key, value)
 
     def get_client_id(self):
-        return self.specs.get_metadata("client_id")
+        return self.claims.get_usage("client_id")
+
+    def collect_usage(self):
+        return self.claims.use
+
+    def supports(self):
+        res = {}
+        if self.upstream_get:
+            services = self.upstream_get('services')
+            if not services:
+                pass
+            else:
+                for service in services.values():
+                    res.update(service.supports())
+                    res = service.extends(res)
+        res.update(self.claims.supports())
+        return res
+
+    def prefers(self):
+        return self.claims.prefer
+
+    def get_preference(self, claim, default=None):
+        return self.claims.get_preference(claim, default=default)
+
+    def set_preference(self, key, value):
+        self.claims.set_preference(key, value)
+
+    def get_usage(self, claim, default: Optional[str] = None):
+        return self.claims.get_usage(claim, default)
+
+    def set_usage(self, claim, value):
+        return self.claims.set_usage(claim, value)
+
+    def _callback_per_service(self):
+        _cb = {}
+        for service in self.upstream_get('services').values():
+            _cbs = service._callback_path.keys()
+            if _cbs:
+                _cb[service.service_name] = _cbs
+        return _cb
+
+    def construct_uris(self, response_types: Optional[list] = None):
+        _hash = hashlib.sha256()
+        _hash.update(self.hash_seed)
+        _hash.update(as_bytes(self.issuer))
+        _hex = _hash.hexdigest()
+
+        self.iss_hash = _hex
+
+        _base_url = self.get("base_url")
+
+        _callback_uris = self.get_preference('callback_uris', {})
+        if self.upstream_get:
+            services = self.upstream_get('services')
+            if services:
+                for service in services.values():
+                    _callback_uris.update(service.construct_uris(base_url=_base_url, hex=_hex,
+                                                                 context=self,
+                                                                 response_types=response_types))
+
+        self.set_preference('callback_uris', _callback_uris)
+        if 'redirect_uris' in _callback_uris:
+            _redirect_uris = set()
+            for flow, _uris in _callback_uris['redirect_uris'].items():
+                _redirect_uris.update(set(_uris))
+            self.set_preference('redirect_uris', list(_redirect_uris))
+
+    def prefer_or_support(self, claim):
+        if claim in self.claims.prefer:
+            return 'prefer'
+        else:
+            for service in self.upstream_get('services').values():
+                _res = service.prefer_or_support(claim)
+                if _res:
+                    return _res
+
+        if claim in self.claims.supported(claim):
+            return 'support'
+        return None
+
+    def map_supported_to_preferred(self, info: Optional[dict] = None):
+        self.claims.prefer = supported_to_preferred(self.supports(),
+                                                    self.claims.prefer,
+                                                    base_url=self.base_url,
+                                                    info=info)
+        return self.claims.prefer
+
+    def map_preferred_to_registered(self, registration_response: Optional[dict] = None):
+        self.claims.use = preferred_to_registered(
+            self.claims.prefer,
+            supported=self.supports(),
+            registration_response=registration_response)
+        return self.claims.use
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/specification/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,185 +1,147 @@
+import logging
 from typing import Optional
+from typing import Union
 
-from cryptojwt.utils import importer
+from idpyoidc.message import Message
+from idpyoidc.message.oidc import RefreshAccessTokenRequest
+from idpyoidc.server.session.token import RefreshToken
+from idpyoidc.server.token.exception import UnknownToken
+from idpyoidc.time_util import utc_time_sans_frac
+from . import TokenEndpointHelper
+
+logger = logging.getLogger(__name__)
+
+
+class RefreshTokenHelper(TokenEndpointHelper):
+
+    def process_request(self, req: Union[Message, dict], **kwargs):
+        _context = self.endpoint.upstream_get("context")
+        _mngr = _context.session_manager
+        logger.debug("Refresh Token")
+
+        if req["grant_type"] != "refresh_token":
+            return self.error_cls(error="invalid_request", error_description="Wrong grant_type")
+
+        token_value = req["refresh_token"]
+        _session_info = _mngr.get_session_info_by_token(
+            token_value, grant=True, handler_key="refresh_token"
+        )
+        logger.debug("Session info: {}".format(_session_info))
+
+        if _session_info["client_id"] != req["client_id"]:
+            logger.debug("{} owner of token".format(_session_info["client_id"]))
+            logger.warning("Client using token it was not given")
+            return self.error_cls(error="invalid_grant", error_description="Wrong client")
+
+        _grant = _session_info["grant"]
+
+        token_type = "Bearer"
+
+        # Is DPOP supported
+        if "dpop_signing_alg_values_supported" in _context.provider_info:
+            _dpop_jkt = req.get("dpop_jkt")
+            if _dpop_jkt:
+                _grant.extra["dpop_jkt"] = _dpop_jkt
+                token_type = "DPoP"
+
+        token = _grant.get_token(token_value)
+        scope = _grant.find_scope(token)
+        if "scope" in req:
+            scope = req["scope"]
+        access_token = self._mint_token(
+            token_class="access_token",
+            grant=_grant,
+            session_id=_session_info["branch_id"],
+            client_id=_session_info["client_id"],
+            based_on=token,
+            scope=scope,
+            token_type=token_type,
+        )
+
+        _resp = {
+            "access_token": access_token.value,
+            "token_type": access_token.token_type,
+            "scope": scope,
+        }
+
+        if access_token.expires_at:
+            _resp["expires_in"] = access_token.expires_at - utc_time_sans_frac()
+
+        _mints = token.usage_rules.get("supports_minting")
+        issue_refresh = kwargs.get("issue_refresh", False)
+        if "refresh_token" in _mints and issue_refresh:
+            refresh_token = self._mint_token(
+                token_class="refresh_token",
+                grant=_grant,
+                session_id=_session_info["branch_id"],
+                client_id=_session_info["client_id"],
+                based_on=token,
+                scope=scope,
+            )
+            refresh_token.usage_rules = token.usage_rules.copy()
+            _resp["refresh_token"] = refresh_token.value
+
+        token.register_usage()
+
+        if (
+                "client_id" in req
+                and req["client_id"] in _context.cdb
+                and "revoke_refresh_on_issue" in _context.cdb[req["client_id"]]
+        ):
+            revoke_refresh = _context.cdb[req["client_id"]].get("revoke_refresh_on_issue")
+        else:
+            revoke_refresh = self.endpoint.revoke_refresh_on_issue
+
+        if revoke_refresh:
+            token.revoke()
+
+        return _resp
+
+    def post_parse_request(
+            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+    ):
+        """
+        This is where clients come to refresh their access tokens
+
+        :param request: The request
+        :param client_id: Client identifier
+        :returns:
+        """
+
+        request = RefreshAccessTokenRequest(**request.to_dict())
+        _context = self.endpoint.upstream_get("context")
+
+        request.verify(
+            keyjar=self.endpoint.upstream_get('sttribute', 'keyjar'),
+            opponent_id=client_id)
+
+        _mngr = _context.session_manager
+        try:
+            _session_info = _mngr.get_session_info_by_token(
+                request["refresh_token"], grant=True, handler_key="refresh_token"
+            )
+        except (KeyError, UnknownToken):
+            logger.error("Refresh token invalid")
+            return self.error_cls(error="invalid_grant", error_description="Invalid refresh token")
+
+        grant = _session_info["grant"]
+        token = grant.get_token(request["refresh_token"])
+
+        if not isinstance(token, RefreshToken):
+            return self.error_cls(error="invalid_request", error_description="Wrong token type")
+
+        if token.is_active() is False:
+            return self.error_cls(
+                error="invalid_request", error_description="Refresh token inactive"
+            )
+
+        if "scope" in request:
+            req_scopes = set(request["scope"])
+            scopes = set(grant.find_scope(token.based_on))
+            if not req_scopes.issubset(scopes):
+                return self.error_cls(
+                    error="invalid_request",
+                    error_description="Invalid refresh scopes",
+                )
 
-from idpyoidc.client.service import Service
-from idpyoidc.impexp import ImpExp
-from idpyoidc.util import qualified_name
-
-
-def specification_dump(info, exclude_attributes):
-    return {qualified_name(info.__class__): info.dump(exclude_attributes=exclude_attributes)}
-
-
-def specification_load(item: dict, **kwargs):
-    _class_name = list(item.keys())[0]  # there is only one
-    _cls = importer(_class_name)
-    _cls = _cls().load(item[_class_name])
-    return _cls
-
-
-class Specification(ImpExp):
-    parameter = {
-        "metadata": None,
-        "usage": None,
-        "behaviour": None,
-        "callback": None,
-        "_local": None
-    }
-
-    attributes = {
-        "redirect_uris": None,
-        "grant_types": ["authorization_code", "implicit", "refresh_token"],
-        "response_types": ["code"],
-        "client_name": None,
-        "client_uri": None,
-        "logo_uri": None,
-        "contacts": None,
-        "scope": None,
-        "tos_uri": None,
-        "policy_uri": None,
-        "jwks_uri": None,
-        "jwks": None,
-    }
-
-    rules = {
-        "jwks": None,
-        "jwks_uri": None,
-        "scope": ["openid"],
-        "verify_args": None,
-    }
-
-    callback_path = {
-        "requests": "req",
-        "code": "authz_cb",
-        "implicit": "authz_im_cb",
-    }
-
-    callback_uris = ["redirect_uris"]
-
-    def __init__(self,
-                 metadata: Optional[dict] = None,
-                 usage: Optional[dict] = None,
-                 behaviour: Optional[dict] = None
-                 ):
-
-        ImpExp.__init__(self)
-        if isinstance(metadata, dict):
-            self.metadata = {k: v for k, v in metadata.items() if k in self.attributes}
-        else:
-            self.metadata = {}
-
-        if isinstance(usage, dict):
-            self.usage = {k: v for k, v in usage.items() if k in self.rules}
-        else:
-            self.usage = {}
-
-        if isinstance(behaviour, dict):
-            self.behaviour = {k: v for k, v in behaviour.items() if k in self.attributes}
-        else:
-            self.behaviour = {}
-
-        self.callback = {}
-        self._local = {}
-
-    def get_all(self):
-        return self.metadata
-
-    def get_metadata(self, key, default=None):
-        if key in self.metadata:
-            return self.metadata[key]
-        else:
-            return default
-
-    def get_usage(self, key, default=None):
-        if key in self.usage:
-            return self.usage[key]
-        else:
-            return default
-
-    def set_metadata(self, key, value):
-        self.metadata[key] = value
-
-    def set_usage(self, key, value):
-        self.usage[key] = value
-
-    def _callback_uris(self, base_url, hex):
-        _red = {}
-        for type in self.get_metadata("response_types", ["code"]):
-            if "code" in type:
-                _red['code'] = True
-            elif type in ["id_token", "id_token token"]:
-                _red['implicit'] = True
-
-        if "form_post" in self.usage:
-            _red["form_post"] = True
-
-        callback_uri = {}
-        for key in _red.keys():
-            _uri = Service.get_uri(base_url, self.callback_path[key], hex)
-            callback_uri[key] = _uri
-        return callback_uri
-
-    def construct_redirect_uris(self, base_url, hex, callbacks):
-        if not callbacks:
-            callbacks = self._callback_uris(base_url, hex)
-
-        if callbacks:
-            self.set_metadata("redirect_uris", [v for k, v in callbacks.items()])
-
-        self.callback = callbacks
-
-    def verify_rules(self):
-        return True
-
-    def locals(self, info):
-        pass
-
-    def load_conf(self, info):
-        for attr, val in info.items():
-            if attr == "usage":
-                for k, v in val.items():
-                    if k in self.rules:
-                        self.set_usage(k, v)
-            elif attr == "metadata":
-                for k, v in val.items():
-                    if k in self.attributes:
-                        self.set_metadata(k, v)
-            elif attr == "behaviour":
-                self.behaviour = val
-            elif attr in self.attributes:
-                self.set_metadata(attr, val)
-            elif attr in self.rules:
-                self.set_usage(attr, val)
-
-        # defaults is nothing else is given
-        for key, val in self.attributes.items():
-            if val and key not in self.metadata:
-                self.set_metadata(key, val)
-
-        for key, val in self.rules.items():
-            if val and key not in self.usage:
-                self.set_usage(key, val)
-
-        self.locals(info)
-        self.verify_rules()
-
-    def bm_get(self, key, default=None):
-        if key in self.behaviour:
-            return self.behaviour[key]
-        elif key in self.metadata:
-            return self.metadata[key]
-
-        return default
-
-    def get(self, key, default=None):
-        if key in self._local:
-            return self._local[key]
-        else:
-            return default
-
-    def set(self, key, val):
-        self._local[key] = val
-
-    def construct_uris(self, *args):
-        pass
+        return request
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/client/util.py` & `idpyoidc-2.0.0/src/idpyoidc/client/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,25 +7,17 @@
 from urllib.parse import urlsplit
 from urllib.parse import urlunsplit
 
 from idpyoidc.constant import DEFAULT_POST_CONTENT_TYPE
 from idpyoidc.constant import JOSE_ENCODED
 from idpyoidc.constant import JSON_ENCODED
 from idpyoidc.constant import URL_ENCODED
+from idpyoidc.defaults import BASECHR
 from idpyoidc.exception import UnSupported
 from idpyoidc.util import importer
-
-# Since SystemRandom is not available on all systems
-try:
-    import SystemRandom as rnd
-except ImportError:
-    import random as rnd
-
-from idpyoidc.defaults import BASECHR
-
 from .exception import TimeFormatError
 from .exception import WrongContentType
 
 logger = logging.getLogger(__name__)
 
 __author__ = "roland"
 
@@ -264,17 +256,17 @@
     logger.debug("resp.headers: %s" % (sanitize(reqresp.headers),))
     logger.debug("resp.txt: %s" % (sanitize(reqresp.text),))
 
     _ctype = reqresp.headers.get("content-type")
     if not _ctype:
         # let's try to detect the format
         try:
-            content = reqresp.json()
+            reqresp.json()
             return "json"
-        except:
+        except Exception:
             return "urlencoded"  # reasonable default ??
 
     if match_to_("application/json", _ctype) or match_to_("application/jrd+json", _ctype):
         deser_method = "json"
     elif match_to_("application/jwt", _ctype):
         deser_method = "jwt"
     elif match_to_("application/jose", _ctype):
@@ -311,7 +303,25 @@
 
 
 def lower_or_upper(config, param, default=None):
     res = config.get(param.lower(), default)
     if not res:
         res = config.get(param.upper(), default)
     return res
+
+
+IMPLICIT_RESPONSE_TYPES = [
+    {'id_token'}, {'id_token', 'token'}, {'code', 'token'}, ['code', 'id_token'],
+    {'code', 'id_token', 'token'}, {'token'}
+]
+
+
+def implicit_response_types(a):
+    res = []
+    for typ in a:
+        if set(typ.split(' ')) in IMPLICIT_RESPONSE_TYPES:
+            res.append(typ)
+    return res
+
+
+def get_uri(base_url, path, hex):
+    return f"{base_url}/{path}/{hex}"
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/configure.py` & `idpyoidc-2.0.0/src/idpyoidc/configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         else:
             self.logger = logging.getLogger("client")
 
         self.web_conf = lower_or_upper(self.conf, "webserver")
 
         if entity_conf:
             skip = [ec["path"] for ec in entity_conf if "path" in ec]
-            check = [l[0] for l in skip]
+            check = [word[0] for word in skip]
 
             self.extend(
                 conf=self.conf,
                 base_path=base_path,
                 domain=self.domain,
                 port=self.port,
                 entity_conf=entity_conf,
@@ -294,15 +294,15 @@
     filename: str,
     base_path: Optional[str] = "",
     entity_conf: Optional[List[dict]] = None,
     file_attributes: Optional[List[str]] = None,
     domain: Optional[str] = "",
     port: Optional[int] = 0,
     dir_attributes: Optional[List[str]] = None,
-):
+) -> Base:
     return cls(
         load_config_file(filename),
         entity_conf=entity_conf,
         base_path=base_path,
         file_attributes=file_attributes,
         domain=domain,
         port=port,
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/converter.py` & `idpyoidc-2.0.0/src/idpyoidc/converter.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/encrypter.py` & `idpyoidc-2.0.0/src/idpyoidc/encrypter.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/exception.py` & `idpyoidc-2.0.0/src/idpyoidc/exception.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/impexp.py` & `idpyoidc-2.0.0/src/idpyoidc/impexp.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,26 +74,24 @@
 
         return info
 
     def local_load_adjustments(self, **kwargs):
         pass
 
     def load_attr(
-        self,
-        cls: Any,
-        item: dict,
-        init_args: Optional[dict] = None,
-        load_args: Optional[dict] = None,
+            self,
+            cls: Any,
+            item: dict,
+            init_args: Optional[dict] = None,
+            load_args: Optional[dict] = None,
     ) -> Any:
         if load_args:
             _kwargs = {"load_args": load_args}
-            _load_args = load_args
         else:
             _kwargs = {}
-            _load_args = {}
 
         if init_args:
             _kwargs["init_args"] = init_args
 
         if cls in [None, 0, "", [], {}, bool, b""]:
             if cls == b"":
                 val = as_bytes(item)
@@ -139,15 +137,19 @@
             _kwargs = {"load_args": load_args}
             _load_args = load_args
         else:
             _kwargs = {}
             _load_args = {}
 
         if init_args:
-            _kwargs["init_args"] = init_args
+            for attr, val in init_args.items():
+                if attr in self.init_args:
+                    setattr(self, attr, val)
+
+        _kwargs["init_args"] = init_args
 
         for attr, cls in self.parameter.items():
             if attr not in item or attr in self.special_load_dump:
                 continue
 
             setattr(self, attr, self.load_attr(cls, item[attr], **_kwargs))
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/item.py` & `idpyoidc-2.0.0/src/idpyoidc/item.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/logging.py` & `idpyoidc-2.0.0/src/idpyoidc/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Common logging functions"""
 import logging
 import os
 from logging.config import dictConfig
 from typing import Optional
 
-import yaml
-
 from idpyoidc.util import load_config_file
 
 LOGGING_CONF = "logging.yaml"
 
 LOGGING_DEFAULT = {
     "version": 1,
     "formatters": {"default": {"format": "%(asctime)s %(name)s %(levelname)s %(message)s"}},
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/message/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/message/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     def set_defaults(self):
         """
         Based on specification set a parameters value to the default value.
         """
         for key, val in self.c_default.items():
             self._dict.setdefault(key, val)
 
-    def to_urlencoded(self, lev=0):
+    def to_urlencoded(self):
         """
         Creates a string using the application/x-www-form-urlencoded format
 
         :return: A string of the application/x-www-form-urlencoded format
         """
 
         _spec = self.c_param
@@ -110,55 +110,54 @@
                 continue
 
             if isinstance(val, str):
                 # Should I allow parameters with "" as value ???
                 params.append((key, val.encode("utf-8")))
             elif isinstance(val, list):
                 if _ser:
-                    params.append((key, str(_ser(val, sformat="urlencoded", lev=lev))))
+                    params.append((key, str(_ser(val, sformat="urlencoded"))))
                 else:
                     for item in val:
                         params.append((key, str(item).encode("utf-8")))
             elif isinstance(val, Message):
                 try:
-                    _val = json.dumps(_ser(val, sformat="dict", lev=lev + 1))
+                    _val = json.dumps(_ser(val, sformat="dict"))
                     params.append((key, _val))
                 except TypeError:
                     params.append((key, val))
             elif val is None:
                 params.append((key, val))
             else:
                 try:
-                    params.append((key, _ser(val, lev=lev)))
+                    params.append((key, _ser(val)))
                 except Exception:
                     params.append((key, str(val)))
 
         try:
             return urlencode(params)
         except UnicodeEncodeError:
             _val = []
             for k, v in params:
                 try:
                     _val.append((k, v.encode("utf-8")))
                 except TypeError:
                     _val.append((k, v))
             return urlencode(_val)
 
-    def serialize(self, method="urlencoded", lev=0, **kwargs):
+    def serialize(self, method="urlencoded", **kwargs):
         """
         Convert this instance to another representation. Which representation
         is given by the choice of serialization method.
 
         :param method: A serialization method. Presently 'urlencoded', 'json',
             'jwt' and 'dict' is supported.
-        :param lev:
         :param kwargs: Extra key word arguments
         :return: THe content of this message serialized using a chosen method
         """
-        return getattr(self, "to_%s" % method)(lev=lev, **kwargs)
+        return getattr(self, "to_%s" % method)(**kwargs)
 
     def deserialize(self, info, method="urlencoded", **kwargs):
         """
         Convert from an external representation to an internal.
 
         :param info: The input
         :param method: The method used to deserialize the info
@@ -227,45 +226,44 @@
                     else:
                         self._dict[key] = val[0]
                 else:
                     raise TooManyValues("{}".format(key))
 
         return self
 
-    def to_dict(self, lev=0):
+    def to_dict(self):
         """
         Return a dictionary representation of the class
 
         :return: A dict
         """
 
         _spec = self.c_param
 
         _res = {}
-        lev += 1
         for key, val in self._dict.items():
             try:
                 _ser = _spec[str(key)][2]
             except KeyError:
                 try:
                     _key = key.split("#")[0]
                     _ser = _spec[_key][2]
                 except (ValueError, KeyError):
                     try:
                         _ser = _spec["*"][2]
                     except KeyError:
                         _ser = None
 
             if _ser:
-                val = _ser(val, "dict", lev)
+                val = _ser(val, "dict")
 
             if isinstance(val, Message):
-                _res[key] = val.to_dict(lev + 1)
+                _res[key] = val.to_dict()
             elif isinstance(val, list) and isinstance(next(iter(val or []), None), Message):
-                _res[key] = [v.to_dict(lev) for v in val]
+                _res[key] = [v.to_dict() for v in val]
             else:
                 _res[key] = val
 
         return _res
 
     def from_dict(self, dictionary, **kwargs):
         """
@@ -414,51 +412,46 @@
                         if isinstance(val, (dict, str)):
                             self._dict[skey] = val
                         else:
                             raise ValueError('"{}", wrong type of value for "{}"'.format(val, skey))
                     else:
                         raise ValueError('"{}", wrong type of value for "{}"'.format(val, skey))
 
-    def to_json(self, lev=0, indent=None):
+    def to_json(self, indent=None):
         """
         Serialize the content of this instance into a JSON string.
 
-        :param lev:
         :param indent: Number of spaces that should be used for indentation
         :return:
         """
-        if lev:
-            return self.to_dict(lev + 1)
-        else:
-            return json.dumps(self.to_dict(1), indent=indent)
+        return json.dumps(self.to_dict(), indent=indent)
 
     def from_json(self, txt, **kwargs):
         """
         Convert from a JSON string to an instance of this class.
 
         :param txt: The JSON string (a ``str``, ``bytes`` or ``bytearray``
             instance containing a JSON document)
         :param kwargs: extra keyword arguments
         :return: The instantiated instance
         """
         _dict = json.loads(txt)
         return self.from_dict(_dict)
 
-    def to_jwt(self, key=None, algorithm="", lev=0, lifetime=0):
+    def to_jwt(self, key=None, algorithm="", lifetime=0):
         """
         Create a signed JWT representation of the class instance
 
         :param key: The signing key
         :param algorithm: The signature algorithm to use
-        :param lev:
         :param lifetime: The lifetime of the JWS
         :return: A signed JWT
         """
 
-        _jws = JWS(self.to_json(lev), alg=algorithm)
+        _jws = JWS(self.to_json(), alg=algorithm)
         return _jws.sign_compact(key)
 
     def _gather_keys(self, keyjar, jwt, header, **kwargs):
         key = []
 
         if keyjar:
             _keys = keyjar.get_jwt_verify_keys(jwt, **kwargs)
@@ -676,14 +669,17 @@
         :param location: A URL
         :param fragment_enc: Whether the information should be placed in a
             fragment (True) or in a query part (False)
         :return: The extended URL
         """
         _l = as_unicode(location)
         _qp = as_unicode(self.to_urlencoded())
+        if not _qp:
+            return _l
+
         if fragment_enc:
             return "%s#%s" % (_l, _qp)
         else:
             if "?" in location:
                 return "%s&%s" % (_l, _qp)
             else:
                 return "%s?%s" % (_l, _qp)
@@ -759,29 +755,28 @@
             self._dict.update(item)
         elif isinstance(item, Message):
             for key, val in item.items():
                 self._dict[key] = val
         else:
             raise ValueError("Can't update message using: '%s'" % (item,))
 
-    def to_jwe(self, keys, enc, alg, lev=0):
+    def to_jwe(self, keys, enc, alg):
         """
         Place the information in this instance in a JSON object. Make that
         JSON object the body of a JWT. Then encrypt that JWT using the
         specified algorithms and the given keys. Return the encrypted JWT.
 
         :param keys: list or KeyJar instance
         :param enc: Content Encryption Algorithm
         :param alg: Key Management Algorithm
-        :param lev: Used for JSON construction
         :return: An encrypted JWT. If encryption failed an exception will be
             raised.
         """
 
-        _jwe = JWE(self.to_json(lev), alg=alg, enc=enc)
+        _jwe = JWE(self.to_json(), alg=alg, enc=enc)
         return _jwe.encrypt(keys)
 
     def from_jwe(self, msg, keys):
         """
         Decrypt an encrypted JWT and load the JSON object that was the body
         of the JWT into this object.
 
@@ -857,15 +852,15 @@
         if key not in msg1.c_param:
             msg1[key] = val
 
 
 # =============================================================================
 
 
-def list_serializer(vals, sformat="urlencoded", lev=0):
+def list_serializer(vals, sformat="urlencoded"):
     if isinstance(vals, str) and sformat == "dict":
         return [vals]
 
     if not isinstance(vals, list):
         raise ValueError("Expected list: %s" % vals)
 
     if sformat == "urlencoded":
@@ -883,15 +878,15 @@
     elif sformat == "dict":
         if isinstance(val, str):
             val = [val]
 
     return val
 
 
-def sp_sep_list_serializer(vals, sformat="urlencoded", lev=0):
+def sp_sep_list_serializer(vals, sformat="urlencoded"):
     if isinstance(vals, str):
         return vals
     else:
         return " ".join(vals)
 
 
 def sp_sep_list_deserializer(val, sformat="urlencoded"):
@@ -899,15 +894,15 @@
         return val.split(" ")
     elif isinstance(val, list) and len(val) == 1:
         return val[0].split(" ")
     else:
         return val
 
 
-def json_serializer(obj, sformat="urlencoded", lev=0):
+def json_serializer(obj, sformat="urlencoded"):
     return json.dumps(obj)
 
 
 def json_deserializer(txt, sformat="urlencoded"):
     return json.loads(txt)
 
 
@@ -917,51 +912,51 @@
     elif sformat in ["dict", "json"]:
         if not isinstance(val, str):
             val = json.dumps(val)
             sformat = "json"
     return Message().deserialize(val, sformat)
 
 
-def msg_ser(inst, sformat, lev=0):
+def msg_ser(inst, sformat):
     if sformat in ["urlencoded", "json"]:
         if isinstance(inst, dict):
             if sformat == "json":
                 res = json.dumps(inst)
             else:
                 res = urlencode([(k, v) for k, v in inst.items()])
         elif isinstance(inst, Message):
-            res = inst.serialize(sformat, lev)
+            res = inst.serialize(sformat)
         else:
             res = inst
     elif sformat == "dict":
         if isinstance(inst, Message):
-            res = inst.serialize(sformat, lev)
+            res = inst.serialize(sformat)
         elif isinstance(inst, dict):
             res = inst
         elif isinstance(inst, str):  # Iff ID Token
             res = inst
         else:
             raise MessageException("Wrong type: %s" % type(inst))
     else:
         raise OidcMsgError("Unknown sformat", inst)
 
     return res
 
 
-def msg_list_deser(val, sformat="urlencoded", lev=0):
+def msg_list_deser(val, sformat="urlencoded"):
     if isinstance(val, dict):
         return [Message(**val)]
 
     _res = []
     for v in val:
         _res.append(msg_deser(v, sformat))
     return _res
 
 
-def msg_list_ser(val, sformat="urlencoded", lev=0):
+def msg_list_ser(val, sformat="urlencoded"):
     _res = []
     for v in val:
         _res.append(msg_ser(v, sformat))
     return _res
 
 
 VTYPE = 0
@@ -1000,28 +995,28 @@
 
 OPTIONAL_MESSAGE = (Message, False, msg_ser, msg_deser, False)
 REQUIRED_MESSAGE = (Message, True, msg_ser, msg_deser, False)
 
 OPTIONAL_LIST_OF_MESSAGES = ([Message], False, msg_list_ser, msg_list_deser, False)
 
 
-def any_ser(val, sformat="urlencoded", lev=0):
+def any_ser(val, sformat="urlencoded"):
     if isinstance(val, (str, int, bool)):
         return val
     elif isinstance(val, Message):
-        return msg_ser(val, sformat, lev)
+        return msg_ser(val, sformat)
     elif isinstance(val, dict):
         return json.dumps(val)
     elif isinstance(val, list):
         return msg_list_ser(val)
     else:
         raise ValueError("Can't serialize this type of data")
 
 
-def any_deser(val, sformat="urlencoded", lev=0):
+def any_deser(val, sformat="urlencoded"):
     if isinstance(val, dict):
         return Message(**val)
     elif isinstance(val, list):
         return [msg_deser(v, sformat) for v in val]
     else:
         raise ValueError("Can't deserialize this type of data")
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/message/oauth2/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/message/oauth2/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import inspect
+import json
 import logging
 import string
 import sys
 
 from idpyoidc import verified_claim_name
+from idpyoidc.exception import FormatError
 from idpyoidc.exception import MissingAttribute
+from idpyoidc.exception import MissingRequiredAttribute
 from idpyoidc.exception import VerificationError
+from idpyoidc.message import Message
+from idpyoidc.message import msg_ser
 from idpyoidc.message import OPTIONAL_LIST_OF_SP_SEP_STRINGS
 from idpyoidc.message import OPTIONAL_LIST_OF_STRINGS
 from idpyoidc.message import REQUIRED_LIST_OF_SP_SEP_STRINGS
 from idpyoidc.message import REQUIRED_LIST_OF_STRINGS
 from idpyoidc.message import SINGLE_OPTIONAL_INT
 from idpyoidc.message import SINGLE_OPTIONAL_JSON
 from idpyoidc.message import SINGLE_OPTIONAL_STRING
 from idpyoidc.message import SINGLE_REQUIRED_BOOLEAN
 from idpyoidc.message import SINGLE_REQUIRED_INT
 from idpyoidc.message import SINGLE_REQUIRED_STRING
-from idpyoidc.message import Message
 
 logger = logging.getLogger(__name__)
 
 
 def is_error_message(msg):
     if "error" in msg:
         return True
@@ -41,15 +45,15 @@
         "error_description": SINGLE_OPTIONAL_STRING,
         "error_uri": SINGLE_OPTIONAL_STRING,
     }
 
     def verify(self, **kwargs):
         super(ResponseMessage, self).verify(**kwargs)
         if "error_description" in self:
-            # Verify that the characters used are within the allow ranges
+            # Verify that the characters used are within the allowed ranges
             # %x20-21 / %x23-5B / %x5D-7E
             if not all(x in error_chars for x in self["error_description"]):
                 raise ValueError("Characters outside allowed set")
         return True
 
 
 class AuthorizationErrorResponse(ResponseMessage):
@@ -104,25 +108,39 @@
         "client_id": SINGLE_OPTIONAL_STRING,
         "client_secret": SINGLE_OPTIONAL_STRING,
         "state": SINGLE_OPTIONAL_STRING,
     }
     c_default = {"grant_type": "authorization_code"}
 
 
+CLAIMS_WITH_VERIFIED = ["request"]
+
+
+def clear_verified_claims(msg):
+    for claim in CLAIMS_WITH_VERIFIED:
+        _vc_name = verified_claim_name(claim)
+        try:
+            del msg[_vc_name]
+        except KeyError:
+            pass
+    return msg
+
+
 class AuthorizationRequest(Message):
     """
     An authorization request
     """
 
     c_param = {
         "response_type": REQUIRED_LIST_OF_SP_SEP_STRINGS,
         "client_id": SINGLE_REQUIRED_STRING,
         "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS,
         "redirect_uri": SINGLE_OPTIONAL_STRING,
         "state": SINGLE_OPTIONAL_STRING,
+        "request": SINGLE_OPTIONAL_STRING,
     }
 
     def merge(self, request_object, treatement="strict", whitelist=None):
         """
         How to combine parameter that appear in the request with parameters that
         appear in the request object.
 
@@ -145,14 +163,60 @@
             params = list(self.keys())
             for param in params:
                 if param not in whitelist:
                     del self[param]
 
         self.update(request_object)
 
+    def verify(self, **kwargs):
+        """Authorization Request parameters that are OPTIONAL in the OAuth 2.0
+        specification MAY be included in the OpenID Request Object without also
+        passing them as OAuth 2.0 Authorization Request parameters, with one
+        exception: The scope parameter MUST always be present in OAuth 2.0
+        Authorization Request parameters.
+        All parameter values that are present both in the OAuth 2.0
+        Authorization Request and in the OpenID Request Object MUST exactly
+        match."""
+        super(AuthorizationRequest, self).verify(**kwargs)
+
+        clear_verified_claims(self)
+
+        args = {}
+        for arg in ["keyjar", "opponent_id", "sender", "alg", "encalg", "encenc"]:
+            try:
+                args[arg] = kwargs[arg]
+            except KeyError:
+                pass
+
+        if "opponent_id" not in kwargs:
+            args["opponent_id"] = self["client_id"]
+
+        if "request" in self:
+            if isinstance(self["request"], str):
+                # Try to decode the JWT, checks the signature
+                oidr = AuthorizationRequest().from_jwt(str(self["request"]), **args)
+
+                # check if something is change in the original message
+                for key, val in oidr.items():
+                    if key in self:
+                        if self[key] != val:
+                            # log but otherwise ignore
+                            logger.warning("{} != {}".format(self[key], val))
+
+                # remove all claims
+                _keys = list(self.keys())
+                for key in _keys:
+                    if key not in oidr:
+                        del self[key]
+
+                self.update(oidr)
+
+                # replace the JWT with the parsed and verified instance
+                self[verified_claim_name("request")] = oidr
+
 
 class AuthorizationResponse(ResponseMessage):
     """
     An authorization response.
     If *client_id* is returned in the response it will be checked against
     a client_id value provided when calling the verify method.
     The same with *iss* (issuer).
@@ -219,25 +283,34 @@
     """
 
     c_param = {
         "grant_type": SINGLE_REQUIRED_STRING,
         "username": SINGLE_OPTIONAL_STRING,
         "password": SINGLE_OPTIONAL_STRING,
         "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS,
+        "client_id": SINGLE_OPTIONAL_STRING,
+        "client_secret": SINGLE_OPTIONAL_STRING,
     }
 
 
 class CCAccessTokenRequest(Message):
     """
     Client Credential grant flow access token request
     """
 
-    c_param = {"grant_type": SINGLE_REQUIRED_STRING, "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS}
-    c_default = {"grant_type": "client_credentials"}
-    c_allowed_values = {"grant_type": ["client_credentials"]}
+    c_param = {
+        "client_id": SINGLE_OPTIONAL_STRING,
+        "client_secret": SINGLE_OPTIONAL_STRING,
+        "grant_type": SINGLE_REQUIRED_STRING,
+        "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS
+    }
+
+    def verify(self, **kwargs):
+        if self['grant_type'] != 'client_credentials':
+            raise ValueError('Grant type MUST be client_credentials')
 
 
 class RefreshAccessTokenRequest(Message):
     """
     Access token refresh request
     """
 
@@ -275,21 +348,96 @@
             "grant_types_supported": REQUIRED_LIST_OF_STRINGS,
             "token_endpoint_auth_methods_supported": OPTIONAL_LIST_OF_STRINGS,
             "token_endpoint_auth_signing_alg_values_supported": OPTIONAL_LIST_OF_STRINGS,
             "service_documentation": SINGLE_OPTIONAL_STRING,
             "ui_locales_supported": OPTIONAL_LIST_OF_STRINGS,
             "op_policy_uri": SINGLE_OPTIONAL_STRING,
             "op_tos_uri": SINGLE_OPTIONAL_STRING,
+            "code_challenge_methods_supported": OPTIONAL_LIST_OF_STRINGS,
             "revocation_endpoint": SINGLE_OPTIONAL_STRING,
             "introspection_endpoint": SINGLE_OPTIONAL_STRING,
         }
     )
     c_default = {"version": "3.0"}
 
 
+def deserialize_from_one_of(val, msgtype, sformat):
+    if sformat in ["dict", "json"]:
+        flist = ["json", "urlencoded"]
+        if not isinstance(val, str):
+            val = json.dumps(val)
+    else:
+        flist = ["urlencoded", "json"]
+
+    for _format in flist:
+        try:
+            return msgtype().deserialize(val, _format)
+        except FormatError:
+            pass
+    raise FormatError("Unexpected format")
+
+
+class OauthClientMetadata(Message):
+    """Metadata for an OAuth2 Client."""
+    c_param = {
+        "redirect_uris": OPTIONAL_LIST_OF_STRINGS,
+        "token_endpoint_auth_method": SINGLE_OPTIONAL_STRING,
+        "grant_type": OPTIONAL_LIST_OF_STRINGS,
+        "response_types": OPTIONAL_LIST_OF_STRINGS,
+        "client_name": SINGLE_OPTIONAL_STRING,
+        "client_uri": SINGLE_OPTIONAL_STRING,
+        "logo_uri": SINGLE_OPTIONAL_STRING,
+        "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS,
+        "contacts": OPTIONAL_LIST_OF_STRINGS,
+        "tos_uri": SINGLE_OPTIONAL_STRING,
+        "policy_uri": SINGLE_OPTIONAL_STRING,
+        "jwks_uri": SINGLE_OPTIONAL_STRING,
+        "jwks": SINGLE_OPTIONAL_JSON,
+        "software_id": SINGLE_OPTIONAL_STRING,
+        "software_version": SINGLE_OPTIONAL_STRING
+    }
+
+
+def oauth_client_metadata_deser(val, sformat="json"):
+    """Deserializes a JSON object (most likely) into a OauthClientMetadata."""
+    return deserialize_from_one_of(val, OauthClientMetadata, sformat)
+
+
+OPTIONAL_OAUTH_CLIENT_METADATA = (Message, False, msg_ser,
+                                  oauth_client_metadata_deser, False)
+
+
+class OauthClientInformationResponse(OauthClientMetadata):
+    """The information returned by a OAuth2 Server about an OAuth2 client."""
+    c_param = OauthClientMetadata.c_param.copy()
+    c_param.update({
+        "client_id": SINGLE_REQUIRED_STRING,
+        "client_secret": SINGLE_OPTIONAL_STRING,
+        "client_id_issued_at": SINGLE_OPTIONAL_INT,
+        "client_secret_expires_at": SINGLE_OPTIONAL_INT
+    })
+
+    def verify(self, **kwargs):
+        super(OauthClientInformationResponse, self).verify(**kwargs)
+
+        if "client_secret" in self:
+            if "client_secret_expires_at" not in self:
+                raise MissingRequiredAttribute(
+                    "client_secret_expires_at is a MUST if client_secret is present")
+
+
+def oauth_client_registration_response_deser(val, sformat="json"):
+    """Deserializes a JSON object (most likely) into a OauthClientInformationResponse."""
+    return deserialize_from_one_of(val, OauthClientInformationResponse, sformat)
+
+
+OPTIONAL_OAUTH_CLIENT_REGISTRATION_RESPONSE = (
+    Message, False, msg_ser, oauth_client_registration_response_deser, False)
+
+
 # RFC 7662
 class TokenIntrospectionRequest(Message):
     c_param = {
         "token": SINGLE_REQUIRED_STRING,
         "token_type_hint": SINGLE_OPTIONAL_STRING,
         # The ones below are part of authentication information
         "client_id": SINGLE_OPTIONAL_STRING,
@@ -401,14 +549,80 @@
         "exp": SINGLE_OPTIONAL_INT,
         "events": SINGLE_OPTIONAL_JSON,
         "txt": SINGLE_OPTIONAL_STRING,
         "toe": SINGLE_OPTIONAL_INT,
     }
 
 
+class JWTAccessToken(Message):
+    c_param = {
+        "iss": SINGLE_REQUIRED_STRING,
+        "exp": SINGLE_REQUIRED_INT,
+        "aud": REQUIRED_LIST_OF_STRINGS,
+        "sub": SINGLE_REQUIRED_STRING,
+        "client_id": SINGLE_REQUIRED_STRING,
+        "iat": SINGLE_REQUIRED_INT,
+        "jti": SINGLE_REQUIRED_STRING,
+        "auth_time": SINGLE_OPTIONAL_INT,
+        "acr": SINGLE_OPTIONAL_STRING,
+        "amr": OPTIONAL_LIST_OF_STRINGS,
+        'scope': OPTIONAL_LIST_OF_SP_SEP_STRINGS,
+        'groups': OPTIONAL_LIST_OF_STRINGS,
+        'roles': OPTIONAL_LIST_OF_STRINGS,
+        'entitlements': OPTIONAL_LIST_OF_STRINGS
+    }
+
+
+class JSONWebToken(Message):
+    # implements RFC 9068
+    c_param = {
+        'iss': SINGLE_REQUIRED_STRING,
+        'exp': SINGLE_REQUIRED_STRING,
+        'aud': SINGLE_REQUIRED_STRING,
+        'sub': SINGLE_REQUIRED_STRING,
+        "client_id": SINGLE_REQUIRED_STRING,
+        'iat': SINGLE_REQUIRED_STRING,
+        'jti': SINGLE_REQUIRED_STRING,
+        'auth_time': SINGLE_OPTIONAL_INT,
+        'acr': SINGLE_OPTIONAL_STRING,
+        'amr': OPTIONAL_LIST_OF_STRINGS,
+        'scope': OPTIONAL_LIST_OF_SP_SEP_STRINGS,
+        'groups': OPTIONAL_LIST_OF_STRINGS,
+        'roles': OPTIONAL_LIST_OF_STRINGS,
+        'entitlements': OPTIONAL_LIST_OF_STRINGS
+    }
+
+
+# RFC 7009
+class TokenRevocationRequest(Message):
+    c_param = {
+        "token": SINGLE_REQUIRED_STRING,
+        "token_type_hint": SINGLE_OPTIONAL_STRING,
+        # The ones below are part of authentication information
+        "client_id": SINGLE_OPTIONAL_STRING,
+        "client_secret": SINGLE_OPTIONAL_STRING,
+    }
+
+
+class TokenRevocationResponse(Message):
+    pass
+
+
+class TokenRevocationErrorResponse(ResponseMessage):
+    """
+    Error response from the revocation endpoint
+    """
+    c_allowed_values = ResponseMessage.c_allowed_values.copy()
+    c_allowed_values.update({
+        "error": [
+            "unsupported_token_type"
+        ]
+    })
+
+
 def factory(msgtype, **kwargs):
     """
     Factory method that can be used to easily instansiate a class instance
 
     :param msgtype: The name of the class
     :param kwargs: Keyword arguments
     :return: An instance of the class or None if the name doesn't match any
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/message/oauth2/device_authorization.py` & `idpyoidc-2.0.0/src/idpyoidc/message/oauth2/device_authorization.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/message/oidc/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/message/oidc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,19 @@
         try:
             return msgtype().deserialize(val, _format)
         except FormatError:
             pass
     raise FormatError("Unexpected format")
 
 
-def json_ser(val, sformat=None, lev=0):
+def json_ser(val, sformat=None):
     return json.dumps(val)
 
 
-def json_deser(val, sformat=None, lev=0):
+def json_deser(val, sformat=None):
     return json.loads(val)
 
 
 # value type, required, serializer, deserializer, null value allowed
 SINGLE_OPTIONAL_BOOLEAN = (bool, False, None, None, False)
 SINGLE_OPTIONAL_JSON_WN = (dict, False, json_ser, json_deser, True)
 # SINGLE_OPTIONAL_JSON_CONV = (dict, False, json_conv, json_rest, True)
@@ -104,61 +104,58 @@
     return deserialize_from_one_of(val, AddressClaim, sformat)
 
 
 def claims_deser(val, sformat="urlencoded"):
     return deserialize_from_one_of(val, Claims, sformat)
 
 
-def msg_ser_json(inst, sformat="json", lev=0):
+def msg_ser_json(inst, sformat="json"):
     # sformat = "json" always except when dict
-    if lev:
-        sformat = "dict"
+    # if lev:
+    #     sformat = "dict"
 
     if sformat == "dict":
         if isinstance(inst, Message):
-            res = inst.serialize(sformat, lev)
+            res = inst.serialize(sformat)
         elif isinstance(inst, dict):
             res = inst
         else:
             raise MessageException("Wrong type: %s" % type(inst))
     else:
         sformat = "json"
         if isinstance(inst, dict):
             res = json.dumps(inst)
         elif isinstance(inst, Message):
-            res = inst.serialize(sformat, lev)
+            res = inst.serialize(sformat)
         else:
             res = inst
 
     return res
 
 
-def msg_list_ser(insts, sformat, lev=0):
-    return [msg_ser(inst, sformat, lev) for inst in insts]
+def msg_list_ser(insts, sformat):
+    return [msg_ser(inst, sformat) for inst in insts]
 
 
-def claims_ser(val, sformat="urlencoded", lev=0):
+def claims_ser(val, sformat="urlencoded"):
     # everything in c_extension
     if isinstance(val, str):
         item = val
     elif isinstance(val, list):
         item = val[0]
     else:
         item = val
 
     if isinstance(item, Message):
-        return item.serialize(method=sformat, lev=lev + 1)
+        return item.serialize(method=sformat)
 
     if sformat == "urlencoded":
         res = urlencode(item)
     elif sformat == "json":
-        if lev:
-            res = item
-        else:
-            res = json.dumps(item)
+        res = json.dumps(item)
     elif sformat == "dict":
         if isinstance(item, dict):
             res = item
         else:
             raise MessageException("Wrong type: %s" % type(item))
     else:
         raise OidcMsgError("Unknown sformat: %s" % sformat, val)
@@ -287,15 +284,15 @@
     if not _jws:
         raise ValueError("{} not a signed JWT".format(claim))
 
     if _jws.jwt.headers["alg"] == "none":
         _signed = False
         _sign_alg = kwargs.get("sigalg")
         if _sign_alg == "none":
-            _allowed = True
+            pass
         else:  # There might or might not be a specified signing alg
             if kwargs.get("allow_sign_alg_none", False) is False:
                 logger.info("Signing algorithm None not allowed")
                 raise UnsupportedAlgorithm("Signing algorithm None not allowed")
     else:
         _signed = True
         if "allowed_sign_alg" in kwargs:
@@ -450,16 +447,14 @@
         exception: The scope parameter MUST always be present in OAuth 2.0
         Authorization Request parameters.
         All parameter values that are present both in the OAuth 2.0
         Authorization Request and in the OpenID Request Object MUST exactly
         match."""
         super(AuthorizationRequest, self).verify(**kwargs)
 
-        clear_verified_claims(self)
-
         args = {}
         for arg in ["keyjar", "opponent_id", "sender", "alg", "encalg", "encenc"]:
             try:
                 args[arg] = kwargs[arg]
             except KeyError:
                 pass
 
@@ -634,16 +629,16 @@
         # "client_secret": SINGLE_OPTIONAL_STRING,
         # "access_token": SINGLE_OPTIONAL_STRING,
         "post_logout_redirect_uri": SINGLE_OPTIONAL_STRING,
         "frontchannel_logout_uri": SINGLE_OPTIONAL_STRING,
         "frontchannel_logout_session_required": SINGLE_OPTIONAL_BOOLEAN,
         "backchannel_logout_uri": SINGLE_OPTIONAL_STRING,
         "backchannel_logout_session_required": SINGLE_OPTIONAL_BOOLEAN,
-        "federation_type": OPTIONAL_LIST_OF_STRINGS,
-        "organization_name": SINGLE_OPTIONAL_STRING,
+        # "federation_type": OPTIONAL_LIST_OF_STRINGS,
+        # "organization_name": SINGLE_OPTIONAL_STRING,
     }
     c_default = {"application_type": "web", "response_types": ["code"]}
     c_allowed_values = {
         "application_type": ["native", "web"],
         "subject_type": ["public", "pairwise"],
     }
 
@@ -767,17 +762,17 @@
         self.val_hash(alg)
 
         if "lifetime" in kwargs:
             self.pack_init(kwargs["lifetime"])
         else:
             self.pack_init()
 
-    def to_jwt(self, key=None, algorithm="", lev=0, lifetime=0):
+    def to_jwt(self, key=None, algorithm="", lifetime=0):
         self.pack(alg=algorithm, lifetime=lifetime)
-        return Message.to_jwt(self, key=key, algorithm=algorithm, lev=lev)
+        return Message.to_jwt(self, key=key, algorithm=algorithm)
 
     def verify(self, **kwargs):
         super(IdToken, self).verify(**kwargs)
 
         try:
             if kwargs["iss"] != self["iss"]:
                 raise IssuerMismatch("{} != {}".format(kwargs["iss"], self["iss"]))
@@ -899,28 +894,29 @@
             "op_policy_uri": SINGLE_OPTIONAL_STRING,
             "op_tos_uri": SINGLE_OPTIONAL_STRING,
             "check_session_iframe": SINGLE_OPTIONAL_STRING,
             "end_session_endpoint": SINGLE_OPTIONAL_STRING,
             "frontchannel_logout_supported": SINGLE_OPTIONAL_BOOLEAN,
             "frontchannel_logout_session_required": SINGLE_OPTIONAL_BOOLEAN,
             "backchannel_logout_supported": SINGLE_OPTIONAL_BOOLEAN,
-            "backchannel_logout_session_required": SINGLE_OPTIONAL_BOOLEAN
+            "backchannel_logout_session_required": SINGLE_OPTIONAL_BOOLEAN,
+            "code_challenge_methods_supported": OPTIONAL_LIST_OF_STRINGS,
             # "jwk_encryption_url": SINGLE_OPTIONAL_STRING,
             # "x509_url": SINGLE_REQUIRED_STRING,
             # "x509_encryption_url": SINGLE_OPTIONAL_STRING,
         }
     )
     c_default = {
         "version": "3.0",
         "token_endpoint_auth_methods_supported": ["client_secret_basic"],
         "claims_parameter_supported": False,
         "request_parameter_supported": False,
         "request_uri_parameter_supported": True,
         "require_request_uri_registration": True,
-        "grant_types_supported": ["authorization_code", "implicit"],
+        "grant_types_supported": ["authorization_code"],
     }
 
     def verify(self, **kwargs):
         super(ProviderConfigurationResponse, self).verify(**kwargs)
 
         if "scopes_supported" in self:
             if "openid" not in self["scopes_supported"]:
@@ -1086,41 +1082,41 @@
 def link_deser(val, sformat="urlencoded"):
     if isinstance(val, list):
         return [_l_deser(v, sformat) for v in val]
     else:
         return _l_deser(val, sformat)
 
 
-def link_ser(inst, sformat, lev=0):
+def link_ser(inst, sformat):
     if sformat in ["urlencoded", "json"]:
         if isinstance(inst, dict):
             if sformat == "json":
                 res = json.dumps(inst)
             else:
                 res = urlencode([(k, v) for k, v in inst.items()])
         elif isinstance(inst, Link):
-            res = inst.serialize(sformat, lev)
+            res = inst.serialize(sformat)
         else:
             res = inst
     elif sformat == "dict":
         if isinstance(inst, Link):
-            res = inst.serialize(sformat, lev)
+            res = inst.serialize(sformat)
         elif isinstance(inst, dict):
             res = inst
         elif isinstance(inst, str):  # Iff ID Token
             res = inst
         else:
             raise MessageException("Wrong type: %s" % type(inst))
     else:
         raise OidcMsgError("Unknown sformat", inst)
 
     return res
 
 
-def link_list_ser(inst, sformat, lev=0):
+def link_list_ser(inst, sformat):
     if isinstance(inst, list):
         return [link_ser(v, sformat) for v in inst]
     else:
         return link_ser(inst, sformat)
 
 
 REQUIRED_LINKS = ([Link], True, link_list_ser, link_deser, False)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/message/oidc/backchannel_authentication.py` & `idpyoidc-2.0.0/src/idpyoidc/message/oidc/backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/message/oidc/session.py` & `idpyoidc-2.0.0/src/idpyoidc/message/oidc/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import logging
 
 from cryptojwt.exception import UnsupportedAlgorithm
 
 from idpyoidc.exception import MessageException
 from idpyoidc.exception import NotForMe
+from idpyoidc.message import Message
 from idpyoidc.message import OPTIONAL_LIST_OF_SP_SEP_STRINGS
 from idpyoidc.message import REQUIRED_LIST_OF_STRINGS
 from idpyoidc.message import SINGLE_OPTIONAL_STRING
 from idpyoidc.message import SINGLE_REQUIRED_INT
 from idpyoidc.message import SINGLE_REQUIRED_JSON
 from idpyoidc.message import SINGLE_REQUIRED_STRING
-from idpyoidc.message import Message
 from idpyoidc.time_util import utc_time_sans_frac
-
 from ..oauth2 import ResponseMessage
+from ..oidc import clear_verified_claims
 from ..oidc import ID_TOKEN_VERIFY_ARGS
-from ..oidc import SINGLE_OPTIONAL_IDTOKEN
 from ..oidc import IdToken
 from ..oidc import MessageWithIdToken
-from ..oidc import clear_verified_claims
+from ..oidc import SINGLE_OPTIONAL_IDTOKEN
 from ..oidc import verified_claim_name
 from ..oidc import verify_id_token
 
 logger = logging.getLogger(__name__)
 
 
 class RefreshSessionRequest(MessageWithIdToken):
@@ -132,21 +131,16 @@
         _now = utc_time_sans_frac()
 
         try:
             _skew = kwargs["skew"]
         except KeyError:
             _skew = 0
 
-        try:
-            _exp = self["iat"]
-        except KeyError:
-            pass
-        else:
-            if self["iat"] > (_now + _skew):
-                raise ValueError("Invalid issued_at time")
+        if 'iat' in self and self["iat"] > (_now + _skew):
+            raise ValueError("Invalid issued_at time")
 
         _allowed = kwargs.get("allowed_sign_alg")
         if _allowed and self.jws_header["alg"] != _allowed:
             _msg = "Wrong token signing algorithm, {} != {}".format(
                 self.jws_header["alg"], kwargs["allowed_sign_alg"]
             )
             raise UnsupportedAlgorithm(_msg)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/authn_event.py` & `idpyoidc-2.0.0/src/idpyoidc/server/authn_event.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/authz/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/server/authz/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 
 logger = logging.getLogger(__name__)
 
 
 class AuthzHandling(object):
     """Class that allow an entity to manage authorization"""
 
-    def __init__(self, server_get, grant_config=None, **kwargs):
-        self.server_get = server_get
+    def __init__(self, upstream_get, grant_config=None, **kwargs):
+        self.upstream_get = upstream_get
         self.grant_config = grant_config or {}
         self.kwargs = kwargs
 
     def usage_rules(self, client_id: Optional[str] = ""):
         if "usage_rules" in self.grant_config:
             _usage_rules = copy.deepcopy(self.grant_config["usage_rules"])
         else:
             _usage_rules = {}
 
         if not client_id:
             return _usage_rules
 
         try:
-            _per_client = self.server_get("endpoint_context").cdb[client_id]["token_usage_rules"]
+            _per_client = self.upstream_get("context").cdb[client_id]["token_usage_rules"]
         except KeyError:
             pass
         else:
             if _usage_rules:
                 for _token_type, _rule in _usage_rules.items():
                     _pc = _per_client.get(_token_type)
                     if _pc:
@@ -57,69 +57,75 @@
 
     def __call__(
         self,
         session_id: str,
         request: Union[dict, Message],
         resources: Optional[list] = None,
     ) -> Grant:
-        session_info = self.server_get("endpoint_context").session_manager.get_session_info(
+        _context = self.upstream_get("context")
+        session_info = _context.session_manager.get_session_info(
             session_id=session_id, grant=True
         )
         grant = session_info["grant"]
+        _client_id = session_info['client_id']
 
         args = self.grant_config.copy()
 
         for key, val in args.items():
             if key == "expires_in":
                 grant.set_expires_at(val)
             elif key == "usage_rules":
-                setattr(grant, key, self.usage_rules(request.get("client_id")))
+                setattr(grant, key, self.usage_rules(_client_id))
             else:
                 setattr(grant, key, val)
 
         if resources is None:
-            grant.resources = [session_info["client_id"]]
+            grant.resources = [_client_id]
         else:
             grant.resources = resources
 
-        # After this is where user consent should be handled
+        # Scope handling. If allowed scopes are defined for the client filter using that
         scopes = grant.scope
         if not scopes:
             scopes = request.get("scope", [])
-            grant.scope = scopes
-        grant.claims = self.server_get("endpoint_context").claims_interface.get_claims_all_usage(
+        else:
+            scopes = _context.scopes_handler.filter_scopes(scopes, client_id=_client_id)
+        grant.scope = scopes
+
+        # After this is where user consent should be handled
+        grant.claims = self.upstream_get("context").claims_interface.get_claims_all_usage(
             session_id=session_id, scopes=scopes
         )
 
         return grant
 
 
 class Implicit(AuthzHandling):
     def __call__(
         self,
         session_id: str,
         request: Union[dict, Message],
         resources: Optional[list] = None,
     ) -> Grant:
         args = self.grant_config.copy()
-        grant = self.server_get("endpoint_context").session_manager.get_grant(session_id=session_id)
+        grant = self.upstream_get("context").session_manager.get_grant(session_id=session_id)
         for arg, val in args:
             setattr(grant, arg, val)
         return grant
 
 
-def factory(msgtype, server_get, **kwargs):
+def factory(msgtype, upstream_get, **kwargs):
     """
     Factory method that can be used to easily instantiate a class instance
 
     :param msgtype: The name of the class
     :param kwargs: Keyword arguments
     :return: An instance of the class or None if the name doesn't match any
         known class.
     """
     for name, obj in inspect.getmembers(sys.modules[__name__]):
         if inspect.isclass(obj) and issubclass(obj, AuthzHandling):
             try:
                 if obj.__name__ == msgtype:
-                    return obj(server_get, **kwargs)
+                    return obj(upstream_get, **kwargs)
             except AttributeError:
                 pass
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/client_authn.py` & `idpyoidc-2.0.0/src/idpyoidc/server/client_authn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,90 @@
 import base64
 import logging
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Union
-from urllib.parse import unquote_plus
 
 from cryptojwt.exception import BadSignature
 from cryptojwt.exception import Invalid
 from cryptojwt.exception import MissingKey
 from cryptojwt.jwt import JWT
 from cryptojwt.jwt import utc_time_sans_frac
 from cryptojwt.utils import as_bytes
 from cryptojwt.utils import as_unicode
 
 from idpyoidc.message import Message
 from idpyoidc.message.oidc import JsonWebToken
 from idpyoidc.message.oidc import verified_claim_name
 from idpyoidc.server.constant import JWT_BEARER
-from idpyoidc.server.endpoint_context import EndpointContext
 from idpyoidc.server.exception import BearerTokenAuthenticationError
 from idpyoidc.server.exception import ClientAuthenticationError
 from idpyoidc.server.exception import InvalidClient
 from idpyoidc.server.exception import InvalidToken
 from idpyoidc.server.exception import ToOld
-from idpyoidc.server.exception import UnAuthorizedClient
 from idpyoidc.server.exception import UnknownClient
 from idpyoidc.util import importer
 from idpyoidc.util import sanitize
 
 logger = logging.getLogger(__name__)
 
 __author__ = "roland hedberg"
 
 
 class ClientAuthnMethod(object):
     tag = None
 
-    def __init__(self, server_get):
+    def __init__(self, upstream_get):
         """
-        :param server_get: A method that can be used to get general server information.
+        :param upstream_get: A method that can be used to get general server information.
         """
-        self.server_get = server_get
+        self.upstream_get = upstream_get
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            **kwargs,
     ):
         """
         Verify authentication information in a request
         :param kwargs:
         :return:
         """
         raise NotImplementedError()
 
     def verify(
-        self,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        get_client_id_from_token: Optional[Callable] = None,
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            get_client_id_from_token: Optional[Callable] = None,
+            **kwargs,
     ):
         """
         Verify authentication information in a request
         :param kwargs:
         :return:
         """
         res = self._verify(
-            self.server_get("endpoint_context"),
             request=request,
             authorization_token=authorization_token,
             endpoint=endpoint,
             get_client_id_from_token=get_client_id_from_token,
             **kwargs,
         )
         res["method"] = self.tag
         return res
 
     def is_usable(
-        self,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
     ):
         """
         Verify that this authentication method is applicable.
 
         :param request: The request
         :param authorization_token: The authorization token
         :return: True/False
@@ -118,20 +113,19 @@
 
     tag = "none"
 
     def is_usable(self, request=None, authorization_token=None):
         return request is not None
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            **kwargs,
     ):
         return {"client_id": request.get("client_id")}
 
 
 class PublicAuthn(ClientAuthnMethod):
     """
     Used for public clients, that don't require any form of authentication other
@@ -140,20 +134,19 @@
 
     tag = "public"
 
     def is_usable(self, request=None, authorization_token=None):
         return request and "client_id" in request
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            **kwargs,
     ):
         return {"client_id": request["client_id"]}
 
 
 class ClientSecretBasic(ClientAuthnMethod):
     """
     Clients that have received a client_secret value from the Authorization
@@ -165,24 +158,23 @@
 
     def is_usable(self, request=None, authorization_token=None):
         if authorization_token is not None and authorization_token.startswith("Basic "):
             return True
         return False
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            **kwargs,
     ):
         client_info = basic_authn(authorization_token)
-
-        if endpoint_context.cdb[client_info["id"]]["client_secret"] == client_info["secret"]:
+        _context = self.upstream_get('context')
+        if _context.cdb[client_info["id"]]["client_secret"] == client_info["secret"]:
             return {"client_id": client_info["id"]}
         else:
             raise ClientAuthenticationError()
 
 
 class ClientSecretPost(ClientSecretBasic):
     """
@@ -198,22 +190,22 @@
         if request is None:
             return False
         if "client_id" in request and "client_secret" in request:
             return True
         return False
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            **kwargs,
     ):
-        if endpoint_context.cdb[request["client_id"]]["client_secret"] == request["client_secret"]:
+        _context = self.upstream_get('context')
+        if _context.cdb[request["client_id"]]["client_secret"] == request["client_secret"]:
             return {"client_id": request["client_id"]}
         else:
             raise ClientAuthenticationError("secrets doesn't match")
 
 
 class BearerHeader(ClientSecretBasic):
     """"""
@@ -222,25 +214,25 @@
 
     def is_usable(self, request=None, authorization_token=None):
         if authorization_token is not None and authorization_token.startswith("Bearer "):
             return True
         return False
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        get_client_id_from_token: Optional[Callable] = None,
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            get_client_id_from_token: Optional[Callable] = None,
+            **kwargs,
     ):
         token = authorization_token.split(" ", 1)[1]
+        _context = self.upstream_get('context')
         try:
-            client_id = get_client_id_from_token(endpoint_context, token, request)
+            client_id = get_client_id_from_token(_context, token, request)
         except ToOld:
             raise BearerTokenAuthenticationError("Expired token")
         except KeyError:
             raise BearerTokenAuthenticationError("Unknown token")
         return {"token": token, "client_id": client_id}
 
 
@@ -253,92 +245,95 @@
 
     def is_usable(self, request=None, authorization_token=None):
         if request is not None and "access_token" in request:
             return True
         return False
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            get_client_id_from_token: Optional[Callable] = None,
+            **kwargs,
     ):
         _token = request.get("access_token")
         if _token is None:
             raise ClientAuthenticationError("No access token")
 
         res = {"token": _token}
-        _client_id = request.get("client_id")
+        _context = self.upstream_get('context')
+        _client_id = get_client_id_from_token(_context, _token, request)
         if _client_id:
             res["client_id"] = _client_id
         return res
 
 
 class JWSAuthnMethod(ClientAuthnMethod):
+
     def is_usable(self, request=None, authorization_token=None):
         if request is None:
             return False
         if "client_assertion" in request:
             return True
         return False
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        key_type: Optional[str] = None,
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            key_type: Optional[str] = None,
+            **kwargs,
     ):
-        _jwt = JWT(endpoint_context.keyjar, msg_cls=JsonWebToken)
+        _context = self.upstream_get('context')
+        _keyjar = self.upstream_get('attribute', 'keyjar')
+        _jwt = JWT(_keyjar, msg_cls=JsonWebToken)
         try:
             ca_jwt = _jwt.unpack(request["client_assertion"])
         except (Invalid, MissingKey, BadSignature) as err:
             logger.info("%s" % sanitize(err))
             raise ClientAuthenticationError("Could not verify client_assertion.")
 
         _sign_alg = ca_jwt.jws_header.get("alg")
         if _sign_alg and _sign_alg.startswith("HS"):
             if key_type == "private_key":
                 raise AttributeError("Wrong key type")
-            keys = endpoint_context.keyjar.get(
+            keys = _keyjar.get(
                 "sig", "oct", ca_jwt["iss"], ca_jwt.jws_header.get("kid")
             )
-            _secret = endpoint_context.cdb[ca_jwt["iss"]].get("client_secret")
+            _secret = _context.cdb[ca_jwt["iss"]].get("client_secret")
             if _secret and keys[0].key != as_bytes(_secret):
                 raise AttributeError("Oct key used for signing not client_secret")
         else:
             if key_type == "client_secret":
                 raise AttributeError("Wrong key type")
 
         authtoken = sanitize(ca_jwt.to_dict())
         logger.debug("authntoken: {}".format(authtoken))
 
         if endpoint is None or not endpoint:
-            if endpoint_context.issuer in ca_jwt["aud"]:
+            if _context.issuer in ca_jwt["aud"]:
                 pass
             else:
                 raise InvalidToken("Not for me!")
         else:
             if set(ca_jwt["aud"]).intersection(endpoint.allowed_target_uris()):
                 pass
             else:
                 raise InvalidToken("Not for me!")
 
         # If there is a jti use it to make sure one-time usage is true
         _jti = ca_jwt.get("jti")
         if _jti:
             _key = "{}:{}".format(ca_jwt["iss"], _jti)
-            if _key in endpoint_context.jti_db:
+            if _key in _context.jti_db:
                 raise InvalidToken("Have seen this token once before")
             else:
-                endpoint_context.jti_db[_key] = utc_time_sans_frac()
+                _context.jti_db[_key] = utc_time_sans_frac()
 
         request[verified_claim_name("client_assertion")] = ca_jwt
         client_id = kwargs.get("client_id") or ca_jwt["iss"]
 
         return {"client_id": client_id, "jwt": ca_jwt}
 
 
@@ -349,45 +344,42 @@
     The HMAC (Hash-based Message Authentication Code) is calculated using the
     bytes of the UTF-8 representation of the client_secret as the shared key.
     """
 
     tag = "client_secret_jwt"
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            **kwargs,
     ):
         res = super()._verify(
-            endpoint_context, request=request, key_type="client_secret", endpoint=endpoint, **kwargs
+            request=request, key_type="client_secret", endpoint=endpoint, **kwargs
         )
         # Verify that a HS alg was used
         return res
 
 
 class PrivateKeyJWT(JWSAuthnMethod):
     """
     Clients that have registered a public key sign a JWT using that key.
     """
 
     tag = "private_key_jwt"
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            **kwargs,
     ):
         res = super()._verify(
-            endpoint_context,
             request=request,
             authorization_token=authorization_token,
             endpoint=endpoint,
             **kwargs,
             key_type="private_key",
         )
         # Verify that an RS or ES alg was used ?
@@ -398,36 +390,36 @@
     tag = "request_param"
 
     def is_usable(self, request=None, authorization_token=None):
         if request and "request" in request:
             return True
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        **kwargs,
+            self,
+            request: Optional[Union[dict, Message]] = None,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            **kwargs,
     ):
-        _jwt = JWT(endpoint_context.keyjar, msg_cls=JsonWebToken)
+        _context = self.upstream_get('context')
+        _jwt = JWT(self.upstream_get('attribute', 'keyjar'), msg_cls=JsonWebToken)
         try:
             _jwt = _jwt.unpack(request["request"])
         except (Invalid, MissingKey, BadSignature) as err:
             logger.info("%s" % sanitize(err))
             raise ClientAuthenticationError("Could not verify client_assertion.")
 
         # If there is a jti use it to make sure one-time usage is true
         _jti = _jwt.get("jti")
         if _jti:
             _key = "{}:{}".format(_jwt["iss"], _jti)
-            if _key in endpoint_context.jti_db:
+            if _key in _context.jti_db:
                 raise InvalidToken("Have seen this token once before")
             else:
-                endpoint_context.jti_db[_key] = utc_time_sans_frac()
+                _context.jti_db[_key] = utc_time_sans_frac()
 
         request[verified_claim_name("client_assertion")] = _jwt
         client_id = kwargs.get("client_id") or _jwt["iss"]
 
         return {"client_id": client_id, "jwt": _jwt}
 
 
@@ -450,27 +442,26 @@
     eta = cinfo.get("client_secret_expires_at", 0)
     if eta != 0 and eta < utc_time_sans_frac():
         return False
     return True
 
 
 def verify_client(
-    endpoint_context: EndpointContext,
-    request: Union[dict, Message],
-    http_info: Optional[dict] = None,
-    get_client_id_from_token: Optional[Callable] = None,
-    endpoint=None,  # Optional[Endpoint]
-    also_known_as: Optional[Dict[str, str]] = None,
-):
+        request: Union[dict, Message],
+        http_info: Optional[dict] = None,
+        get_client_id_from_token: Optional[Callable] = None,
+        endpoint=None,  # Optional[Endpoint]
+        also_known_as: Optional[Dict[str, str]] = None,
+) -> dict:
     """
     Initiated Guessing !
 
     :param also_known_as:
     :param endpoint: Endpoint instance
-    :param endpoint_context: EndpointContext instance
+    :param context: EndpointContext instance
     :param request: The request
     :param http_info: Client authentication information
     :param get_client_id_from_token: Function that based on a token returns a client id.
     :return: dictionary containing client id, client authentication method and
         possibly access token.
     """
 
@@ -478,88 +469,94 @@
         authorization_token = http_info["headers"].get("authorization")
         if not authorization_token:
             authorization_token = http_info["headers"].get("Authorization")
     else:
         authorization_token = None
 
     auth_info = {}
-    methods = endpoint_context.client_authn_method
+    _context = endpoint.upstream_get('context')
+    methods = _context.client_authn_methods
+    client_id = None
     allowed_methods = getattr(endpoint, "client_authn_method")
     if not allowed_methods:
-        allowed_methods = list(methods.keys())
+        allowed_methods = list(methods.keys())  # If not specific for this endpoint then all
 
     _method = None
     for _method in (methods[meth] for meth in allowed_methods):
         if not _method.is_usable(request=request, authorization_token=authorization_token):
             continue
         try:
             logger.info(f"Verifying client authentication using {_method.tag}")
             auth_info = _method.verify(
+                keyjar=endpoint.upstream_get('attribute', 'keyjar'),
                 request=request,
                 authorization_token=authorization_token,
                 endpoint=endpoint,
                 get_client_id_from_token=get_client_id_from_token,
             )
-            break
         except (BearerTokenAuthenticationError, ClientAuthenticationError):
             raise
         except Exception as err:
             logger.info("Verifying auth using {} failed: {}".format(_method.tag, err))
+            continue
 
-    if auth_info.get("method") == "none":
-        return auth_info
+        if auth_info.get("method") == "none" and auth_info.get("client_id") is None:
+            break
 
-    client_id = auth_info.get("client_id")
-    if client_id is None:
-        raise ClientAuthenticationError("Failed to verify client")
-
-    if also_known_as:
-        client_id = also_known_as[client_id]
-        auth_info["client_id"] = client_id
-
-    if client_id not in endpoint_context.cdb:
-        raise UnknownClient("Unknown Client ID")
-
-    _cinfo = endpoint_context.cdb[client_id]
-
-    if not valid_client_info(_cinfo):
-        logger.warning("Client registration has timed out or " "client secret is expired.")
-        raise InvalidClient("Not valid client")
-
-    # Validate that the used method is allowed for this client/endpoint
-    client_allowed_methods = _cinfo.get(
-        f"{endpoint.endpoint_name}_client_authn_method", _cinfo.get("client_authn_method")
-    )
-    if client_allowed_methods is not None and _method and _method.tag not in client_allowed_methods:
-        logger.info(
-            f"Allowed methods for client: {client_id} at endpoint: {endpoint.name} are: "
-            f"`{', '.join(client_allowed_methods)}`"
-        )
-        raise UnAuthorizedClient(
-            f"Authentication method: {_method.tag} not allowed for client: {client_id} in "
-            f"endpoint: {endpoint.name}"
+        client_id = auth_info.get("client_id")
+        if client_id is None:
+            raise ClientAuthenticationError("Failed to verify client")
+
+        if also_known_as:
+            client_id = also_known_as[client_id]
+            auth_info["client_id"] = client_id
+
+        if client_id not in _context.cdb:
+            raise UnknownClient("Unknown Client ID")
+
+        _cinfo = _context.cdb[client_id]
+
+        if not valid_client_info(_cinfo):
+            logger.warning("Client registration has timed out or " "client secret is expired.")
+            raise InvalidClient("Not valid client")
+
+        # Validate that the used method is allowed for this client/endpoint
+        client_allowed_methods = _cinfo.get(
+            f"{endpoint.endpoint_name}_client_authn_method", _cinfo.get("client_authn_method")
         )
+        if client_allowed_methods is not None and auth_info["method"] not in client_allowed_methods:
+            logger.info(
+                f"Allowed methods for client: {client_id} at endpoint: {endpoint.name} are: "
+                f"`{', '.join(client_allowed_methods)}`"
+            )
+            auth_info = {}
+            continue
+        break
 
     # store what authn method was used
-    if auth_info.get("method"):
+    if "method" in auth_info and client_id:
         _request_type = request.__class__.__name__
         _used_authn_method = _cinfo.get("auth_method")
         if _used_authn_method:
-            endpoint_context.cdb[client_id]["auth_method"][_request_type] = auth_info["method"]
+            _context.cdb[client_id]["auth_method"][_request_type] = auth_info["method"]
         else:
-            endpoint_context.cdb[client_id]["auth_method"] = {_request_type: auth_info["method"]}
+            _context.cdb[client_id]["auth_method"] = {_request_type: auth_info["method"]}
 
     return auth_info
 
 
-def client_auth_setup(server_get, auth_set=None):
+def client_auth_setup(upstream_get, auth_set=None):
     if auth_set is None:
         auth_set = CLIENT_AUTHN_METHOD
     else:
         auth_set.update(CLIENT_AUTHN_METHOD)
     res = {}
 
     for name, cls in auth_set.items():
         if isinstance(cls, str):
             cls = importer(cls)
-        res[name] = cls(server_get)
+        res[name] = cls(upstream_get)
     return res
+
+
+def get_client_authn_methods():
+    return list(CLIENT_AUTHN_METHOD.keys())
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/client_configure.py` & `idpyoidc-2.0.0/src/idpyoidc/server/client_configure.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,20 +31,14 @@
             # "registration_access_token": SINGLE_OPTIONAL_STRING
             # "auth_method": SINGLE_OPTIONAL_DICT,
         }
     )
 
     def verify(self, **kwargs):
         RegistrationResponse.verify(self, **kwargs)
-        _server_get = kwargs.get("server_get")
-        if _server_get:
-            _endpoint_context = _server_get("endpoint_context")
-        else:
-            _endpoint_context = None
-
         if "add_claims" in self:
             if not set(self["add_claims"].keys()).issubset({"always", "by_scope"}):
                 _diff = set(self["add_claims"].keys()).difference({"always", "by_scope"})
                 logger.warning(f"Undefined add_claims parameter '{_diff}' used")
 
         if "token_usage_rules" in self:
             for _typ, _rule in self["token_usage_rules"].items():
@@ -65,18 +59,18 @@
                         logger.warning(f"Unknown supports_minting token '{_diff}' used")
 
         if "token_exchange" in self:
             pass
 
 
 def verify_oidc_client_information(
-    conf: dict, server_get: Optional[Callable] = None, **kwargs
+    conf: dict, upstream_get: Optional[Callable] = None, **kwargs
 ) -> dict:
     res = {}
     for key, item in conf.items():
         _rr = ClientConfiguration(**item)
-        _rr.verify(server_get=server_get, **kwargs)
+        _rr.verify(upstream_get=upstream_get, **kwargs)
         if _rr.extra():
             logger.info(f"Extras: {_rr.extra()}")
         res[key] = _rr
 
     return res
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/configure.py` & `idpyoidc-2.0.0/src/idpyoidc/server/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 """Configuration management for OP"""
 import copy
 import logging
 import os
+from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from idpyoidc.configure import Base
 from idpyoidc.server.client_configure import verify_oidc_client_information
 from idpyoidc.server.scopes import SCOPE2CLAIMS
 
 logger = logging.getLogger(__name__)
 
 OP_DEFAULT_CONFIG = {
-    "capabilities": {
+    "preference": {
         "subject_types_supported": ["public", "pairwise"],
-        "grant_types_supported": [
-            "authorization_code",
-            "implicit",
-            "urn:ietf:params:oauth:grant-type:jwt-bearer",
-            "refresh_token",
-        ],
     },
     "cookie_handler": {
         "class": "idpyoidc.server.cookie_handler.CookieHandler",
         "kwargs": {
             "encrypter": {
                 "kwargs": {
                     "keys": {
@@ -152,29 +147,32 @@
         "client_db": None,
         "client_authn_methods": {},
         "cookie_handler": None,
         "endpoint": {},
         "httpc_params": {},
         "issuer": "",
         "key_conf": None,
+        'preference': {},
         "session_params": None,
         "template_dir": None,
         "token_handler_args": {},
         "userinfo": None,
+        "scopes_handler": None
     }
 
     def __init__(
         self,
         conf: Dict,
         base_path: Optional[str] = "",
         entity_conf: Optional[List[dict]] = None,
         domain: Optional[str] = "",
         port: Optional[int] = 0,
         file_attributes: Optional[List[str]] = None,
         dir_attributes: Optional[List[str]] = None,
+        upstream_get: Optional[Callable] = None
     ):
 
         conf = copy.deepcopy(conf)
         Base.__init__(
             self,
             conf,
             base_path,
@@ -338,23 +336,26 @@
                 "page_header": "Testing log in",
                 "submit_btn": "Get me in!",
                 "user_label": "Nickname",
                 "passwd_label": "Secret sauce",
             },
         }
     },
-    "capabilities": {
+    "preference": {
         "subject_types_supported": ["public", "pairwise"],
         "grant_types_supported": [
             "authorization_code",
-            "implicit",
+            # "implicit",
             "urn:ietf:params:oauth:grant-type:jwt-bearer",
             "refresh_token",
         ],
     },
+    "scopes_handler": {
+        "class": "idpyoidc.server.scopes.Scopes"
+    },
     "claims_interface": {"class": "idpyoidc.server.session.claims.ClaimsInterface", "kwargs": {}},
     "cookie_handler": {
         "class": "idpyoidc.server.cookie_handler.CookieHandler",
         "kwargs": {
             "encrypter": {
                 "kwargs": {
                     "keys": {
@@ -457,15 +458,15 @@
                 "backchannel_logout_session_required": True,
                 "check_session_iframe": "check_session_iframe",
             },
         },
     },
     "httpc_params": {"verify": False, "timeout": 4},
     "issuer": "https://{domain}:{port}",
-    "keys": {
+    "key_conf": {
         "private_path": "private/jwks.json",
         "key_defs": [
             {"type": "RSA", "use": ["sig"]},
             {"type": "EC", "crv": "P-256", "use": ["sig"]},
         ],
         "public_path": "static/jwks.json",
         "read_only": False,
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/construct.py` & `idpyoidc-2.0.0/src/idpyoidc/server/construct.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/cookie_handler.py` & `idpyoidc-2.0.0/src/idpyoidc/server/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/endpoint.py` & `idpyoidc-2.0.0/src/idpyoidc/server/endpoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import json
 import logging
 from typing import Callable
 from typing import Optional
 from typing import Union
 from urllib.parse import urlparse
 
+from cryptojwt.exception import IssuerNotFound
+
 from idpyoidc.exception import MissingRequiredAttribute
 from idpyoidc.exception import MissingRequiredValue
 from idpyoidc.exception import ParameterError
 from idpyoidc.message import Message
 from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.message.oidc import RegistrationRequest
+from idpyoidc.node import Node
 from idpyoidc.server.client_authn import verify_client
-from idpyoidc.server.construct import construct_provider_info
 from idpyoidc.server.exception import UnAuthorizedClient
 from idpyoidc.server.util import OAUTH2_NOCACHE_HEADERS
 from idpyoidc.util import sanitize
 
 __author__ = "Roland Hedberg"
 
 LOGGER = logging.getLogger(__name__)
@@ -72,38 +74,41 @@
 def fragment_encoding(return_type):
     if return_type == ["code"]:
         return False
     else:
         return True
 
 
-class Endpoint(object):
+class Endpoint(Node):
     request_cls = Message
     response_cls = Message
     error_cls = ResponseMessage
     endpoint_name = ""
     endpoint_path = ""
     name = ""
     request_format = "urlencoded"
     request_placement = "query"
     response_format = "json"
     response_placement = "body"
+    response_content_type = ""
     client_authn_method = ""
-    default_capabilities = None
-    provider_info_attributes = None
     auth_method_attribute = ""
 
-    def __init__(self, server_get: Callable, **kwargs):
-        self.server_get = server_get
+    _supports = {}
+
+    def __init__(self, upstream_get: Callable, **kwargs):
+        self.upstream_get = upstream_get
         self.pre_construct = []
         self.post_construct = []
         self.post_parse_request = []
         self.kwargs = kwargs
         self.full_path = ""
 
+        Node.__init__(self, upstream_get=upstream_get)
+
         for param in [
             "request_cls",
             "response_cls",
             "request_format",
             "request_placement",
             "response_format",
             "response_placement",
@@ -128,102 +133,122 @@
 
         if _methods:
             self.client_authn_method = _methods
             if self.auth_method_attribute:
                 kwargs[self.auth_method_attribute] = _methods
         elif _methods is not None:  # [] or '' or something not None but regarded as nothing.
             self.client_authn_method = ["none"]  # Ignore default value
+        # self.endpoint_info = construct_provider_info(self.default_capabilities, **kwargs)
         return kwargs
 
-    def get_provider_info_attributes(self):
-        _pia = construct_provider_info(self.provider_info_attributes, **self.kwargs)
-        if self.endpoint_name:
-            _pia[self.endpoint_name] = self.full_path
-        return _pia
-
     def process_verify_error(self, exception):
         _error = "invalid_request"
         return self.error_cls(error=_error, error_description="%s" % exception)
 
+    def find_client_keys(self, iss):
+        return False
+
+    def verify_request(self, request, keyjar, client_id, verify_args, lap=0):
+        # verify that the request message is correct, may have to do it twice
+        try:
+            if verify_args is None:
+                request.verify(keyjar=keyjar, opponent_id=client_id)
+            else:
+                request.verify(keyjar=keyjar, opponent_id=client_id, **verify_args)
+        except (MissingRequiredAttribute, ValueError, MissingRequiredValue, ParameterError) as err:
+            _error = "invalid_request"
+            if isinstance(err, ValueError) and self.request_cls == RegistrationRequest:
+                if len(err.args) > 1:
+                    if err.args[1] == "initiate_login_uri":
+                        _error = "invalid_client_metadata"
+
+            return self.error_cls(error=_error, error_description="%s" % err)
+        except IssuerNotFound as err:
+            if lap:
+                return self.error_cls(error=err)
+            client_id = self.find_client_keys(err.args[0])
+            if not client_id:
+                return self.error_cls(error=err)
+            else:
+                # Fund a client ID I believe will work
+                self.verify_request(request=request, keyjar=keyjar, client_id=client_id,
+                                    verify_args=verify_args, lap=1)
+        return None
+
     def parse_request(
-        self,
-        request: Union[Message, dict, str],
-        http_info: Optional[dict] = None,
-        verify_args: Optional[dict] = None,
-        **kwargs
+            self,
+            request: Union[Message, dict, str],
+            http_info: Optional[dict] = None,
+            verify_args: Optional[dict] = None,
+            **kwargs
     ):
         """
 
         :param request: The request the server got
         :param http_info: HTTP information in connection with the request.
             This is a dictionary with keys: headers, url, cookies.
         :param kwargs: extra keyword arguments
         :return:
         """
         LOGGER.debug("- {} -".format(self.endpoint_name))
         LOGGER.info("Request: %s" % sanitize(request))
 
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
+        _keyjar = self.upstream_get('attribute', 'keyjar')
 
         if http_info is None:
             http_info = {}
 
         if request:
             if isinstance(request, (dict, Message)):
                 req = self.request_cls(**request)
             else:
                 _cls_inst = self.request_cls()
                 if self.request_format == "jwt":
                     req = _cls_inst.deserialize(
                         request,
                         "jwt",
-                        keyjar=_context.keyjar,
+                        keyjar=_keyjar,
                         verify=_context.httpc_params["verify"],
                         **kwargs
                     )
-                elif self.request_format == "url":
+                elif self.request_format == "url":  # A whole URL not just the query part
                     parts = urlparse(request)
                     scheme, netloc, path, params, query, fragment = parts[:6]
                     req = _cls_inst.deserialize(query, "urlencoded")
                 else:
                     req = _cls_inst.deserialize(request, self.request_format)
         else:
             req = self.request_cls()
 
         # Verify that the client is allowed to do this
         auth_info = self.client_authentication(req, http_info, endpoint=self, **kwargs)
 
         if "client_id" in auth_info:
             req["client_id"] = auth_info["client_id"]
+
+            _auth_method = auth_info.get('method')
+            if _auth_method and _auth_method not in ['public', 'none']:
+                req['authenticated'] = True
+
             _client_id = auth_info["client_id"]
         else:
             _client_id = req.get("client_id")
 
-        keyjar = _context.keyjar
-
-        # verify that the request message is correct
-        try:
-            if verify_args is None:
-                req.verify(keyjar=keyjar, opponent_id=_client_id)
-            else:
-                req.verify(keyjar=keyjar, opponent_id=_client_id, **verify_args)
-        except (MissingRequiredAttribute, ValueError, MissingRequiredValue, ParameterError) as err:
-            _error = "invalid_request"
-            if isinstance(err, ValueError) and self.request_cls == RegistrationRequest:
-                if len(err.args) > 1:
-                    if err.args[1] == "initiate_login_uri":
-                        _error = "invalid_client_metadata"
-
-            return self.error_cls(error=_error, error_description="%s" % err)
+        # verify that the request message is correct, may have to do it twice
+        err_response = self.verify_request(request=req, keyjar=_keyjar, client_id=_client_id,
+                                           verify_args=verify_args)
+        if err_response:
+            return err_response
 
         LOGGER.info("Parsed and verified request: %s" % sanitize(req))
 
         # Do any endpoint specific parsing
         return self.do_post_parse_request(
-            request=req, client_id=_client_id, http_info=http_info, **kwargs
+            request=req, client_id=_client_id, http_info=http_info, auth_info=auth_info, **kwargs
         )
 
     def client_authentication(self, request: Message, http_info: Optional[dict] = None, **kwargs):
         """
         Do client authentication
 
         :param request: Parsed request, a self.request_cls class instance
@@ -235,77 +260,77 @@
             kwargs["endpoint"] = self
 
         get_client_id_from_token = kwargs.get("get_client_id_from_token")
         if not get_client_id_from_token:
             kwargs["get_client_id_from_token"] = getattr(self, "get_client_id_from_token", None)
 
         authn_info = verify_client(
-            endpoint_context=self.server_get("endpoint_context"),
             request=request,
             http_info=http_info,
             **kwargs
         )
 
         LOGGER.debug("authn_info: %s", authn_info)
         if authn_info == {} and self.client_authn_method and len(self.client_authn_method):
             LOGGER.debug("client_authn_method: %s", self.client_authn_method)
             raise UnAuthorizedClient("Authorization failed")
-
+        if "client_id" not in authn_info and authn_info.get("method") != "none":
+            raise UnAuthorizedClient("Authorization failed")
         return authn_info
 
     def do_post_parse_request(
-        self, request: Message, client_id: Optional[str] = "", **kwargs
+            self, request: Message, client_id: Optional[str] = "", **kwargs
     ) -> Message:
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         for meth in self.post_parse_request:
             if isinstance(request, self.error_cls):
                 break
-            request = meth(request, client_id, endpoint_context=_context, **kwargs)
+            request = meth(request, client_id, context=_context, **kwargs)
         return request
 
     def do_pre_construct(
-        self, response_args: dict, request: Optional[Union[Message, dict]] = None, **kwargs
+            self, response_args: dict, request: Optional[Union[Message, dict]] = None, **kwargs
     ) -> dict:
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         for meth in self.pre_construct:
-            response_args = meth(response_args, request, endpoint_context=_context, **kwargs)
+            response_args = meth(response_args, request, context=_context, **kwargs)
 
         return response_args
 
     def do_post_construct(
-        self,
-        response_args: Union[Message, dict],
-        request: Optional[Union[Message, dict]] = None,
-        **kwargs
+            self,
+            response_args: Union[Message, dict],
+            request: Optional[Union[Message, dict]] = None,
+            **kwargs
     ) -> dict:
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         for meth in self.post_construct:
-            response_args = meth(response_args, request, endpoint_context=_context, **kwargs)
+            response_args = meth(response_args, request, context=_context, **kwargs)
 
         return response_args
 
     def process_request(
-        self,
-        request: Optional[Union[Message, dict]] = None,
-        http_info: Optional[dict] = None,
-        **kwargs
+            self,
+            request: Optional[Union[Message, dict]] = None,
+            http_info: Optional[dict] = None,
+            **kwargs
     ) -> Union[Message, dict]:
         """
 
         :param http_info: Information on the HTTP request
         :param request: The request, can be in a number of formats
         :return: Arguments for the do_response method
         """
         return {}
 
     def construct(
-        self,
-        response_args: Optional[dict] = None,
-        request: Optional[Union[Message, dict]] = None,
-        **kwargs
+            self,
+            response_args: Optional[dict] = None,
+            request: Optional[Union[Message, dict]] = None,
+            **kwargs
     ):
         """
         Construct the response
 
         :param response_args: response arguments
         :param request: The parsed request, a self.request_cls class instance
         :param kwargs: Extra keyword arguments
@@ -315,27 +340,27 @@
 
         # LOGGER.debug("kwargs: %s" % sanitize(kwargs))
         response = self.response_cls(**response_args)
 
         return self.do_post_construct(response, request, **kwargs)
 
     def response_info(
-        self,
-        response_args: Optional[dict] = None,
-        request: Optional[Union[Message, dict]] = None,
-        **kwargs
+            self,
+            response_args: Optional[dict] = None,
+            request: Optional[Union[Message, dict]] = None,
+            **kwargs
     ) -> dict:
         return self.construct(response_args, request, **kwargs)
 
     def do_response(
-        self,
-        response_args: Optional[dict] = None,
-        request: Optional[Union[Message, dict]] = None,
-        error: Optional[str] = "",
-        **kwargs
+            self,
+            response_args: Optional[dict] = None,
+            request: Optional[Union[Message, dict]] = None,
+            error: Optional[str] = "",
+            **kwargs
     ) -> dict:
         """
         :param response_args: Information to use when constructing the response
         :param request: The original request
         :param error: Possible error encountered while processing the request
         """
         do_placement = True
@@ -356,15 +381,17 @@
         elif "response_msg" in kwargs:
             resp = kwargs["response_msg"]
             _response_placement = kwargs.get("response_placement")
             do_placement = False
             _response = ""
             content_type = kwargs.get("content_type")
             if content_type is None:
-                if self.response_format == "json":
+                if self.response_content_type:
+                    content_type = self.response_content_type
+                elif self.response_format == "json":
                     content_type = "application/json"
                 elif self.response_format in ["jws", "jwe", "jose"]:
                     content_type = "application/jose"
                 else:
                     content_type = "application/x-www-form-urlencoded"
         else:
             _response = self.response_info(response_args, request, **kwargs)
@@ -376,15 +403,18 @@
                     if self.response_format == "json":
                         content_type = "application/json; charset=utf-8"
                         if isinstance(_response, Message):
                             resp = _response.to_json()
                         else:
                             resp = json.dumps(_response)
                     elif self.response_format in ["jws", "jwe", "jose"]:
-                        content_type = "application/jose; charset=utf-8"
+                        if self.response_content_type:
+                            content_type = self.response_content_type
+                        else:
+                            content_type = "application/jose; charset=utf-8"
                         resp = _response
                     else:
                         content_type = "application/x-www-form-urlencoded"
                         resp = _response.to_urlencoded()
                 elif self.response_placement == "url":
                     content_type = "application/x-www-form-urlencoded"
                     fragment_enc = kwargs.get("fragment_enc")
@@ -432,14 +462,23 @@
         except KeyError:
             pass
 
         return _resp
 
     def allowed_target_uris(self):
         res = []
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         for t in self.allowed_targets:
             if t == "":
                 res.append(_context.issuer)
             else:
-                res.append(self.server_get("endpoint", t).full_path)
+                res.append(self.upstream_get("endpoint", t).full_path)
         return set(res)
+
+    def supports(self):
+        res = {}
+        for key, val in self._supports.items():
+            if isinstance(val, Callable):
+                res[key] = val()
+            else:
+                res[key] = val
+        return res
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/endpoint_context.py` & `idpyoidc-2.0.0/src/idpyoidc/server/endpoint_context.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,59 +4,50 @@
 from typing import Callable
 from typing import Optional
 from typing import Union
 
 from cryptojwt import KeyJar
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
+from requests import request
 
-import requests
 from idpyoidc.context import OidcContext
+from idpyoidc.server import authz
+from idpyoidc.server.claims import Claims
+from idpyoidc.server.claims.oauth2 import Claims as OAUTH2_Claims
+from idpyoidc.server.claims.oidc import Claims as OIDC_Claims
+from idpyoidc.server.client_authn import client_auth_setup
 from idpyoidc.server.configure import OPConfiguration
 from idpyoidc.server.scopes import SCOPE2CLAIMS
 from idpyoidc.server.scopes import Scopes
+from idpyoidc.server.session.manager import create_session_manager
 from idpyoidc.server.session.manager import SessionManager
 from idpyoidc.server.template_handler import Jinja2TemplateHandler
+from idpyoidc.server.user_authn.authn_context import populate_authn_broker
 from idpyoidc.server.util import get_http_params
 from idpyoidc.util import importer
 from idpyoidc.util import rndstr
 
 logger = logging.getLogger(__name__)
 
 
-def get_provider_capabilities(conf, endpoints):
-    _cap = conf.get("capabilities", {})
-    if _cap is None:
-        _cap = {}
-
-    for endpoint, endpoint_instance in endpoints.items():
-        if endpoint in ["webfinger", "provider_config"]:
-            continue
-
-        for key, val in endpoint_instance.get_provider_info_attributes().items():
-            if key not in _cap:
-                _cap[key] = val
-
-    return _cap
-
-
 def init_user_info(conf, cwd: str):
     kwargs = conf.get("kwargs", {})
 
     if isinstance(conf["class"], str):
         return importer(conf["class"])(**kwargs)
 
     return conf["class"](**kwargs)
 
 
-def init_service(conf, server_get=None):
+def init_service(conf, upstream_get=None):
     kwargs = conf.get("kwargs", {})
 
-    if server_get:
-        kwargs["server_get"] = server_get
+    if upstream_get:
+        kwargs["upstream_get"] = upstream_get
 
     if isinstance(conf["class"], str):
         try:
             return importer(conf["class"])(**kwargs)
         except TypeError as err:
             logger.error("Could not init service class: {}".format(conf["class"]), err)
             raise
@@ -107,36 +98,52 @@
         "sso_ttl": None,
         "symkey": "",
         "token_args_methods": [],
         # "userinfo": UserInfo,
         "client_authn_method": {},
     }
 
+    init_args = ['upstream_get', 'handler']
+
     def __init__(
-        self,
-        conf: Union[dict, OPConfiguration],
-        server_get: Callable,
-        keyjar: Optional[KeyJar] = None,
-        cwd: Optional[str] = "",
-        cookie_handler: Optional[Any] = None,
-        httpc: Optional[Any] = None,
+            self,
+            conf: Union[dict, OPConfiguration],
+            upstream_get: Callable,
+            cwd: Optional[str] = "",
+            cookie_handler: Optional[Any] = None,
+            httpc: Optional[Any] = None,
+            server_type: Optional[str] = '',
+            entity_id: Optional[str] = "",
+            keyjar: Optional[KeyJar] = None,
+            claims_class: Optional[Claims] = None
     ):
-        OidcContext.__init__(self, conf, keyjar, entity_id=conf.get("issuer", ""))
+        _id = entity_id or conf.get("issuer", "")
+        OidcContext.__init__(self, conf, entity_id=_id)
         self.conf = conf
-        self.server_get = server_get
+        self.upstream_get = upstream_get
+
+        if claims_class:
+            self.claims = claims_class
+        else:
+            if not server_type or server_type == "oidc":
+                self.claims = OIDC_Claims()
+            elif server_type == "oauth2":
+                self.claims = OAUTH2_Claims()
+            else:
+                raise ValueError(f"Unknown server type: {server_type}")
 
         _client_db = conf.get("client_db")
         if _client_db:
             logger.debug(f"Loading client db using: {_client_db}")
             self.cdb = importer(_client_db["class"])(**_client_db["kwargs"])
         else:
             logger.debug("No special client db, will use memory based dictionary")
             self.cdb = {}
 
-        # For my Dev environment
+        # For my Dev claims
         self.jti_db = {}
         self.registration_access_token = {}
         # self.session_db = {}
 
         self.cwd = cwd
 
         # Default values, to be changed below depending on configuration
@@ -144,18 +151,18 @@
         self.add_on = {}
         self.args = {}
         self.authn_broker = None
         self.authz = None
         self.cookie_handler = cookie_handler
         self.claims_interface = None
         self.endpoint_to_authn_method = {}
-        self.httpc = httpc or requests
+        self.httpc = httpc or request
         self.idtoken = None
         self.issuer = ""
-        self.jwks_uri = None
+        # self.jwks_uri = None
         self.login_hint_lookup = None
         self.login_hint2acrs = None
         self.par_db = {}
         self.provider_info = {}
         self.remove_token = None
         self.scope2claims = conf.get("scopes_to_claims", SCOPE2CLAIMS)
         self.session_manager = None
@@ -194,24 +201,14 @@
                 _template_dir = conf.get("template_dir")
                 if _template_dir:
                     _loader = Environment(loader=FileSystemLoader(_template_dir), autoescape=True)
 
             if _loader:
                 self.template_handler = Jinja2TemplateHandler(_loader)
 
-        # self.setup = {}
-        _keys_conf = conf.get("key_conf")
-        if _keys_conf:
-            jwks_uri_path = _keys_conf["uri_path"]
-
-            if self.issuer.endswith("/"):
-                self.jwks_uri = "{}{}".format(self.issuer, jwks_uri_path)
-            else:
-                self.jwks_uri = "{}/{}".format(self.issuer, jwks_uri_path)
-
         for item in [
             "cookie_handler",
             "authentication",
             "id_token",
         ]:
             _func = getattr(self, "do_{}".format(item), None)
             if _func:
@@ -230,31 +227,94 @@
         if _cnf:
             self.httpc_params = get_http_params(_cnf)
         else:  # Backward compatibility
             self.httpc_params = {"verify": conf.get("verify_ssl", True)}
 
         self.set_scopes_handler()
         self.dev_auth_db = None
-        self.claims_interface = init_service(conf["claims_interface"], self.server_get)
+        _interface = conf.get("claims_interface")
+        if _interface:
+            self.claims_interface = init_service(_interface, self.upstream_get)
+
+        if isinstance(conf, OPConfiguration):
+            conf = conf.conf
+        _supports = self.supports()
+        self.keyjar = self.claims.load_conf(conf, supports=_supports, keyjar=keyjar)
+        self.provider_info = self.claims.provider_info(_supports)
+        self.provider_info['issuer'] = self.issuer
+        self.provider_info.update(self._get_endpoint_info())
+
+        # INTERFACES
+
+        self.authz = self.setup_authz()
+
+        self.setup_authentication()
+
+        self.session_manager = create_session_manager(
+            self.unit_get,
+            self.th_args,
+            sub_func=self._sub_func,
+            conf=self.conf,
+        )
+
+        self.do_userinfo()
+
+        # Must be done after userinfo
+        self.setup_login_hint_lookup()
+        self.set_remember_token()
+
+        self.setup_client_authn_methods()
+
+        # _id_token_handler = self.session_manager.token_handler.handler.get("id_token")
+        # if _id_token_handler:
+        #     self.provider_info.update(_id_token_handler.provider_info)
+
+    def setup_authz(self):
+        authz_spec = self.conf.get("authz")
+        if authz_spec:
+            return init_service(authz_spec, self.unit_get)
+        else:
+            return authz.Implicit(self.unit_get)
+
+    def setup_client_authn_methods(self):
+        self.client_authn_methods = client_auth_setup(
+            self.upstream_get, self.conf.get("client_authn_methods")
+        )
+
+    def setup_login_hint_lookup(self):
+        _conf = self.conf.get("login_hint_lookup")
+        if _conf:
+            _userinfo = None
+            _kwargs = _conf.get("kwargs")
+            if _kwargs:
+                _userinfo_conf = _kwargs.get("userinfo")
+                if _userinfo_conf:
+                    _userinfo = init_user_info(_userinfo_conf, self.cwd)
+
+            if _userinfo is None:
+                _userinfo = self.userinfo
+
+            self.login_hint_lookup = init_service(_conf)
+            self.login_hint_lookup.userinfo = _userinfo
 
     def new_cookie(self, name: str, max_age: Optional[int] = 0, **kwargs):
         cookie_cont = self.cookie_handler.make_cookie_content(
             name=name, value=json.dumps(kwargs), max_age=max_age
         )
         return cookie_cont
 
     def set_scopes_handler(self):
         _spec = self.conf.get("scopes_handler")
         if _spec:
             _kwargs = _spec.get("kwargs", {})
             _cls = importer(_spec["class"])
-            self.scopes_handler = _cls(self.server_get, **_kwargs)
+            self.scopes_handler = _cls(self.upstream_get, **_kwargs)
         else:
             self.scopes_handler = Scopes(
-                self.server_get,
+                self.upstream_get,
                 allowed_scopes=self.conf.get("allowed_scopes"),
                 scopes_to_claims=self.conf.get("scopes_to_claims"),
             )
 
     def do_add_on(self, endpoints):
         _add_on_conf = self.conf.get("add_on")
         if _add_on_conf:
@@ -301,44 +361,14 @@
                 self._sub_func[key] = init_service(args)
             elif "function" in args:
                 if isinstance(args["function"], str):
                     self._sub_func[key] = importer(args["function"])
                 else:
                     self._sub_func[key] = args["function"]
 
-    def create_providerinfo(self, capabilities):
-        """
-        Dynamically create the provider info response
-
-        :param capabilities:
-        :return:
-        """
-
-        _provider_info = capabilities
-        _provider_info["issuer"] = self.issuer
-        _provider_info["version"] = "3.0"
-
-        # acr_values
-        if self.authn_broker:
-            acr_values = self.authn_broker.get_acr_values()
-            if acr_values is not None:
-                _provider_info["acr_values_supported"] = acr_values
-
-        if self.jwks_uri and self.keyjar:
-            _provider_info["jwks_uri"] = self.jwks_uri
-
-        if "scopes_supported" not in _provider_info:
-            _provider_info["scopes_supported"] = self.scopes_handler.get_allowed_scopes()
-        if "claims_supported" not in _provider_info:
-            _provider_info["claims_supported"] = list(
-                self.scopes_handler.scopes_to_claims(_provider_info["scopes_supported"]).keys()
-            )
-
-        return _provider_info
-
     def set_remember_token(self):
         ses_par = self.conf.get("session_params") or {}
 
         self.session_manager.remove_inactive_token = ses_par.get("remove_inactive_token", False)
 
         _rm = ses_par.get("remember_token", {})
         if "class" in _rm:
@@ -361,7 +391,100 @@
                     _userinfo = init_user_info(_userinfo_conf, self.cwd)
 
             if _userinfo is None:
                 _userinfo = self.userinfo
 
             self.login_hint_lookup = init_service(_conf)
             self.login_hint_lookup.userinfo = _userinfo
+
+    def supports(self):
+        res = {}
+        if self.upstream_get:
+            for endpoint in self.upstream_get('endpoints').values():
+                res.update(endpoint.supports())
+        res.update(self.claims.supports())
+        return res
+
+    def set_provider_info(self):
+        _info = self.claims.provider_info(self.supports())
+        _info.update({'issuer': self.issuer, 'version': "3.0"})
+
+        for endp in self.upstream_get('endpoints').values():
+            if endp.endpoint_name:
+                _info[endp.endpoint_name] = endp.full_path
+
+        # acr_values
+        if 'acr_values_supported' not in _info:
+            if self.authn_broker:
+                acr_values = self.authn_broker.get_acr_values()
+                if acr_values is not None:
+                    _info["acr_values_supported"] = acr_values
+
+        self.provider_info = _info
+
+    def get_preference(self, claim, default=None):
+        return self.claims.get_preference(claim, default=default)
+
+    def set_preference(self, key, value):
+        self.claims.set_preference(key, value)
+
+    def get_usage(self, claim, default: Optional[str] = None):
+        return self.claims.get_usage(claim, default)
+
+    def set_usage(self, claim, value):
+        return self.claims.set_usage(claim, value)
+
+    def setup_authentication(self):
+        _conf = self.conf.get("authentication")
+        if _conf:
+            self.authn_broker = populate_authn_broker(
+                _conf, self.upstream_get, self.template_handler
+            )
+        else:
+            self.authn_broker = {}
+
+        self.endpoint_to_authn_method = {}
+        for method in self.authn_broker:
+            try:
+                self.endpoint_to_authn_method[method.action] = method
+            except AttributeError:
+                pass
+
+    def unit_get(self, what, *arg):
+        _func = getattr(self, f"get_{what}", None)
+        if _func:
+            return _func(*arg)
+        return None
+
+    def get_attribute(self, attr, *args):
+        try:
+            val = getattr(self, attr)
+        except AttributeError:
+            if self.upstream_get:
+                return self.upstream_get("attribute", attr)
+            else:
+                return None
+        else:
+            if val is None and self.upstream_get:
+                return self.upstream_get("attribute", attr)
+            else:
+                return val
+
+    def set_attribute(self, attr, val):
+        setattr(self, attr, val)
+
+    def get_unit(self, *args):
+        return self
+
+    def get_context(self, *args):
+        return self
+
+    def map_supported_to_preferred(self):
+        self.claims.supported_to_preferred(self.supports())
+        return self.claims.prefer
+
+    def _get_endpoint_info(self):
+        _res = {}
+        for name, endp in self.upstream_get('endpoints').items():
+            if endp.endpoint_name:
+                _res[endp.endpoint_name] = endp.full_path
+        return _res
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/exception.py` & `idpyoidc-2.0.0/src/idpyoidc/server/exception.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/login_hint.py` & `idpyoidc-2.0.0/src/idpyoidc/server/login_hint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from urllib.parse import urlparse
 
 
 class LoginHintLookup(object):
-    def __init__(self, userinfo=None, server_get=None):
+    def __init__(self, userinfo=None, upstream_get=None):
         self.userinfo = userinfo
         self.default_country_code = "46"
-        self.server_get = server_get
+        self.upstream_get = upstream_get
 
     def __call__(self, arg):
         if arg.startswith("tel:"):
             _pnr = arg[4:]
             if _pnr[0] == "+":
                 pass
             else:
@@ -21,17 +21,17 @@
 
 
 class LoginHint2Acrs(object):
     """
     OIDC Login hint support
     """
 
-    def __init__(self, scheme_map, server_get=None):
+    def __init__(self, scheme_map, upstream_get=None):
         self.scheme_map = scheme_map
-        self.server_get = server_get
+        self.upstream_get = upstream_get
 
     def __call__(self, hint):
         p = urlparse(hint)
         try:
             return self.scheme_map[p.scheme]
         except KeyError:
             return []
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oauth2/add_on/dpop.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/dpop.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,22 +80,22 @@
                 raise Exception()
 
             return self
         else:
             return None
 
 
-def post_parse_request(request, client_id, endpoint_context, **kwargs):
+def post_parse_request(request, client_id, context, **kwargs):
     """
     Expect http_info attribute in kwargs. http_info should be a dictionary
     containing HTTP information.
 
     :param request:
     :param client_id:
-    :param endpoint_context:
+    :param context:
     :param kwargs:
     :return:
     """
 
     _http_info = kwargs.get("http_info")
     if not _http_info:
         return request
@@ -115,43 +115,41 @@
         _dpop.key = key_from_jwk_dict(_dpop["jwk"])
 
     # Need something I can add as a reference when minting tokens
     request["dpop_jkt"] = as_unicode(_dpop.key.thumbprint("SHA-256"))
     return request
 
 
-def token_args(endpoint_context, client_id, token_args: Optional[dict] = None):
-    dpop_jkt = endpoint_context.cdb[client_id]["dpop_jkt"]
+def token_args(context, client_id, token_args: Optional[dict] = None):
+    dpop_jkt = context.cdb[client_id]["dpop_jkt"]
     _jkt = list(dpop_jkt.keys())[0]
-    if "dpop_jkt" in endpoint_context.cdb[client_id]:
+    if "dpop_jkt" in context.cdb[client_id]:
         if token_args is None:
             token_args = {"cnf": {"jkt": _jkt}}
         else:
-            token_args.update({"cnf": {"jkt": endpoint_context.cdb[client_id]["dpop_jkt"]}})
+            token_args.update({"cnf": {"jkt": context.cdb[client_id]["dpop_jkt"]}})
 
     return token_args
 
 
-def add_support(endpoint, **kwargs):
+def add_support(endpoint: dict, **kwargs):
     #
     _token_endp = endpoint["token"]
     _token_endp.post_parse_request.append(post_parse_request)
 
-    # Endpoint Context stuff
-    # _endp.endpoint_context.token_args_methods.append(token_args)
     _algs_supported = kwargs.get("dpop_signing_alg_values_supported")
     if not _algs_supported:
         _algs_supported = ["RS256"]
 
-    _token_endp.server_get("endpoint_context").provider_info[
+    _token_endp.upstream_get("context").provider_info[
         "dpop_signing_alg_values_supported"
     ] = _algs_supported
 
-    _endpoint_context = _token_endp.server_get("endpoint_context")
-    _endpoint_context.dpop_enabled = True
+    _context = _token_endp.upstream_get("context")
+    _context.dpop_enabled = True
 
 
 # DPoP-bound access token in the "Authorization" header and the DPoP proof in the "DPoP" header
 
 
 class DPoPClientAuth(ClientAuthnMethod):
     tag = "dpop_client_auth"
@@ -159,12 +157,12 @@
     def is_usable(self, request=None, authorization_info=None, http_headers=None):
         if authorization_info is not None and authorization_info.startswith("DPoP "):
             return True
         return False
 
     def verify(self, authorization_info, **kwargs):
         client_info = basic_authn(authorization_info)
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         if _context.cdb[client_info["id"]]["client_secret"] == client_info["secret"]:
             return {"client_id": client_info["id"]}
         else:
             raise ClientAuthenticationError()
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oauth2/add_on/extra_args.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/extra_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from idpyoidc.message.oauth2 import AccessTokenResponse
 from idpyoidc.message.oauth2 import AuthorizationResponse
 from idpyoidc.message.oauth2 import TokenExchangeResponse
 from idpyoidc.message.oauth2 import TokenIntrospectionResponse
 from idpyoidc.message.oidc import OpenIDSchema
 
 
-def pre_construct(response_args, request, endpoint_context, **kwargs):
+def pre_construct(response_args, request, context, **kwargs):
     """
     Add extra arguments to the request.
 
     :param response_args:
     :param request:
-    :param endpoint_context:
+    :param context:
     :param kwargs:
     :return:
     """
 
-    _extra = endpoint_context.add_on.get("extra_args")
+    _extra = context.add_on.get("extra_args")
     if _extra:
         if isinstance(response_args, AuthorizationResponse):
             _args = _extra.get("authorization", {})
         elif isinstance(response_args, AccessTokenResponse):
             _args = _extra.get("accesstoken", {})
         elif isinstance(response_args, TokenExchangeResponse):
             _args = _extra.get("token_exchange", {})
@@ -28,24 +28,24 @@
             _args = _extra.get("token_introspection", {})
         elif isinstance(response_args, OpenIDSchema):
             _args = _extra.get("userinfo", {})
         else:
             _args = {}
 
         for arg, _param in _args.items():
-            _val = getattr(endpoint_context, _param)
+            _val = getattr(context, _param)
             if _val:
                 response_args[arg] = _val
 
     return response_args
 
 
 def add_support(endpoint, **kwargs):
     #
     _added = False
     for endpoint_name in list(kwargs.keys()):
         _endp = endpoint[endpoint_name]
         _endp.pre_construct.append(pre_construct)
 
         if _added is False:
-            _endp.server_get("endpoint_context").add_on["extra_args"] = kwargs
+            _endp.upstream_get("context").add_on["extra_args"] = kwargs
             _added = True
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oauth2/authorization.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/authorization.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from cryptojwt import as_unicode
 from cryptojwt import b64d
 from cryptojwt.jwe.exception import JWEException
 from cryptojwt.jws.exception import NoSuitableSigningKeys
 from cryptojwt.utils import as_bytes
 from cryptojwt.utils import b64e
 
+from idpyoidc import claims
 from idpyoidc.exception import ImproperlyConfigured
 from idpyoidc.exception import ParameterError
 from idpyoidc.exception import URIError
 from idpyoidc.message import Message
 from idpyoidc.message import oauth2
 from idpyoidc.message.oauth2 import AuthorizationRequest
 from idpyoidc.message.oidc import AuthorizationResponse
@@ -38,14 +39,15 @@
 from idpyoidc.server.token.exception import UnknownToken
 from idpyoidc.server.user_authn.authn_context import pick_auth
 from idpyoidc.time_util import utc_time_sans_frac
 from idpyoidc.util import rndstr
 from idpyoidc.util import split_uri
 from idpyoidc.util import importer
 
+
 logger = logging.getLogger(__name__)
 
 # For the time being. This is JAR specific and should probably be configurable.
 ALG_PARAMS = {
     "sign": [
         "request_object_signing_alg",
         "request_object_signing_alg_values_supported",
@@ -87,25 +89,25 @@
 
 def max_age(request):
     verified_request = verified_claim_name("request")
     return request.get(verified_request, {}).get("max_age") or request.get("max_age", 0)
 
 
 def verify_uri(
-        endpoint_context: EndpointContext,
+    context: EndpointContext,
         request: Union[dict, Message],
         uri_type: str,
         client_id: Optional[str] = None,
 ):
     """
     A redirect URI
     MUST NOT contain a fragment
     MAY contain query component
 
-    :param endpoint_context: An EndpointContext instance
+    :param context: An EndpointContext instance
     :param request: The authorization request
     :param uri_type: redirect_uri or post_logout_redirect_uri
     :return: An error response if the redirect URI is faulty otherwise
         None
     """
     _cid = request.get("client_id", client_id)
 
@@ -122,15 +124,15 @@
     part = urlparse(_redirect_uri)
     if part.fragment:
         raise URIError("Contains fragment")
 
     (_base, _query) = split_uri(_redirect_uri)
 
     # Get the clients registered redirect uris
-    client_info = endpoint_context.cdb.get(_cid)
+    client_info = context.cdb.get(_cid)
     if client_info is None:
         raise KeyError("No such client")
 
     if uri_type == "redirect_uri":
         redirect_uris = client_info.get(f"{uri_type}s")
     else:
         redirect_uris = client_info.get(f"{uri_type}")
@@ -188,32 +190,32 @@
     """
     if query:
         return "{}?{}".format(base, urlencode(query, doseq=True))
     else:
         return base
 
 
-def get_uri(endpoint_context, request, uri_type):
+def get_uri(context, request, uri_type):
     """verify that the redirect URI is reasonable.
 
-    :param endpoint_context: An EndpointContext instance
+    :param context: An EndpointContext instance
     :param request: The Authorization request
     :param uri_type: 'redirect_uri' or 'post_logout_redirect_uri'
     :return: redirect_uri
     """
     uri = ""
 
     if uri_type in request:
-        verify_uri(endpoint_context, request, uri_type)
+        verify_uri(context, request, uri_type)
         uri = request[uri_type]
     else:
         uris = f"{uri_type}s"
         client_id = str(request["client_id"])
-        if client_id in endpoint_context.cdb:
-            _specs = endpoint_context.cdb[client_id].get(uris)
+        if client_id in context.cdb:
+            _specs = context.cdb[client_id].get(uris)
             if not _specs:
                 raise ParameterError(f"Missing '{uri_type}' and none registered")
 
             if len(_specs) > 1:
                 raise ParameterError(f"Missing '{uri_type}' and more than one registered")
 
             uri = join_query(*_specs[0])
@@ -261,20 +263,20 @@
     for attr in ["ui_locales", "acr_values", "login_hint"]:
         if request.get(attr):
             authn_args[attr] = request[attr]
 
     return authn_args
 
 
-def check_unknown_scopes_policy(request_info, client_id, endpoint_context):
-    if not endpoint_context.conf["capabilities"].get("deny_unknown_scopes"):
+def check_unknown_scopes_policy(request_info, client_id, context):
+    if not context.get_preference("deny_unknown_scopes"):
         return
 
     scope = request_info["scope"]
-    filtered_scopes = set(endpoint_context.scopes_handler.filter_scopes(scope, client_id=client_id))
+    filtered_scopes = set(context.scopes_handler.filter_scopes(scope, client_id=client_id))
     scopes = set(scope)
     # this prevents that authz would be released for unavailable scopes
     if scopes != filtered_scopes:
         diff = " ".join(scopes - filtered_scopes)
         logger.warning(f"{client_id} requested unauthorized scopes: {diff}")
         raise UnAuthorizedClientScope()
 
@@ -331,39 +333,40 @@
     response_cls = oauth2.AuthorizationResponse
     error_cls = oauth2.AuthorizationErrorResponse
     request_format = "urlencoded"
     response_format = "urlencoded"
     response_placement = "url"
     endpoint_name = "authorization_endpoint"
     name = "authorization"
-    provider_info_attributes = {
+
+    _supports = {
         "claims_parameter_supported": True,
         "request_parameter_supported": True,
         "request_uri_parameter_supported": True,
         "response_types_supported": ["code", "token", "code token"],
         "response_modes_supported": ["query", "fragment", "form_post"],
-        "request_object_signing_alg_values_supported": None,
-        "request_object_encryption_alg_values_supported": None,
-        "request_object_encryption_enc_values_supported": None,
-        "grant_types_supported": ["authorization_code", "implicit"],
+        "request_object_signing_alg_values_supported": claims.get_signing_algs,
+        "request_object_encryption_alg_values_supported": claims.get_encryption_algs,
+        "request_object_encryption_enc_values_supported": claims.get_encryption_encs,
+        # "grant_types_supported": ["authorization_code", "implicit"],
+        "code_challenge_methods_supported": ["S256"],
         "scopes_supported": [],
     }
     default_capabilities = {
         "client_authn_method": ["request_param", "public"],
     }
 
-    def __init__(self, server_get, **kwargs):
-        Endpoint.__init__(self, server_get, **kwargs)
-
-        self.resource_indicators_config = kwargs.get("resource_indicators", None)
+    def __init__(self, upstream_get, **kwargs):
+        Endpoint.__init__(self, upstream_get, **kwargs)
         self.post_parse_request.append(self._do_request_uri)
         self.post_parse_request.append(self._post_parse_request)
         self.allowed_request_algorithms = AllowedAlgorithms(ALG_PARAMS)
+        self.resource_indicators_config = kwargs.get('resource_indicators', None)
 
-    def filter_request(self, endpoint_context, req):
+    def filter_request(self, context, req):
         return req
 
     def extra_response_args(self, aresp):
         return aresp
 
     def authentication_error_response(self, request, error, error_description, **kwargs):
         _error_msg = self.error_cls(error=error, error_description=error_description)
@@ -382,114 +385,117 @@
         # Is the asked for response_type among those that are permitted
         return set(request["response_type"]) in _registered
 
     def mint_token(self, token_class, grant, session_id, based_on=None, **kwargs):
         usage_rules = grant.usage_rules.get(token_class, {})
         token = grant.mint_token(
             session_id=session_id,
-            endpoint_context=self.server_get("endpoint_context"),
+            context=self.upstream_get("context"),
             token_class=token_class,
             based_on=based_on,
             usage_rules=usage_rules,
             **kwargs,
         )
 
         _exp_in = usage_rules.get("expires_in")
         if isinstance(_exp_in, str):
             _exp_in = int(_exp_in)
         if _exp_in:
             token.expires_at = utc_time_sans_frac() + _exp_in
 
-        _mngr = self.server_get("endpoint_context").session_manager
+        _mngr = self.upstream_get("context").session_manager
         _mngr.set(_mngr.unpack_session_key(session_id), grant)
 
         return token
 
-    def _do_request_uri(self, request, client_id, endpoint_context, **kwargs):
+    def _do_request_uri(self, request, client_id, context, **kwargs):
         _request_uri = request.get("request_uri")
         if _request_uri:
             # Do I do pushed authorization requests ?
-            _endp = self.server_get("endpoint", "pushed_authorization")
+            _endp = self.upstream_get("endpoint", "pushed_authorization")
             if _endp:
                 # Is it a UUID urn
                 if _request_uri.startswith("urn:uuid:"):
-                    _req = endpoint_context.par_db.get(_request_uri)
+                    _req = context.par_db.get(_request_uri)
                     if _req:
                         # One time usage
-                        del endpoint_context.par_db[_request_uri]
+                        del context.par_db[_request_uri]
                         return _req
                     else:
                         raise ValueError("Got a request_uri I can not resolve")
 
             # Do I support request_uri ?
-            if endpoint_context.provider_info.get("request_uri_parameter_supported", True) is False:
+            if context.provider_info.get("request_uri_parameter_supported", True) is False:
                 raise ServiceError("Someone is using request_uri which I'm not supporting")
 
-            _registered = endpoint_context.cdb[client_id].get("request_uris")
+            _registered = context.cdb[client_id].get("request_uris")
             # Not registered should be handled else where
             if _registered:
                 # Before matching remove a possible fragment
                 _p = _request_uri.split("#")
                 # ignore registered fragments for now.
                 if _p[0] not in [base for base, qp in _registered]:
                     raise ValueError("A request_uri outside the registered")
 
             # Fetch the request
-            _resp = endpoint_context.httpc.get(_request_uri, **endpoint_context.httpc_params)
+            _resp = context.httpc('GET', _request_uri, **context.httpc_params)
             if _resp.status_code == 200:
-                args = {"keyjar": endpoint_context.keyjar, "issuer": client_id}
+                args = {
+                    "keyjar": self.upstream_get('attribute', 'keyjar'),
+                    "issuer": client_id
+                }
                 _ver_request = self.request_cls().from_jwt(_resp.text, **args)
                 self.allowed_request_algorithms(
                     client_id,
-                    endpoint_context,
+                    context,
                     _ver_request.jws_header.get("alg", "RS256"),
                     "sign",
                 )
                 if _ver_request.jwe_header is not None:
                     self.allowed_request_algorithms(
                         client_id,
-                        endpoint_context,
+                        context,
                         _ver_request.jws_header.get("alg"),
                         "enc_alg",
                     )
                     self.allowed_request_algorithms(
                         client_id,
-                        endpoint_context,
+                        context,
                         _ver_request.jws_header.get("enc"),
                         "enc_enc",
                     )
                 # The protected info overwrites the non-protected
                 for k, v in _ver_request.items():
                     request[k] = v
 
                 request[verified_claim_name("request")] = _ver_request
             else:
                 raise ServiceError("Got a %s response", _resp.status)
 
         return request
 
-    def _post_parse_request(self, request, client_id, endpoint_context, **kwargs):
+    def _post_parse_request(self, request, client_id, context, **kwargs):
         """
         Verify the authorization request.
 
-        :param endpoint_context:
+        :param context:
         :param request:
         :param client_id:
         :param kwargs:
         :return:
         """
         if not request:
             logger.debug("No AuthzRequest")
             return self.authentication_error_response(
                 request, error="invalid_request", error_description="Can not parse AuthzRequest"
             )
 
-        request = self.filter_request(endpoint_context, request)
+        request = self.filter_request(context, request)
 
-        _cinfo = endpoint_context.cdb.get(client_id)
+        _cinfo = context.cdb.get(client_id)
         if not _cinfo:
             logger.error("Client ID ({}) not in client database".format(request["client_id"]))
             return self.authentication_error_response(
                 request, error="unauthorized_client", error_description="unknown client"
             )
 
         # Is the asked for response_type among those that are permitted
@@ -498,65 +504,65 @@
                 request,
                 error="invalid_request",
                 error_description="Trying to use unregistered response_type",
             )
 
         # Get a verified redirect URI
         try:
-            redirect_uri = get_uri(endpoint_context, request, "redirect_uri")
+            redirect_uri = get_uri(context, request, "redirect_uri")
         except (RedirectURIError, ParameterError) as err:
             return self.authentication_error_response(
                 request,
                 error="invalid_request",
                 error_description="{}:{}".format(err.__class__.__name__, err),
             )
         else:
             request["redirect_uri"] = redirect_uri
 
         if ("resource_indicators" in _cinfo
-            and "authorization_code" in _cinfo["resource_indicators"]):
+                and "authorization_code" in _cinfo["resource_indicators"]):
             resource_indicators_config = _cinfo["resource_indicators"]["authorization_code"]
         else:
             resource_indicators_config = self.resource_indicators_config
 
         if resource_indicators_config is not None:
             if "policy" not in resource_indicators_config:
-                policy = {"policy": {"callable": validate_resource_indicators_policy}}
+                policy = {"policy": {"function": validate_resource_indicators_policy}}
                 resource_indicators_config.update(policy)
             request = self._enforce_resource_indicators_policy(request, resource_indicators_config)
 
         return request
 
     def _enforce_resource_indicators_policy(self, request, config):
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
 
         policy = config["policy"]
-        callable = policy["callable"]
+        function = policy["function"]
         kwargs = policy.get("kwargs", {})
 
         if kwargs.get("resource_servers_per_client", None) is None:
             kwargs["resource_servers_per_client"] = {
                 request["client_id"]: request["client_id"]
             }
 
-        if isinstance(callable, str):
+        if isinstance(function, str):
             try:
-                fn = importer(callable)
+                fn = importer(function)
             except Exception:
-                raise ImproperlyConfigured(f"Error importing {callable} policy callable")
+                raise ImproperlyConfigured(f"Error importing {function} policy function")
         else:
-            fn = callable
+            fn = function
         try:
             return fn(request, context=_context, **kwargs)
         except Exception as e:
-            logger.error(f"Error while executing the {fn} policy callable: {e}")
+            logger.error(f"Error while executing the {fn} policy function: {e}")
             return self.error_cls(error="server_error", error_description="Internal server error")
 
     def pick_authn_method(self, request, redirect_uri, acr=None, **kwargs):
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         auth_id = kwargs.get("auth_method_id")
         if auth_id:
             return _context.authn_broker[auth_id]
 
         res = None
         if acr:
             res = _context.authn_broker.pick(acr)
@@ -572,15 +578,15 @@
                 "error": "access_denied",
                 "error_description": "ACR I do not support",
                 "return_uri": redirect_uri,
                 "return_type": request["response_type"],
             }
 
     def create_session(self, request, user_id, acr, time_stamp, authn_method):
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         _mngr = _context.session_manager
         authn_event = create_authn_event(
             user_id,
             authn_info=acr,
             time_stamp=time_stamp,
         )
         _exp_in = authn_method.kwargs.get("expires_in")
@@ -611,20 +617,20 @@
     def _unwrap_identity(self, identity):
         # identity is a dict or a json object
         # the value of 'uid' in the dictionary might be a base64 encoded (b64e) json object
         if isinstance(identity, dict):
             _uid = as_unicode(identity['uid'])
             try:
                 _id = b64d(as_bytes(_uid))
-            except Exception as err:
+            except Exception:
                 return identity
         else:
             try:
                 _id = b64d(as_bytes(identity))
-            except Exception as err:
+            except Exception:
                 return identity
 
         try:
             return json.loads(as_unicode(_id))
         except UnicodeDecodeError:
             return identity
 
@@ -650,15 +656,15 @@
 
         res = self.pick_authn_method(request, redirect_uri, acr, **kwargs)
 
         authn = res["method"]
         authn_class_ref = res["acr"]
 
         client_id = request.get("client_id")
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         try:
             _auth_info = kwargs.get("authn", "")
             if "upm_answer" in request and request["upm_answer"] == "true":
                 _max_age = 0
             else:
                 _max_age = max_age(request)
             logger.debug(f"Max age: {_max_age}")
@@ -830,15 +836,15 @@
         aresp = self.response_cls()
         if request.get("state"):
             aresp["state"] = request["state"]
 
         if "response_type" in request and request["response_type"] == ["none"]:
             fragment_enc = False
         else:
-            _context = self.server_get("endpoint_context")
+            _context = self.upstream_get("context")
             _mngr = _context.session_manager
             _sinfo = _mngr.get_session_info(sid, grant=True)
 
             scope = []
             resource_scopes = []
             if request.get("scope"):
                 scope = request.get("scope")
@@ -937,15 +943,15 @@
         :param request: The authorization request
         :param session_id: Session identifier
         :param kwargs:
         :return: A dictionary with 'response_args'
         """
 
         response_info = {}
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         _mngr = _context.session_manager
 
         # Do the authorization
 
         grant = _context.authz(session_id, request=request)
         if grant.is_active() is False:
             return self.error_response(response_info, request, "server_error", "Grant not usable")
@@ -1006,15 +1012,15 @@
         :return: A redirect to the redirect_uri of the client
         """
         try:
             resp_info = self.post_authentication(request, session_id, **kwargs)
         except Exception as err:
             return self.error_by_response_mode({}, request, "server_error", err)
 
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
 
         logger.debug(f"resp_info: {resp_info}")
 
         if "check_session_iframe" in _context.provider_info:
             salt = rndstr()
             try:
                 authn_event = _context.session_manager.get_authentication_event(session_id)
@@ -1078,19 +1084,19 @@
         """The AuthorizationRequest endpoint
 
         :param http_info: Information on the HTTP request
         :param request: The authorization request as a Message instance
         :return: dictionary
         """
 
-        if isinstance(request, self.error_cls):
+        if "error" in request:
             return request
 
         _cid = request["client_id"]
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         cinfo = _context.cdb[_cid]
         # logger.debug("client {}: {}".format(_cid, cinfo))
 
         # this applies the default option deny_unknown_scopes policy
         check_unknown_scopes_policy(request, _cid, _context)
 
         if http_info is None:
@@ -1135,17 +1141,17 @@
             return {"http_response": "Internal error: {}".format(err)}
 
 
 class AllowedAlgorithms:
     def __init__(self, algorithm_parameters):
         self.algorithm_parameters = algorithm_parameters
 
-    def __call__(self, client_id, endpoint_context, alg, alg_type):
-        _cinfo = endpoint_context.cdb[client_id]
-        _pinfo = endpoint_context.provider_info
+    def __call__(self, client_id, context, alg, alg_type):
+        _cinfo = context.cdb[client_id]
+        _pinfo = context.provider_info
 
         _reg, _sup = self.algorithm_parameters[alg_type]
         _allowed = _cinfo.get(_reg)
         if _allowed is None:
             _allowed = _pinfo.get(_sup)
 
         if alg not in _allowed:
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oauth2/introspection.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/introspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 import logging
 from typing import Optional
 
 from idpyoidc.message import oauth2
 from idpyoidc.server.endpoint import Endpoint
 from idpyoidc.server.token.exception import UnknownToken
 from idpyoidc.server.token.exception import WrongTokenClass
+from idpyoidc.server.exception import ToOld
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Introspection(Endpoint):
     """Implements RFC 7662"""
 
     request_cls = oauth2.TokenIntrospectionRequest
     response_cls = oauth2.TokenIntrospectionResponse
     request_format = "urlencoded"
     response_format = "json"
     endpoint_name = "introspection_endpoint"
     name = "introspection"
-    default_capabilities = {
+    _supports = {
         "client_authn_method": [
             "client_secret_basic",
             "client_secret_post",
             "client_secret_jwt",
             "private_key_jwt",
         ]
     }
 
-    def __init__(self, server_get, **kwargs):
-        Endpoint.__init__(self, server_get, **kwargs)
+    def __init__(self, upstream_get, **kwargs):
+        Endpoint.__init__(self, upstream_get, **kwargs)
         self.offset = kwargs.get("offset", 0)
 
     def _introspect(self, token, client_id, grant):
         # Make sure that the token is an access_token or a refresh_token
         if token.token_class not in ["access_token", "refresh_token"]:
             return None
 
@@ -47,15 +48,15 @@
                 scope = grant.find_scope(token.based_on)
             else:
                 scope = grant.scope
         aud = token.resources
         if not aud:
             aud = grant.resources
 
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         ret = {
             "active": True,
             "scope": " ".join(scope),
             "client_id": client_id,
             "token_class": token.token_class,
             "exp": token.expires_at,
             "iat": token.issued_at,
@@ -93,26 +94,33 @@
         """
         _introspect_request = self.request_cls(**request)
         if "error" in _introspect_request:
             return _introspect_request
 
         request_token = _introspect_request["token"]
         _resp = self.response_cls(active=False)
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
 
         try:
             _session_info = _context.session_manager.get_session_info_by_token(
                 request_token, grant=True
             )
-        except (UnknownToken, WrongTokenClass):
+        except (UnknownToken, WrongTokenClass, ToOld):
             return {"response_args": _resp}
 
         grant = _session_info["grant"]
         _token = grant.get_token(request_token)
 
+        aud = _token.resources
+        if not aud:
+            aud = grant.resources
+        
+        if request["client_id"] not in aud:
+            return {"response_args": _resp}
+
         _info = self._introspect(_token, _session_info["client_id"], _session_info["grant"])
         if _info is None:
             return {"response_args": _resp}
 
         if release:
             if "username" in release:
                 try:
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oauth2/pushed_authorization.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/pushed_authorization.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     endpoint_name = "pushed_authorization_request_endpoint"
     request_placement = "body"
     request_format = "urlencoded"
     response_placement = "body"
     response_format = "json"
     name = "pushed_authorization"
 
-    def __init__(self, server_get, **kwargs):
-        Authorization.__init__(self, server_get, **kwargs)
+    def __init__(self, upstream_get, **kwargs):
+        Authorization.__init__(self, upstream_get, **kwargs)
         # self.pre_construct.append(self._pre_construct)
         self.post_parse_request.append(self._post_parse_request)
         self.ttl = kwargs.get("ttl", 3600)
 
     def process_request(self, request=None, **kwargs):
         """
         Store the request and return a URI.
 
         :param request:
         """
         # create URN
 
         _urn = "urn:uuid:{}".format(uuid.uuid4())
-        self.server_get("endpoint_context").par_db[_urn] = request
+        self.upstream_get("context").par_db[_urn] = request
 
         return {
             "http_response": {"request_uri": _urn, "expires_in": self.ttl},
             "return_uri": request["redirect_uri"],
         }
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oauth2/token.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,179 @@
 import logging
 from typing import Optional
 from typing import Union
 
+from cryptojwt import BadSyntax
 from cryptojwt.jwe.exception import JWEException
+from cryptojwt.jws.exception import NoSuitableSigningKeys
+from cryptojwt.jwt import utc_time_sans_frac
 
 from idpyoidc.message import Message
-from idpyoidc.message.oauth2 import AccessTokenResponse
-from idpyoidc.message.oauth2 import ResponseMessage
-from idpyoidc.message.oauth2 import TokenExchangeRequest
-from idpyoidc.message.oidc import TokenErrorResponse
-from idpyoidc.server.constant import DEFAULT_REQUESTED_TOKEN_TYPE
-from idpyoidc.server.endpoint import Endpoint
-from idpyoidc.server.exception import ProcessError
-from idpyoidc.server.oauth2.token_helper import AccessTokenHelper
-from idpyoidc.server.oauth2.token_helper import RefreshTokenHelper
-from idpyoidc.server.oauth2.token_helper import TokenExchangeHelper
-from idpyoidc.server.session import MintingNotAllowed
-from idpyoidc.server.session.token import TOKEN_TYPES_MAPPING
-from idpyoidc.util import importer
+from idpyoidc.message.oidc import RefreshAccessTokenRequest
+from idpyoidc.server.oauth2.token_helper import TokenEndpointHelper
+from idpyoidc.server.session.token import AuthorizationCode
+from idpyoidc.server.session.token import MintingNotAllowed
+from idpyoidc.server.session.token import RefreshToken
+from idpyoidc.server.token.exception import UnknownToken
+from idpyoidc.util import sanitize
 
 logger = logging.getLogger(__name__)
 
+class RefreshTokenHelper(TokenEndpointHelper):
 
-class Token(Endpoint):
-    request_cls = Message
-    response_cls = AccessTokenResponse
-    error_cls = TokenErrorResponse
-    request_format = "json"
-    request_placement = "body"
-    response_format = "json"
-    response_placement = "body"
-    endpoint_name = "token_endpoint"
-    name = "token"
-    default_capabilities = {"token_endpoint_auth_signing_alg_values_supported": None}
-    helper_by_grant_type = {
-        "authorization_code": AccessTokenHelper,
-        "refresh_token": RefreshTokenHelper,
-    }
-
-    def __init__(self, server_get, new_refresh_token=False, **kwargs):
-        Endpoint.__init__(self, server_get, **kwargs)
-        self.post_parse_request.append(self._post_parse_request)
-        self.allow_refresh = False
-        self.new_refresh_token = new_refresh_token
-        self.configure_grant_types(kwargs.get("grant_types_helpers"))
-        self.grant_types_supported = kwargs.get("grant_types_supported", list(self.helper.keys()))
-        self.revoke_refresh_on_issue = kwargs.get("revoke_refresh_on_issue", False)
-
-    def configure_grant_types(self, grant_types_helpers):
-        if grant_types_helpers is None:
-            self.helper = {k: v(self) for k, v in self.helper_by_grant_type.items()}
-            return
-
-        self.helper = {}
-        # TODO: do we want to allow any grant_type?
-        for grant_type, grant_type_options in grant_types_helpers.items():
-            _conf = grant_type_options.get("kwargs", {})
-            if _conf is False:
-                continue
+    def process_request(self, req: Union[Message, dict], **kwargs):
+        _context = self.endpoint.upstream_get("context")
+        _mngr = _context.session_manager
 
+        if req["grant_type"] != "refresh_token":
+            return self.error_cls(error="invalid_request", error_description="Wrong grant_type")
+
+        token_value = req["refresh_token"]
+
+        _session_info = _mngr.get_session_info_by_token(
+            token_value, handler_key="refresh_token", grant=True
+        )
+        if _session_info["client_id"] != req["client_id"]:
+            logger.debug("{} owner of token".format(_session_info["client_id"]))
+            logger.warning("{} using token it was not given".format(req["client_id"]))
+            return self.error_cls(error="invalid_grant", error_description="Wrong client")
+
+        _grant = _session_info["grant"]
+
+        token_type = "Bearer"
+
+        # Is DPOP supported
+        if "dpop_signing_alg_values_supported" in _context.provider_info:
+            _dpop_jkt = req.get("dpop_jkt")
+            if _dpop_jkt:
+                _grant.extra["dpop_jkt"] = _dpop_jkt
+                token_type = "DPoP"
+
+        token = _grant.get_token(token_value)
+        scope = _grant.find_scope(token.based_on)
+        if "scope" in req:
+            scope = req["scope"]
+        access_token = self._mint_token(
+            token_class="access_token",
+            grant=_grant,
+            session_id=_session_info["branch_id"],
+            client_id=_session_info["client_id"],
+            based_on=token,
+            scope=scope,
+            token_type=token_type,
+        )
+
+        _resp = {
+            "access_token": access_token.value,
+            "token_type": token_type,
+            "scope": scope,
+        }
+
+        if access_token.expires_at:
+            _resp["expires_in"] = access_token.expires_at - utc_time_sans_frac()
+
+        _mints = token.usage_rules.get("supports_minting")
+
+        issue_refresh = kwargs.get("issue_refresh", None)
+        # The existence of offline_access scope overwrites issue_refresh
+        if issue_refresh is None and "offline_access" in scope:
+            issue_refresh = True
+
+        if "refresh_token" in _mints and issue_refresh:
+            refresh_token = self._mint_token(
+                token_class="refresh_token",
+                grant=_grant,
+                session_id=_session_info["branch_id"],
+                client_id=_session_info["client_id"],
+                based_on=token,
+                scope=scope,
+            )
+            refresh_token.usage_rules = token.usage_rules.copy()
+            _resp["refresh_token"] = refresh_token.value
+
+        if "id_token" in _mints and "openid" in scope:
             try:
-                grant_class = grant_type_options["class"]
-            except (KeyError, TypeError):
-                raise ProcessError(
-                    "Token Endpoint's grant types must be True, None or a dict with a"
-                    " 'class' key."
+                _idtoken = self._mint_token(
+                    token_class="id_token",
+                    grant=_grant,
+                    session_id=_session_info["branch_id"],
+                    client_id=_session_info["client_id"],
+                    based_on=token,
+                    scope=scope,
+                )
+            except (JWEException, NoSuitableSigningKeys) as err:
+                logger.warning(str(err))
+                resp = self.error_cls(
+                    error="invalid_request",
+                    error_description="Could not sign/encrypt id_token",
                 )
+                return resp
 
-            if isinstance(grant_class, str):
-                try:
-                    grant_class = importer(grant_class)
-                except (ValueError, AttributeError):
-                    raise ProcessError(
-                        f"Token Endpoint's grant type class {grant_class} can't" " be imported."
-                    )
+            _resp["id_token"] = _idtoken.value
 
-            try:
-                self.helper[grant_type] = grant_class(self, _conf)
-            except Exception as e:
-                raise ProcessError(f"Failed to initialize class {grant_class}: {e}")
+        token.register_usage()
 
-    def _post_parse_request(
-        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
-    ):
-        grant_type = request["grant_type"]
-        _helper = self.helper.get(grant_type)
-        client = kwargs["endpoint_context"].cdb[client_id]
-        grant_types_supported = client.get("grant_types_supported", self.grant_types_supported)
-        if grant_type not in grant_types_supported:
-            return self.error_cls(
-                error="invalid_request",
-                error_description=f"Unsupported grant_type: {grant_type}",
-            )
-        if _helper:
-            return _helper.post_parse_request(request, client_id, **kwargs)
+        if (
+                "client_id" in req
+                and req["client_id"] in _context.cdb
+                and "revoke_refresh_on_issue" in _context.cdb[req["client_id"]]
+        ):
+            revoke_refresh = _context.cdb[req["client_id"]].get("revoke_refresh_on_issue")
         else:
-            return self.error_cls(
-                error="invalid_request",
-                error_description=f"Unsupported grant_type: {grant_type}",
-            )
+            revoke_refresh = self.endpoint.revoke_refresh_on_issue
+
+        if revoke_refresh:
+            token.revoke()
 
-    def process_request(self, request: Optional[Union[Message, dict]] = None, **kwargs):
+        return _resp
+
+    def post_parse_request(
+            self,
+            request: Union[Message, dict],
+            client_id: Optional[str] = "",
+            **kwargs
+    ):
         """
+        This is where clients come to refresh their access tokens
 
-        :param request:
-        :param kwargs:
-        :return: Dictionary with response information
+        :param request: The request
+        :param client_id: Client identifier
+        :returns:
         """
-        if isinstance(request, self.error_cls):
-            return request
 
-        if request is None:
-            return self.error_cls(error="invalid_request")
+        request = RefreshAccessTokenRequest(**request.to_dict())
+        _context = self.endpoint.upstream_get("context")
 
+        request.verify(keyjar=self.endpoint.upstream_get('attribute', 'keyjar'),
+                       opponent_id=client_id)
+
+        _mngr = _context.session_manager
         try:
-            _helper = self.helper.get(request["grant_type"])
-            if _helper:
-                response_args = _helper.process_request(request, **kwargs)
-            else:
-                return self.error_cls(
-                    error="invalid_request",
-                    error_description=f"Unsupported grant_type: {request['grant_type']}",
-                )
-        except JWEException as err:
-            return self.error_cls(error="invalid_request", error_description="%s" % err)
-        except MintingNotAllowed as err:
-            return self.error_cls(error="invalid_request", error_description="%s" % err)
+            _session_info = _mngr.get_session_info_by_token(
+                request["refresh_token"], handler_key="refresh_token", grant=True
+            )
+        except (KeyError, UnknownToken, BadSyntax):
+            logger.error("Refresh token invalid")
+            return self.error_cls(error="invalid_grant", error_description="Invalid refresh token")
 
-        if isinstance(response_args, ResponseMessage):
-            return response_args
+        grant = _session_info["grant"]
+        token = grant.get_token(request["refresh_token"])
 
-        _access_token = response_args["access_token"]
-        _context = self.server_get("endpoint_context")
+        if not isinstance(token, RefreshToken):
+            return self.error_cls(error="invalid_request", error_description="Wrong token type")
 
-        if isinstance(_helper, TokenExchangeHelper):
-            _handler_key = _helper.get_handler_key(request, _context)
-        else:
-            _handler_key = "access_token"
+        if token.is_active() is False:
+            return self.error_cls(
+                error="invalid_request", error_description="Refresh token inactive"
+            )
 
-        _session_info = _context.session_manager.get_session_info_by_token(
-            _access_token, grant=True, handler_key=_handler_key
-        )
+        if "scope" in request:
+            req_scopes = set(request["scope"])
+            scopes = set(grant.find_scope(token.based_on))
+            if not req_scopes.issubset(scopes):
+                return self.error_cls(
+                    error="invalid_request",
+                    error_description="Invalid refresh scopes",
+                )
 
-        _cookie = _context.new_cookie(
-            name=_context.cookie_handler.name["session"],
-            sub=_session_info["grant"].sub,
-            sid=_context.session_manager.session_key(
-                _session_info["user_id"],
-                _session_info["client_id"],
-                _session_info["grant"].id,
-            ),
-        )
+        return request
 
-        _headers = [("Content-type", "application/json")]
-        resp = {"response_args": response_args, "http_headers": _headers}
-        if _cookie:
-            resp["cookie"] = [_cookie]
-        return resp
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         "The custom_scopes add on is deprecated. The `scopes_to_claims` config "
         "option should be used instead."
     )
     _endpoint = list(endpoint.values())[0]
 
     _scopes2claims = SCOPE2CLAIMS.copy()
     _scopes2claims.update(kwargs)
-    _context = _endpoint.server_get("endpoint_context")
+    _context = _endpoint.upstream_get("context")
     _context.scopes_handler.set_scopes_mapping(_scopes2claims)
 
     pi = _context.provider_info
     _scopes = set(pi.get("scopes_supported", []))
     _scopes.update(set(kwargs.keys()))
     pi["scopes_supported"] = list(_scopes)
     _context.scopes_handler.allowed_scopes = pi["scopes_supported"]
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/add_on/pkce.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/pkce.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict
 
 from cryptojwt.utils import b64e
 
 from idpyoidc.message.oauth2 import AuthorizationErrorResponse
 from idpyoidc.message.oauth2 import RefreshAccessTokenRequest
 from idpyoidc.message.oauth2 import TokenExchangeRequest
+from idpyoidc.message.oauth2 import CCAccessTokenRequest
 from idpyoidc.message.oidc import TokenErrorResponse
 from idpyoidc.server.endpoint import Endpoint
 
 LOGGER = logging.getLogger(__name__)
 
 
 def hash_fun(f):
@@ -26,40 +27,40 @@
     "plain": lambda x: x,
     "S256": hash_fun(hashlib.sha256),
     "S384": hash_fun(hashlib.sha384),
     "S512": hash_fun(hashlib.sha512),
 }
 
 
-def post_authn_parse(request, client_id, endpoint_context, **kwargs):
+def post_authn_parse(request, client_id, context, **kwargs):
     """
 
     :param request:
     :param client_id:
-    :param endpoint_context:
+    :param context:
     :param kwargs:
     :return:
     """
-    client = endpoint_context.cdb[client_id]
+    client = context.cdb[client_id]
     if "pkce_essential" in client:
         essential = client["pkce_essential"]
     else:
-        essential = endpoint_context.args["pkce"].get("essential", False)
+        essential = context.args["pkce"].get("essential", False)
     if essential and "code_challenge" not in request:
         return AuthorizationErrorResponse(
             error="invalid_request",
             error_description="Missing required code_challenge",
         )
 
     if "code_challenge_method" not in request:
-        request["code_challenge_method"] = "plain"
+        request["code_challenge_method"] = "S256"
 
     if "code_challenge" in request and (
         request["code_challenge_method"]
-        not in endpoint_context.args["pkce"]["code_challenge_methods"]
+        not in context.args["pkce"]["code_challenge_methods"]
     ):
         return AuthorizationErrorResponse(
             error="invalid_request",
             error_description="Unsupported code_challenge_method={}".format(
                 request["code_challenge_method"]
             ),
         )
@@ -80,29 +81,29 @@
         LOGGER.error("PKCE Code Challenge check failed")
         return False
 
     LOGGER.debug("PKCE Code Challenge check succeeded")
     return True
 
 
-def post_token_parse(request, client_id, endpoint_context, **kwargs):
+def post_token_parse(request, client_id, context, **kwargs):
     """
     To be used as a post_parse_request function.
 
     :param token_request:
     :return:
     """
     if isinstance(
         request,
-        (AuthorizationErrorResponse, RefreshAccessTokenRequest, TokenExchangeRequest),
+        (AuthorizationErrorResponse, RefreshAccessTokenRequest, TokenExchangeRequest, CCAccessTokenRequest),
     ):
         return request
 
     try:
-        _session_info = endpoint_context.session_manager.get_session_info_by_token(
+        _session_info = context.session_manager.get_session_info_by_token(
             request["code"], grant=True, handler_key="authorization_code"
         )
     except KeyError:
         return TokenErrorResponse(error="invalid_grant", error_description="Unknown access grant")
 
     _authn_req = _session_info["grant"].authorization_request
 
@@ -136,15 +137,25 @@
         LOGGER.warning("No token endpoint found, skipping PKCE configuration")
         return
 
     authn_endpoint.post_parse_request.append(post_authn_parse)
     token_endpoint.post_parse_request.append(post_token_parse)
 
     code_challenge_methods = kwargs.get("code_challenge_methods", CC_METHOD.keys())
-
+    code_challenge_methods = list(
+        set(code_challenge_methods).intersection(
+            authn_endpoint._supports["code_challenge_methods_supported"]
+        )
+    )
+    if not code_challenge_methods:
+        raise ValueError(
+            "Unsupported method: {}".format(
+                ", ".join(kwargs.get("code_challenge_methods", CC_METHOD.keys()))
+            )
+        )
     kwargs["code_challenge_methods"] = {}
     for method in code_challenge_methods:
         if method not in CC_METHOD:
             raise ValueError("Unsupported method: {}".format(method))
         kwargs["code_challenge_methods"][method] = CC_METHOD[method]
 
-    authn_endpoint.server_get("endpoint_context").args["pkce"] = kwargs
+    authn_endpoint.upstream_get("context").args["pkce"] = kwargs
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/authorization.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/authorization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import Callable
 from urllib.parse import urlsplit
 
+from idpyoidc import claims
 from idpyoidc.message import oidc
 from idpyoidc.message.oidc import Claims
 from idpyoidc.message.oidc import verified_claim_name
 from idpyoidc.server.oauth2 import authorization
 
 logger = logging.getLogger(__name__)
 
@@ -70,48 +71,41 @@
     response_cls = oidc.AuthorizationResponse
     error_cls = oidc.AuthorizationErrorResponse
     request_format = "urlencoded"
     response_format = "urlencoded"
     response_placement = "url"
     endpoint_name = "authorization_endpoint"
     name = "authorization"
-    provider_info_attributes = {
-        "claims_parameter_supported": True,
-        "client_authn_method": ["request_param", "public"],
-        "request_parameter_supported": True,
-        "request_uri_parameter_supported": True,
-        "response_types_supported": [
-            "code",
-            "token",
-            "id_token",
-            "code token",
-            "code id_token",
-            "id_token token",
-            "code id_token token",
-        ],
-        "response_modes_supported": ["query", "fragment", "form_post"],
-        "request_object_signing_alg_values_supported": None,
-        "request_object_encryption_alg_values_supported": None,
-        "request_object_encryption_enc_values_supported": None,
-        "grant_types_supported": ["authorization_code", "implicit"],
-        "claim_types_supported": ["normal", "aggregated", "distributed"],
-    }
-    default_capabilities = {
-        "client_authn_method": ["request_param", "public"],
+
+    _supports = {
+        **authorization.Authorization._supports,
+        **{
+            "claims_parameter_supported": True,
+            "encrypt_request_object_supported": False,
+            "request_object_signing_alg_values_supported": claims.get_signing_algs,
+            "request_object_encryption_alg_values_supported": claims.get_encryption_algs,
+            "request_object_encryption_enc_values_supported": claims.get_encryption_encs,
+            "request_parameter_supported": True,
+            "request_uri_parameter_supported": True,
+            "require_request_uri_registration": False,
+            "response_types_supported": ["code", "token", "code token", 'id_token', 'id_token token',
+                                     'code id_token', 'code id_token token'],
+            "response_modes_supported": ['query', 'fragment', 'form_post'],
+            "subject_types_supported": ["public", "pairwise", "ephemeral"],
+          },
     }
 
-    def __init__(self, server_get: Callable, **kwargs):
-        authorization.Authorization.__init__(self, server_get, **kwargs)
-        # self.pre_construct.append(self._pre_construct)
+    def __init__(self, upstream_get: Callable, **kwargs):
+        authorization.Authorization.__init__(self, upstream_get, **kwargs)
         self.post_parse_request.append(self._do_request_uri)
         self.post_parse_request.append(self._post_parse_request)
 
     def do_request_user(self, request_info, **kwargs):
         if proposed_user(request_info):
             kwargs["req_user"] = proposed_user(request_info)
         else:
             _login_hint = request_info.get("login_hint")
             if _login_hint:
-                _context = self.server_get("endpoint_context")
+                _context = self.upstream_get("context")
                 if _context.login_hint_lookup:
                     kwargs["req_user"] = _context.login_hint_lookup(_login_hint)
         return kwargs
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/backchannel_authentication.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/backchannel_authentication.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import logging
-import uuid
 from typing import Callable
 from typing import Optional
 from typing import Union
+import uuid
 
 from cryptojwt.jwe.exception import JWEException
 from cryptojwt.jws.exception import NoSuitableSigningKeys
 from cryptojwt.jwt import utc_time_sans_frac
 
 from idpyoidc import verified_claim_name
 from idpyoidc.message import Message
 from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.message.oidc.backchannel_authentication import AuthenticationRequest
 from idpyoidc.message.oidc.backchannel_authentication import AuthenticationResponse
 from idpyoidc.server import Endpoint
-from idpyoidc.server import EndpointContext
 from idpyoidc.server.client_authn import ClientSecretBasic
 from idpyoidc.server.exception import NoSuchAuthentication
-from idpyoidc.server.oidc.token_helper import AccessTokenHelper
+from idpyoidc.server.oidc.token_helper.access_token import AccessTokenHelper
 from idpyoidc.server.session.token import MintingNotAllowed
 from idpyoidc.server.util import execute
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_EXPIRES_IN = 120
 DEFAULT_INTERVAL = 2
@@ -32,22 +31,23 @@
     response_cls = AuthenticationResponse
     error_cls = ResponseMessage
     request_format = "urlencoded"
     response_format = "urlencoded"
     response_placement = "url"
     endpoint_name = "backchannel_authentication_endpoint"
     name = "backchannel_authentication"
-    provider_info_attributes = {
+
+    _supports = {
         "backchannel_token_delivery_modes_supported": ["poll", "ping", "push"],
         "backchannel_authentication_request_signing_alg_values_supported": None,
         "backchannel_user_code_parameter_supported": True,
     }
 
-    def __init__(self, server_get: Callable, **kwargs):
-        Endpoint.__init__(self, server_get, **kwargs)
+    def __init__(self, upstream_get: Callable, **kwargs):
+        Endpoint.__init__(self, upstream_get, **kwargs)
         # self.pre_construct.append(self._pre_construct)
         # self.post_parse_request.append(self._do_request_uri)
         # self.post_parse_request.append(self._post_parse_request)
         self.parse_login_hint_token = kwargs.get("parse_login_hint_token")
         self.expires_in = kwargs.get("expires_in", DEFAULT_EXPIRES_IN)
         self.interval = kwargs.get("interval", DEFAULT_INTERVAL)
 
@@ -55,56 +55,56 @@
         cn = verified_claim_name("id_token_hint")
         _request_user = ""
         if request.get(cn):
             _request_user = request[cn].get("sub", "")
         elif request.get("login_hint"):
             _login_hint = request.get("login_hint")
             if _login_hint:
-                _context = self.server_get("endpoint_context")
+                _context = self.upstream_get("context")
                 if _context.login_hint_lookup:
                     _request_user = _context.login_hint_lookup(_login_hint)
         elif request.get("login_hint_token"):
-            _context = self.server_get("endpoint_context")
+            _context = self.upstream_get("context")
             _request_user = execute(
                 self.parse_login_hint_token,
-                keyjar=_context.keyjar,
+                keyjar=self.upstream_get('attribute', 'keyjar'),
                 login_hint_token=request.get("login_hint_token"),
                 context=_context,
             )
 
         return _request_user
 
     def allowed_target_uris(self):
         """
         The OP MUST accept its Issuer Identifier, Token Endpoint URL, or Backchannel
         Authentication Endpoint URL as values that identify it as an intended audience.
         """
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         res = [_context.issuer]
         res.append(self.full_path)
-        res.append(self.server_get("endpoint", "token").full_path)
+        res.append(self.upstream_get("endpoint", "token").full_path)
         return set(res)
 
     def process_request(
-        self,
-        request: Optional[Union[Message, dict]] = None,
-        http_info: Optional[dict] = None,
-        **kwargs,
+            self,
+            request: Optional[Union[Message, dict]] = None,
+            http_info: Optional[dict] = None,
+            **kwargs,
     ):
         try:
             request_user = self.do_request_user(request)
         except KeyError:
             logger.error("Login hint didn't lead to a known user")
             _error_msg = self.error_cls(
                 error="invalid_request", error_description="Login hint didn't lead to a known user"
             )
             return _error_msg
 
         if request_user:  # Got a request for a legitimate user, create a session
-            _context = self.server_get("endpoint_context")
+            _context = self.upstream_get("context")
             _sid = _context.session_manager.create_session(
                 None, request, request_user, client_id=request["client_id"]
             )
 
             auth_req_id = uuid.uuid4().hex
             _context.session_manager.auth_req_id_map[auth_req_id] = _sid
 
@@ -132,17 +132,17 @@
             "client_id": _path[1],
             "grant_id": _path[2],
             "session_id": request["_session_id"],
         }
         return session_info, _grant
 
     def post_parse_request(
-        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ) -> Union[Message, dict]:
-        _context = self.endpoint.server_get("endpoint_context")
+        _context = self.endpoint.upstream_get("context")
         _mngr = _context.session_manager
         _session_id = _mngr.auth_req_id_map[request["auth_req_id"]]
         _info = _mngr.get_session_info(_session_id)
         # There should be 2 grants for the user_id, client_id combination
         # one without authentication information, the other one with
         logger.debug(f"Session info: {_info}")
         # There should be zero or one
@@ -175,15 +175,15 @@
     def process_request(self, req: Union[Message, dict], **kwargs):
         """
 
         :param req:
         :param kwargs:
         :return:
         """
-        _context = self.endpoint.server_get("endpoint_context")
+        _context = self.endpoint.upstream_get("context")
 
         _mngr = _context.session_manager
         logger.debug("OIDC Access Token")
 
         _session_info, grant = self._get_session_info(req, _mngr)
 
         logger.debug(f"Session info: {_session_info}")
@@ -294,22 +294,22 @@
     request_format = "json"
     endpoint_name = "client_notification_endpoint"
     name = "client_notification"
     provider_info_attributes = {
         "backchannel_client_notification_endpoint": None,
     }
 
-    def __init__(self, server_get: Callable, **kwargs):
-        Endpoint.__init__(self, server_get, **kwargs)
+    def __init__(self, upstream_get: Callable, **kwargs):
+        Endpoint.__init__(self, upstream_get, **kwargs)
 
     def process_request(
-        self,
-        request: Optional[Union[Message, dict]] = None,
-        http_info: Optional[dict] = None,
-        **kwargs,
+            self,
+            request: Optional[Union[Message, dict]] = None,
+            http_info: Optional[dict] = None,
+            **kwargs,
     ) -> Union[Message, dict]:
         return {}
 
 
 class ClientNotificationAuthn(ClientSecretBasic):
     """The authentication method used at the notification endpoint."""
 
@@ -317,21 +317,19 @@
 
     def is_usable(self, request=None, authorization_token=None):
         if authorization_token is not None and authorization_token.startswith("Bearer "):
             return True
         return False
 
     def _verify(
-        self,
-        endpoint_context: EndpointContext,
-        request: Optional[Union[dict, Message]] = None,
-        authorization_token: Optional[str] = None,
-        endpoint=None,  # Optional[Endpoint]
-        get_client_id_from_token: Optional[Callable] = None,
-        **kwargs,
+            self,
+            authorization_token: Optional[str] = None,
+            endpoint=None,  # Optional[Endpoint]
+            get_client_id_from_token: Optional[Callable] = None,
+            **kwargs,
     ):
         ttype, token = authorization_token.split(" ", 1)
         if ttype != "Bearer":
             raise NoSuchAuthentication(f"No support for {ttype}")
         if get_client_id_from_token:
             client_id = get_client_id_from_token(token)
         else:
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/discovery.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/discovery.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,9 +33,9 @@
         }
 
         return info
 
     def process_request(self, request=None, **kwargs):
         return {
             "subject": request["resource"],
-            "hrefs": [self.server_get("endpoint_context").issuer],
+            "hrefs": [self.upstream_get("context").issuer],
         }
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/read_registration.py` & `idpyoidc-2.0.0/src/idpyoidc/client/provider/linkedin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,43 @@
+from idpyoidc.client.oauth2 import access_token
+from idpyoidc.client.oidc import userinfo
+from idpyoidc.client.client_auth import get_client_authn_methods
 from idpyoidc.message import Message
-from idpyoidc.message.oauth2 import ResponseMessage
-from idpyoidc.message.oidc import RegistrationResponse
-from idpyoidc.server.endpoint import Endpoint
-from idpyoidc.server.oidc.registration import comb_uri
-
-
-class RegistrationRead(Endpoint):
-    request_cls = Message
-    response_cls = RegistrationResponse
-    error_response = ResponseMessage
-    request_format = "urlencoded"
-    request_placement = "url"
-    response_format = "json"
-    name = "registration_read"
-
-    def get_client_id_from_token(self, endpoint_context, token, request=None):
-        if "client_id" in request:
-            if (
-                request["client_id"]
-                == self.server_get("endpoint_context").registration_access_token[token]
-            ):
-                return request["client_id"]
-        return ""
-
-    def process_request(self, request=None, **kwargs):
-        _cli_info = self.server_get("endpoint_context").cdb[request["client_id"]]
-        args = {k: v for k, v in _cli_info.items() if k in RegistrationResponse.c_param}
-        comb_uri(args)
-        return {"response_args": RegistrationResponse(**args)}
+from idpyoidc.message import SINGLE_OPTIONAL_JSON
+from idpyoidc.message import SINGLE_OPTIONAL_STRING
+from idpyoidc.message import SINGLE_REQUIRED_INT
+from idpyoidc.message import SINGLE_REQUIRED_STRING
+from idpyoidc.message import oauth2
+from idpyoidc.claims import get_signing_algs
+
+
+class AccessTokenResponse(Message):
+    """
+    Access token response
+    """
+
+    c_param = {"access_token": SINGLE_REQUIRED_STRING, "expires_in": SINGLE_REQUIRED_INT}
+
+
+class UserSchema(Message):
+    c_param = {
+        "firstName": SINGLE_OPTIONAL_STRING,
+        "headline": SINGLE_OPTIONAL_STRING,
+        "id": SINGLE_REQUIRED_STRING,
+        "lastName": SINGLE_OPTIONAL_STRING,
+        "siteStandardProfileRequest": SINGLE_OPTIONAL_JSON,
+    }
+
+
+class AccessToken(access_token.AccessToken):
+    msg_type = oauth2.AccessTokenRequest
+    response_cls = AccessTokenResponse
+    error_msg = oauth2.TokenErrorResponse
+
+    _supports = {
+        "token_endpoint_auth_methods_supported": get_client_authn_methods,
+        "token_endpoint_auth_signing_alg_values_supported": get_signing_algs
+    }
+
+
+class UserInfo(userinfo.UserInfo):
+    response_cls = UserSchema
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/registration.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/registration.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,33 +21,14 @@
 from idpyoidc.server.exception import InvalidSectorIdentifier
 from idpyoidc.time_util import utc_time_sans_frac
 from idpyoidc.util import importer
 from idpyoidc.util import rndstr
 from idpyoidc.util import sanitize
 from idpyoidc.util import split_uri
 
-PREFERENCE2PROVIDER = {
-    # "require_signed_request_object": "request_object_algs_supported",
-    "request_object_signing_alg": "request_object_signing_alg_values_supported",
-    "request_object_encryption_alg": "request_object_encryption_alg_values_supported",
-    "request_object_encryption_enc": "request_object_encryption_enc_values_supported",
-    "userinfo_signed_response_alg": "userinfo_signing_alg_values_supported",
-    "userinfo_encrypted_response_alg": "userinfo_encryption_alg_values_supported",
-    "userinfo_encrypted_response_enc": "userinfo_encryption_enc_values_supported",
-    "id_token_signed_response_alg": "id_token_signing_alg_values_supported",
-    "id_token_encrypted_response_alg": "id_token_encryption_alg_values_supported",
-    "id_token_encrypted_response_enc": "id_token_encryption_enc_values_supported",
-    "default_acr_values": "acr_values_supported",
-    "subject_type": "subject_types_supported",
-    "token_endpoint_auth_method": "token_endpoint_auth_methods_supported",
-    "token_endpoint_auth_signing_alg": "token_endpoint_auth_signing_alg_values_supported",
-    "response_types": "response_types_supported",
-    "grant_types": "grant_types_supported",
-}
-
 logger = logging.getLogger(__name__)
 
 
 def match_sp_sep(first, second):
     """
     Verify that all the values in 'first' appear in 'second'.
     The values can either be in the form of lists or as space separated
@@ -120,63 +101,97 @@
             if frag:
                 val.append("{}#{}".format(base, frag))
             else:
                 val.append(base)
         args["request_uris"] = val
 
 
-def random_client_id(length: int = 16, reserved: list = [], **kwargs):
+def random_client_id(length: int = 16, reserved: list = None, **kwargs):
     # create new id och secret
     client_id = rndstr(16)
     # cdb client_id MUST be unique!
-    while client_id in reserved:
-        client_id = rndstr(16)
+    if reserved:
+        while client_id in reserved:
+            client_id = rndstr(16)
     return client_id
 
 
 class Registration(Endpoint):
     request_cls = RegistrationRequest
     response_cls = RegistrationResponse
     error_response = ClientRegistrationErrorResponse
     request_format = "json"
     request_placement = "body"
     response_format = "json"
     endpoint_name = "registration_endpoint"
     name = "registration"
 
-    # default
-    # response_placement = 'body'
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Those that use seed wants bytes but I can only store str.
         # seed
         _seed = kwargs.get("seed") or rndstr(32)
         self.seed = as_bytes(_seed)
 
-    def match_client_request(self, request):
-        _context = self.server_get("endpoint_context")
-        for _pref, _prov in PREFERENCE2PROVIDER.items():
-            if _pref in request:
-                if _pref in ["response_types", "default_acr_values"]:
-                    if not match_sp_sep(request[_pref], _context.provider_info[_prov]):
-                        raise CapabilitiesMisMatch(_pref)
+    def match_claim(self, claim, val):
+        _context = self.upstream_get("context")
+
+        # Use my defaults
+        _my_key = _context.claims.register2preferred.get(claim, claim)
+        try:
+            _val = _context.provider_info[_my_key]
+        except KeyError:
+            return val
+
+        try:
+            _claim_spec = _context.claims.registration_response.c_param[claim]
+        except KeyError:  # something I don't know anything about
+            return None
+
+        if _val:
+            if isinstance(_claim_spec[0], list):
+                if isinstance(val, str):
+                    if val in _val:
+                        return val
+                    else:
+                        return None
                 else:
-                    if isinstance(request[_pref], str):
-                        if request[_pref] not in _context.provider_info[_prov]:
-                            raise CapabilitiesMisMatch(_pref)
+                    _ret = list(set(_val).intersection(set(val)))
+                    if len(_ret) > 0:
+                        return _ret
                     else:
-                        if not set(request[_pref]).issubset(set(_context.provider_info[_prov])):
-                            raise CapabilitiesMisMatch(_pref)
+                        raise CapabilitiesMisMatch(_my_key)
+            else:
+                if val == _val:
+                    return val
+                else:
+                    return None
+        else:
+            return None
+
+    def filter_client_request(self, request: dict) -> dict:
+        _args = {}
+        _context = self.upstream_get("context")
+        for key, val in request.items():
+            if key not in _context.claims.register2preferred:
+                _args[key] = val
+                continue
+
+            _val = self.match_claim(key, val)
+            if _val:
+                _args[key] = _val
+            else:
+                logger.error(f"Capabilities mismatch: {key}={val} not supported")
+        return _args
 
     def do_client_registration(self, request, client_id, ignore=None):
         if ignore is None:
             ignore = []
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         _cinfo = _context.cdb[client_id].copy()
         logger.debug("_cinfo: %s" % sanitize(_cinfo))
 
         for key, val in request.items():
             if key not in ignore:
                 _cinfo[key] = val
 
@@ -231,44 +246,44 @@
                     _cinfo[item] = request[item]
                 else:
                     return ResponseMessage(
                         error="invalid_configuration_parameter",
                         error_description="%s pointed to illegal URL" % item,
                     )
 
+        _keyjar = self.upstream_get('attribute', 'keyjar')
         # Do I have the necessary keys
         for item in ["id_token_signed_response_alg", "userinfo_signed_response_alg"]:
             if item in request:
-                if request[item] in _context.provider_info[PREFERENCE2PROVIDER[item]]:
+                if request[item] in _context.provider_info[
+                        _context.claims.register2preferred[item]]:
                     ktyp = alg2keytype(request[item])
                     # do I have this ktyp and for EC type keys the curve
                     if ktyp not in ["none", "oct"]:
                         _k = []
                         for iss in ["", _context.issuer]:
                             _k.extend(
-                                _context.keyjar.get_signing_key(
-                                    ktyp, alg=request[item], issuer_id=iss
-                                )
+                                _keyjar.get_signing_key(ktyp, alg=request[item], issuer_id=iss)
                             )
                         if not _k:
                             logger.warning('Lacking support for "{}"'.format(request[item]))
                             del _cinfo[item]
 
         t = {"jwks_uri": "", "jwks": None}
 
         for item in ["jwks_uri", "jwks"]:
             if item in request:
                 t[item] = request[item]
 
         # if it can't load keys because the URL is false it will
         # just silently fail. Waiting for better times.
-        _context.keyjar.load_keys(client_id, jwks_uri=t["jwks_uri"], jwks=t["jwks"])
+        _keyjar.load_keys(client_id, jwks_uri=t["jwks_uri"], jwks=t["jwks"])
 
         n_keys = 0
-        for kb in _context.keyjar.get(client_id, []):
+        for kb in _keyjar.get(client_id, []):
             n_keys += len(kb.keys())
         msg = "found {} keys for client_id={}"
         logger.debug(msg.format(n_keys, client_id))
 
         return _cinfo
 
     @staticmethod
@@ -326,16 +341,16 @@
 
         :param request: Provider registration request
         :return: si_redirects, sector_id
         :raises: InvalidSectorIdentifier
         """
         si_url = request["sector_identifier_uri"]
         try:
-            res = self.server_get("endpoint_context").httpc.get(
-                si_url, **self.server_get("endpoint_context").httpc_params
+            res = self.upstream_get("context").httpc(
+                "GET", si_url, **self.upstream_get("context").httpc_params
             )
             logger.debug("sector_identifier_uri => %s", sanitize(res.text))
         except Exception as err:
             logger.error(err)
             # res = None
             raise InvalidSectorIdentifier("Couldn't read from sector_identifier_uri")
 
@@ -352,15 +367,15 @@
 
         return si_redirects, si_url
 
     def add_registration_api(self, cinfo, client_id, context):
         _rat = rndstr(32)
 
         cinfo["registration_access_token"] = _rat
-        endpoint = self.server_get("endpoints")
+        endpoint = self.upstream_get("endpoints")
         cinfo["registration_client_uri"] = "{}?client_id={}".format(
             endpoint["registration_read"].full_path, client_id
         )
 
         context.registration_access_token[_rat] = client_id
 
     def client_secret_expiration_time(self):
@@ -386,28 +401,29 @@
         try:
             request.verify()
         except (MessageException, ValueError) as err:
             logger.error("request.verify() error on %s", request)
             _error = "invalid_configuration_request"
             if len(err.args) > 1:
                 if err.args[1] == "initiate_login_uri":
-                    _error = "invalid_client_metadata"
+                    _error = "invalid_client_claims"
 
             return ResponseMessage(error=_error, error_description="%s" % err)
 
         request.rm_blanks()
+        _context = self.upstream_get("context")
+
         try:
-            self.match_client_request(request)
+            request = self.filter_client_request(request)
         except CapabilitiesMisMatch as err:
             return ResponseMessage(
                 error="invalid_request",
                 error_description="Don't support proposed %s" % err,
             )
 
-        _context = self.server_get("endpoint_context")
         if new_id:
             if self.kwargs.get("client_id_generator"):
                 cid_generator = importer(self.kwargs["client_id_generator"]["class"])
                 cid_gen_kwargs = self.kwargs["client_id_generator"].get("kwargs", {})
             else:
                 cid_generator = importer("idpyoidc.server.oidc.registration.random_client_id")
                 cid_gen_kwargs = {}
@@ -417,15 +433,15 @@
         else:
             client_id = request.get("client_id")
             if not client_id:
                 raise ValueError("Missing client_id")
 
         _cinfo = {"client_id": client_id, "client_salt": rndstr(8)}
 
-        if self.server_get("endpoint", "registration_read"):
+        if self.upstream_get("endpoint", "registration_read"):
             self.add_registration_api(_cinfo, client_id, _context)
 
         if new_id:
             _cinfo["client_id_issued_at"] = utc_time_sans_frac()
 
         client_secret = ""
         if set_secret:
@@ -445,15 +461,15 @@
         args = dict([(k, v) for k, v in _cinfo.items() if k in self.response_cls.c_param])
 
         comb_uri(args)
         response = self.response_cls(**args)
 
         # Add the client_secret as a symmetric key to the key jar
         if client_secret:
-            _context.keyjar.add_symmetric(client_id, str(client_secret))
+            self.upstream_get('attribute', 'keyjar').add_symmetric(client_id, str(client_secret))
 
         logger.debug("Stored updated client info in CDB under cid={}".format(client_id))
         logger.debug("ClientInfo: {}".format(_cinfo))
         _context.cdb[client_id] = _cinfo
 
         # Not all databases can be sync'ed
         if hasattr(_context.cdb, "sync") and callable(_context.cdb.sync):
@@ -472,23 +488,23 @@
             return ResponseMessage(
                 error="invalid_configuration_request", error_description="%s" % err
             )
 
         if "error" in reg_resp:
             return reg_resp
         else:
-            _context = self.server_get("endpoint_context")
+            _context = self.upstream_get("context")
             _cookie = _context.new_cookie(
                 name=_context.cookie_handler.name["register"],
                 client_id=reg_resp["client_id"],
             )
 
             return {"response_args": reg_resp, "cookie": _cookie, "response_code": 201}
 
     def process_verify_error(self, exception):
         _error = "invalid_request"
         if isinstance(exception, ValueError):
             if len(exception.args) > 1:
                 if exception.args[1] == "initiate_login_uri":
-                    _error = "invalid_client_metadata"
+                    _error = "invalid_client_claims"
 
         return self.error_cls(error=_error, error_description=f"{exception}")
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/session.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,49 +76,51 @@
     request_cls = EndSessionRequest
     response_cls = Message
     request_format = "urlencoded"
     response_format = "urlencoded"
     response_placement = "url"
     endpoint_name = "end_session_endpoint"
     name = "session"
-    provider_info_attributes = {
+
+    _supports = {
         "frontchannel_logout_supported": True,
         "frontchannel_logout_session_required": True,
         "backchannel_logout_supported": True,
         "backchannel_logout_session_required": True,
         "check_session_iframe": None,
     }
 
-    def __init__(self, server_get, **kwargs):
+    def __init__(self, upstream_get, **kwargs):
         _csi = kwargs.get("check_session_iframe")
         if _csi and not _csi.startswith("http"):
-            kwargs["check_session_iframe"] = add_path(server_get("endpoint_context").issuer, _csi)
-        Endpoint.__init__(self, server_get, **kwargs)
+            # unit since context does not exist at this point in time
+            kwargs["check_session_iframe"] = add_path(upstream_get("unit").issuer, _csi)
+        Endpoint.__init__(self, upstream_get, **kwargs)
         self.iv = as_bytes(rndstr(24))
 
     def _encrypt_sid(self, sid):
-        encrypter = AES_GCMEncrypter(key=as_bytes(self.server_get("endpoint_context").symkey))
+        encrypter = AES_GCMEncrypter(key=as_bytes(self.upstream_get("context").symkey))
         enc_msg = encrypter.encrypt(as_bytes(sid), iv=self.iv)
         return as_unicode(b64e(enc_msg))
 
     def _decrypt_sid(self, enc_msg):
         _msg = b64d(as_bytes(enc_msg))
-        encrypter = AES_GCMEncrypter(key=as_bytes(self.server_get("endpoint_context").symkey))
+        encrypter = AES_GCMEncrypter(key=as_bytes(self.upstream_get("context").symkey))
         ctx, tag = split_ctx_and_tag(_msg)
         return as_unicode(encrypter.decrypt(as_bytes(ctx), iv=self.iv, tag=as_bytes(tag)))
 
     def do_back_channel_logout(self, cinfo, sid):
         """
 
         :param cinfo: Client information
         :param sid: The session ID
         :return: Tuple with logout URI and signed logout token
         """
 
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
 
         try:
             back_channel_logout_uri = cinfo["backchannel_logout_uri"]
         except KeyError:
             return None
 
         # Create the logout token
@@ -130,28 +132,31 @@
         payload = {"sid": sid, "events": {BACK_CHANNEL_LOGOUT_EVENT: {}}}
 
         try:
             alg = cinfo["id_token_signed_response_alg"]
         except KeyError:
             alg = _context.provider_info["id_token_signing_alg_values_supported"][0]
 
-        _jws = JWT(_context.keyjar, iss=_context.issuer, lifetime=86400, sign_alg=alg)
+        _jws = JWT(self.upstream_get('attribute', 'keyjar'),
+                   iss=_context.issuer,
+                   lifetime=86400,
+                   sign_alg=alg)
         _jws.with_jti = True
         _logout_token = _jws.pack(payload=payload, recv=cinfo["client_id"])
 
         return back_channel_logout_uri, _logout_token
 
     def clean_sessions(self, usids):
         # Revoke all sessions
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         for sid in usids:
             _context.session_manager.revoke_client_session(sid)
 
     def logout_all_clients(self, sid):
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         _mngr = _context.session_manager
         _session_info = _mngr.get_session_info(sid)
 
         # Front-/Backchannel logout ?
         _cdb = _context.cdb
         _iss = _context.issuer
         _user_id = _session_info["user_id"]
@@ -212,22 +217,22 @@
         _jwt = factory(sjwt)
         if _jwt:
             if sig_alg:
                 alg = sig_alg
             else:
                 alg = self.kwargs["signing_alg"]
 
-            sign_keys = self.server_get("endpoint_context").keyjar.get_signing_key(alg2keytype(alg))
+            sign_keys = self.upstream_get('attribute', 'keyjar').get_signing_key(alg2keytype(alg))
             _info = _jwt.verify_compact(keys=sign_keys, sigalg=alg)
             return _info
         else:
             raise ValueError("Not a signed JWT")
 
     def logout_from_client(self, sid):
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         _cdb = _context.cdb
         _session_information = _context.session_manager.get_session_info(sid, grant=True)
         _client_id = _session_information["client_id"]
 
         res = {}
         if "backchannel_logout_uri" in _cdb[_client_id]:
             _spec = self.do_back_channel_logout(_cdb[_client_id], sid)
@@ -252,15 +257,15 @@
         Perform user logout
 
         :param request:
         :param http_info:
         :param kwargs:
         :return:
         """
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         _mngr = _context.session_manager
 
         if "post_logout_redirect_uri" in request:
             if "id_token_hint" not in request:
                 raise InvalidRequest("If post_logout_redirect_uri then id_token_hint is a MUST")
         _cookies = http_info.get("cookie")
         _session_info = None
@@ -333,15 +338,15 @@
             payload["state"] = request["state"]
 
         payload["redirect_uri"] = _uri
 
         logger.debug("JWS payload: {}".format(payload))
         # From me to me
         _jws = JWT(
-            _context.keyjar,
+            self.upstream_get('attribute', 'keyjar'),
             iss=_context.issuer,
             lifetime=86400,
             sign_alg=self.kwargs["signing_alg"],
         )
         sjwt = _jws.pack(payload=payload, recv=_context.issuer)
 
         location = "{}?{}".format(self.kwargs["logout_verify_url"], urlencode({"sjwt": sjwt}))
@@ -357,26 +362,26 @@
         """
 
         if not request:
             request = {}
 
         # Verify that the client is allowed to do this
         auth_info = self.client_authentication(request, http_info, **kwargs)
-        if not auth_info or auth_info["method"] == "none":
+        if not auth_info:
             pass
         elif isinstance(auth_info, ResponseMessage):
             return auth_info
         else:
             request["client_id"] = auth_info["client_id"]
             request["access_token"] = auth_info["token"]
 
         if isinstance(request, dict):
-            _context = self.server_get("endpoint_context")
+            _context = self.upstream_get("context")
             request = self.request_cls(**request)
-            if not request.verify(keyjar=_context.keyjar, sigalg=""):
+            if not request.verify(keyjar=self.upstream_get('attribute', 'keyjar'), sigalg=""):
                 raise InvalidRequest("Request didn't verify")
             # id_token_signing_alg_values_supported
             try:
                 _ith = request[verified_claim_name("id_token_hint")]
             except KeyError:
                 pass
             else:
@@ -393,21 +398,22 @@
         if alla:
             _res = self.logout_all_clients(sid=sid)
         else:
             _res = self.logout_from_client(sid=sid)
 
         bcl = _res.get("blu")
         if bcl:
-            _context = self.server_get("endpoint_context")
+            _context = self.upstream_get("context")
             # take care of Back channel logout first
             for _cid, spec in bcl.items():
                 _url, sjwt = spec
                 logger.info("logging out from {} at {}".format(_cid, _url))
 
-                res = _context.httpc.post(
+                res = _context.httpc(
+                    "POST",
                     _url,
                     data="logout_token={}".format(sjwt),
                     headers={"Content-Type": "application/x-www-form-urlencoded"},
                     **_context.httpc_params,
                 )
 
                 if res.status_code < 300:
@@ -416,14 +422,14 @@
                     logger.info("Got a %s which is acceptable", res.status_code)
                 elif res.status_code >= 400:
                     logger.info("failed to logout from {}".format(_cid))
 
         return _res["flu"].values() if _res.get("flu") else []
 
     def kill_cookies(self):
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         _handler = _context.cookie_handler
         session_mngmnt = _handler.make_cookie_content(
             value="", name=_handler.name["session_management"], max_age=-1
         )
         session = _handler.make_cookie_content(value="", name=_handler.name["session"], max_age=-1)
         return [session_mngmnt, session]
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/token.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/token.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 
+from idpyoidc import claims
+
 from idpyoidc.message import Message
 from idpyoidc.message import oidc
 from idpyoidc.message.oidc import TokenErrorResponse
 from idpyoidc.server.oauth2 import token
 from idpyoidc.server.oidc.backchannel_authentication import CIBATokenHelper
-from idpyoidc.server.oidc.token_helper import AccessTokenHelper
-from idpyoidc.server.oidc.token_helper import RefreshTokenHelper
-from idpyoidc.server.oidc.token_helper import TokenExchangeHelper
+from idpyoidc.server.oidc.token_helper.access_token import AccessTokenHelper
+from idpyoidc.server.oidc.token_helper.refresh_token import RefreshTokenHelper
+from idpyoidc.server.oidc.token_helper.token_exchange import TokenExchangeHelper
 
 logger = logging.getLogger(__name__)
 
 
 class Token(token.Token):
     request_cls = Message
     response_cls = oidc.AccessTokenResponse
@@ -19,23 +21,26 @@
     request_format = "urlencoded"
     request_placement = "body"
     response_format = "json"
     response_placement = "body"
     endpoint_name = "token_endpoint"
     name = "token"
     default_capabilities = None
-    provider_info_attributes = {
+
+    _supports = {
         "token_endpoint_auth_methods_supported": [
             "client_secret_post",
             "client_secret_basic",
             "client_secret_jwt",
             "private_key_jwt",
         ],
-        "token_endpoint_auth_signing_alg_values_supported": None,
+        "token_endpoint_auth_signing_alg_values_supported": claims.get_signing_algs,
     }
-    auth_method_attribute = "token_endpoint_auth_methods_supported"
+
     helper_by_grant_type = {
         "authorization_code": AccessTokenHelper,
         "refresh_token": RefreshTokenHelper,
         "urn:openid:params:grant-type:ciba": CIBATokenHelper,
         "urn:ietf:params:oauth:grant-type:token-exchange": TokenExchangeHelper,
     }
+
+    token_exchange_helper = TokenExchangeHelper
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/oidc/userinfo.py` & `idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/access_token.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,193 +1,203 @@
-import json
 import logging
-from datetime import datetime
-from typing import Callable
 from typing import Optional
 from typing import Union
 
-from cryptojwt.exception import MissingValue
-from cryptojwt.jwt import JWT
+from cryptojwt.jwe.exception import JWEException
+from cryptojwt.jws.exception import NoSuitableSigningKeys
 from cryptojwt.jwt import utc_time_sans_frac
 
 from idpyoidc.message import Message
-from idpyoidc.message import oidc
-from idpyoidc.message.oauth2 import ResponseMessage
-from idpyoidc.server.endpoint import Endpoint
-from idpyoidc.server.exception import ClientAuthenticationError
-from idpyoidc.server.util import OAUTH2_NOCACHE_HEADERS
+from idpyoidc.server.oauth2.token_helper import TokenEndpointHelper
+from idpyoidc.server.session.token import AuthorizationCode
+from idpyoidc.server.session.token import MintingNotAllowed
+from idpyoidc.server.token.exception import UnknownToken
+from idpyoidc.util import sanitize
 
 logger = logging.getLogger(__name__)
 
 
-class UserInfo(Endpoint):
-    request_cls = Message
-    response_cls = oidc.OpenIDSchema
-    request_format = "json"
-    response_format = "json"
-    response_placement = "body"
-    endpoint_name = "userinfo_endpoint"
-    name = "userinfo"
-    provider_info_attributes = {
-        "claim_types_supported": ["normal", "aggregated", "distributed"],
-        "userinfo_signing_alg_values_supported": None,
-        "userinfo_encryption_alg_values_supported": None,
-        "userinfo_encryption_enc_values_supported": None,
-    }
-    default_capabilities = {
-        "client_authn_method": ["bearer_header", "bearer_body"],
-    }
-
-    def __init__(self, server_get: Callable, add_claims_by_scope: Optional[bool] = True, **kwargs):
-        Endpoint.__init__(
-            self,
-            server_get,
-            add_claims_by_scope=add_claims_by_scope,
-            **kwargs,
-        )
-        # Add the issuer ID as an allowed JWT target
-        self.allowed_targets.append("")
+class AccessTokenHelper(TokenEndpointHelper):
+
+    def _get_session_info(self, request, session_manager):
+        if request["grant_type"] != "authorization_code":
+            return self.error_cls(error="invalid_request", error_description="Unknown grant_type")
 
-    def get_client_id_from_token(self, endpoint_context, token, request=None):
-        _info = endpoint_context.session_manager.get_session_info_by_token(
-            token, handler_key="access_token"
+        try:
+            _access_code = request["code"].replace(" ", "+")
+        except KeyError:  # Missing code parameter - absolutely fatal
+            return self.error_cls(error="invalid_request", error_description="Missing code")
+
+        _session_info = session_manager.get_session_info_by_token(
+            _access_code, grant=True, handler_key="authorization_code"
         )
-        return _info["client_id"]
+        logger.debug(f"Session info: {_session_info}")
+        return _session_info, _access_code
 
-    def do_response(
-        self,
-        response_args: Optional[Union[Message, dict]] = None,
-        request: Optional[Union[Message, dict]] = None,
-        client_id: Optional[str] = "",
-        **kwargs
-    ) -> dict:
-
-        if "error" in kwargs and kwargs["error"]:
-            return Endpoint.do_response(self, response_args, request, **kwargs)
-
-        _context = self.server_get("endpoint_context")
-        if not client_id:
-            raise MissingValue("client_id")
+    def process_request(self, req: Union[Message, dict], **kwargs):
+        """
 
-        # Should I return a JSON or a JWT ?
-        _cinfo = _context.cdb[client_id]
+        :param req:
+        :param kwargs:
+        :return:
+        """
+        _context = self.endpoint.upstream_get("context")
 
-        # default is not to sign or encrypt
-        try:
-            sign_alg = _cinfo["userinfo_signed_response_alg"]
-            sign = True
-        except KeyError:
-            sign_alg = ""
-            sign = False
+        _mngr = _context.session_manager
+        logger.debug("OIDC Access Token")
 
-        try:
-            enc_enc = _cinfo["userinfo_encrypted_response_enc"]
-            enc_alg = _cinfo["userinfo_encrypted_response_alg"]
-            encrypt = True
-        except KeyError:
-            encrypt = False
-            enc_alg = enc_enc = ""
-
-        if encrypt or sign:
-            _jwt = JWT(
-                _context.keyjar,
-                iss=_context.issuer,
-                sign=sign,
-                sign_alg=sign_alg,
-                encrypt=encrypt,
-                enc_enc=enc_enc,
-                enc_alg=enc_alg,
-            )
+        _session_info, _access_code = self._get_session_info(req, _mngr)
+        logger.debug(f"Session info: {_session_info}")
 
-            resp = _jwt.pack(response_args, recv=client_id)
-            content_type = "application/jwt"
-        else:
-            if isinstance(response_args, dict):
-                resp = json.dumps(response_args)
-            else:
-                resp = response_args.to_json()
-            content_type = "application/json"
+        client_id = _session_info["client_id"]
+        if client_id != req["client_id"]:
+            logger.debug("{} owner of token".format(client_id))
+            logger.warning("{} using token it was not given".format(req["client_id"]))
+            return self.error_cls(error="invalid_grant", error_description="Wrong client")
 
-        http_headers = [("Content-type", content_type)]
-        http_headers.extend(OAUTH2_NOCACHE_HEADERS)
+        if "grant_types_supported" in _context.cdb[client_id]:
+            grant_types_supported = _context.cdb[client_id].get("grant_types_supported")
+        else:
+            grant_types_supported = _context.provider_info["grant_types_supported"]
+        grant = _session_info["grant"]
 
-        return {"response": resp, "http_headers": http_headers}
+        token_type = "Bearer"
 
-    def process_request(self, request=None, **kwargs):
-        _mngr = self.server_get("endpoint_context").session_manager
+        # Is DPOP supported
         try:
-            _session_info = _mngr.get_session_info_by_token(
-                request["access_token"], grant=True, handler_key="access_token"
-            )
-        except (KeyError, ValueError):
-            return self.error_cls(error="invalid_token", error_description="Invalid Token")
-
-        _grant = _session_info["grant"]
-        token = _grant.get_token(request["access_token"])
-        # should be an access token
-        if token and token.token_class != "access_token":
-            return self.error_cls(error="invalid_token", error_description="Wrong type of token")
-
-        # And it should be valid
-        if token.is_active() is False:
-            return self.error_cls(error="invalid_token", error_description="Invalid Token")
-
-        allowed = True
-        _auth_event = _grant.authentication_event
-        # if the authenticate is still active or offline_access is granted.
-        if not _auth_event["valid_until"] >= utc_time_sans_frac():
-            logger.debug(
-                "authentication not valid: {} > {}".format(
-                    datetime.fromtimestamp(_auth_event["valid_until"]),
-                    datetime.fromtimestamp(utc_time_sans_frac()),
+            _dpop_enabled = _context.dpop_enabled
+        except AttributeError:
+            _dpop_enabled = False
+
+        if _dpop_enabled:
+            _dpop_jkt = req.get("dpop_jkt")
+            if _dpop_jkt:
+                grant.extra["dpop_jkt"] = _dpop_jkt
+                token_type = "DPoP"
+
+        _based_on = grant.get_token(_access_code)
+        _supports_minting = _based_on.usage_rules.get("supports_minting", [])
+
+        _authn_req = grant.authorization_request
+
+        # If redirect_uri was in the initial authorization request
+        # verify that the one given here is the correct one.
+        if "redirect_uri" in _authn_req:
+            if req["redirect_uri"] != _authn_req["redirect_uri"]:
+                return self.error_cls(
+                    error="invalid_request", error_description="redirect_uri mismatch"
                 )
-            )
-            allowed = False
 
-            # This has to be made more fine grained.
-            # if "offline_access" in session["authn_req"]["scope"]:
-            #     pass
-
-        if allowed:
-            _cntxt = self.server_get("endpoint_context")
-            _claims_restriction = _cntxt.claims_interface.get_claims(
-                _session_info["branch_id"], scopes=token.scope, claims_release_point="userinfo"
-            )
-            info = _cntxt.claims_interface.get_user_claims(
-                _session_info["user_id"], claims_restriction=_claims_restriction
-            )
-            info["sub"] = _grant.sub
-            if _grant.add_acr_value("userinfo"):
-                info["acr"] = _grant.authentication_event["authn_info"]
-        else:
-            info = {
-                "error": "invalid_request",
-                "error_description": "Access not granted",
-            }
+        logger.debug("All checks OK")
 
-        return {"response_args": info, "client_id": _session_info["client_id"]}
+        issue_refresh = kwargs.get("issue_refresh", None)
+        # The existence of offline_access scope overwrites issue_refresh
+        if issue_refresh is None and "offline_access" in grant.scope:
+            issue_refresh = True
+
+        _response = {
+            "token_type": token_type,
+            "scope": grant.scope,
+        }
+
+        if "access_token" in _supports_minting:
+            try:
+                token = self._mint_token(
+                    token_class="access_token",
+                    grant=grant,
+                    session_id=_session_info["branch_id"],
+                    client_id=_session_info["client_id"],
+                    based_on=_based_on,
+                    token_type=token_type,
+                )
+            except MintingNotAllowed as err:
+                logger.warning(err)
+            else:
+                _response["access_token"] = token.value
+                if token.expires_at:
+                    _response["expires_in"] = token.expires_at - utc_time_sans_frac()
+
+        if (
+                issue_refresh
+                and "refresh_token" in _supports_minting
+        ):
+            try:
+                refresh_token = self._mint_token(
+                    token_class="refresh_token",
+                    grant=grant,
+                    session_id=_session_info["branch_id"],
+                    client_id=_session_info["client_id"],
+                    based_on=_based_on,
+                )
+            except MintingNotAllowed as err:
+                logger.warning(err)
+            else:
+                _response["refresh_token"] = refresh_token.value
 
-    def parse_request(self, request, http_info=None, **kwargs):
-        """
+        # since the grant content has changed. Make sure it's stored
+        _mngr[_session_info["branch_id"]] = grant
 
-        :param request:
-        :param auth:
-        :param kwargs:
-        :return:
+        if "openid" in _authn_req["scope"] and "id_token" in _supports_minting:
+            if "id_token" in _based_on.usage_rules.get("supports_minting"):
+                try:
+                    _idtoken = self._mint_token(
+                        token_class="id_token",
+                        grant=grant,
+                        session_id=_session_info["branch_id"],
+                        client_id=_session_info["client_id"],
+                        based_on=_based_on,
+                    )
+                except (JWEException, NoSuitableSigningKeys) as err:
+                    logger.warning(str(err))
+                    resp = self.error_cls(
+                        error="invalid_request",
+                        error_description="Could not sign/encrypt id_token",
+                    )
+                    return resp
+
+                _response["id_token"] = _idtoken.value
+
+        _based_on.register_usage()
+
+        return _response
+
+    def post_parse_request(
+            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+    ) -> Union[Message, dict]:
         """
+        This is where clients come to get their access tokens
 
-        if not request:
-            request = {}
+        :param request: The request
+        :param client_id: Client identifier
+        :returns:
+        """
 
-        # Verify that the client is allowed to do this
+        _mngr = self.endpoint.upstream_get("context").session_manager
         try:
-            auth_info = self.client_authentication(request, http_info, **kwargs)
-        except ClientAuthenticationError as e:
-            return self.error_cls(error="invalid_token", error_description=e.args[0])
+            _session_info = _mngr.get_session_info_by_token(
+                request["code"], grant=True, handler_key="authorization_code"
+            )
+        except (KeyError, UnknownToken):
+            logger.error("Access Code invalid")
+            return self.error_cls(error="invalid_grant", error_description="Unknown code")
 
-        if isinstance(auth_info, ResponseMessage):
-            return auth_info
-        else:
-            request["client_id"] = auth_info["client_id"]
-            request["access_token"] = auth_info["token"]
+        grant = _session_info["grant"]
+        code = grant.get_token(request["code"])
+        if not isinstance(code, AuthorizationCode):
+            return self.error_cls(error="invalid_request", error_description="Wrong token type")
+
+        if code.used:  # Has been used already
+            # invalidate all tokens that has been minted using this code
+            grant.revoke_token(based_on=request["code"], recursive=True)
+            return self.error_cls(error="invalid_grant", error_description="Code inactive")
+
+        if code.is_active() is False:
+            return self.error_cls(error="invalid_grant", error_description="Code inactive")
+
+        _auth_req = grant.authorization_request
+
+        if "client_id" not in request:  # Optional for access token request
+            request["client_id"] = _auth_req["client_id"]
+
+        logger.debug("%s: %s" % (request.__class__.__name__, sanitize(request)))
 
         return request
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/scopes.py` & `idpyoidc-2.0.0/src/idpyoidc/server/scopes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from idpyoidc.server.exception import ConfigurationError
-
 # default set can be changed by configuration
 
 SCOPE2CLAIMS = {
     "openid": ["sub"],
     "profile": [
         "name",
         "given_name",
@@ -45,45 +43,45 @@
             except KeyError:
                 continue
 
     return res
 
 
 class Scopes:
-    def __init__(self, server_get, allowed_scopes=None, scopes_to_claims=None):
-        self.server_get = server_get
+    def __init__(self, upstream_get, allowed_scopes=None, scopes_to_claims=None):
+        self.upstream_get = upstream_get
         if not scopes_to_claims:
             scopes_to_claims = dict(SCOPE2CLAIMS)
         self._scopes_to_claims = scopes_to_claims
         self.allowed_scopes = list(scopes_to_claims.keys())
 
     def get_allowed_scopes(self, client_id=None):
         """
         Returns the set of scopes that a specific client can use.
 
         :param client_id: The client identifier
         :returns: List of scope names. Can be empty.
         """
         allowed_scopes = self.allowed_scopes
         if client_id:
-            client = self.server_get("endpoint_context").cdb.get(client_id)
+            client = self.upstream_get("context").cdb.get(client_id)
             if client is not None:
                 allowed_scopes = client.get("allowed_scopes", allowed_scopes)
         return allowed_scopes
 
     def get_scopes_mapping(self, client_id=None):
         """
         Returns the mapping of scopes to claims fora specific client.
 
         :param client_id: The client identifier
         :returns: Dict of scopes to claims. Can be empty.
         """
         scopes_to_claims = self._scopes_to_claims
         if client_id:
-            client = self.server_get("endpoint_context").cdb.get(client_id)
+            client = self.upstream_get("context").cdb.get(client_id)
             if client is not None:
                 scopes_to_claims = client.get("scopes_to_claims", scopes_to_claims)
         return scopes_to_claims
 
     def filter_scopes(self, scopes, client_id=None):
         allowed_scopes = self.get_allowed_scopes(client_id)
         return [s for s in scopes if s in allowed_scopes]
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/session/claims.py` & `idpyoidc-2.0.0/src/idpyoidc/server/session/claims.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,73 +10,73 @@
 
 # USAGE = Literal["userinfo", "id_token", "introspection"]
 
 IGNORE = ["error", "error_description", "error_uri", "_claim_names", "_claim_sources"]
 STANDARD_CLAIMS = [c for c in OpenIDSchema.c_param.keys() if c not in IGNORE]
 
 
-def available_claims(endpoint_context):
-    _supported = endpoint_context.provider_info.get("claims_supported")
+def available_claims(context):
+    _supported = context.provider_info.get("claims_supported")
     if _supported:
         return _supported
     else:
         return STANDARD_CLAIMS
 
 
 class ClaimsInterface:
     init_args = {"add_claims_by_scope": False, "enable_claims_per_client": False}
     claims_release_points = ["userinfo", "introspection", "id_token", "access_token"]
 
-    def __init__(self, server_get):
-        self.server_get = server_get
+    def __init__(self, upstream_get):
+        self.upstream_get = upstream_get
 
     def authorization_request_claims(
         self,
         authorization_request: dict,
         claims_release_point: Optional[str] = "",
     ) -> dict:
         if authorization_request and "claims" in authorization_request:
             return authorization_request["claims"].get(claims_release_point, {})
 
         return {}
 
-    def _get_module(self, usage, endpoint_context):
+    def _get_module(self, usage, context):
         module = None
         if usage == "userinfo":
-            module = self.server_get("endpoint", "userinfo")
+            module = self.upstream_get("endpoint", "userinfo")
         elif usage == "id_token":
             try:
-                module = endpoint_context.session_manager.token_handler["id_token"]
+                module = context.session_manager.token_handler["id_token"]
             except KeyError:
                 raise ServiceError("No support for ID Tokens")
         elif usage == "introspection":
-            module = self.server_get("endpoint", "introspection")
+            module = self.upstream_get("endpoint", "introspection")
         elif usage == "access_token":
             try:
-                module = endpoint_context.session_manager.token_handler["access_token"]
+                module = context.session_manager.token_handler["access_token"]
             except KeyError:
                 raise ServiceError("No support for Access Tokens")
 
         return module
 
     def _client_claims(
         self,
         client_id: str,
         module: object,
         claims_release_point: str,
         secondary_identifier: Optional[str] = "",
     ):
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         add_claims_by_scope = _context.cdb[client_id].get("add_claims", {}).get("by_scope", {})
         if add_claims_by_scope:
-            _claims_by_scope = add_claims_by_scope.get(claims_release_point, False)
-            if not _claims_by_scope and secondary_identifier:
+            _claims_by_scope = add_claims_by_scope.get(claims_release_point)
+            if _claims_by_scope is None and secondary_identifier:
                 _claims_by_scope = add_claims_by_scope.get(secondary_identifier, False)
 
-            if not _claims_by_scope:
+            if _claims_by_scope is None:
                 _claims_by_scope = module.kwargs.get("add_claims_by_scope", {})
         else:
             _claims_by_scope = module.kwargs.get("add_claims_by_scope", {})
 
         add_claims_always = _context.cdb[client_id].get("add_claims", {}).get("always", {})
         _always_add = add_claims_always.get(claims_release_point, [])
         if secondary_identifier:
@@ -89,15 +89,15 @@
         self,
         auth_req: dict,
         claims_release_point: str,
         scopes: str = None,
         client_id: str = None,
         secondary_identifier: str = "",
     ) -> dict:
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         # which endpoint module configuration to get the base claims from
         module = self._get_module(claims_release_point, _context)
 
         # claims that are always returned to any client.
         if module:
             base_claims = module.kwargs.get("base_claims", {}).copy()
         else:
@@ -155,15 +155,15 @@
             release_point.
         :param session_id: Session identifier
         :param scopes: Scopes
         :param claims_release_point: Where to release the claims. One of
             "userinfo"/"id_token"/"introspection"/"access_token"
         :return: Claims specification as a dictionary.
         """
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         session_info = _context.session_manager.get_session_info(session_id, grant=True)
         client_id = session_info["client_id"]
         grant = session_info["grant"]
 
         if grant.authorization_request:
             auth_req = grant.authorization_request
         else:
@@ -185,29 +185,29 @@
         for usage in self.claims_release_points:
             _claims[usage] = self.get_claims_from_request(
                 auth_req, usage, scopes=scopes, client_id=client_id
             )
         return _claims
 
     def get_claims_all_usage(self, session_id: str, scopes: str) -> dict:
-        grant = self.server_get("endpoint_context").session_manager.get_grant(session_id)
+        grant = self.upstream_get("context").session_manager.get_grant(session_id)
         if grant.authorization_request:
             auth_req = grant.authorization_request
         else:
             auth_req = {}
         return self.get_claims_all_usage_from_request(auth_req, scopes)
 
     def get_user_claims(self, user_id: str, claims_restriction: dict) -> dict:
         """
 
         :param user_id: User identifier
         :param claims_restriction: Specifies the upper limit of which claims can be returned
         :return:
         """
-        meth = self.server_get("endpoint_context").userinfo
+        meth = self.upstream_get("context").userinfo
         if not meth:
             raise ImproperlyConfigured("userinfo MUST be defined in the configuration")
         if claims_restriction:
             # Get all possible claims
             user_info = meth(user_id, client_id=None)
             # Filter out the claims that can be returned
             return {
@@ -269,21 +269,21 @@
     """
     return dict([(key, val) for key, val in kwa.items() if key in cls.c_param])
 
 
 class OAuth2ClaimsInterface(ClaimsInterface):
     claims_release_points = ["introspection", "access_token"]
 
-    def _get_module(self, usage, endpoint_context):
+    def _get_module(self, usage, context):
         module = None
         if usage == "introspection":
-            module = self.server_get("endpoint", "introspection")
+            module = self.upstream_get("endpoint", "introspection")
         elif usage == "access_token":
             try:
-                module = endpoint_context.session_manager.token_handler["access_token"]
+                module = context.session_manager.token_handler["access_token"]
             except KeyError:
                 raise ServiceError("No support for Access Tokens")
 
         return module
 
     def get_claims_all_usage(self, session_id: str, scopes: str) -> dict:
         _claims = {}
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/session/database.py` & `idpyoidc-2.0.0/src/idpyoidc/server/session/database.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/session/grant.py` & `idpyoidc-2.0.0/src/idpyoidc/server/session/grant.py`

 * *Files 11% similar despite different names*

```diff
@@ -177,24 +177,25 @@
             _used_acr = self.authentication_event.get("authn_info")
             return claims_match(_used_acr, _acr_request)
         return False
 
     def payload_arguments(
             self,
             session_id: str,
-            endpoint_context,
+            context: object,
             item: SessionToken,
             claims_release_point: str,
+            scope: Optional[dict] = None,
             extra_payload: Optional[dict] = None,
             secondary_identifier: str = "",
     ) -> dict:
         """
 
         :param session_id: Session ID
-        :param endpoint_context: EndPoint Context
+        :param context: EndPoint Context
         :param item: A SessionToken instance
         :param claims_release_point: One of "userinfo", "introspection", "id_token", "access_token"
         :param extra_payload:
         :param secondary_identifier: Used if the claims returned are also based on rules for
             another release_point
         :type item: SessionToken
         :return: dictionary containing information to place in a token value
@@ -207,14 +208,18 @@
             else:
                 _val = getattr(self, _in)
                 if _val:
                     payload[_out] = _val
 
         payload["jti"] = uuid1().hex
 
+        if scope is None:
+            scope = self.scope
+        payload["scope"] = scope
+
         if extra_payload:
             payload.update(extra_payload)
 
         _jkt = self.extra.get("dpop_jkt")
         if _jkt:
             payload["cnf"] = {"jkt": _jkt}
 
@@ -222,54 +227,54 @@
             client_id = self.authorization_request.get("client_id")
             if client_id:
                 payload.update({"client_id": client_id, "sub": self.sub})
 
         if item.claims:
             _claims_restriction = item.claims
         else:
-            _claims_restriction = endpoint_context.claims_interface.get_claims(
+            _claims_restriction = context.claims_interface.get_claims(
                 session_id,
                 scopes=payload["scope"],
                 claims_release_point=claims_release_point,
                 secondary_identifier=secondary_identifier,
             )
 
-        if endpoint_context.session_manager.node_type[0] == "user":
-            user_id, _, _ = endpoint_context.session_manager.decrypt_branch_id(session_id)
-            user_info = endpoint_context.claims_interface.get_user_claims(user_id,
-                                                                          _claims_restriction)
+        if context.session_manager.node_type[0] == "user":
+            user_id, _, _ = context.session_manager.decrypt_branch_id(session_id)
+            user_info = context.claims_interface.get_user_claims(user_id,
+                                                                 _claims_restriction)
             payload.update(user_info)
 
         # Should I add the acr value
         if self.add_acr_value(claims_release_point):
             payload["acr"] = self.authentication_event["authn_info"]
         elif self.add_acr_value(secondary_identifier):
             payload["acr"] = self.authentication_event["authn_info"]
 
         return payload
 
     def mint_token(
             self,
             session_id: str,
-            endpoint_context: object,
+            context: object,
             token_class: str,
             token_handler: TokenHandler = None,
             based_on: Optional[SessionToken] = None,
             usage_rules: Optional[dict] = None,
             scope: Optional[list] = None,
             token_type: Optional[str] = "",
             expires_in: Optional[int] = 0,
             not_before: Optional[int] = 0,
             claims: Optional[List[str]] = None,
             **kwargs,
     ) -> Optional[SessionToken]:
         """
 
         :param session_id:
-        :param endpoint_context:
+        :param context:
         :param token_type:
         :param token_handler:
         :param based_on:
         :param usage_rules:
         :param scope:
         :param kwargs:
         :return:
@@ -334,17 +339,17 @@
                 scope=scope,
                 expires_in=expires_in,
                 not_before=not_before,
                 claims=claims,
                 **class_args,
             )
             if token_handler is None:
-                token_handler = endpoint_context.session_manager.token_handler.handler[token_class]
+                token_handler = context.session_manager.token_handler.handler[token_class]
 
-            if token_class in endpoint_context.claims_interface.claims_release_points:
+            if token_class in context.claims_interface.claims_release_points:
                 claims_release_point = token_class
             else:
                 claims_release_point = ""
 
             _secondary_identifier = kwargs.get("as_if")
             logger.debug(
                 f"claims_release_point: {claims_release_point}, secondary_identifier: "
@@ -352,17 +357,18 @@
             )
 
             if token_class == "id_token":
                 item.session_id = session_id
 
             token_payload = self.payload_arguments(
                 session_id,
-                endpoint_context,
+                context,
                 item=item,
                 claims_release_point=claims_release_point,
+                scope=scope,
                 extra_payload=handler_args,
                 secondary_identifier=_secondary_identifier,
             )
 
             logger.debug(f"token_payload: {token_payload}")
 
             item.value = token_handler(
@@ -445,48 +451,50 @@
         "expires_in": 300,
     },
     "access_token": {"supports_minting": [], "expires_in": 3600},
     "refresh_token": {"supports_minting": ["access_token", "refresh_token", "id_token"]},
 }
 
 
-def get_usage_rules(token_type, endpoint_context, grant, client_id):
+def get_usage_rules(token_type, context, grant, client_id):
     """
     The order of importance:
     Grant, Client, EndPointContext, Default
 
     :param token_type: The type of token
-    :param endpoint_context: An EndpointContext instance
+    :param context: An EndpointContext instance
     :param grant: A Grant instance
     :param client_id: The client identifier
     :return: Usage specification
     """
 
-    _usage = endpoint_context.authz.usage_rules_for(client_id, token_type)
+    _usage = context.authz.usage_rules_for(client_id, token_type)
     if not _usage:
         _usage = DEFAULT_USAGE[token_type]
 
     _grant_usage = grant.usage_rules.get(token_type)
     if _grant_usage:
         _usage.update(_grant_usage)
 
     return _usage
 
 
 class ExchangeGrant(Grant):
     parameter = Grant.parameter.copy()
-    parameter.update({"users": []})
+    parameter.update({"exchange_request": TokenExchangeRequest, "original_session_id": ""})
     type = "exchange_grant"
 
     def __init__(
             self,
             scope: Optional[list] = None,
             claims: Optional[dict] = None,
             resources: Optional[list] = None,
             authorization_details: Optional[dict] = None,
+            authorization_request: Optional[Message] = None,
+            authentication_event: Optional[AuthnEvent] = None,
             issued_token: Optional[list] = None,
             usage_rules: Optional[dict] = None,
             exchange_request: Optional[TokenExchangeRequest] = None,
             original_branch_id: str = "",
             issued_at: int = 0,
             expires_in: int = 0,
             expires_at: int = 0,
@@ -497,14 +505,16 @@
     ):
         Grant.__init__(
             self,
             scope=scope,
             claims=claims,
             resources=resources,
             authorization_details=authorization_details,
+            authorization_request=authorization_request,
+            authentication_event=authentication_event,
             issued_token=issued_token,
             usage_rules=usage_rules,
             issued_at=issued_at,
             expires_in=expires_in,
             expires_at=expires_at,
             revoked=revoked,
             token_map=token_map,
@@ -513,7 +523,80 @@
 
         self.users = users or []
         self.usage_rules = {
             "access_token": {"supports_minting": ["access_token"], "expires_in": 60}
         }
         self.exchange_request = exchange_request
         self.original_branch_id = original_branch_id
+
+    def payload_arguments(
+            self,
+            session_id: str,
+            endpoint_context,
+            item: SessionToken,
+            claims_release_point: str,
+            scope: Optional[dict] = None,
+            extra_payload: Optional[dict] = None,
+            secondary_identifier: str = "",
+    ) -> dict:
+        """
+        :param session_id: Session ID
+        :param endpoint_context: EndPoint Context
+        :param claims_release_point: One of "userinfo", "introspection", "id_token", "access_token"
+        :param scope: scope from the request
+        :param extra_payload:
+        :param secondary_identifier: Used if the claims returned are also based on rules for
+            another release_point
+        :param item: A SessionToken instance
+        :type item: SessionToken
+        :return: dictionary containing information to place in a token value
+        """
+        payload = {}
+        for _in, _out in [("scope", "scope"), ("resources", "aud")]:
+            _val = getattr(item, _in)
+            if _val:
+                payload[_out] = _val
+            else:
+                _val = getattr(self, _in)
+                if _val:
+                    payload[_out] = _val
+
+        payload["jti"] = uuid1().hex
+
+        if scope is None:
+            scope = self.scope
+
+        payload = {"scope": scope, "aud": self.resources, "jti": uuid1().hex}
+
+        if extra_payload:
+            payload.update(extra_payload)
+
+        _jkt = self.extra.get("dpop_jkt")
+        if _jkt:
+            payload["cnf"] = {"jkt": _jkt}
+
+        if self.exchange_request:
+            client_id = self.exchange_request.get("client_id")
+            if client_id:
+                payload.update({"client_id": client_id, "sub": self.sub})
+
+        if item.claims:
+            _claims_restriction = item.claims
+        else:
+            _claims_restriction = endpoint_context.claims_interface.get_claims(
+                session_id,
+                scopes=scope,
+                claims_release_point=claims_release_point,
+                secondary_identifier=secondary_identifier,
+            )
+
+        user_id, _, _ = endpoint_context.session_manager.decrypt_session_id(session_id)
+        user_info = endpoint_context.claims_interface.get_user_claims(user_id, _claims_restriction)
+        payload.update(user_info)
+
+        # Should I add the acr value
+        if self.add_acr_value(claims_release_point):
+            payload["acr"] = self.authentication_event["authn_info"]
+        elif self.add_acr_value(secondary_identifier):
+            payload["acr"] = self.authentication_event["authn_info"]
+
+        return payload
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/session/grant_manager.py` & `idpyoidc-2.0.0/src/idpyoidc/server/session/grant_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,10 +283,10 @@
     # def get_branch_id_by_token(self, token_value: str) -> str:
     #     _token_info = self.token_handler.info(token_value)
     #     sid = _token_info.get("sid")
     #     return self._compatible_sid(sid)
     #
 
 
-def create_grant_manager(server_get, token_handler_args, conf=None, **kwargs):
-    _token_handler = handler.factory(server_get, **token_handler_args)
+def create_grant_manager(upstream_get, token_handler_args, conf=None, **kwargs):
+    _token_handler = handler.factory(upstream_get, **token_handler_args)
     return GrantManager(_token_handler, conf=conf)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/session/info.py` & `idpyoidc-2.0.0/src/idpyoidc/server/session/info.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/session/manager.py` & `idpyoidc-2.0.0/src/idpyoidc/server/session/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 from typing import Callable
 from typing import List
 from typing import Optional
 import uuid
 
 from idpyoidc.encrypter import default_crypt_config
-from idpyoidc.encrypter import get_crypt_config
 from idpyoidc.message.oauth2 import AuthorizationRequest
 from idpyoidc.message.oauth2 import TokenExchangeRequest
 from idpyoidc.server.authn_event import AuthnEvent
 from idpyoidc.server.exception import ConfigurationError
 from idpyoidc.server.session.grant_manager import GrantManager
 from idpyoidc.util import rndstr
 from .database import Database
@@ -90,16 +89,15 @@
             sub_func: Optional[dict] = None,
             remember_token: Optional[Callable] = None,
             remove_inactive_token: Optional[bool] = False,
     ):
         self.conf = conf or {"session_params": {"encrypter": default_crypt_config()}}
 
         session_params = self.conf.get("session_params") or {}
-        _crypt_config = get_crypt_config(session_params)
-        super(SessionManager, self).__init__(handler, _crypt_config)
+        super(SessionManager, self).__init__(handler, self.conf)
 
         self.node_type = session_params.get("node_type", ["user", "client", "grant"])
         # Make sure node_type is a list and must contain at least one element.
         if not isinstance(self.node_type, list):
             raise ValueError("Wrong type of value for SessionManager node_type")
         if len(self.node_type) == 0:
             raise ValueError("SessionManager node_type must at least contain one value")
@@ -192,41 +190,34 @@
             sector_identifier = ""
             _claims = {}
 
         resources = []
         if "resource" in auth_req:
             resources = auth_req["resource"]
 
-        if self.node_type[0] == "user":
-            kwargs = {
-                "sub": self.sub_func[sub_type](
-                    user_id, salt=self.get_salt(), sector_identifier=sector_identifier)
-            }
-        else:
-            kwargs = {}
-
         return self.add_grant(
             path=self.make_path(user_id=user_id, client_id=client_id),
             token_usage_rules=token_usage_rules,
             authorization_request=auth_req,
             authentication_event=authn_event,
             sub=self.sub_func[sub_type](
                 user_id, salt=self.get_salt(), sector_identifier=sector_identifier
             ),
             usage_rules=token_usage_rules,
             scope=scopes,
             claims=_claims,
             remember_token=self.remember_token,
             remove_inactive_token=self.remove_inactive_token,
-            resources=resources
+            resources=resources,
         )
 
     def create_exchange_grant(
             self,
             exchange_request: TokenExchangeRequest,
+            original_grant: Grant,
             original_session_id: str,
             user_id: str,
             client_id: Optional[str] = "",
             sub_type: Optional[str] = "public",
             token_usage_rules: Optional[dict] = None,
             scopes: Optional[list] = None,
     ) -> str:
@@ -237,19 +228,21 @@
         :param user_id:
         :param client_id:
         :param sub_type:
         :return:
         """
 
         return self.add_exchange_grant(
+            authentication_event=original_grant.authentication_event,
+            authorization_request=original_grant.authorization_request,
             exchange_request=exchange_request,
             original_branch_id=original_session_id,
             path=self.make_path(user_id=user_id, client_id=client_id),
+            sub=original_grant.sub,
             token_usage_rules=token_usage_rules,
-            sub=self.sub_func[sub_type](user_id, salt=self.get_salt(), sector_identifier=""),
             scope=scopes
         )
 
     def create_session(
             self,
             authn_event: AuthnEvent,
             auth_req: AuthorizationRequest,
@@ -282,14 +275,15 @@
             token_usage_rules=token_usage_rules,
             scopes=scopes,
         )
 
     def create_exchange_session(
             self,
             exchange_request: TokenExchangeRequest,
+            original_grant: Grant,
             original_session_id: str,
             user_id: str,
             client_id: Optional[str] = "",
             sub_type: Optional[str] = "public",
             token_usage_rules: Optional[dict] = None,
             scopes: Optional[list] = None,
     ) -> str:
@@ -305,14 +299,15 @@
         :param sub_type: What kind of subject will be assigned
         :param token_usage_rules: Rules for how tokens can be used
         :return: Session key
         """
 
         return self.create_exchange_grant(
             exchange_request=exchange_request,
+            original_grant=original_grant,
             original_session_id=original_session_id,
             user_id=user_id,
             client_id=client_id,
             sub_type=sub_type,
             token_usage_rules=token_usage_rules,
             scopes=scopes,
         )
@@ -491,14 +486,15 @@
             user_session_info: Optional[bool] = False,
             client_session_info: Optional[bool] = False,
             grant: Optional[bool] = False,
             authentication_event: Optional[bool] = False,
             authorization_request: Optional[bool] = False,
             handler_key: Optional[str] = "",
     ) -> dict:
+
         if handler_key:
             _token_info = self.token_handler.handler[handler_key].info(token_value)
         else:
             _token_info = self.token_handler.info(token_value)
 
         sid = _token_info.get("sid")
         # If the token is an ID Token then the sid will not be in the
@@ -535,10 +531,10 @@
     def encrypted_session_id(self, *args):
         return self.encrypted_branch_id(*args)
 
     def unpack_session_key(self, key):
         return self.unpack_branch_key(key)
 
 
-def create_session_manager(server_get, token_handler_args, sub_func=None, conf=None):
-    _token_handler = handler.factory(server_get, **token_handler_args)
+def create_session_manager(upstream_get, token_handler_args, sub_func=None, conf=None):
+    _token_handler = handler.factory(upstream_get, **token_handler_args)
     return SessionManager(_token_handler, sub_func=sub_func, conf=conf)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/session/token.py` & `idpyoidc-2.0.0/src/idpyoidc/server/session/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,14 @@
             "based_on": "",
             "claims": {},
             "id": "",
             "name": "",
             "resources": [],
             "scope": [],
             "token_class": "",
-            "usage_rules": {},
-            "used": 0,
             "value": "",
         }
     )
 
     def __init__(
         self,
         token_class: str = "",
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/token/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/server/token/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import base64
 import logging
 from typing import Optional
 
 from cryptojwt import as_unicode
-from cryptojwt.jwe.fernet import FernetEncrypter
 
 from idpyoidc.encrypter import init_encrypter
 from idpyoidc.server.util import lv_pack
 from idpyoidc.server.util import lv_unpack
 from idpyoidc.time_util import utc_time_sans_frac
 from idpyoidc.util import rndstr
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/token/handler.py` & `idpyoidc-2.0.0/src/idpyoidc/server/token/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 from cryptojwt.exception import Invalid
 from cryptojwt.key_jar import init_key_jar
 from cryptojwt.utils import as_unicode
 
 from idpyoidc.impexp import ImpExp
 from idpyoidc.item import DLDict
 from idpyoidc.util import importer
-
 from . import DefaultToken
 from . import Token
 from . import UnknownToken
 from .exception import TokenException
 
 __author__ = "Roland Hedberg"
 
 logger = logging.getLogger(__name__)
 
 
 class TokenHandler(ImpExp):
     parameter = {"handler": DLDict, "handler_order": [""]}
 
     def __init__(
-        self,
-        access_token: Optional[Token] = None,
-        authorization_code: Optional[Token] = None,
-        refresh_token: Optional[Token] = None,
-        id_token: Optional[Token] = None,
+            self,
+            access_token: Optional[Token] = None,
+            authorization_code: Optional[Token] = None,
+            refresh_token: Optional[Token] = None,
+            id_token: Optional[Token] = None,
     ):
         ImpExp.__init__(self)
         self.handler = {"authorization_code": authorization_code, "access_token": access_token}
 
         self.handler_order = ["authorization_code", "access_token"]
 
         if refresh_token:
@@ -79,15 +78,15 @@
 
         return None, None
 
     def keys(self):
         return self.handler.keys()
 
 
-def init_token_handler(server_get, spec, token_class):
+def init_token_handler(upstream_get, spec, token_class):
     _kwargs = spec.get("kwargs", {})
 
     _lt = spec.get("lifetime")
     if _lt:
         _kwargs["lifetime"] = _lt
 
     try:
@@ -105,15 +104,15 @@
             warnings.warn(
                 "Token initialisation arguments should be grouped under 'kwargs'.",
                 DeprecationWarning,
                 stacklevel=2,
             )
         _kwargs = spec
 
-    return cls(token_class=token_class, server_get=server_get, **_kwargs)
+    return cls(token_class=token_class, upstream_get=upstream_get, **_kwargs)
 
 
 def _add_passwd(keyjar, conf, kid):
     if keyjar:
         _keys = keyjar.get_encrypt_key(key_type="oct", kid=kid)
         if _keys:
             pw = as_unicode(_keys[0].k)
@@ -138,21 +137,21 @@
         return False
 
 
 JWKS_FILE = "private/token_jwks.json"
 
 
 def factory(
-    server_get,
-    code: Optional[dict] = None,
-    token: Optional[dict] = None,
-    refresh: Optional[dict] = None,
-    id_token: Optional[dict] = None,
-    jwks_file: Optional[str] = "",
-    **kwargs
+        upstream_get,
+        code: Optional[dict] = None,
+        token: Optional[dict] = None,
+        refresh: Optional[dict] = None,
+        id_token: Optional[dict] = None,
+        jwks_file: Optional[str] = "",
+        **kwargs
 ) -> TokenHandler:
     """
     Create a token handler
 
     :param code:
     :param token:
     :param refresh:
@@ -165,15 +164,15 @@
         "token": "access_token",
         "refresh": "refresh_token",
         "idtoken": "id_token",
     }
 
     key_defs = []
     read_only = False
-    cwd = server_get("endpoint_context").cwd
+    cwd = upstream_get("attribute", "cwd")
     if kwargs.get("jwks_def"):
         defs = kwargs["jwks_def"]
         if not jwks_file:
             jwks_file = defs.get("private_path", os.path.join(cwd, JWKS_FILE))
         read_only = defs.get("read_only", read_only)
         key_defs = defs.get("key_defs", [])
 
@@ -191,13 +190,13 @@
         ("token", token, "access_token"),
         ("refresh", refresh, "refresh_token"),
     ]:
         if cnf is not None:
             if default_token(cnf):
                 if kj:
                     _add_passwd(kj, cnf, cls)
-            args[attr] = init_token_handler(server_get, cnf, token_class_map[cls])
+            args[attr] = init_token_handler(upstream_get, cnf, token_class_map[cls])
 
     if id_token is not None:
-        args["id_token"] = init_token_handler(server_get, id_token, token_class="")
+        args["id_token"] = init_token_handler(upstream_get, id_token, token_class="")
 
     return TokenHandler(**args)
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/token/id_token.py` & `idpyoidc-2.0.0/src/idpyoidc/server/token/id_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,57 +23,57 @@
     "userinfo": "RS256",
     "request_object": "RS256",
     "client_secret_jwt": "HS256",
     "private_key_jwt": "RS256",
 }
 
 
-def include_session_id(endpoint_context, client_id, where):
+def include_session_id(context, client_id, where):
     """
 
-    :param endpoint_context:
+    :param context:
     :param client_id:
     :param where: front or back
     :return:
     """
-    _pinfo = endpoint_context.provider_info
+    _pinfo = context.provider_info
 
     # Am the OP supposed to support {dir}-channel log out and if so can
     # it pass sid in logout token and ID Token
     for param in ["{}channel_logout_supported", "{}channel_logout_session_supported"]:
         try:
             _supported = _pinfo[param.format(where)]
         except KeyError:
             return False
         else:
             if not _supported:
                 return False
 
     # Does the client support back-channel logout ?
     try:
-        endpoint_context.cdb[client_id]["{}channel_logout_uri".format(where)]
+        context.cdb[client_id]["{}channel_logout_uri".format(where)]
     except KeyError:
         return False
 
     return True
 
 
 def get_sign_and_encrypt_algorithms(
-    endpoint_context, client_info, payload_type, sign=False, encrypt=False
+    context, client_info, payload_type, sign=False, encrypt=False
 ):
     args = {"sign": sign, "encrypt": encrypt}
     if sign:
         try:
             args["sign_alg"] = client_info["{}_signed_response_alg".format(payload_type)]
         except KeyError:  # Fall back to default
             try:
-                args["sign_alg"] = endpoint_context.jwx_def["signing_alg"][payload_type]
+                args["sign_alg"] = context.jwx_def["signing_alg"][payload_type]
             except KeyError:
                 _def_sign_alg = DEF_SIGN_ALG[payload_type]
-                _supported = endpoint_context.provider_info.get(
+                _supported = context.provider_info.get(
                     "{}_signing_alg_values_supported".format(payload_type)
                 )
 
                 if not _supported:
                     args["sign_alg"] = _def_sign_alg
                 else:
                     if _def_sign_alg in _supported:
@@ -82,57 +82,58 @@
                         args["sign_alg"] = _supported[0]
 
     if encrypt:
         try:
             args["enc_alg"] = client_info["%s_encrypted_response_alg" % payload_type]
         except KeyError:
             try:
-                args["enc_alg"] = endpoint_context.jwx_def["encryption_alg"][payload_type]
+                args["enc_alg"] = context.jwx_def["encryption_alg"][payload_type]
             except KeyError:
-                _supported = endpoint_context.provider_info.get(
+                _supported = context.provider_info.get(
                     "{}_encryption_alg_values_supported".format(payload_type)
                 )
                 if _supported:
                     args["enc_alg"] = _supported[0]
 
         try:
             args["enc_enc"] = client_info["%s_encrypted_response_enc" % payload_type]
         except KeyError:
             try:
-                args["enc_enc"] = endpoint_context.jwx_def["encryption_enc"][payload_type]
+                args["enc_enc"] = context.jwx_def["encryption_enc"][payload_type]
             except KeyError:
-                _supported = endpoint_context.provider_info.get(
+                _supported = context.provider_info.get(
                     "{}_encryption_enc_values_supported".format(payload_type)
                 )
                 if _supported:
                     args["enc_enc"] = _supported[0]
 
     return args
 
 
 class IDToken(Token):
-    default_capabilities = {
+    _supports = {
+        "encrypt_id_token_supported": None,
         "id_token_signing_alg_values_supported": None,
         "id_token_encryption_alg_values_supported": None,
         "id_token_encryption_enc_values_supported": None,
     }
 
     def __init__(
         self,
         token_class: Optional[str] = "id_token",
         lifetime: Optional[int] = 300,
-        server_get: Callable = None,
+        upstream_get: Callable = None,
         **kwargs,
     ):
         Token.__init__(self, token_class, **kwargs)
         self.lifetime = lifetime
-        self.server_get = server_get
+        self.upstream_get = upstream_get
         self.kwargs = kwargs
         self.scope_to_claims = None
-        self.provider_info = construct_provider_info(self.default_capabilities, **kwargs)
+        self.provider_info = construct_provider_info(self._supports, **kwargs)
 
     def payload(
         self,
         session_id,
         alg="RS256",
         code=None,
         access_token=None,
@@ -146,15 +147,15 @@
         :param alg: Which signing algorithm to use for the IdToken
         :param code: Access grant
         :param access_token: Access Token
         :param extra_claims: extra claims to be added to the ID Token
         :return: IDToken instance
         """
 
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         _mngr = _context.session_manager
         session_information = _mngr.get_session_info(session_id, grant=True)
         grant = session_information["grant"]
         _args = {"sub": grant.sub, "sid": session_id}
         if grant.authentication_event:
             for claim, attr in {"authn_time": "auth_time", "authn_info": "acr"}.items():
                 _val = grant.authentication_event.get(claim)
@@ -232,15 +233,15 @@
         :param access_token: Access Token
         :param sign: If the JWT should be signed
         :param encrypt: If the JWT should be encrypted
         :param extra_claims: Extra claims to be added to the ID Token
         :return: IDToken as a signed and/or encrypted JWT
         """
 
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
 
         client_info = _context.cdb[client_id]
         alg_dict = get_sign_and_encrypt_algorithms(
             _context, client_info, "id_token", sign=sign, encrypt=encrypt
         )
 
         _payload = self.payload(
@@ -251,29 +252,33 @@
             extra_claims=extra_claims,
             user_info=user_info,
         )
 
         if lifetime is None:
             lifetime = self.lifetime
 
-        _jwt = JWT(_context.keyjar, iss=_context.issuer, lifetime=lifetime, **alg_dict)
+        _jwt = JWT(
+            self.upstream_get('attribute', 'keyjar'),
+            iss=_context.issuer,
+            lifetime=lifetime,
+            **alg_dict)
 
         return _jwt.pack(_payload, recv=client_id)
 
     def __call__(
         self,
         session_id: Optional[str] = "",
         ttype: Optional[str] = "",
         encrypt=False,
         code=None,
         access_token=None,
         usage_rules: Optional[dict] = None,
         **kwargs,
     ) -> str:
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
 
         user_id, client_id, grant_id = _context.session_manager.decrypt_session_id(session_id)
 
         # Should I add session ID. This is about Single Logout.
         if include_session_id(_context, client_id, "back") or include_session_id(
             _context, client_id, "front"
         ):
@@ -303,36 +308,38 @@
         Return type of Token (A=Access code, T=Token, R=Refresh token) and
         the session id.
 
         :param token: A token
         :return: tuple of token type and session id
         """
 
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
 
         _jwt = factory(token)
         if not _jwt:
             raise InvalidToken("Not valid token")
 
         _payload = _jwt.jwt.payload()
         client_id = _payload["aud"][0]
         client_info = _context.cdb[client_id]
         alg_dict = get_sign_and_encrypt_algorithms(_context, client_info, "id_token", sign=True)
 
-        verifier = JWT(key_jar=_context.keyjar, allowed_sign_algs=alg_dict["sign_alg"])
+        verifier = JWT(
+            key_jar=self.upstream_get('attribute', 'keyjar'),
+            allowed_sign_algs=alg_dict["sign_alg"])
         try:
             _payload = verifier.unpack(token)
         except JWSException:
             raise UnknownToken()
 
         logger.debug(f"Received ID Token payload: {_payload}")
 
         if is_expired(_payload["exp"]):
             raise ToOld("Token has expired")
-        # All the token metadata
+        # All the token claims
         return {
             "sid": _payload.get("sid", ""),  # TODO: would sid be there?
             # "type": _payload["ttype"],
             "exp": _payload["exp"],
             "aud": client_id,
             "handler": self,
         }
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/token/jwt_token.py` & `idpyoidc-2.0.0/src/idpyoidc/server/token/jwt_token.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,75 @@
 from typing import Callable
 from typing import Optional
+from typing import Union
 
 from cryptojwt import JWT
 from cryptojwt.jws.exception import JWSException
+from cryptojwt.utils import importer
 
-from idpyoidc.encrypter import init_encrypter
 from idpyoidc.server.exception import ToOld
-
-from ..constant import DEFAULT_TOKEN_LIFETIME
 from . import Token
 from . import is_expired
 from .exception import UnknownToken
 from .exception import WrongTokenClass
+from ..constant import DEFAULT_TOKEN_LIFETIME
+from ...message import Message
+from ...message.oauth2 import JWTAccessToken
 
 
 class JWTToken(Token):
+
     def __init__(
-        self,
-        token_class,
-        # keyjar: KeyJar = None,
-        issuer: str = None,
-        aud: Optional[list] = None,
-        alg: str = "ES256",
-        lifetime: int = DEFAULT_TOKEN_LIFETIME,
-        server_get: Callable = None,
-        token_type: str = "Bearer",
-        **kwargs
+            self,
+            token_class,
+            # keyjar: KeyJar = None,
+            issuer: str = None,
+            aud: Optional[list] = None,
+            alg: str = "ES256",
+            lifetime: int = DEFAULT_TOKEN_LIFETIME,
+            upstream_get: Callable = None,
+            token_type: str = "Bearer",
+            profile: Optional[Union[Message, str]] = JWTAccessToken,
+            with_jti: Optional[bool] = False,
+            **kwargs
     ):
         Token.__init__(self, token_class, **kwargs)
         self.token_type = token_type
         self.lifetime = lifetime
 
         self.kwargs = kwargs
-        _context = server_get("endpoint_context")
-        # self.key_jar = keyjar or _context.keyjar
+        _context = upstream_get("context")
+        # self.key_jar = keyjar or upstream_get('attribute','keyjar')
         self.issuer = issuer or _context.issuer
         self.cdb = _context.cdb
-        self.server_get = server_get
+        self.upstream_get = upstream_get
 
         self.def_aud = aud or []
         self.alg = alg
+        if isinstance(profile, str):
+            self.profile = importer(profile)
+        else:
+            self.profile = profile
+        self.with_jti = with_jti
+
+        if self.with_jti is False and profile == JWTAccessToken:
+            self.with_jti = True
 
     def load_custom_claims(self, payload: dict = None):
         # inherit me and do your things here
         return payload
 
     def __call__(
-        self,
-        session_id: Optional[str] = "",
-        token_class: Optional[str] = "",
-        usage_rules: Optional[dict] = None,
-        **payload
+            self,
+            session_id: Optional[str] = "",
+            token_class: Optional[str] = "",
+            usage_rules: Optional[dict] = None,
+            profile: Optional[Message] = None,
+            with_jti: Optional[bool] = None,
+            **payload
     ) -> str:
         """
         Return a token.
 
         :param session_id: Session id
         :param token_class: Token class
         :param payload: A dictionary with information that is part of the payload of the JWT.
@@ -66,31 +81,42 @@
             else:
                 token_class = "authorization_code"
 
         payload.update({"sid": session_id, "token_class": token_class})
         payload = self.load_custom_claims(payload)
 
         # payload.update(kwargs)
-        _context = self.server_get("endpoint_context")
         if usage_rules and "expires_in" in usage_rules:
             lifetime = usage_rules.get("expires_in")
         else:
             lifetime = self.lifetime
         signer = JWT(
-            key_jar=_context.keyjar,
+            key_jar=self.upstream_get('attribute', 'keyjar'),
             iss=self.issuer,
             lifetime=lifetime,
             sign_alg=self.alg,
         )
+        if isinstance(payload, Message):  # don't mess with it.
+            pass
+        else:
+            if profile:
+                payload = profile(**payload).to_dict()
+            elif self.profile:
+                payload = self.profile(**payload).to_dict()
+
+        if with_jti:
+            signer.with_jti = True
+        elif with_jti is None:
+            signer.with_jti = self.with_jti
 
         return signer.pack(payload)
 
     def get_payload(self, token):
-        _context = self.server_get("endpoint_context")
-        verifier = JWT(key_jar=_context.keyjar, allowed_sign_algs=[self.alg])
+        verifier = JWT(key_jar=self.upstream_get('attribute', 'keyjar'),
+                       allowed_sign_algs=[self.alg])
         try:
             _payload = verifier.unpack(token)
         except JWSException:
             raise UnknownToken()
 
         return _payload
 
@@ -110,15 +136,15 @@
         if _class not in [self.token_class, self.alt_token_name]:
             raise WrongTokenClass(_payload["token_class"])
         else:
             _payload["token_class"] = self.token_class
 
         if is_expired(_payload["exp"]):
             raise ToOld("Token has expired")
-        # All the token metadata
+        # All the token claims
         _res = {
             "sid": _payload["sid"],
             "token_class": _payload["token_class"],
             "exp": _payload["exp"],
             "handler": self,
         }
         return _res
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/user_authn/authn_context.py` & `idpyoidc-2.0.0/src/idpyoidc/server/user_authn/authn_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.db = {}
         self.acr2id = {}
 
     def __setitem__(self, key, info):
         """
         Adds a new authentication method.
 
-        :param value: A dictionary with metadata and configuration information
+        :param value: A dictionary with claims and configuration information
         """
 
         for attr in ["acr", "method"]:
             if attr not in info:
                 raise ValueError('Required attribute "{}" missing'.format(attr))
 
         self.db[key] = info
@@ -116,77 +116,77 @@
             if "value" in _acr:
                 return [_acr["value"]]
             elif "values" in _acr:
                 return _acr["values"]
     return None
 
 
-def pick_auth(endpoint_context, areq, pick_all=False):
+def pick_auth(context, areq, pick_all=False):
     """
     Pick authentication method
 
     :param areq: AuthorizationRequest instance
     :return: A dictionary with the authentication method and its authn class ref
     """
     acrs = []
-    if len(endpoint_context.authn_broker) == 1:
-        return endpoint_context.authn_broker.default()
+    if len(context.authn_broker) == 1:
+        return context.authn_broker.default()
 
     if "acr_values" in areq:
         if not isinstance(areq["acr_values"], list):
             areq["acr_values"] = [areq["acr_values"]]
         acrs = areq["acr_values"]
     else:
         acrs = _acr_claim(areq)
         if not acrs:
             _ith = verified_claim_name("id_token_hint")
             if areq.get(_ith):
                 _ith = areq[verified_claim_name("id_token_hint")]
                 if _ith.get("acr"):
                     acrs = [_ith["acr"]]
             else:
-                if areq.get("login_hint") and endpoint_context.login_hint2acrs:
-                    acrs = endpoint_context.login_hint2acrs(areq["login_hint"])
+                if areq.get("login_hint") and context.login_hint2acrs:
+                    acrs = context.login_hint2acrs(areq["login_hint"])
 
     if not acrs:
-        return endpoint_context.authn_broker.default()
+        return context.authn_broker.default()
 
     for acr in acrs:
-        res = endpoint_context.authn_broker.pick(acr)
+        res = context.authn_broker.pick(acr)
         logger.debug(f"Picked AuthN broker for ACR {str(acr)}: {str(res)}")
         if res:
             return res if pick_all else res[0]
 
     return None
 
 
-def init_method(authn_spec, server_get, template_handler=None):
+def init_method(authn_spec, upstream_get, template_handler=None):
     try:
         _args = authn_spec["kwargs"]
     except KeyError:
         _args = {}
 
     if "template" in _args:
         _args["template_handler"] = template_handler
 
-    _args["server_get"] = server_get
+    _args["upstream_get"] = upstream_get
 
     args = {"method": instantiate(authn_spec["class"], **_args)}
     args.update({k: v for k, v in authn_spec.items() if k not in ["class", "kwargs"]})
     return args
 
 
-def populate_authn_broker(methods, server_get, template_handler=None):
+def populate_authn_broker(methods, upstream_get, template_handler=None):
     """
 
     :param methods: Authentication method specifications
-    :param server_get: method that returns things from server
+    :param upstream_get: method that returns things from server
     :param template_handler: A class used to render templates
     :return:
     """
     authn_broker = AuthnBroker()
 
     for id, authn_spec in methods.items():
-        args = init_method(authn_spec, server_get, template_handler)
+        args = init_method(authn_spec, upstream_get, template_handler)
         authn_broker[id] = args
 
     return authn_broker
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/user_authn/user.py` & `idpyoidc-2.0.0/src/idpyoidc/server/user_authn/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 
 class UserAuthnMethod(object):
     # override in subclass specifying suitable url endpoint to POST user input
     url_endpoint = "/verify"
     FAILED_AUTHN = (None, True)
 
-    def __init__(self, server_get=None, **kwargs):
+    def __init__(self, upstream_get=None, **kwargs):
         self.query_param = "upm_answer"
-        self.server_get = server_get
+        self.upstream_get = upstream_get
         self.kwargs = kwargs
 
     def __call__(self, **kwargs):
         """
         Display user interaction.
 
         :param args:
@@ -86,15 +86,15 @@
         """
         Callback to verify user input
         :return: username of the authenticated user
         """
         raise NotImplementedError
 
     def unpack_token(self, token):
-        return verify_signed_jwt(token=token, keyjar=self.server_get("endpoint_context").keyjar)
+        return verify_signed_jwt(token=token, keyjar=self.upstream_get("context").keyjar)
 
     def done(self, areq):
         """
 
         :param areq: Authentication request
         :return: True if the 'query_parameter' doesn't appear in the request
         """
@@ -102,15 +102,15 @@
             _ = areq[self.query_param]
         except KeyError:
             return True
         else:
             return False
 
     def cookie_info(self, cookie: List[dict], client_id: str) -> dict:
-        _context = self.server_get("endpoint_context")
+        _context = self.upstream_get("context")
         logger.debug("Value cookies: {}".format(cookie))
 
         if cookie is None:
             pass
         else:
             for val in cookie:
                 _info = json.loads(val["value"])
@@ -153,20 +153,20 @@
     url_endpoint = "/verify/user_pass_jinja"
 
     def __init__(
             self,
             db,
             template_handler,
             template="user_pass.jinja2",
-            server_get=None,
+            upstream_get=None,
             verify_endpoint="",
             **kwargs,
     ):
 
-        super(UserPassJinja2, self).__init__(server_get=server_get)
+        super(UserPassJinja2, self).__init__(upstream_get=upstream_get)
         self.template_handler = template_handler
         self.template = template
 
         self.action = verify_endpoint or self.url_endpoint
 
         self.user_db = instantiate(db["class"], **db["kwargs"])
 
@@ -186,20 +186,21 @@
         warnings.warn(
             (
                 'Do not use the "UserPassJinja2" authentication method in a '
                 "production environment"
             ),
             OnlyForTestingWarning,
         )
-        if not self.server_get:
-            raise Exception(f"{self.__class__.__name__} doesn't have a working server_get")
-        _context = self.server_get("endpoint_context")
+        if not self.upstream_get:
+            raise Exception(f"{self.__class__.__name__} doesn't have a working upstream_get")
+        _context = self.upstream_get("context")
+        _keyjar = self.upstream_get("attribute", 'keyjar')
         # Stores information need afterwards in a signed JWT that then
         # appears as a hidden input in the form
-        jws = create_signed_jwt(_context.issuer, _context.keyjar, **kwargs)
+        jws = create_signed_jwt(_context.issuer, _keyjar, **kwargs)
         _kwargs = self.kwargs.copy()
         for attr in ["policy", "tos", "logo"]:
             _uri = "{}_uri".format(attr)
             try:
                 _kwargs[_uri] = kwargs[_uri]
             except KeyError:
                 pass
@@ -213,17 +214,41 @@
         username = kwargs["username"]
         if username in self.user_db and self.user_db[username] == kwargs["password"]:
             return username
         else:
             raise FailedAuthentication()
 
 
+class UserPass(UserAuthnMethod):
+
+    def __init__(
+            self,
+            db_conf,
+            upstream_get=None,
+            **kwargs,
+    ):
+
+        super(UserPass, self).__init__(upstream_get=upstream_get)
+        self.user_db = instantiate(db_conf["class"], **db_conf["kwargs"])
+
+    def __call__(self, **kwargs):
+        pass
+
+    def verify(self, *args, **kwargs):
+        username = kwargs["username"]
+        if username in self.user_db and self.user_db[username] == kwargs["password"]:
+            return username
+        else:
+            raise FailedAuthentication()
+
+
 class BasicAuthn(UserAuthnMethod):
-    def __init__(self, pwd, ttl=5, server_get=None):
-        UserAuthnMethod.__init__(self, server_get=server_get)
+
+    def __init__(self, pwd, ttl=5, upstream_get=None):
+        UserAuthnMethod.__init__(self, upstream_get=upstream_get)
         self.passwd = pwd
         self.ttl = ttl
 
     def verify_password(self, user, password):
         if password != self.passwd[user]:
             raise FailedAuthentication("Wrong password")
 
@@ -244,18 +269,19 @@
         res = {"uid": user}
         if cookie:
             res.update(self.cookie_info(cookie, client_id))
         return res, utc_time_sans_frac()
 
 
 class SymKeyAuthn(UserAuthnMethod):
+
     # user authentication using a token
 
-    def __init__(self, ttl, symkey, server_get=None):
-        UserAuthnMethod.__init__(self, server_get=server_get)
+    def __init__(self, ttl, symkey, upstream_get=None):
+        UserAuthnMethod.__init__(self, upstream_get=upstream_get)
 
         if symkey is not None and symkey == "":
             msg = "SymKeyAuthn.symkey cannot be an empty value"
             raise ImproperlyConfigured(msg)
         self.symkey = symkey.encode() if isinstance(symkey, str) else symkey
         self.ttl = ttl
 
@@ -278,18 +304,19 @@
         if cookie:
             res.update(self.cookie_info(cookie, client_id))
 
         return res, utc_time_sans_frac()
 
 
 class NoAuthn(UserAuthnMethod):
+
     # Just for testing allows anyone it without authentication
 
-    def __init__(self, user, server_get=None):
-        UserAuthnMethod.__init__(self, server_get=server_get)
+    def __init__(self, user, upstream_get=None):
+        UserAuthnMethod.__init__(self, upstream_get=upstream_get)
         self.user = user
         self.fail = None
 
     def authenticated_as(self, client_id="", cookie=None, authorization="", **kwargs):
         """
 
         :param cookie: A list of Cookie information
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/user_info/__init__.py` & `idpyoidc-2.0.0/src/idpyoidc/server/user_info/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/server/util.py` & `idpyoidc-2.0.0/src/idpyoidc/server/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import json
 import logging
 
 from idpyoidc.util import importer
-
 from .exception import OidcEndpointError
 
 logger = logging.getLogger(__name__)
 
 OAUTH2_NOCACHE_HEADERS = [("Pragma", "no-cache"), ("Cache-Control", "no-store")]
 
 
-def build_endpoints(conf, server_get, issuer):
+def build_endpoints(conf, upstream_get, issuer):
     """
     conf typically contains::
 
         'provider_config': {
             'path': '.well-known/openid-configuration',
             'class': ProviderConfiguration,
             'kwargs': {}
         },
 
     This function uses class and kwargs to instantiate a class instance with kwargs.
 
     :param conf:
-    :param server_get: Callback function
+    :param upstream_get: Callback function
     :param issuer:
     :return:
     """
 
     if issuer.endswith("/"):
         _url = issuer[:-1]
     else:
@@ -35,39 +34,34 @@
 
     endpoint = {}
     for name, spec in conf.items():
         kwargs = spec.get("kwargs", {})
 
         # class can be a string (class path) or a class reference
         if isinstance(spec["class"], str):
-            _instance = importer(spec["class"])(server_get=server_get, **kwargs)
+            _instance = importer(spec["class"])(upstream_get=upstream_get, **kwargs)
         else:
-            _instance = spec["class"](server_get=server_get, **kwargs)
+            _instance = spec["class"](upstream_get=upstream_get, **kwargs)
 
         try:
             _path = spec["path"]
         except KeyError:
             # Should there be a default ?
             raise
 
         _instance.endpoint_path = _path
         _instance.full_path = "{}/{}".format(_url, _path)
 
-        # if _instance.endpoint_name:
-        #     try:
-        #         _instance.endpoint_info[_instance.endpoint_name] = _instance.full_path
-        #     except TypeError:
-        #         _instance.endpoint_info = {_instance.endpoint_name: _instance.full_path}
-
         endpoint[_instance.name] = _instance
 
     return endpoint
 
 
 class JSONDictDB(object):
+
     def __init__(self, filename):
         with open(filename, "r") as f:
             self._db = json.load(f)
 
     def __getitem__(self, item):
         return self._db[item]
 
@@ -96,15 +90,15 @@
     :return: a list og values
     """
     txt = txt.strip()
     res = []
     while txt:
         l, v = txt.split(":", 1)
         res.append(v[: int(l)])
-        txt = v[int(l) :]
+        txt = v[int(l):]
     return res
 
 
 def get_http_params(config):
     _verify_ssl = config.get("verify")
     if _verify_ssl is None:
         _verify_ssl = config.get("verify_ssl")
@@ -123,25 +117,25 @@
             params["cert"] = _cert
     elif _key:
         raise ValueError("Key without cert is no good")
 
     return params
 
 
-def allow_refresh_token(endpoint_context):
+def allow_refresh_token(context):
     # Are there a refresh_token handler
-    refresh_token_handler = endpoint_context.session_manager.token_handler.handler.get(
+    refresh_token_handler = context.session_manager.token_handler.handler.get(
         "refresh_token"
     )
 
     # Is refresh_token grant type supported
     _token_supported = False
-    _cap = endpoint_context.conf.get("capabilities")
-    if _cap:
-        if "refresh_token" in _cap["grant_types_supported"]:
+    _supported = context.get_preference("grant_types_supported")
+    if _supported:
+        if "refresh_token" in _supported:
             # self.allow_refresh = kwargs.get("allow_refresh", True)
             _token_supported = True
 
     if refresh_token_handler and _token_supported:
         return True
     elif refresh_token_handler:
         logger.warning("Refresh Token handler available but grant type not supported")
@@ -171,39 +165,7 @@
             if isinstance(_function, str):
                 _func = importer(_function)
             else:
                 _func = _function
             return _func(**kwargs)
         else:
             return kwargs
-
-
-# def sector_id_from_redirect_uris(uris):
-#     if not uris:
-#         return ""
-#
-#     _parts = urlparse(uris[0])
-#     hostname = _parts.netloc
-#     scheme = _parts.scheme
-#     for uri in uris[1:]:
-#         parsed = urlparse(uri)
-#         if scheme != parsed.scheme or hostname != parsed.netloc:
-#             raise ValueError(
-#                 "All redirect_uris must have the same hostname in order to generate sector_id."
-#             )
-#
-#     return urlunsplit((scheme, hostname, "", "", ""))
-
-
-# def get_logout_id(endpoint_context, user_id, client_id):
-#     _item = NodeInfo()
-#     _item.user_id = user_id
-#     _item.client_id = client_id
-#
-#     # Note that this session ID is not the session ID the session manager is using.
-#     # It must be possible to map from one to the other.
-#     logout_session_id = uuid.uuid4().hex
-#     # Store the map
-#     _mngr = endpoint_context.session_manager
-#     _mngr.set([logout_session_id], _item)
-#
-#     return logout_session_id
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/ssl_context.py` & `idpyoidc-2.0.0/src/idpyoidc/ssl_context.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-1.4.0/src/idpyoidc/storage/abfile.py` & `idpyoidc-2.0.0/src/idpyoidc/storage/abfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,27 @@
 from idpyoidc.util import QPKey
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractFileSystem(DictType):
     """
-    FileSystem implements a simple file based database.
+    FileSystem implements a simple read-only file based database.
     It has a dictionary like interface.
     Each key maps one-to-one to a file on disc, where the content of the
     file is the value.
     ONLY goes one level deep.
     Not directories in directories.
     """
 
     def __init__(
-        self, fdir: Optional[str] = "", key_conv: Optional[str] = "", value_conv: Optional[str] = ""
+        self, fdir: Optional[str] = "",
+            key_conv: Optional[str] = "",
+            value_conv: Optional[str] = "",
+            **kwargs
     ):
         """
         items = FileSystem(
             {
                 'fdir': fdir,
                 'key_conv':{'to': quote_plus, 'from': unquote_plus},
                 'value_conv':{'to': keyjar_to_jwks, 'from': jwks_to_keyjar}
@@ -83,14 +86,15 @@
 
         if self.is_changed(item):
             logger.info("File content change in {}".format(item))
             fname = os.path.join(self.fdir, item)
             self.storage[item] = self._read_info(fname)
 
         logger.debug('Read from "%s"', item)
+        # storage values are already value converted
         return self.storage[item]
 
     def __setitem__(self, key, value):
         """
         Binds a value to a specific key. If the file that the key maps to
         does not exist it will be created. The content of the file will be
         set to the value given.
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/time_util.py` & `idpyoidc-2.0.0/src/idpyoidc/time_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 
 TIME_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 TIME_FORMAT_WITH_FRAGMENT = re.compile("^(\d{4,4}-\d{2,2}-\d{2,2}T\d{2,2}:\d{2,2}:\d{2,2})\.\d*Z$")
 
-
 logger = logging.getLogger(__name__)
 
 
 class TimeUtilError(Exception):
     pass
 
 
@@ -101,19 +100,19 @@
                     raise TimeUtilError("Not allowed to end with 'T'")
             else:
                 raise TimeUtilError("Missing T")
         else:
             try:
                 mod = duration[index:].index(code)
                 try:
-                    dic[typ] = int(duration[index : index + mod])
+                    dic[typ] = int(duration[index: index + mod])
                 except ValueError:
                     if code == "S":
                         try:
-                            dic[typ] = float(duration[index : index + mod])
+                            dic[typ] = float(duration[index: index + mod])
                         except ValueError:
                             raise TimeUtilError("Not a float")
                     else:
                         raise TimeUtilError("Fractions not allow on anything byt seconds")
                 index = mod + index + 1
             except ValueError:
                 dic[typ] = 0
@@ -182,15 +181,15 @@
     """
     delta = timedelta(days, seconds, microseconds, milliseconds, minutes, hours, weeks)
     res = datetime.now(timezone.utc) + delta
     return res.replace(tzinfo=None)
 
 
 def time_a_while_ago(
-    days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0
+        days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0
 ):
     """
     Will return a time specification for a time sometime in the past.
 
     :param days:
     :param seconds:
     :param microseconds:
@@ -202,22 +201,22 @@
     """
     delta = timedelta(days, seconds, microseconds, milliseconds, minutes, hours, weeks)
     res = datetime.now(timezone.utc) - delta
     return res.replace(tzinfo=None)
 
 
 def in_a_while(
-    days=0,
-    seconds=0,
-    microseconds=0,
-    milliseconds=0,
-    minutes=0,
-    hours=0,
-    weeks=0,
-    time_format=TIME_FORMAT,
+        days=0,
+        seconds=0,
+        microseconds=0,
+        milliseconds=0,
+        minutes=0,
+        hours=0,
+        weeks=0,
+        time_format=TIME_FORMAT,
 ):
     """
     :param days:
     :param seconds:
     :param microseconds:
     :param milliseconds:
     :param minutes:
@@ -231,22 +230,22 @@
 
     return time_in_a_while(
         days, seconds, microseconds, milliseconds, minutes, hours, weeks
     ).strftime(time_format)
 
 
 def a_while_ago(
-    days=0,
-    seconds=0,
-    microseconds=0,
-    milliseconds=0,
-    minutes=0,
-    hours=0,
-    weeks=0,
-    time_format=TIME_FORMAT,
+        days=0,
+        seconds=0,
+        microseconds=0,
+        milliseconds=0,
+        minutes=0,
+        hours=0,
+        weeks=0,
+        time_format=TIME_FORMAT,
 ):
     """
 
     :param days:
     :param seconds:
     :param microseconds:
     :param milliseconds:
@@ -358,15 +357,15 @@
 
 
 def time_sans_frac():
     return int("%d" % time.time())
 
 
 def epoch_in_a_while(
-    days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0
+        days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0
 ):
     """
     Return the number of seconds since epoch a while from now.
 
     :param days:
     :param seconds:
     :param microseconds:
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc/util.py` & `idpyoidc-2.0.0/src/idpyoidc/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,30 +80,33 @@
         return [base, None]
 
 
 # Converters
 
 
 class QPKey:
+
     def serialize(self, str):
         return quote_plus(str)
 
     def deserialize(self, str):
         return unquote_plus(str)
 
 
 class JSON:
+
     def serialize(self, str):
         return json.dumps(str)
 
     def deserialize(self, str):
         return json.loads(str)
 
 
 class PassThru:
+
     def serialize(self, str):
         return str
 
     def deserialize(self, str):
         return str
 
 
@@ -135,14 +138,15 @@
             return "{}{}".format(url, path)
     else:
         if path.startswith("/"):
             return "{}{}".format(url, path)
         else:
             return "{}/{}".format(url, path)
 
+
 def qualified_name(cls):
     """Does both classes and class instances
 
     :param cls: The item, class or class instance
     :return: fully qualified class name
     """
```

### Comparing `idpyoidc-1.4.0/src/idpyoidc.egg-info/PKG-INFO` & `idpyoidc-2.0.0/src/idpyoidc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: idpyoidc
-Version: 1.4.0
+Version: 2.0.0
 Summary: Python implementation of everything OAuth2 and OpenID Connect
 Home-page: https://github.com/IdentityPython/idpy-oidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # idpyoidc
 
 ![CI build](https://github.com/IdentityPython/idpy-oidc/workflows/idpy-oidc/badge.svg)
```

