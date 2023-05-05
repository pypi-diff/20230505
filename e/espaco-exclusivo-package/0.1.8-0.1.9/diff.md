# Comparing `tmp/espaco_exclusivo_package-0.1.8.tar.gz` & `tmp/espaco_exclusivo_package-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espaco_exclusivo_package-0.1.8.tar", last modified: Sat Feb 19 18:39:08 2022, max compression
+gzip compressed data, was "espaco_exclusivo_package-0.1.9.tar", last modified: Mon Apr  4 21:51:49 2022, max compression
```

## Comparing `espaco_exclusivo_package-0.1.8.tar` & `espaco_exclusivo_package-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.329944 espaco_exclusivo_package-0.1.8/
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1091 2021-07-21 17:46:22.000000 espaco_exclusivo_package-0.1.8/LICENSE
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1937 2022-02-19 18:39:08.330078 espaco_exclusivo_package-0.1.8/PKG-INFO
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1263 2021-12-10 11:32:22.000000 espaco_exclusivo_package-0.1.8/README.md
--rwxrwxrwx   0 diego     (1000) diego     (1000)      108 2021-07-21 16:45:09.000000 espaco_exclusivo_package-0.1.8/pyproject.toml
--rwxrwxrwx   0 diego     (1000) diego     (1000)      790 2022-02-19 18:39:08.330706 espaco_exclusivo_package-0.1.8/setup.cfg
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1064 2022-02-19 18:33:52.000000 espaco_exclusivo_package-0.1.8/setup.py
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.291098 espaco_exclusivo_package-0.1.8/src/
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.296616 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/
--rwxrwxrwx   0 diego     (1000) diego     (1000)      122 2021-07-22 00:35:08.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/__init__.py
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.298747 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/auth/
--rwxrwxrwx   0 diego     (1000) diego     (1000)      555 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/auth/__init__.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     3939 2022-02-10 16:37:03.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/auth/auth_manager.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     5858 2022-02-19 18:12:23.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/configuration.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)      915 2021-12-10 11:20:03.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/enum_produto.py
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.300919 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/
--rwxrwxrwx   0 diego     (1000) diego     (1000)      578 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/__init__.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1276 2021-08-25 17:33:38.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/base_produto.py
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.303040 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/file_viewer/
--rwxrwxrwx   0 diego     (1000) diego     (1000)      562 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/file_viewer/__init__.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     2991 2022-02-10 14:37:48.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/file_viewer/file_viewer.py
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.313754 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1023 2021-12-10 11:16:33.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/__init__.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     5455 2022-02-01 20:15:53.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     3594 2022-02-01 20:15:53.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado_cenario.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     3111 2022-02-01 20:15:53.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado_cenario_bloco.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     3433 2022-02-10 14:37:53.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/ena_diaria.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     4048 2022-02-10 14:37:56.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_automatrico.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     3181 2022-02-10 14:37:59.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_ec_46.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     3175 2022-02-10 14:38:02.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_gt.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     3223 2022-02-10 14:38:04.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_historico.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     6768 2022-02-10 14:38:31.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_personalizado.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     5990 2022-02-10 14:37:44.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_upload.py
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.324597 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1052 2022-02-19 18:27:47.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/__init__.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     5398 2021-08-18 12:27:52.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/body_chuva_observada.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)    15128 2021-11-23 18:14:11.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/body_comparador.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)      998 2021-07-23 21:52:27.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_dias_modelos.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)      640 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_meteorologia_prazo.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1138 2021-08-25 17:42:44.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_modelos.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1147 2022-02-19 18:20:22.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_modelos_data_store.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)      715 2022-02-19 18:28:08.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_niveis_atm.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)      640 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_tipo_comparacao.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)      628 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_tipo_periodo.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)      799 2022-02-19 18:28:55.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_variaveis_meteorologicas.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     9098 2022-02-19 18:32:52.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/meteorologia.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     7709 2021-07-23 22:49:56.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/request_manager.py
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.326051 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/utils/
--rwxrwxrwx   0 diego     (1000) diego     (1000)      629 2021-07-23 21:41:04.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/utils/__init__.py
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1188 2022-02-01 20:15:53.000000 espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/utils/modelos_max_date.py
-drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-02-19 18:39:08.329436 espaco_exclusivo_package-0.1.8/src/espaco_exclusivo_package.egg-info/
--rwxrwxrwx   0 diego     (1000) diego     (1000)     1937 2022-02-19 18:39:08.000000 espaco_exclusivo_package-0.1.8/src/espaco_exclusivo_package.egg-info/PKG-INFO
--rwxrwxrwx   0 diego     (1000) diego     (1000)     2387 2022-02-19 18:39:08.000000 espaco_exclusivo_package-0.1.8/src/espaco_exclusivo_package.egg-info/SOURCES.txt
--rwxrwxrwx   0 diego     (1000) diego     (1000)        1 2022-02-19 18:39:08.000000 espaco_exclusivo_package-0.1.8/src/espaco_exclusivo_package.egg-info/dependency_links.txt
--rwxrwxrwx   0 diego     (1000) diego     (1000)       27 2022-02-19 18:39:08.000000 espaco_exclusivo_package-0.1.8/src/espaco_exclusivo_package.egg-info/requires.txt
--rwxrwxrwx   0 diego     (1000) diego     (1000)       22 2022-02-19 18:39:08.000000 espaco_exclusivo_package-0.1.8/src/espaco_exclusivo_package.egg-info/top_level.txt
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.435009 espaco_exclusivo_package-0.1.9/
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1091 2021-07-21 17:46:22.000000 espaco_exclusivo_package-0.1.9/LICENSE
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1937 2022-04-04 21:51:49.435186 espaco_exclusivo_package-0.1.9/PKG-INFO
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1263 2021-12-10 11:32:22.000000 espaco_exclusivo_package-0.1.9/README.md
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      108 2021-07-21 16:45:09.000000 espaco_exclusivo_package-0.1.9/pyproject.toml
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      790 2022-04-04 21:51:49.435996 espaco_exclusivo_package-0.1.9/setup.cfg
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1064 2022-04-04 21:51:16.000000 espaco_exclusivo_package-0.1.9/setup.py
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.392490 espaco_exclusivo_package-0.1.9/src/
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.399643 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      122 2021-07-22 00:35:08.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/__init__.py
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.401453 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/auth/
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      555 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/auth/__init__.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     3939 2022-02-10 16:37:03.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/auth/auth_manager.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     5858 2022-02-19 18:12:23.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/configuration.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      915 2021-12-10 11:20:03.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/enum_produto.py
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.403217 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      578 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/__init__.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1276 2021-08-25 17:33:38.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/base_produto.py
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.404946 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/file_viewer/
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      562 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/file_viewer/__init__.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     2991 2022-02-10 14:37:48.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/file_viewer/file_viewer.py
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.416539 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1023 2021-12-10 11:16:33.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/__init__.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     5455 2022-02-01 20:15:53.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     3594 2022-02-01 20:15:53.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado_cenario.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     3111 2022-02-01 20:15:53.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado_cenario_bloco.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     3439 2022-04-04 21:49:40.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/ena_diaria.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     4048 2022-02-10 14:37:56.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_automatrico.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     3181 2022-02-10 14:37:59.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_ec_46.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     3175 2022-02-10 14:38:02.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_gt.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     3223 2022-02-10 14:38:04.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_historico.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     6768 2022-02-10 14:38:31.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_personalizado.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     5990 2022-02-10 14:37:44.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_upload.py
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.429038 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1052 2022-02-19 18:27:47.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/__init__.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     5398 2021-08-18 12:27:52.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/body_chuva_observada.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)    15128 2021-11-23 18:14:11.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/body_comparador.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      998 2021-07-23 21:52:27.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_dias_modelos.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      640 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_meteorologia_prazo.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1138 2021-08-25 17:42:44.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_modelos.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1147 2022-02-19 18:20:22.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_modelos_data_store.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      715 2022-02-19 18:28:08.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_niveis_atm.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      640 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_tipo_comparacao.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      628 2021-07-22 02:05:44.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_tipo_periodo.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      799 2022-02-19 18:28:55.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_variaveis_meteorologicas.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     9098 2022-02-19 18:32:52.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/meteorologia.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     7709 2021-07-23 22:49:56.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/request_manager.py
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.431155 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/utils/
+-rwxrwxrwx   0 diego     (1000) diego     (1000)      629 2021-07-23 21:41:04.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/utils/__init__.py
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1188 2022-02-01 20:15:53.000000 espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/utils/modelos_max_date.py
+drwxrwxrwx   0 diego     (1000) diego     (1000)        0 2022-04-04 21:51:49.434258 espaco_exclusivo_package-0.1.9/src/espaco_exclusivo_package.egg-info/
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     1937 2022-04-04 21:51:48.000000 espaco_exclusivo_package-0.1.9/src/espaco_exclusivo_package.egg-info/PKG-INFO
+-rwxrwxrwx   0 diego     (1000) diego     (1000)     2387 2022-04-04 21:51:49.000000 espaco_exclusivo_package-0.1.9/src/espaco_exclusivo_package.egg-info/SOURCES.txt
+-rwxrwxrwx   0 diego     (1000) diego     (1000)        1 2022-04-04 21:51:49.000000 espaco_exclusivo_package-0.1.9/src/espaco_exclusivo_package.egg-info/dependency_links.txt
+-rwxrwxrwx   0 diego     (1000) diego     (1000)       27 2022-04-04 21:51:49.000000 espaco_exclusivo_package-0.1.9/src/espaco_exclusivo_package.egg-info/requires.txt
+-rwxrwxrwx   0 diego     (1000) diego     (1000)       22 2022-04-04 21:51:49.000000 espaco_exclusivo_package-0.1.9/src/espaco_exclusivo_package.egg-info/top_level.txt
```

### Comparing `espaco_exclusivo_package-0.1.8/LICENSE` & `espaco_exclusivo_package-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/PKG-INFO` & `espaco_exclusivo_package-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espaco_exclusivo_package
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pacote de métodos usados para implementação da API de acesso aos produtos Ampere Consultoria
 Home-page: https://gitlab.com/diego.yosiura.ampere/espaco-exclusivo-package.git
 Author: Diego Isaac Haruwo Yosiura
 Author-email: diego@ampereconsultoria.com.br
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/diego.yosiura.ampere/espaco-exclusivo-package/-/issues
 Platform: UNKNOWN
```

### Comparing `espaco_exclusivo_package-0.1.8/README.md` & `espaco_exclusivo_package-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/setup.cfg` & `espaco_exclusivo_package-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = espaco_exclusivo_package
-version = 0.1.8
+version = 0.1.9
 author = Diego Isaac Haruwo Yosiura
 author_email = diego@ampereconsultoria.com.br
 description = Pacote de métodos usados para implementação da API de acesso aos produtos Ampere Consultoria
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = 
 project_urls = https://gitlab.com/diego.yosiura.ampere/espaco-exclusivo-package.git
```

### Comparing `espaco_exclusivo_package-0.1.8/setup.py` & `espaco_exclusivo_package-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="espaco_exclusivo_package",
-    version="0.1.8",
+    version="0.1.9",
     author="Diego Isaac Haruwo Yosiura",
     author_email="diego@ampereconsultoria.com.br",
     description="Pacote de métodos usados para implementação da API de acesso aos produtos Ampere Consultoria",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/diego.yosiura.ampere/espaco-exclusivo-package.git",
     project_urls={
```

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/auth/__init__.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/auth/auth_manager.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/configuration.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/configuration.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/enum_produto.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/enum_produto.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/__init__.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/__init__.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/base_produto.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/base_produto.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/file_viewer/__init__.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/file_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/file_viewer/file_viewer.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/file_viewer/file_viewer.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/__init__.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/__init__.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado_cenario.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado_cenario.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado_cenario_bloco.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/body_flux_personalizado_cenario_bloco.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/ena_diaria.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/ena_diaria.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         :type versao: str
         :param subdivisao: Subdivisão - Submercado, REE, BACIA ETC.
         :type subdivisao: str
         :return: Retorna uma lista com as ENAs para os dados selecionados.
         :rtype: dict
         """
         try:
-            p_key = self.request.request_prod_key(Produto.FLUX_EC46.value)
+            p_key = self.request.request_prod_key(Produto.FLUX_AUTOMATICO.value)
             response = self.request.request_json('flux.ena_diaria.get_cenario?product_key={}'.format(p_key), dumps({
                 "run_time": run_time,
                 "modelo": modelo,
                 "versao": versao,
                 "subdivisao": subdivisao
             }))
             if response is not None:
```

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_automatrico.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_automatrico.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_ec_46.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_ec_46.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_gt.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_gt.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_historico.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_historico.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_personalizado.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_personalizado.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/flux/flux_upload.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/flux/flux_upload.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/__init__.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/__init__.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/body_chuva_observada.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/body_chuva_observada.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/body_comparador.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/body_comparador.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_dias_modelos.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_dias_modelos.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_meteorologia_prazo.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_meteorologia_prazo.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_modelos.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_modelos.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_modelos_data_store.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_modelos_data_store.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_niveis_atm.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_niveis_atm.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_tipo_comparacao.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_tipo_comparacao.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_tipo_periodo.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_tipo_periodo.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/enum_variaveis_meteorologicas.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/enum_variaveis_meteorologicas.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/produtos/meteorologia/meteorologia.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/produtos/meteorologia/meteorologia.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/request_manager.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/request_manager.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/utils/__init__.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/ee_ampere_consultoria/utils/modelos_max_date.py` & `espaco_exclusivo_package-0.1.9/src/ee_ampere_consultoria/utils/modelos_max_date.py`

 * *Files identical despite different names*

### Comparing `espaco_exclusivo_package-0.1.8/src/espaco_exclusivo_package.egg-info/PKG-INFO` & `espaco_exclusivo_package-0.1.9/src/espaco_exclusivo_package.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espaco-exclusivo-package
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pacote de métodos usados para implementação da API de acesso aos produtos Ampere Consultoria
 Home-page: https://gitlab.com/diego.yosiura.ampere/espaco-exclusivo-package.git
 Author: Diego Isaac Haruwo Yosiura
 Author-email: diego@ampereconsultoria.com.br
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/diego.yosiura.ampere/espaco-exclusivo-package/-/issues
 Platform: UNKNOWN
```

### Comparing `espaco_exclusivo_package-0.1.8/src/espaco_exclusivo_package.egg-info/SOURCES.txt` & `espaco_exclusivo_package-0.1.9/src/espaco_exclusivo_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

