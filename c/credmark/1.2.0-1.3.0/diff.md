# Comparing `tmp/credmark-1.2.0.tar.gz` & `tmp/credmark-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credmark-1.2.0.tar", max compression
+gzip compressed data, was "credmark-1.3.0.tar", max compression
```

## Comparing `credmark-1.2.0.tar` & `credmark-1.3.0.tar`

### file list

```diff
@@ -1,148 +1,142 @@
--rw-r--r--   0        0        0     4502 2023-04-14 09:02:54.717263 credmark-1.2.0/README.md
--rw-r--r--   0        0        0      110 2023-04-14 08:56:27.665903 credmark-1.2.0/credmark/__init__.py
--rw-r--r--   0        0        0       47 2023-04-14 08:56:24.698799 credmark-1.2.0/credmark/api/__init__.py
--rw-r--r--   0        0        0     9019 2023-04-14 08:56:27.884998 credmark-1.2.0/credmark/api/defi_api/__init__.py
--rw-r--r--   0        0        0     6959 2023-04-14 08:56:27.970634 credmark-1.2.0/credmark/api/defi_api/get_cached_model_results.py
--rw-r--r--   0        0        0     3679 2023-04-14 08:56:27.807883 credmark-1.2.0/credmark/api/defi_api/get_model_by_slug.py
--rw-r--r--   0        0        0     4016 2023-04-14 08:56:27.836973 credmark-1.2.0/credmark/api/defi_api/get_model_deployments_by_slug.py
--rw-r--r--   0        0        0     3513 2023-04-14 08:56:27.868895 credmark-1.2.0/credmark/api/defi_api/get_model_runtime_stats.py
--rw-r--r--   0        0        0     3725 2023-04-14 08:56:27.889006 credmark-1.2.0/credmark/api/defi_api/list_models.py
--rw-r--r--   0        0        0     3912 2023-04-14 08:56:27.900632 credmark-1.2.0/credmark/api/defi_api/run_model.py
--rw-r--r--   0        0        0    56689 2023-04-14 08:56:29.045156 credmark-1.2.0/credmark/api/token_api/__init__.py
--rw-r--r--   0        0        0     5906 2023-04-14 08:56:27.981855 credmark-1.2.0/credmark/api/token_api/get_token_abi.py
--rw-r--r--   0        0        0     7744 2023-04-14 08:56:28.020839 credmark-1.2.0/credmark/api/token_api/get_token_balance.py
--rw-r--r--   0        0        0    10931 2023-04-14 08:56:28.121722 credmark-1.2.0/credmark/api/token_api/get_token_balance_historical.py
--rw-r--r--   0        0        0     6164 2023-04-14 08:56:27.997295 credmark-1.2.0/credmark/api/token_api/get_token_creation_block.py
--rw-r--r--   0        0        0     6016 2023-04-14 08:56:28.034610 credmark-1.2.0/credmark/api/token_api/get_token_decimals.py
--rw-r--r--   0        0        0     8312 2023-04-14 08:56:28.108309 credmark-1.2.0/credmark/api/token_api/get_token_holders.py
--rw-r--r--   0        0        0     6270 2023-04-14 08:56:28.073692 credmark-1.2.0/credmark/api/token_api/get_token_holders_count.py
--rw-r--r--   0        0        0     9481 2023-04-14 08:56:28.174134 credmark-1.2.0/credmark/api/token_api/get_token_holders_count_historical.py
--rw-r--r--   0        0        0    11003 2023-04-14 08:56:28.204227 credmark-1.2.0/credmark/api/token_api/get_token_holders_historical.py
--rw-r--r--   0        0        0     5928 2023-04-14 08:56:28.104616 credmark-1.2.0/credmark/api/token_api/get_token_logo.py
--rw-r--r--   0        0        0     5997 2023-04-14 08:56:28.154689 credmark-1.2.0/credmark/api/token_api/get_token_metadata.py
--rw-r--r--   0        0        0     5928 2023-04-14 08:56:28.181157 credmark-1.2.0/credmark/api/token_api/get_token_name.py
--rw-r--r--   0        0        0     8463 2023-04-14 08:56:28.284400 credmark-1.2.0/credmark/api/token_api/get_token_price.py
--rw-r--r--   0        0        0    11037 2023-04-14 08:56:28.396076 credmark-1.2.0/credmark/api/token_api/get_token_price_historical.py
--rw-r--r--   0        0        0     5972 2023-04-14 08:56:28.212532 credmark-1.2.0/credmark/api/token_api/get_token_symbol.py
--rw-r--r--   0        0        0     6688 2023-04-14 08:56:28.288316 credmark-1.2.0/credmark/api/token_api/get_token_total_supply.py
--rw-r--r--   0        0        0     9871 2023-04-14 08:56:28.502047 credmark-1.2.0/credmark/api/token_api/get_token_total_supply_historical.py
--rw-r--r--   0        0        0     8342 2023-04-14 08:56:28.445443 credmark-1.2.0/credmark/api/token_api/get_token_volume.py
--rw-r--r--   0        0        0     9947 2023-04-14 08:56:28.528577 credmark-1.2.0/credmark/api/token_api/get_token_volume_historical.py
--rw-r--r--   0        0        0     5344 2023-04-14 08:56:28.274887 credmark-1.2.0/credmark/api/utilities/__init__.py
--rw-r--r--   0        0        0     3575 2023-04-14 08:56:28.336469 credmark-1.2.0/credmark/api/utilities/check_health.py
--rw-r--r--   0        0        0     5572 2023-04-14 08:56:28.469894 credmark-1.2.0/credmark/api/utilities/get_daily_model_usage.py
--rw-r--r--   0        0        0     3373 2023-04-14 08:56:28.393005 credmark-1.2.0/credmark/api/utilities/get_top_models.py
--rw-r--r--   0        0        0     3351 2023-04-14 08:56:28.363551 credmark-1.2.0/credmark/api/utilities/get_total_model_usage.py
--rw-r--r--   0        0        0     2645 2023-04-14 08:56:28.445048 credmark-1.2.0/credmark/client.py
--rw-r--r--   0        0        0      320 2023-04-14 08:56:24.676118 credmark-1.2.0/credmark/docs/CheckHealthResponse200.md
--rw-r--r--   0        0        0       79 2023-04-14 08:56:24.674820 credmark-1.2.0/credmark/docs/CheckHealthResponse200Details.md
--rw-r--r--   0        0        0      172 2023-04-14 08:56:24.674111 credmark-1.2.0/credmark/docs/CheckHealthResponse200DetailsAdditionalProperty.md
--rw-r--r--   0        0        0       33 2023-04-14 08:56:24.673351 credmark-1.2.0/credmark/docs/CheckHealthResponse200Error.md
--rw-r--r--   0        0        0      170 2023-04-14 08:56:24.672714 credmark-1.2.0/credmark/docs/CheckHealthResponse200ErrorAdditionalProperty.md
--rw-r--r--   0        0        0       76 2023-04-14 08:56:24.671916 credmark-1.2.0/credmark/docs/CheckHealthResponse200Info.md
--rw-r--r--   0        0        0      169 2023-04-14 08:56:24.671265 credmark-1.2.0/credmark/docs/CheckHealthResponse200InfoAdditionalProperty.md
--rw-r--r--   0        0        0      320 2023-04-14 08:56:24.685073 credmark-1.2.0/credmark/docs/CheckHealthResponse503.md
--rw-r--r--   0        0        0      140 2023-04-14 08:56:24.683093 credmark-1.2.0/credmark/docs/CheckHealthResponse503Details.md
--rw-r--r--   0        0        0      172 2023-04-14 08:56:24.681879 credmark-1.2.0/credmark/docs/CheckHealthResponse503DetailsAdditionalProperty.md
--rw-r--r--   0        0        0      108 2023-04-14 08:56:24.680640 credmark-1.2.0/credmark/docs/CheckHealthResponse503Error.md
--rw-r--r--   0        0        0      170 2023-04-14 08:56:24.679588 credmark-1.2.0/credmark/docs/CheckHealthResponse503ErrorAdditionalProperty.md
--rw-r--r--   0        0        0       76 2023-04-14 08:56:24.678427 credmark-1.2.0/credmark/docs/CheckHealthResponse503Info.md
--rw-r--r--   0        0        0      169 2023-04-14 08:56:24.677184 credmark-1.2.0/credmark/docs/CheckHealthResponse503InfoAdditionalProperty.md
--rw-r--r--   0        0        0     2390 2023-04-14 08:56:24.852030 credmark-1.2.0/credmark/docs/DefiApi.md
--rw-r--r--   0        0        0      390 2023-04-14 08:56:24.630981 credmark-1.2.0/credmark/docs/ModelCallStackEntry.md
--rw-r--r--   0        0        0      259 2023-04-14 08:56:24.583458 credmark-1.2.0/credmark/docs/ModelDeployment.md
--rw-r--r--   0        0        0      519 2023-04-14 08:56:24.582365 credmark-1.2.0/credmark/docs/ModelMetadata.md
--rw-r--r--   0        0        0      753 2023-04-14 08:56:24.634974 credmark-1.2.0/credmark/docs/ModelRunResponse.md
--rw-r--r--   0        0        0      637 2023-04-14 08:56:24.633299 credmark-1.2.0/credmark/docs/ModelRunResponseError.md
--rw-r--r--   0        0        0      418 2023-04-14 08:56:24.585965 credmark-1.2.0/credmark/docs/ModelRuntimeStatistics.md
--rw-r--r--   0        0        0      165 2023-04-14 08:56:24.609660 credmark-1.2.0/credmark/docs/ModelRuntimeStatsResponse.md
--rw-r--r--   0        0        0      485 2023-04-14 08:56:24.629868 credmark-1.2.0/credmark/docs/RunModelDto.md
--rw-r--r--   0        0        0      597 2023-04-14 08:56:24.648253 credmark-1.2.0/credmark/docs/TokenAbiResponse.md
--rw-r--r--   0        0        0    10810 2023-04-14 08:56:24.948548 credmark-1.2.0/credmark/docs/TokenApi.md
--rw-r--r--   0        0        0      318 2023-04-14 08:56:24.655738 credmark-1.2.0/credmark/docs/TokenBalanceHistoricalItem.md
--rw-r--r--   0        0        0      646 2023-04-14 08:56:24.657361 credmark-1.2.0/credmark/docs/TokenBalanceHistoricalResponse.md
--rw-r--r--   0        0        0      530 2023-04-14 08:56:24.654720 credmark-1.2.0/credmark/docs/TokenBalanceResponse.md
--rw-r--r--   0        0        0      371 2023-04-14 08:56:24.646446 credmark-1.2.0/credmark/docs/TokenCreationBlockResponse.md
--rw-r--r--   0        0        0      347 2023-04-14 08:56:24.640804 credmark-1.2.0/credmark/docs/TokenDecimalsResponse.md
--rw-r--r--   0        0        0      491 2023-04-14 08:56:24.637582 credmark-1.2.0/credmark/docs/TokenErrorResponse.md
--rw-r--r--   0        0        0      518 2023-04-14 08:56:24.670518 credmark-1.2.0/credmark/docs/TokenHistoricalHoldersCountResponse.md
--rw-r--r--   0        0        0      214 2023-04-14 08:56:24.662523 credmark-1.2.0/credmark/docs/TokenHolder.md
--rw-r--r--   0        0        0      283 2023-04-14 08:56:24.668823 credmark-1.2.0/credmark/docs/TokenHoldersCountHistoricalItem.md
--rw-r--r--   0        0        0      357 2023-04-14 08:56:24.667985 credmark-1.2.0/credmark/docs/TokenHoldersCountResponse.md
--rw-r--r--   0        0        0      336 2023-04-14 08:56:24.665253 credmark-1.2.0/credmark/docs/TokenHoldersHistoricalItem.md
--rw-r--r--   0        0        0      646 2023-04-14 08:56:24.666945 credmark-1.2.0/credmark/docs/TokenHoldersHistoricalResponse.md
--rw-r--r--   0        0        0      613 2023-04-14 08:56:24.664174 credmark-1.2.0/credmark/docs/TokenHoldersResponse.md
--rw-r--r--   0        0        0      341 2023-04-14 08:56:24.645373 credmark-1.2.0/credmark/docs/TokenLogoResponse.md
--rw-r--r--   0        0        0      399 2023-04-14 08:56:24.636255 credmark-1.2.0/credmark/docs/TokenMetadataResponse.md
--rw-r--r--   0        0        0      333 2023-04-14 08:56:24.638623 credmark-1.2.0/credmark/docs/TokenNameResponse.md
--rw-r--r--   0        0        0      379 2023-04-14 08:56:24.651782 credmark-1.2.0/credmark/docs/TokenPriceHistoricalItem.md
--rw-r--r--   0        0        0      582 2023-04-14 08:56:24.653344 credmark-1.2.0/credmark/docs/TokenPriceHistoricalResponse.md
--rw-r--r--   0        0        0      531 2023-04-14 08:56:24.650158 credmark-1.2.0/credmark/docs/TokenPriceResponse.md
--rw-r--r--   0        0        0      339 2023-04-14 08:56:24.639730 credmark-1.2.0/credmark/docs/TokenSymbolResponse.md
--rw-r--r--   0        0        0      284 2023-04-14 08:56:24.642757 credmark-1.2.0/credmark/docs/TokenTotalSupplyHistoricalItem.md
--rw-r--r--   0        0        0      581 2023-04-14 08:56:24.644260 credmark-1.2.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md
--rw-r--r--   0        0        0      423 2023-04-14 08:56:24.641941 credmark-1.2.0/credmark/docs/TokenTotalSupplyResponse.md
--rw-r--r--   0        0        0      404 2023-04-14 08:56:24.659805 credmark-1.2.0/credmark/docs/TokenVolumeHistoricalItem.md
--rw-r--r--   0        0        0      565 2023-04-14 08:56:24.661611 credmark-1.2.0/credmark/docs/TokenVolumeHistoricalResponse.md
--rw-r--r--   0        0        0      537 2023-04-14 08:56:24.658717 credmark-1.2.0/credmark/docs/TokenVolumeResponse.md
--rw-r--r--   0        0        0     1213 2023-04-14 08:56:24.828376 credmark-1.2.0/credmark/docs/Utilities.md
--rw-r--r--   0        0        0      592 2023-04-14 08:56:28.312151 credmark-1.2.0/credmark/errors.py
--rw-r--r--   0        0        0     5618 2023-04-14 08:56:24.693188 credmark-1.2.0/credmark/models/__init__.py
--rw-r--r--   0        0        0     4203 2023-04-14 08:56:28.620678 credmark-1.2.0/credmark/models/check_health_response_200.py
--rw-r--r--   0        0        0     2144 2023-04-14 08:56:28.501048 credmark-1.2.0/credmark/models/check_health_response_200_details.py
--rw-r--r--   0        0        0     1658 2023-04-14 08:56:28.446169 credmark-1.2.0/credmark/models/check_health_response_200_details_additional_property.py
--rw-r--r--   0        0        0     2061 2023-04-14 08:56:28.531334 credmark-1.2.0/credmark/models/check_health_response_200_error.py
--rw-r--r--   0        0        0     1648 2023-04-14 08:56:28.509615 credmark-1.2.0/credmark/models/check_health_response_200_error_additional_property.py
--rw-r--r--   0        0        0     2074 2023-04-14 08:56:28.570637 credmark-1.2.0/credmark/models/check_health_response_200_info.py
--rw-r--r--   0        0        0     1643 2023-04-14 08:56:28.550145 credmark-1.2.0/credmark/models/check_health_response_200_info_additional_property.py
--rw-r--r--   0        0        0     4364 2023-04-14 08:56:28.700870 credmark-1.2.0/credmark/models/check_health_response_503.py
--rw-r--r--   0        0        0     2205 2023-04-14 08:56:28.559117 credmark-1.2.0/credmark/models/check_health_response_503_details.py
--rw-r--r--   0        0        0     1658 2023-04-14 08:56:28.570637 credmark-1.2.0/credmark/models/check_health_response_503_details_additional_property.py
--rw-r--r--   0        0        0     2149 2023-04-14 08:56:28.605205 credmark-1.2.0/credmark/models/check_health_response_503_error.py
--rw-r--r--   0        0        0     1648 2023-04-14 08:56:28.597488 credmark-1.2.0/credmark/models/check_health_response_503_error_additional_property.py
--rw-r--r--   0        0        0     2074 2023-04-14 08:56:28.613731 credmark-1.2.0/credmark/models/check_health_response_503_info.py
--rw-r--r--   0        0        0     1643 2023-04-14 08:56:28.612026 credmark-1.2.0/credmark/models/check_health_response_503_info_additional_property.py
--rw-r--r--   0        0        0      165 2023-04-14 08:56:26.619117 credmark-1.2.0/credmark/models/get_cached_model_results_order.py
--rw-r--r--   0        0        0      166 2023-04-14 08:56:26.582381 credmark-1.2.0/credmark/models/get_token_price_align.py
--rw-r--r--   0        0        0      163 2023-04-14 08:56:26.527688 credmark-1.2.0/credmark/models/get_token_price_historical_src.py
--rw-r--r--   0        0        0      153 2023-04-14 08:56:26.623362 credmark-1.2.0/credmark/models/get_token_price_src.py
--rw-r--r--   0        0        0     2470 2023-04-14 08:56:28.691391 credmark-1.2.0/credmark/models/model_call_stack_entry.py
--rw-r--r--   0        0        0     1894 2023-04-14 08:56:28.644365 credmark-1.2.0/credmark/models/model_deployment.py
--rw-r--r--   0        0        0     3325 2023-04-14 08:56:28.740310 credmark-1.2.0/credmark/models/model_metadata.py
--rw-r--r--   0        0        0     4190 2023-04-14 08:56:28.753517 credmark-1.2.0/credmark/models/model_run_response.py
--rw-r--r--   0        0        0     3362 2023-04-14 08:56:28.726084 credmark-1.2.0/credmark/models/model_run_response_error.py
--rw-r--r--   0        0        0     2412 2023-04-14 08:56:28.723461 credmark-1.2.0/credmark/models/model_runtime_statistics.py
--rw-r--r--   0        0        0     2042 2023-04-14 08:56:28.712727 credmark-1.2.0/credmark/models/model_runtime_stats_response.py
--rw-r--r--   0        0        0     3294 2023-04-14 08:56:28.762660 credmark-1.2.0/credmark/models/run_model_dto.py
--rw-r--r--   0        0        0      204 2023-04-14 08:56:26.554457 credmark-1.2.0/credmark/models/run_model_dto_block_number_type_1.py
--rw-r--r--   0        0        0     5771 2023-04-14 08:56:28.762877 credmark-1.2.0/credmark/models/token_abi_response.py
--rw-r--r--   0        0        0     2319 2023-04-14 08:56:28.726249 credmark-1.2.0/credmark/models/token_balance_historical_item.py
--rw-r--r--   0        0        0     4365 2023-04-14 08:56:28.798583 credmark-1.2.0/credmark/models/token_balance_historical_response.py
--rw-r--r--   0        0        0     3378 2023-04-14 08:56:28.796025 credmark-1.2.0/credmark/models/token_balance_response.py
--rw-r--r--   0        0        0     2692 2023-04-14 08:56:28.782576 credmark-1.2.0/credmark/models/token_creation_block_response.py
--rw-r--r--   0        0        0     2587 2023-04-14 08:56:28.799948 credmark-1.2.0/credmark/models/token_decimals_response.py
--rw-r--r--   0        0        0     2779 2023-04-14 08:56:28.818334 credmark-1.2.0/credmark/models/token_error_response.py
--rw-r--r--   0        0        0     3856 2023-04-14 08:56:28.844892 credmark-1.2.0/credmark/models/token_historical_holders_count_response.py
--rw-r--r--   0        0        0     1836 2023-04-14 08:56:28.800079 credmark-1.2.0/credmark/models/token_holder.py
--rw-r--r--   0        0        0     2104 2023-04-14 08:56:28.814430 credmark-1.2.0/credmark/models/token_holders_count_historical_item.py
--rw-r--r--   0        0        0     2589 2023-04-14 08:56:28.854384 credmark-1.2.0/credmark/models/token_holders_count_response.py
--rw-r--r--   0        0        0     2693 2023-04-14 08:56:28.866891 credmark-1.2.0/credmark/models/token_holders_historical_item.py
--rw-r--r--   0        0        0     4365 2023-04-14 08:56:28.937892 credmark-1.2.0/credmark/models/token_holders_historical_response.py
--rw-r--r--   0        0        0     4074 2023-04-14 08:56:28.971375 credmark-1.2.0/credmark/models/token_holders_response.py
--rw-r--r--   0        0        0     2711 2023-04-14 08:56:28.938164 credmark-1.2.0/credmark/models/token_logo_response.py
--rw-r--r--   0        0        0     2951 2023-04-14 08:56:28.948089 credmark-1.2.0/credmark/models/token_metadata_response.py
--rw-r--r--   0        0        0     2527 2023-04-14 08:56:28.942016 credmark-1.2.0/credmark/models/token_name_response.py
--rw-r--r--   0        0        0     2551 2023-04-14 08:56:28.937111 credmark-1.2.0/credmark/models/token_price_historical_item.py
--rw-r--r--   0        0        0     4118 2023-04-14 08:56:28.981032 credmark-1.2.0/credmark/models/token_price_historical_response.py
--rw-r--r--   0        0        0     3387 2023-04-14 08:56:28.968433 credmark-1.2.0/credmark/models/token_price_response.py
--rw-r--r--   0        0        0     2553 2023-04-14 08:56:28.976542 credmark-1.2.0/credmark/models/token_symbol_response.py
--rw-r--r--   0        0        0     2168 2023-04-14 08:56:28.970052 credmark-1.2.0/credmark/models/token_total_supply_historical_item.py
--rw-r--r--   0        0        0     4072 2023-04-14 08:56:29.013026 credmark-1.2.0/credmark/models/token_total_supply_historical_response.py
--rw-r--r--   0        0        0     2881 2023-04-14 08:56:29.010022 credmark-1.2.0/credmark/models/token_total_supply_response.py
--rw-r--r--   0        0        0     2758 2023-04-14 08:56:29.006541 credmark-1.2.0/credmark/models/token_volume_historical_item.py
--rw-r--r--   0        0        0     4001 2023-04-14 08:56:29.033418 credmark-1.2.0/credmark/models/token_volume_historical_response.py
--rw-r--r--   0        0        0     3465 2023-04-14 08:56:29.022878 credmark-1.2.0/credmark/models/token_volume_response.py
--rw-r--r--   0        0        0       25 2023-04-14 08:56:24.547674 credmark-1.2.0/credmark/py.typed
--rw-r--r--   0        0        0      964 2023-04-14 08:56:28.981297 credmark-1.2.0/credmark/types.py
--rw-r--r--   0        0        0      853 2023-04-14 09:04:30.076824 credmark-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5384 1970-01-01 00:00:00.000000 credmark-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4502 2023-04-18 12:36:26.442770 credmark-1.3.0/README.md
+-rw-r--r--   0        0        0      110 2023-05-05 12:58:23.125826 credmark-1.3.0/credmark/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-05 12:58:20.691648 credmark-1.3.0/credmark/api/__init__.py
+-rw-r--r--   0        0        0     9643 2023-05-05 12:58:23.217765 credmark-1.3.0/credmark/api/defi_api/__init__.py
+-rw-r--r--   0        0        0     8159 2023-05-05 12:58:23.251810 credmark-1.3.0/credmark/api/defi_api/get_cached_model_results.py
+-rw-r--r--   0        0        0     3679 2023-05-05 12:58:23.191652 credmark-1.3.0/credmark/api/defi_api/get_model_by_slug.py
+-rw-r--r--   0        0        0     4016 2023-05-05 12:58:23.197737 credmark-1.3.0/credmark/api/defi_api/get_model_deployments_by_slug.py
+-rw-r--r--   0        0        0     3513 2023-05-05 12:58:23.195403 credmark-1.3.0/credmark/api/defi_api/get_model_runtime_stats.py
+-rw-r--r--   0        0        0     3725 2023-05-05 12:58:23.205315 credmark-1.3.0/credmark/api/defi_api/list_models.py
+-rw-r--r--   0        0        0     3912 2023-05-05 12:58:23.208691 credmark-1.3.0/credmark/api/defi_api/run_model.py
+-rw-r--r--   0        0        0    79472 2023-05-05 13:02:14.091929 credmark-1.3.0/credmark/api/token_api/__init__.py
+-rw-r--r--   0        0        0     7328 2023-05-05 12:58:23.254320 credmark-1.3.0/credmark/api/token_api/get_token_abi.py
+-rw-r--r--   0        0        0    11298 2023-05-05 12:58:23.291430 credmark-1.3.0/credmark/api/token_api/get_token_balance.py
+-rw-r--r--   0        0        0    15309 2023-05-05 12:58:23.345687 credmark-1.3.0/credmark/api/token_api/get_token_balance_historical.py
+-rw-r--r--   0        0        0     8410 2023-05-05 12:58:23.279601 credmark-1.3.0/credmark/api/token_api/get_token_creation_block.py
+-rw-r--r--   0        0        0     8274 2023-05-05 12:58:23.302161 credmark-1.3.0/credmark/api/token_api/get_token_decimals.py
+-rw-r--r--   0        0        0    11822 2023-05-05 12:58:23.343893 credmark-1.3.0/credmark/api/token_api/get_token_holders.py
+-rw-r--r--   0        0        0     7940 2023-05-05 12:58:23.305865 credmark-1.3.0/credmark/api/token_api/get_token_holders_count.py
+-rw-r--r--   0        0        0    12559 2023-05-05 12:58:23.358950 credmark-1.3.0/credmark/api/token_api/get_token_holders_count_historical.py
+-rw-r--r--   0        0        0     8170 2023-05-05 12:58:23.313369 credmark-1.3.0/credmark/api/token_api/get_token_logo.py
+-rw-r--r--   0        0        0     8255 2023-05-05 12:58:23.329081 credmark-1.3.0/credmark/api/token_api/get_token_metadata.py
+-rw-r--r--   0        0        0     8170 2023-05-05 12:58:23.364176 credmark-1.3.0/credmark/api/token_api/get_token_name.py
+-rw-r--r--   0        0        0    11243 2023-05-05 12:58:23.394357 credmark-1.3.0/credmark/api/token_api/get_token_price.py
+-rw-r--r--   0        0        0    16235 2023-05-05 12:58:23.469327 credmark-1.3.0/credmark/api/token_api/get_token_price_historical.py
+-rw-r--r--   0        0        0     8222 2023-05-05 12:58:23.407436 credmark-1.3.0/credmark/api/token_api/get_token_symbol.py
+-rw-r--r--   0        0        0     9238 2023-05-05 12:58:23.445394 credmark-1.3.0/credmark/api/token_api/get_token_total_supply.py
+-rw-r--r--   0        0        0    13225 2023-05-05 12:58:23.517891 credmark-1.3.0/credmark/api/token_api/get_token_total_supply_historical.py
+-rw-r--r--   0        0        0    11276 2023-05-05 12:58:23.485870 credmark-1.3.0/credmark/api/token_api/get_token_volume.py
+-rw-r--r--   0        0        0    13437 2023-05-05 12:58:23.527021 credmark-1.3.0/credmark/api/token_api/get_token_volume_historical.py
+-rw-r--r--   0        0        0     5822 2023-05-05 12:58:23.407441 credmark-1.3.0/credmark/api/utilities/__init__.py
+-rw-r--r--   0        0        0     3575 2023-05-05 12:58:23.410726 credmark-1.3.0/credmark/api/utilities/check_health.py
+-rw-r--r--   0        0        0     6512 2023-05-05 12:58:23.520382 credmark-1.3.0/credmark/api/utilities/get_daily_model_usage.py
+-rw-r--r--   0        0        0     3373 2023-05-05 12:58:23.458974 credmark-1.3.0/credmark/api/utilities/get_top_models.py
+-rw-r--r--   0        0        0     3351 2023-05-05 12:58:23.503111 credmark-1.3.0/credmark/api/utilities/get_total_model_usage.py
+-rw-r--r--   0        0        0     2645 2023-05-05 12:58:23.492532 credmark-1.3.0/credmark/client.py
+-rw-r--r--   0        0        0      320 2023-05-05 12:58:20.677683 credmark-1.3.0/credmark/docs/CheckHealthResponse200.md
+-rw-r--r--   0        0        0       79 2023-05-05 12:58:20.676539 credmark-1.3.0/credmark/docs/CheckHealthResponse200Details.md
+-rw-r--r--   0        0        0      172 2023-05-05 12:58:20.675934 credmark-1.3.0/credmark/docs/CheckHealthResponse200DetailsAdditionalProperty.md
+-rw-r--r--   0        0        0       33 2023-05-05 12:58:20.675270 credmark-1.3.0/credmark/docs/CheckHealthResponse200Error.md
+-rw-r--r--   0        0        0      170 2023-05-05 12:58:20.674662 credmark-1.3.0/credmark/docs/CheckHealthResponse200ErrorAdditionalProperty.md
+-rw-r--r--   0        0        0       76 2023-05-05 12:58:20.674010 credmark-1.3.0/credmark/docs/CheckHealthResponse200Info.md
+-rw-r--r--   0        0        0      169 2023-05-05 12:58:20.673413 credmark-1.3.0/credmark/docs/CheckHealthResponse200InfoAdditionalProperty.md
+-rw-r--r--   0        0        0      320 2023-05-05 12:58:20.683024 credmark-1.3.0/credmark/docs/CheckHealthResponse503.md
+-rw-r--r--   0        0        0      140 2023-05-05 12:58:20.681933 credmark-1.3.0/credmark/docs/CheckHealthResponse503Details.md
+-rw-r--r--   0        0        0      172 2023-05-05 12:58:20.681317 credmark-1.3.0/credmark/docs/CheckHealthResponse503DetailsAdditionalProperty.md
+-rw-r--r--   0        0        0      108 2023-05-05 12:58:20.680669 credmark-1.3.0/credmark/docs/CheckHealthResponse503Error.md
+-rw-r--r--   0        0        0      170 2023-05-05 12:58:20.679966 credmark-1.3.0/credmark/docs/CheckHealthResponse503ErrorAdditionalProperty.md
+-rw-r--r--   0        0        0       76 2023-05-05 12:58:20.679223 credmark-1.3.0/credmark/docs/CheckHealthResponse503Info.md
+-rw-r--r--   0        0        0      169 2023-05-05 12:58:20.678419 credmark-1.3.0/credmark/docs/CheckHealthResponse503InfoAdditionalProperty.md
+-rw-r--r--   0        0        0     2629 2023-05-05 12:58:20.751191 credmark-1.3.0/credmark/docs/DefiApi.md
+-rw-r--r--   0        0        0      390 2023-05-05 12:58:20.638588 credmark-1.3.0/credmark/docs/ModelCallStackEntry.md
+-rw-r--r--   0        0        0      259 2023-05-05 12:58:20.592875 credmark-1.3.0/credmark/docs/ModelDeployment.md
+-rw-r--r--   0        0        0      519 2023-05-05 12:58:20.591849 credmark-1.3.0/credmark/docs/ModelMetadata.md
+-rw-r--r--   0        0        0      795 2023-05-05 12:58:20.642466 credmark-1.3.0/credmark/docs/ModelRunResponse.md
+-rw-r--r--   0        0        0      637 2023-05-05 12:58:20.640825 credmark-1.3.0/credmark/docs/ModelRunResponseError.md
+-rw-r--r--   0        0        0      418 2023-05-05 12:58:20.595290 credmark-1.3.0/credmark/docs/ModelRuntimeStatistics.md
+-rw-r--r--   0        0        0      165 2023-05-05 12:58:20.618305 credmark-1.3.0/credmark/docs/ModelRuntimeStatsResponse.md
+-rw-r--r--   0        0        0      471 2023-05-05 12:58:20.637545 credmark-1.3.0/credmark/docs/RunModelDto.md
+-rw-r--r--   0        0        0      597 2023-05-05 12:58:20.655516 credmark-1.3.0/credmark/docs/TokenAbiResponse.md
+-rw-r--r--   0        0        0    20809 2023-05-05 12:58:20.808162 credmark-1.3.0/credmark/docs/TokenApi.md
+-rw-r--r--   0        0        0      318 2023-05-05 12:58:20.661673 credmark-1.3.0/credmark/docs/TokenBalanceHistoricalItem.md
+-rw-r--r--   0        0        0      646 2023-05-05 12:58:20.663241 credmark-1.3.0/credmark/docs/TokenBalanceHistoricalResponse.md
+-rw-r--r--   0        0        0      530 2023-05-05 12:58:20.660767 credmark-1.3.0/credmark/docs/TokenBalanceResponse.md
+-rw-r--r--   0        0        0      371 2023-05-05 12:58:20.653813 credmark-1.3.0/credmark/docs/TokenCreationBlockResponse.md
+-rw-r--r--   0        0        0      347 2023-05-05 12:58:20.648254 credmark-1.3.0/credmark/docs/TokenDecimalsResponse.md
+-rw-r--r--   0        0        0      491 2023-05-05 12:58:20.645100 credmark-1.3.0/credmark/docs/TokenErrorResponse.md
+-rw-r--r--   0        0        0      518 2023-05-05 12:58:20.672722 credmark-1.3.0/credmark/docs/TokenHistoricalHoldersCountResponse.md
+-rw-r--r--   0        0        0      214 2023-05-05 12:58:20.667973 credmark-1.3.0/credmark/docs/TokenHolder.md
+-rw-r--r--   0        0        0      283 2023-05-05 12:58:20.671377 credmark-1.3.0/credmark/docs/TokenHoldersCountHistoricalItem.md
+-rw-r--r--   0        0        0      357 2023-05-05 12:58:20.670576 credmark-1.3.0/credmark/docs/TokenHoldersCountResponse.md
+-rw-r--r--   0        0        0      613 2023-05-05 12:58:20.669537 credmark-1.3.0/credmark/docs/TokenHoldersResponse.md
+-rw-r--r--   0        0        0      341 2023-05-05 12:58:20.652797 credmark-1.3.0/credmark/docs/TokenLogoResponse.md
+-rw-r--r--   0        0        0      399 2023-05-05 12:58:20.643671 credmark-1.3.0/credmark/docs/TokenMetadataResponse.md
+-rw-r--r--   0        0        0      333 2023-05-05 12:58:20.646118 credmark-1.3.0/credmark/docs/TokenNameResponse.md
+-rw-r--r--   0        0        0      379 2023-05-05 12:58:20.657848 credmark-1.3.0/credmark/docs/TokenPriceHistoricalItem.md
+-rw-r--r--   0        0        0      582 2023-05-05 12:58:20.659450 credmark-1.3.0/credmark/docs/TokenPriceHistoricalResponse.md
+-rw-r--r--   0        0        0      531 2023-05-05 12:58:20.656841 credmark-1.3.0/credmark/docs/TokenPriceResponse.md
+-rw-r--r--   0        0        0      339 2023-05-05 12:58:20.647119 credmark-1.3.0/credmark/docs/TokenSymbolResponse.md
+-rw-r--r--   0        0        0      284 2023-05-05 12:58:20.650206 credmark-1.3.0/credmark/docs/TokenTotalSupplyHistoricalItem.md
+-rw-r--r--   0        0        0      581 2023-05-05 12:58:20.651782 credmark-1.3.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md
+-rw-r--r--   0        0        0      423 2023-05-05 12:58:20.649377 credmark-1.3.0/credmark/docs/TokenTotalSupplyResponse.md
+-rw-r--r--   0        0        0      404 2023-05-05 12:58:20.665741 credmark-1.3.0/credmark/docs/TokenVolumeHistoricalItem.md
+-rw-r--r--   0        0        0      565 2023-05-05 12:58:20.667197 credmark-1.3.0/credmark/docs/TokenVolumeHistoricalResponse.md
+-rw-r--r--   0        0        0      537 2023-05-05 12:58:20.664647 credmark-1.3.0/credmark/docs/TokenVolumeResponse.md
+-rw-r--r--   0        0        0     1421 2023-05-05 12:58:20.742237 credmark-1.3.0/credmark/docs/Utilities.md
+-rw-r--r--   0        0        0      592 2023-05-05 12:58:23.422483 credmark-1.3.0/credmark/errors.py
+-rw-r--r--   0        0        0     5318 2023-05-05 12:58:20.687784 credmark-1.3.0/credmark/models/__init__.py
+-rw-r--r--   0        0        0     4203 2023-05-05 12:58:23.559507 credmark-1.3.0/credmark/models/check_health_response_200.py
+-rw-r--r--   0        0        0     2144 2023-05-05 12:58:23.505245 credmark-1.3.0/credmark/models/check_health_response_200_details.py
+-rw-r--r--   0        0        0     1658 2023-05-05 12:58:23.499383 credmark-1.3.0/credmark/models/check_health_response_200_details_additional_property.py
+-rw-r--r--   0        0        0     2061 2023-05-05 12:58:23.517069 credmark-1.3.0/credmark/models/check_health_response_200_error.py
+-rw-r--r--   0        0        0     1648 2023-05-05 12:58:23.544210 credmark-1.3.0/credmark/models/check_health_response_200_error_additional_property.py
+-rw-r--r--   0        0        0     2074 2023-05-05 12:58:23.537806 credmark-1.3.0/credmark/models/check_health_response_200_info.py
+-rw-r--r--   0        0        0     1643 2023-05-05 12:58:23.542897 credmark-1.3.0/credmark/models/check_health_response_200_info_additional_property.py
+-rw-r--r--   0        0        0     4364 2023-05-05 12:58:23.609660 credmark-1.3.0/credmark/models/check_health_response_503.py
+-rw-r--r--   0        0        0     2205 2023-05-05 12:58:23.556933 credmark-1.3.0/credmark/models/check_health_response_503_details.py
+-rw-r--r--   0        0        0     1658 2023-05-05 12:58:23.551649 credmark-1.3.0/credmark/models/check_health_response_503_details_additional_property.py
+-rw-r--r--   0        0        0     2149 2023-05-05 12:58:23.567359 credmark-1.3.0/credmark/models/check_health_response_503_error.py
+-rw-r--r--   0        0        0     1648 2023-05-05 12:58:23.561995 credmark-1.3.0/credmark/models/check_health_response_503_error_additional_property.py
+-rw-r--r--   0        0        0     2074 2023-05-05 12:58:23.566967 credmark-1.3.0/credmark/models/check_health_response_503_info.py
+-rw-r--r--   0        0        0     1643 2023-05-05 12:58:23.569688 credmark-1.3.0/credmark/models/check_health_response_503_info_additional_property.py
+-rw-r--r--   0        0        0      165 2023-05-05 12:58:21.830432 credmark-1.3.0/credmark/models/get_cached_model_results_order.py
+-rw-r--r--   0        0        0      163 2023-05-05 12:58:21.768992 credmark-1.3.0/credmark/models/get_token_price_historical_src.py
+-rw-r--r--   0        0        0      153 2023-05-05 12:58:21.833451 credmark-1.3.0/credmark/models/get_token_price_src.py
+-rw-r--r--   0        0        0     2470 2023-05-05 12:58:23.617959 credmark-1.3.0/credmark/models/model_call_stack_entry.py
+-rw-r--r--   0        0        0     1894 2023-05-05 12:58:23.591293 credmark-1.3.0/credmark/models/model_deployment.py
+-rw-r--r--   0        0        0     3325 2023-05-05 12:58:23.636706 credmark-1.3.0/credmark/models/model_metadata.py
+-rw-r--r--   0        0        0     4460 2023-05-05 12:58:23.657788 credmark-1.3.0/credmark/models/model_run_response.py
+-rw-r--r--   0        0        0     3362 2023-05-05 12:58:23.637117 credmark-1.3.0/credmark/models/model_run_response_error.py
+-rw-r--r--   0        0        0     2412 2023-05-05 12:58:23.636927 credmark-1.3.0/credmark/models/model_runtime_statistics.py
+-rw-r--r--   0        0        0     2042 2023-05-05 12:58:23.620457 credmark-1.3.0/credmark/models/model_runtime_stats_response.py
+-rw-r--r--   0        0        0     3280 2023-05-05 12:58:23.655632 credmark-1.3.0/credmark/models/run_model_dto.py
+-rw-r--r--   0        0        0      180 2023-05-05 12:58:21.788363 credmark-1.3.0/credmark/models/run_model_dto_block_number_type_1.py
+-rw-r--r--   0        0        0     5771 2023-05-05 12:58:23.653858 credmark-1.3.0/credmark/models/token_abi_response.py
+-rw-r--r--   0        0        0     2319 2023-05-05 12:58:23.634433 credmark-1.3.0/credmark/models/token_balance_historical_item.py
+-rw-r--r--   0        0        0     4365 2023-05-05 12:58:23.684860 credmark-1.3.0/credmark/models/token_balance_historical_response.py
+-rw-r--r--   0        0        0     3378 2023-05-05 12:58:23.681623 credmark-1.3.0/credmark/models/token_balance_response.py
+-rw-r--r--   0        0        0     2692 2023-05-05 12:58:23.673028 credmark-1.3.0/credmark/models/token_creation_block_response.py
+-rw-r--r--   0        0        0     2587 2023-05-05 12:58:23.680658 credmark-1.3.0/credmark/models/token_decimals_response.py
+-rw-r--r--   0        0        0     2779 2023-05-05 12:58:23.695458 credmark-1.3.0/credmark/models/token_error_response.py
+-rw-r--r--   0        0        0     3856 2023-05-05 12:58:23.705892 credmark-1.3.0/credmark/models/token_historical_holders_count_response.py
+-rw-r--r--   0        0        0     1836 2023-05-05 12:58:23.681752 credmark-1.3.0/credmark/models/token_holder.py
+-rw-r--r--   0        0        0     2104 2023-05-05 12:58:23.681485 credmark-1.3.0/credmark/models/token_holders_count_historical_item.py
+-rw-r--r--   0        0        0     2589 2023-05-05 12:58:23.711832 credmark-1.3.0/credmark/models/token_holders_count_response.py
+-rw-r--r--   0        0        0     4074 2023-05-05 12:58:23.736104 credmark-1.3.0/credmark/models/token_holders_response.py
+-rw-r--r--   0        0        0     2711 2023-05-05 12:58:23.711254 credmark-1.3.0/credmark/models/token_logo_response.py
+-rw-r--r--   0        0        0     2951 2023-05-05 12:58:23.737078 credmark-1.3.0/credmark/models/token_metadata_response.py
+-rw-r--r--   0        0        0     2527 2023-05-05 12:58:23.733880 credmark-1.3.0/credmark/models/token_name_response.py
+-rw-r--r--   0        0        0     2551 2023-05-05 12:58:23.738444 credmark-1.3.0/credmark/models/token_price_historical_item.py
+-rw-r--r--   0        0        0     4118 2023-05-05 12:58:23.756842 credmark-1.3.0/credmark/models/token_price_historical_response.py
+-rw-r--r--   0        0        0     3387 2023-05-05 12:58:23.746549 credmark-1.3.0/credmark/models/token_price_response.py
+-rw-r--r--   0        0        0     2553 2023-05-05 12:58:23.742689 credmark-1.3.0/credmark/models/token_symbol_response.py
+-rw-r--r--   0        0        0     2168 2023-05-05 12:58:23.743722 credmark-1.3.0/credmark/models/token_total_supply_historical_item.py
+-rw-r--r--   0        0        0     4072 2023-05-05 12:58:23.769114 credmark-1.3.0/credmark/models/token_total_supply_historical_response.py
+-rw-r--r--   0        0        0     2881 2023-05-05 12:58:23.759899 credmark-1.3.0/credmark/models/token_total_supply_response.py
+-rw-r--r--   0        0        0     2758 2023-05-05 12:58:23.759863 credmark-1.3.0/credmark/models/token_volume_historical_item.py
+-rw-r--r--   0        0        0     4001 2023-05-05 12:58:23.783603 credmark-1.3.0/credmark/models/token_volume_historical_response.py
+-rw-r--r--   0        0        0     3465 2023-05-05 12:58:23.778417 credmark-1.3.0/credmark/models/token_volume_response.py
+-rw-r--r--   0        0        0       25 2023-05-05 12:58:20.546306 credmark-1.3.0/credmark/py.typed
+-rw-r--r--   0        0        0      964 2023-05-05 12:58:23.757166 credmark-1.3.0/credmark/types.py
+-rw-r--r--   0        0        0      853 2023-05-05 13:03:00.626630 credmark-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5384 1970-01-01 00:00:00.000000 credmark-1.3.0/PKG-INFO
```

### Comparing `credmark-1.2.0/README.md` & `credmark-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/api/defi_api/__init__.py` & `credmark-1.3.0/credmark/api/defi_api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -209,19 +209,22 @@
     ) -> ModelRuntimeStatsResponse:
         """Cached model results
 
          Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
         and get results, use `POST /v1/model/run`.
 
         Args:
-            slug (str):
-            sort (Union[Unset, None, str]):
-            order (Union[Unset, None, GetCachedModelResultsOrder]):
-            limit (Union[Unset, None, float]):
-            offset (Union[Unset, None, float]):
+            slug (str): Model slug
+            sort (Union[Unset, None, str]): Field to sort results by: 'time', 'runtime'. Defaults to
+                'time'.
+            order (Union[Unset, None, GetCachedModelResultsOrder]): "asc" ascending order or "desc"
+                descending order. Default is "desc".
+            limit (Union[Unset, None, float]): Maximum number of results to return. Defaults to 100.
+            offset (Union[Unset, None, float]): Offset index of results to return for pagination.
+                Defaults to 0.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelRuntimeStatsResponse]
@@ -247,19 +250,22 @@
     ) -> ModelRuntimeStatsResponse:
         """Cached model results
 
          Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
         and get results, use `POST /v1/model/run`.
 
         Args:
-            slug (str):
-            sort (Union[Unset, None, str]):
-            order (Union[Unset, None, GetCachedModelResultsOrder]):
-            limit (Union[Unset, None, float]):
-            offset (Union[Unset, None, float]):
+            slug (str): Model slug
+            sort (Union[Unset, None, str]): Field to sort results by: 'time', 'runtime'. Defaults to
+                'time'.
+            order (Union[Unset, None, GetCachedModelResultsOrder]): "asc" ascending order or "desc"
+                descending order. Default is "desc".
+            limit (Union[Unset, None, float]): Maximum number of results to return. Defaults to 100.
+            offset (Union[Unset, None, float]): Offset index of results to return for pagination.
+                Defaults to 0.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelRuntimeStatsResponse]
```

### Comparing `credmark-1.2.0/credmark/api/defi_api/get_model_by_slug.py` & `credmark-1.3.0/credmark/api/defi_api/get_model_by_slug.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/api/defi_api/get_model_deployments_by_slug.py` & `credmark-1.3.0/credmark/api/defi_api/get_model_deployments_by_slug.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/api/defi_api/get_model_runtime_stats.py` & `credmark-1.3.0/credmark/api/defi_api/get_model_runtime_stats.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/api/defi_api/list_models.py` & `credmark-1.3.0/credmark/api/defi_api/list_models.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/api/defi_api/run_model.py` & `credmark-1.3.0/credmark/api/defi_api/run_model.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/api/token_api/__init__.py` & `credmark-1.3.0/credmark/api/token_api/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, Optional, Union, cast
 
-from ...models.get_token_price_align import GetTokenPriceAlign
 from ...models.get_token_price_historical_src import GetTokenPriceHistoricalSrc
 from ...models.get_token_price_src import GetTokenPriceSrc
 from ...models.token_abi_response import TokenAbiResponse
 from ...models.token_balance_historical_response import TokenBalanceHistoricalResponse
 from ...models.token_balance_response import TokenBalanceResponse
 from ...models.token_creation_block_response import TokenCreationBlockResponse
 from ...models.token_decimals_response import TokenDecimalsResponse
 from ...models.token_error_response import TokenErrorResponse
 from ...models.token_historical_holders_count_response import TokenHistoricalHoldersCountResponse
 from ...models.token_holders_count_response import TokenHoldersCountResponse
-from ...models.token_holders_historical_response import TokenHoldersHistoricalResponse
 from ...models.token_holders_response import TokenHoldersResponse
 from ...models.token_logo_response import TokenLogoResponse
 from ...models.token_metadata_response import TokenMetadataResponse
 from ...models.token_name_response import TokenNameResponse
 from ...models.token_price_historical_response import TokenPriceHistoricalResponse
 from ...models.token_price_response import TokenPriceResponse
 from ...models.token_symbol_response import TokenSymbolResponse
@@ -34,15 +32,14 @@
     get_token_balance,
     get_token_balance_historical,
     get_token_creation_block,
     get_token_decimals,
     get_token_holders,
     get_token_holders_count,
     get_token_holders_count_historical,
-    get_token_holders_historical,
     get_token_logo,
     get_token_metadata,
     get_token_name,
     get_token_price,
     get_token_price_historical,
     get_token_symbol,
     get_token_total_supply,
@@ -54,29 +51,40 @@
 
 class TokenApi:
     def __init__(self, client: "Credmark"):
         self.__client = client
 
     def get_token_metadata(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenMetadataResponse:
         """Get token metadata
 
          Returns metadata for a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the metadata. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenMetadataResponse]
@@ -88,29 +96,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_metadata_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenMetadataResponse:
         """Get token metadata
 
          Returns metadata for a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the metadata. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenMetadataResponse]
@@ -122,29 +141,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     def get_token_name(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenNameResponse:
         """Get token name
 
          Returns name of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the name. Defaults to the latest
+                block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenNameResponse]
@@ -156,29 +186,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_name_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenNameResponse:
         """Get token name
 
          Returns name of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the name. Defaults to the latest
+                block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenNameResponse]
@@ -190,29 +231,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     def get_token_symbol(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenSymbolResponse:
         """Get token symbol
 
          Returns symbol of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the symbol. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenSymbolResponse]
@@ -224,29 +276,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_symbol_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenSymbolResponse:
         """Get token symbol
 
          Returns symbol of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the symbol. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenSymbolResponse]
@@ -258,29 +321,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     def get_token_decimals(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenDecimalsResponse:
         """Get token decimals
 
          Returns decimals of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the decimals. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenDecimalsResponse]
@@ -292,29 +366,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_decimals_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenDecimalsResponse:
         """Get token decimals
 
          Returns decimals of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the decimals. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenDecimalsResponse]
@@ -326,31 +411,43 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     def get_token_total_supply(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
         scaled: Union[Unset, None, bool] = True,
     ) -> TokenTotalSupplyResponse:
         """Get token's total supply
 
          Returns total supply of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
-            scaled (Union[Unset, None, bool]):  Default: True.
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the total supply. Defaults to
+                the latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
+            scaled (Union[Unset, None, bool]): Scale total supply by token decimals. Defaults to
+                `true`. Default: True.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenTotalSupplyResponse]
@@ -363,31 +460,43 @@
             block_number=block_number,
             timestamp=timestamp,
             scaled=scaled,
         )
 
     async def get_token_total_supply_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
         scaled: Union[Unset, None, bool] = True,
     ) -> TokenTotalSupplyResponse:
         """Get token's total supply
 
          Returns total supply of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
-            scaled (Union[Unset, None, bool]):  Default: True.
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the total supply. Defaults to
+                the latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
+            scaled (Union[Unset, None, bool]): Scale total supply by token decimals. Defaults to
+                `true`. Default: True.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenTotalSupplyResponse]
@@ -400,15 +509,15 @@
             block_number=block_number,
             timestamp=timestamp,
             scaled=scaled,
         )
 
     def get_token_total_supply_historical(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
@@ -416,23 +525,33 @@
         scaled: Union[Unset, None, bool] = True,
     ) -> TokenTotalSupplyHistoricalResponse:
         """Get historical total supply
 
          Returns historical total supply for a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
-            scaled (Union[Unset, None, bool]):  Default: True.
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            start_block_number (Union[Unset, None, float]): Start block number of the balance.
+                Defaults to token's creation block.
+            end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+                the latest block.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
+            scaled (Union[Unset, None, bool]): Scale total supply by token decimals. Defaults to
+                `true`. Default: True.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenTotalSupplyHistoricalResponse]
@@ -449,15 +568,15 @@
             end_timestamp=end_timestamp,
             time_interval=time_interval,
             scaled=scaled,
         )
 
     async def get_token_total_supply_historical_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
@@ -465,23 +584,33 @@
         scaled: Union[Unset, None, bool] = True,
     ) -> TokenTotalSupplyHistoricalResponse:
         """Get historical total supply
 
          Returns historical total supply for a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
-            scaled (Union[Unset, None, bool]):  Default: True.
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            start_block_number (Union[Unset, None, float]): Start block number of the balance.
+                Defaults to token's creation block.
+            end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+                the latest block.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
+            scaled (Union[Unset, None, bool]): Scale total supply by token decimals. Defaults to
+                `true`. Default: True.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenTotalSupplyHistoricalResponse]
@@ -498,29 +627,40 @@
             end_timestamp=end_timestamp,
             time_interval=time_interval,
             scaled=scaled,
         )
 
     def get_token_logo(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenLogoResponse:
         """Get token logo
 
          Returns logo of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the logo. Defaults to the latest
+                block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenLogoResponse]
@@ -532,29 +672,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_logo_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenLogoResponse:
         """Get token logo
 
          Returns logo of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the logo. Defaults to the latest
+                block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenLogoResponse]
@@ -566,29 +717,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     def get_token_creation_block(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenCreationBlockResponse:
         """Get token creation block
 
          Returns creation block number of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the token. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenCreationBlockResponse]
@@ -600,29 +762,40 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_creation_block_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenCreationBlockResponse:
         """Get token creation block
 
          Returns creation block number of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the token. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenCreationBlockResponse]
@@ -634,29 +807,34 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     def get_token_abi(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenAbiResponse:
         """Get token ABI
 
          Returns ABI of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the ABI. Defaults to the latest
+                block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenAbiResponse]
@@ -668,29 +846,34 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_abi_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenAbiResponse:
         """Get token ABI
 
          Returns ABI of a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the ABI. Defaults to the latest
+                block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenAbiResponse]
@@ -702,35 +885,48 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     def get_token_price(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         quote_address: Union[Unset, None, str] = UNSET,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
         src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
-        align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
     ) -> TokenPriceResponse:
         """Get token price data
 
          Returns price data for a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            quote_address (Union[Unset, None, str]):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
-            src (Union[Unset, None, GetTokenPriceSrc]):  Default: GetTokenPriceSrc.DEX.
-            align (Union[Unset, None, GetTokenPriceAlign]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            block_number (Union[Unset, None, float]): Block number of the price quote. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
+            src (Union[Unset, None, GetTokenPriceSrc]): (Optional) specify preferred source to be
+                queried first, choices: "dex" (pre-calculated, default), or "cex" (from call to
+                price.quote model) Default: GetTokenPriceSrc.DEX.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenPriceResponse]
@@ -740,40 +936,52 @@
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             quote_address=quote_address,
             block_number=block_number,
             timestamp=timestamp,
             src=src,
-            align=align,
         )
 
     async def get_token_price_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         quote_address: Union[Unset, None, str] = UNSET,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
         src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
-        align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
     ) -> TokenPriceResponse:
         """Get token price data
 
          Returns price data for a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            quote_address (Union[Unset, None, str]):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
-            src (Union[Unset, None, GetTokenPriceSrc]):  Default: GetTokenPriceSrc.DEX.
-            align (Union[Unset, None, GetTokenPriceAlign]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            block_number (Union[Unset, None, float]): Block number of the price quote. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
+            src (Union[Unset, None, GetTokenPriceSrc]): (Optional) specify preferred source to be
+                queried first, choices: "dex" (pre-calculated, default), or "cex" (from call to
+                price.quote model) Default: GetTokenPriceSrc.DEX.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenPriceResponse]
@@ -783,20 +991,19 @@
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             quote_address=quote_address,
             block_number=block_number,
             timestamp=timestamp,
             src=src,
-            align=align,
         )
 
     def get_token_price_historical(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
@@ -805,25 +1012,43 @@
         src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     ) -> TokenPriceHistoricalResponse:
         """Get historical price
 
          Returns historical price data for a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
-            quote_address (Union[Unset, None, str]):
-            src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
-                GetTokenPriceHistoricalSrc.DEX.
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            start_block_number (Union[Unset, None, float]): Start block number of the balance.
+                Defaults to token's creation block.
+            end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+                the latest block.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            src (Union[Unset, None, GetTokenPriceHistoricalSrc]): (Optional) specify preferred source
+                to be queried first, choices: "dex" (pre-calculated, default), or "cex" (from call to
+                price.quote model) Default: GetTokenPriceHistoricalSrc.DEX.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenPriceHistoricalResponse]
@@ -841,15 +1066,15 @@
             time_interval=time_interval,
             quote_address=quote_address,
             src=src,
         )
 
     async def get_token_price_historical_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
@@ -858,25 +1083,43 @@
         src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     ) -> TokenPriceHistoricalResponse:
         """Get historical price
 
          Returns historical price data for a token.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
-            quote_address (Union[Unset, None, str]):
-            src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
-                GetTokenPriceHistoricalSrc.DEX.
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            start_block_number (Union[Unset, None, float]): Start block number of the balance.
+                Defaults to token's creation block.
+            end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+                the latest block.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            src (Union[Unset, None, GetTokenPriceHistoricalSrc]): (Optional) specify preferred source
+                to be queried first, choices: "dex" (pre-calculated, default), or "cex" (from call to
+                price.quote model) Default: GetTokenPriceHistoricalSrc.DEX.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenPriceHistoricalResponse]
@@ -894,35 +1137,50 @@
             time_interval=time_interval,
             quote_address=quote_address,
             src=src,
         )
 
     def get_token_balance(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         account_address: str,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenBalanceResponse:
         """Get token balance
 
          Returns token balance for an account.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            account_address (str):
-            quote_address (Union[Unset, None, str]):
-            scaled (Union[Unset, None, bool]):  Default: True.
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            account_address (str): The address of the account for which balance of the token will be
+                fetched.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            scaled (Union[Unset, None, bool]): Scale balance by token decimals. Defaults to `true`.
+                Default: True.
+            block_number (Union[Unset, None, float]): Block number of the balance. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenBalanceResponse]
@@ -937,35 +1195,50 @@
             scaled=scaled,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_balance_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         account_address: str,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenBalanceResponse:
         """Get token balance
 
          Returns token balance for an account.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            account_address (str):
-            quote_address (Union[Unset, None, str]):
-            scaled (Union[Unset, None, bool]):  Default: True.
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Ethereum Mainnet
+                `10` - Optimism
+                `56` - BSC
+                `137` - Polygon Mainnet
+                `250` - Fantom Opera
+                `42161` - Arbitrum One
+                `43114` - Avalanche C-Chain
+            token_address (str): The address of the token requested.
+            account_address (str): The address of the account for which balance of the token will be
+                fetched.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            scaled (Union[Unset, None, bool]): Scale balance by token decimals. Defaults to `true`.
+                Default: True.
+            block_number (Union[Unset, None, float]): Block number of the balance. Defaults to the
+                latest block.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenBalanceResponse]
@@ -980,15 +1253,15 @@
             scaled=scaled,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     def get_token_balance_historical(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
@@ -998,25 +1271,38 @@
         scaled: Union[Unset, None, bool] = True,
     ) -> TokenBalanceHistoricalResponse:
         """Get historical balance
 
          Returns historical token balance for an account.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
-            account_address (str):
-            quote_address (Union[Unset, None, str]):
-            scaled (Union[Unset, None, bool]):  Default: True.
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            start_block_number (Union[Unset, None, float]): Start block number of the balance.
+                Defaults to token's creation block.
+            end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+                the latest block.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
+            account_address (str): The address of the account for which balance of the token will be
+                fetched.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            scaled (Union[Unset, None, bool]): Scale balance by token decimals. Defaults to `true`.
+                Default: True.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenBalanceHistoricalResponse]
@@ -1035,15 +1321,15 @@
             account_address=account_address,
             quote_address=quote_address,
             scaled=scaled,
         )
 
     async def get_token_balance_historical_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
@@ -1053,25 +1339,38 @@
         scaled: Union[Unset, None, bool] = True,
     ) -> TokenBalanceHistoricalResponse:
         """Get historical balance
 
          Returns historical token balance for an account.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
-            account_address (str):
-            quote_address (Union[Unset, None, str]):
-            scaled (Union[Unset, None, bool]):  Default: True.
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            start_block_number (Union[Unset, None, float]): Start block number of the balance.
+                Defaults to token's creation block.
+            end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+                the latest block.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
+            account_address (str): The address of the account for which balance of the token will be
+                fetched.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            scaled (Union[Unset, None, bool]): Scale balance by token decimals. Defaults to `true`.
+                Default: True.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenBalanceHistoricalResponse]
@@ -1090,35 +1389,44 @@
             account_address=account_address,
             quote_address=quote_address,
             scaled=scaled,
         )
 
     def get_token_volume(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         scaled: Union[Unset, None, bool] = True,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenVolumeResponse:
         """Get token volume
 
          Returns traded volume for a token over a period of blocks or time.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            scaled (Union[Unset, None, bool]):  Default: True.
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            scaled (Union[Unset, None, bool]): Scale volume by token decimals. Defaults to `true`.
+                Default: True.
+            start_block_number (Union[Unset, None, float]): Start block number of duration for which
+                token volume will be computed.
+            end_block_number (Union[Unset, None, float]): Start block number of duration for which
+                token volume will be computed. Defaults to the latest block.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenVolumeResponse]
@@ -1133,35 +1441,44 @@
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
         )
 
     async def get_token_volume_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         scaled: Union[Unset, None, bool] = True,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenVolumeResponse:
         """Get token volume
 
          Returns traded volume for a token over a period of blocks or time.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            scaled (Union[Unset, None, bool]):  Default: True.
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            scaled (Union[Unset, None, bool]): Scale volume by token decimals. Defaults to `true`.
+                Default: True.
+            start_block_number (Union[Unset, None, float]): Start block number of duration for which
+                token volume will be computed.
+            end_block_number (Union[Unset, None, float]): Start block number of duration for which
+                token volume will be computed. Defaults to the latest block.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenVolumeResponse]
@@ -1176,15 +1493,15 @@
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
         )
 
     def get_token_volume_historical(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         scaled: Union[Unset, None, bool] = True,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
@@ -1192,23 +1509,33 @@
         time_interval: Union[Unset, None, float] = UNSET,
     ) -> TokenVolumeHistoricalResponse:
         """Get historical volume
 
          Returns traded volume for a token over a period of blocks or time divided by intervals.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            scaled (Union[Unset, None, bool]):  Default: True.
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            scaled (Union[Unset, None, bool]): Scale volume by token decimals. Defaults to `true`.
+                Default: True.
+            start_block_number (Union[Unset, None, float]): Start block number of duration for which
+                token volume will be computed.
+            end_block_number (Union[Unset, None, float]): Start block number of duration for which
+                token volume will be computed. Defaults to the latest block.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenVolumeHistoricalResponse]
@@ -1225,15 +1552,15 @@
             end_timestamp=end_timestamp,
             block_interval=block_interval,
             time_interval=time_interval,
         )
 
     async def get_token_volume_historical_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         scaled: Union[Unset, None, bool] = True,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
@@ -1241,23 +1568,33 @@
         time_interval: Union[Unset, None, float] = UNSET,
     ) -> TokenVolumeHistoricalResponse:
         """Get historical volume
 
          Returns traded volume for a token over a period of blocks or time divided by intervals.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            scaled (Union[Unset, None, bool]):  Default: True.
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            scaled (Union[Unset, None, bool]): Scale volume by token decimals. Defaults to `true`.
+                Default: True.
+            start_block_number (Union[Unset, None, float]): Start block number of duration for which
+                token volume will be computed.
+            end_block_number (Union[Unset, None, float]): Start block number of duration for which
+                token volume will be computed. Defaults to the latest block.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenVolumeHistoricalResponse]
@@ -1274,37 +1611,47 @@
             end_timestamp=end_timestamp,
             block_interval=block_interval,
             time_interval=time_interval,
         )
 
     def get_token_holders(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         page_size: float = 100.0,
         cursor: Union[Unset, None, str] = UNSET,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenHoldersResponse:
         """Get token holders
 
          Returns holders of a token at a block or time.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            page_size (float):  Default: 100.0.
-            cursor (Union[Unset, None, str]):
-            quote_address (Union[Unset, None, str]):
-            scaled (Union[Unset, None, bool]):  Default: True.
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            page_size (float): The size of the returned page. Do not change this from page to page
+                when using a cursor. Default: 100.0.
+            cursor (Union[Unset, None, str]): The cursor from the results of a previous page. Use
+                empty string (or undefined/null) for first page.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            scaled (Union[Unset, None, bool]): Scale holders' balance by token decimals. Defaults to
+                `true`. Default: True.
+            block_number (Union[Unset, None, float]): Block number of the balance. Defaults to the
+                latest block. Do not change this from page to page when using a cursor.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenHoldersResponse]
@@ -1320,37 +1667,47 @@
             scaled=scaled,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_holders_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         page_size: float = 100.0,
         cursor: Union[Unset, None, str] = UNSET,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenHoldersResponse:
         """Get token holders
 
          Returns holders of a token at a block or time.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            page_size (float):  Default: 100.0.
-            cursor (Union[Unset, None, str]):
-            quote_address (Union[Unset, None, str]):
-            scaled (Union[Unset, None, bool]):  Default: True.
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            page_size (float): The size of the returned page. Do not change this from page to page
+                when using a cursor. Default: 100.0.
+            cursor (Union[Unset, None, str]): The cursor from the results of a previous page. Use
+                empty string (or undefined/null) for first page.
+            quote_address (Union[Unset, None, str]): The address of the token/currency used as the
+                currency of the returned price. Defaults to USD (address
+                `0x0000000000000000000000000000000000000348`).
+            scaled (Union[Unset, None, bool]): Scale holders' balance by token decimals. Defaults to
+                `true`. Default: True.
+            block_number (Union[Unset, None, float]): Block number of the balance. Defaults to the
+                latest block. Do not change this from page to page when using a cursor.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenHoldersResponse]
@@ -1364,141 +1721,36 @@
             cursor=cursor,
             quote_address=quote_address,
             scaled=scaled,
             block_number=block_number,
             timestamp=timestamp,
         )
 
-    def get_token_holders_historical(
-        self,
-        chain_id: float,
-        token_address: str,
-        *,
-        start_block_number: Union[Unset, None, float] = UNSET,
-        end_block_number: Union[Unset, None, float] = UNSET,
-        block_interval: Union[Unset, None, float] = UNSET,
-        start_timestamp: Union[Unset, None, float] = UNSET,
-        end_timestamp: Union[Unset, None, float] = UNSET,
-        time_interval: Union[Unset, None, float] = UNSET,
-        page_size: float = 100.0,
-        quote_address: Union[Unset, None, str] = UNSET,
-        scaled: Union[Unset, None, bool] = True,
-    ) -> TokenHoldersHistoricalResponse:
-        """Get token historical holders
-
-         Returns historical holders of a token at a block or time.
-
-        Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
-            page_size (float):  Default: 100.0.
-            quote_address (Union[Unset, None, str]):
-            scaled (Union[Unset, None, bool]):  Default: True.
-
-        Raises:
-            errors.CredmarkError: If the server returns a non 2xx status code.
-            httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-        Returns:
-            Response[TokenHoldersHistoricalResponse]
-        """
-
-        return get_token_holders_historical.sync(
-            client=self.__client,
-            chain_id=chain_id,
-            token_address=token_address,
-            start_block_number=start_block_number,
-            end_block_number=end_block_number,
-            block_interval=block_interval,
-            start_timestamp=start_timestamp,
-            end_timestamp=end_timestamp,
-            time_interval=time_interval,
-            page_size=page_size,
-            quote_address=quote_address,
-            scaled=scaled,
-        )
-
-    async def get_token_holders_historical_async(
-        self,
-        chain_id: float,
-        token_address: str,
-        *,
-        start_block_number: Union[Unset, None, float] = UNSET,
-        end_block_number: Union[Unset, None, float] = UNSET,
-        block_interval: Union[Unset, None, float] = UNSET,
-        start_timestamp: Union[Unset, None, float] = UNSET,
-        end_timestamp: Union[Unset, None, float] = UNSET,
-        time_interval: Union[Unset, None, float] = UNSET,
-        page_size: float = 100.0,
-        quote_address: Union[Unset, None, str] = UNSET,
-        scaled: Union[Unset, None, bool] = True,
-    ) -> TokenHoldersHistoricalResponse:
-        """Get token historical holders
-
-         Returns historical holders of a token at a block or time.
-
-        Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
-            page_size (float):  Default: 100.0.
-            quote_address (Union[Unset, None, str]):
-            scaled (Union[Unset, None, bool]):  Default: True.
-
-        Raises:
-            errors.CredmarkError: If the server returns a non 2xx status code.
-            httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-        Returns:
-            Response[TokenHoldersHistoricalResponse]
-        """
-
-        return await get_token_holders_historical.asyncio(
-            client=self.__client,
-            chain_id=chain_id,
-            token_address=token_address,
-            start_block_number=start_block_number,
-            end_block_number=end_block_number,
-            block_interval=block_interval,
-            start_timestamp=start_timestamp,
-            end_timestamp=end_timestamp,
-            time_interval=time_interval,
-            page_size=page_size,
-            quote_address=quote_address,
-            scaled=scaled,
-        )
-
     def get_token_holders_count(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenHoldersCountResponse:
         """Get total number of token holders
 
          Returns total number of holders of a token at a block or time.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the balance. Defaults to the
+                latest block. Do not change this from page to page when using a cursor.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenHoldersCountResponse]
@@ -1510,29 +1762,34 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     async def get_token_holders_count_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
     ) -> TokenHoldersCountResponse:
         """Get total number of token holders
 
          Returns total number of holders of a token at a block or time.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            block_number (Union[Unset, None, float]):
-            timestamp (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            block_number (Union[Unset, None, float]): Block number of the balance. Defaults to the
+                latest block. Do not change this from page to page when using a cursor.
+            timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+                instead of a block number. Finds a block at or before the number of seconds since January
+                1, 1970.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenHoldersCountResponse]
@@ -1544,37 +1801,46 @@
             token_address=token_address,
             block_number=block_number,
             timestamp=timestamp,
         )
 
     def get_token_holders_count_historical(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
     ) -> TokenHistoricalHoldersCountResponse:
         """Get historical total number of token holders
 
          Returns historical total number of holders of a token at a block or time.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            start_block_number (Union[Unset, None, float]): Start block number of the balance.
+                Defaults to token's creation block.
+            end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+                the latest block.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenHistoricalHoldersCountResponse]
@@ -1590,37 +1856,46 @@
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             time_interval=time_interval,
         )
 
     async def get_token_holders_count_historical_async(
         self,
-        chain_id: float,
+        chain_id: int,
         token_address: str,
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
     ) -> TokenHistoricalHoldersCountResponse:
         """Get historical total number of token holders
 
          Returns historical total number of holders of a token at a block or time.
 
         Args:
-            chain_id (float):
-            token_address (str):
-            start_block_number (Union[Unset, None, float]):
-            end_block_number (Union[Unset, None, float]):
-            block_interval (Union[Unset, None, float]):
-            start_timestamp (Union[Unset, None, float]):
-            end_timestamp (Union[Unset, None, float]):
-            time_interval (Union[Unset, None, float]):
+            chain_id (int): Chain identifier. This endpoint supports the following chains
+
+                `1` - Mainnet
+            token_address (str): The address of the token requested.
+            start_block_number (Union[Unset, None, float]): Start block number of the balance.
+                Defaults to token's creation block.
+            end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+                the latest block.
+            block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+            start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+                specified instead of start block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+                specified instead of end block number. Finds a block at or before the number of seconds
+                since January 1, 1970.
+            time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+                Should be in seconds. Defaults to 86,400.
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[TokenHistoricalHoldersCountResponse]
```

### Comparing `credmark-1.2.0/credmark/api/token_api/get_token_balance_historical.py` & `credmark-1.3.0/credmark/api/token_api/get_token_holders_count_historical.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,35 +5,32 @@
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, Union
 
 from ... import errors
-from ...models.token_balance_historical_response import TokenBalanceHistoricalResponse
 from ...models.token_error_response import TokenErrorResponse
+from ...models.token_historical_holders_count_response import TokenHistoricalHoldersCountResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/balance/historical".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/holders/count/historical".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -45,283 +42,277 @@
 
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
     params["timeInterval"] = time_interval
 
-    params["accountAddress"] = account_address
-
-    params["quoteAddress"] = quote_address
-
-    params["scaled"] = scaled
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenBalanceHistoricalResponse:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenHistoricalHoldersCountResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenBalanceHistoricalResponse.from_dict(response.json())
+        response_200 = TokenHistoricalHoldersCountResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         raise errors.CredmarkError(response.status_code, response.content, response_400)
     raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenBalanceHistoricalResponse]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenHistoricalHoldersCountResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[TokenBalanceHistoricalResponse]:
-    """Get historical balance
+) -> Response[TokenHistoricalHoldersCountResponse]:
+    """Get historical total number of token holders
 
-     Returns historical token balance for an account.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        start_block_number (Union[Unset, None, float]):
-        end_block_number (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        start_timestamp (Union[Unset, None, float]):
-        end_timestamp (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
-        account_address (str):
-        quote_address (Union[Unset, None, str]):
-        scaled (Union[Unset, None, bool]):  Default: True.
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        start_block_number (Union[Unset, None, float]): Start block number of the balance.
+            Defaults to token's creation block.
+        end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+            the latest block.
+        block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+        start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+            specified instead of start block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+            specified instead of end block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+            Should be in seconds. Defaults to 86,400.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenBalanceHistoricalResponse]
+        Response[TokenHistoricalHoldersCountResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
-        account_address=account_address,
-        quote_address=quote_address,
-        scaled=scaled,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> TokenBalanceHistoricalResponse:
-    """Get historical balance
+) -> TokenHistoricalHoldersCountResponse:
+    """Get historical total number of token holders
 
-     Returns historical token balance for an account.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        start_block_number (Union[Unset, None, float]):
-        end_block_number (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        start_timestamp (Union[Unset, None, float]):
-        end_timestamp (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
-        account_address (str):
-        quote_address (Union[Unset, None, str]):
-        scaled (Union[Unset, None, bool]):  Default: True.
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        start_block_number (Union[Unset, None, float]): Start block number of the balance.
+            Defaults to token's creation block.
+        end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+            the latest block.
+        block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+        start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+            specified instead of start block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+            specified instead of end block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+            Should be in seconds. Defaults to 86,400.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenBalanceHistoricalResponse]
+        Response[TokenHistoricalHoldersCountResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
-        account_address=account_address,
-        quote_address=quote_address,
-        scaled=scaled,
     ).parsed
 
 
 async def asyncio_detailed(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[TokenBalanceHistoricalResponse]:
-    """Get historical balance
+) -> Response[TokenHistoricalHoldersCountResponse]:
+    """Get historical total number of token holders
 
-     Returns historical token balance for an account.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        start_block_number (Union[Unset, None, float]):
-        end_block_number (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        start_timestamp (Union[Unset, None, float]):
-        end_timestamp (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
-        account_address (str):
-        quote_address (Union[Unset, None, str]):
-        scaled (Union[Unset, None, bool]):  Default: True.
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        start_block_number (Union[Unset, None, float]): Start block number of the balance.
+            Defaults to token's creation block.
+        end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+            the latest block.
+        block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+        start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+            specified instead of start block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+            specified instead of end block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+            Should be in seconds. Defaults to 86,400.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenBalanceHistoricalResponse]
+        Response[TokenHistoricalHoldersCountResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         time_interval=time_interval,
-        account_address=account_address,
-        quote_address=quote_address,
-        scaled=scaled,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
-    account_address: str,
-    quote_address: Union[Unset, None, str] = UNSET,
-    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> TokenBalanceHistoricalResponse:
-    """Get historical balance
+) -> TokenHistoricalHoldersCountResponse:
+    """Get historical total number of token holders
 
-     Returns historical token balance for an account.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        start_block_number (Union[Unset, None, float]):
-        end_block_number (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        start_timestamp (Union[Unset, None, float]):
-        end_timestamp (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
-        account_address (str):
-        quote_address (Union[Unset, None, str]):
-        scaled (Union[Unset, None, bool]):  Default: True.
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        start_block_number (Union[Unset, None, float]): Start block number of the balance.
+            Defaults to token's creation block.
+        end_block_number (Union[Unset, None, float]): End block number of the balance. Defaults to
+            the latest block.
+        block_interval (Union[Unset, None, float]): Number of blocks between each data point.
+        start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+            specified instead of start block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+            specified instead of end block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        time_interval (Union[Unset, None, float]): Can be specified instead of blockInterval.
+            Should be in seconds. Defaults to 86,400.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenBalanceHistoricalResponse]
+        Response[TokenHistoricalHoldersCountResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             block_interval=block_interval,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             time_interval=time_interval,
-            account_address=account_address,
-            quote_address=quote_address,
-            scaled=scaled,
         )
     ).parsed
```

### Comparing `credmark-1.2.0/credmark/api/token_api/get_token_creation_block.py` & `credmark-1.3.0/credmark/api/token_api/get_token_name.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, Union
 
 from ... import errors
-from ...models.token_creation_block_response import TokenCreationBlockResponse
 from ...models.token_error_response import TokenErrorResponse
+from ...models.token_name_response import TokenNameResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/creation-block".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/name".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -43,59 +43,70 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenCreationBlockResponse:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenNameResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenCreationBlockResponse.from_dict(response.json())
+        response_200 = TokenNameResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         raise errors.CredmarkError(response.status_code, response.content, response_400)
     raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenCreationBlockResponse]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenNameResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[TokenCreationBlockResponse]:
-    """Get token creation block
+) -> Response[TokenNameResponse]:
+    """Get token name
 
-     Returns creation block number of a token.
+     Returns name of a token.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Ethereum Mainnet
+            `10` - Optimism
+            `56` - BSC
+            `137` - Polygon Mainnet
+            `250` - Fantom Opera
+            `42161` - Arbitrum One
+            `43114` - Avalanche C-Chain
+        token_address (str): The address of the token requested.
+        block_number (Union[Unset, None, float]): Block number of the name. Defaults to the latest
+            block.
+        timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+            instead of a block number. Finds a block at or before the number of seconds since January
+            1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenCreationBlockResponse]
+        Response[TokenNameResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -107,72 +118,94 @@
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> TokenCreationBlockResponse:
-    """Get token creation block
+) -> TokenNameResponse:
+    """Get token name
 
-     Returns creation block number of a token.
+     Returns name of a token.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Ethereum Mainnet
+            `10` - Optimism
+            `56` - BSC
+            `137` - Polygon Mainnet
+            `250` - Fantom Opera
+            `42161` - Arbitrum One
+            `43114` - Avalanche C-Chain
+        token_address (str): The address of the token requested.
+        block_number (Union[Unset, None, float]): Block number of the name. Defaults to the latest
+            block.
+        timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+            instead of a block number. Finds a block at or before the number of seconds since January
+            1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenCreationBlockResponse]
+        Response[TokenNameResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
         timestamp=timestamp,
     ).parsed
 
 
 async def asyncio_detailed(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[TokenCreationBlockResponse]:
-    """Get token creation block
+) -> Response[TokenNameResponse]:
+    """Get token name
 
-     Returns creation block number of a token.
+     Returns name of a token.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Ethereum Mainnet
+            `10` - Optimism
+            `56` - BSC
+            `137` - Polygon Mainnet
+            `250` - Fantom Opera
+            `42161` - Arbitrum One
+            `43114` - Avalanche C-Chain
+        token_address (str): The address of the token requested.
+        block_number (Union[Unset, None, float]): Block number of the name. Defaults to the latest
+            block.
+        timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+            instead of a block number. Finds a block at or before the number of seconds since January
+            1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenCreationBlockResponse]
+        Response[TokenNameResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -182,37 +215,48 @@
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> TokenCreationBlockResponse:
-    """Get token creation block
+) -> TokenNameResponse:
+    """Get token name
 
-     Returns creation block number of a token.
+     Returns name of a token.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Ethereum Mainnet
+            `10` - Optimism
+            `56` - BSC
+            `137` - Polygon Mainnet
+            `250` - Fantom Opera
+            `42161` - Arbitrum One
+            `43114` - Avalanche C-Chain
+        token_address (str): The address of the token requested.
+        block_number (Union[Unset, None, float]): Block number of the name. Defaults to the latest
+            block.
+        timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+            instead of a block number. Finds a block at or before the number of seconds since January
+            1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenCreationBlockResponse]
+        Response[TokenNameResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.2.0/credmark/api/token_api/get_token_holders_count.py` & `credmark-1.3.0/credmark/api/token_api/get_token_abi.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, Union
 
 from ... import errors
+from ...models.token_abi_response import TokenAbiResponse
 from ...models.token_error_response import TokenErrorResponse
-from ...models.token_holders_count_response import TokenHoldersCountResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/holders/count".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/abi".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -43,59 +43,64 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenHoldersCountResponse:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenAbiResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenHoldersCountResponse.from_dict(response.json())
+        response_200 = TokenAbiResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         raise errors.CredmarkError(response.status_code, response.content, response_400)
     raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenHoldersCountResponse]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenAbiResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[TokenHoldersCountResponse]:
-    """Get total number of token holders
+) -> Response[TokenAbiResponse]:
+    """Get token ABI
 
-     Returns total number of holders of a token at a block or time.
+     Returns ABI of a token.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        block_number (Union[Unset, None, float]): Block number of the ABI. Defaults to the latest
+            block.
+        timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+            instead of a block number. Finds a block at or before the number of seconds since January
+            1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenHoldersCountResponse]
+        Response[TokenAbiResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -107,72 +112,82 @@
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> TokenHoldersCountResponse:
-    """Get total number of token holders
+) -> TokenAbiResponse:
+    """Get token ABI
 
-     Returns total number of holders of a token at a block or time.
+     Returns ABI of a token.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        block_number (Union[Unset, None, float]): Block number of the ABI. Defaults to the latest
+            block.
+        timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+            instead of a block number. Finds a block at or before the number of seconds since January
+            1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenHoldersCountResponse]
+        Response[TokenAbiResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
         timestamp=timestamp,
     ).parsed
 
 
 async def asyncio_detailed(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[TokenHoldersCountResponse]:
-    """Get total number of token holders
+) -> Response[TokenAbiResponse]:
+    """Get token ABI
 
-     Returns total number of holders of a token at a block or time.
+     Returns ABI of a token.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        block_number (Union[Unset, None, float]): Block number of the ABI. Defaults to the latest
+            block.
+        timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+            instead of a block number. Finds a block at or before the number of seconds since January
+            1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenHoldersCountResponse]
+        Response[TokenAbiResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -182,37 +197,42 @@
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> TokenHoldersCountResponse:
-    """Get total number of token holders
+) -> TokenAbiResponse:
+    """Get token ABI
 
-     Returns total number of holders of a token at a block or time.
+     Returns ABI of a token.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        block_number (Union[Unset, None, float]): Block number of the ABI. Defaults to the latest
+            block.
+        timestamp (Union[Unset, None, float]): Timestamp of a block number can be specified
+            instead of a block number. Finds a block at or before the number of seconds since January
+            1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenHoldersCountResponse]
+        Response[TokenAbiResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.2.0/credmark/api/token_api/get_token_name.py` & `credmark-1.3.0/credmark/api/utilities/get_daily_model_usage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,222 +1,207 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Union, cast
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Union
+from typing import List, Union, cast
 
 from ... import errors
-from ...models.token_error_response import TokenErrorResponse
-from ...models.token_name_response import TokenNameResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    chain_id: float,
-    token_address: str,
     *,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
+    days: Union[Unset, None, float] = UNSET,
+    group_by: Union[Unset, None, str] = UNSET,
+    requester: Union[Unset, None, str] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/name".format(
-        client.base_url, chainId=chain_id, tokenAddress=token_address
-    )
+    url = "{}/v1/usage/requests".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["blockNumber"] = block_number
+    params["days"] = days
+
+    params["groupBy"] = group_by
 
-    params["timestamp"] = timestamp
+    params["requester"] = requester
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenNameResponse:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> List[Dict[str, Any]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenNameResponse.from_dict(response.json())
+        response_200 = cast(List[Dict[str, Any]], response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = TokenErrorResponse.from_dict(response.json())
-
-        raise errors.CredmarkError(response.status_code, response.content, response_400)
     raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenNameResponse]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[List[Dict[str, Any]]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    chain_id: float,
-    token_address: str,
     *,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
+    days: Union[Unset, None, float] = UNSET,
+    group_by: Union[Unset, None, str] = UNSET,
+    requester: Union[Unset, None, str] = UNSET,
     client: "Credmark",
-) -> Response[TokenNameResponse]:
-    """Get token name
+) -> Response[List[Dict[str, Any]]]:
+    """Model Request statistics
 
-     Returns name of a token.
+     Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        days (Union[Unset, None, float]): Size of window in days [OPTIONAL]. Defaults to 90.
+        group_by (Union[Unset, None, str]): Group results by "model", "requester-model",
+            "requester" [OPTIONAL]. Only used if `requester` is not specified. Defaults to "model".
+        requester (Union[Unset, None, str]): The NFT Id of the requester [OPTIONAL]
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenNameResponse]
+        Response[List[Dict[str, Any]]]
     """
 
     kwargs = _get_kwargs(
-        chain_id=chain_id,
-        token_address=token_address,
         client=client,
-        block_number=block_number,
-        timestamp=timestamp,
+        days=days,
+        group_by=group_by,
+        requester=requester,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    chain_id: float,
-    token_address: str,
     *,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
+    days: Union[Unset, None, float] = UNSET,
+    group_by: Union[Unset, None, str] = UNSET,
+    requester: Union[Unset, None, str] = UNSET,
     client: "Credmark",
-) -> TokenNameResponse:
-    """Get token name
+) -> List[Dict[str, Any]]:
+    """Model Request statistics
 
-     Returns name of a token.
+     Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        days (Union[Unset, None, float]): Size of window in days [OPTIONAL]. Defaults to 90.
+        group_by (Union[Unset, None, str]): Group results by "model", "requester-model",
+            "requester" [OPTIONAL]. Only used if `requester` is not specified. Defaults to "model".
+        requester (Union[Unset, None, str]): The NFT Id of the requester [OPTIONAL]
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenNameResponse]
+        Response[List[Dict[str, Any]]]
     """
 
     return sync_detailed(
-        chain_id=chain_id,
-        token_address=token_address,
         client=client,
-        block_number=block_number,
-        timestamp=timestamp,
+        days=days,
+        group_by=group_by,
+        requester=requester,
     ).parsed
 
 
 async def asyncio_detailed(
-    chain_id: float,
-    token_address: str,
     *,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
+    days: Union[Unset, None, float] = UNSET,
+    group_by: Union[Unset, None, str] = UNSET,
+    requester: Union[Unset, None, str] = UNSET,
     client: "Credmark",
-) -> Response[TokenNameResponse]:
-    """Get token name
+) -> Response[List[Dict[str, Any]]]:
+    """Model Request statistics
 
-     Returns name of a token.
+     Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        days (Union[Unset, None, float]): Size of window in days [OPTIONAL]. Defaults to 90.
+        group_by (Union[Unset, None, str]): Group results by "model", "requester-model",
+            "requester" [OPTIONAL]. Only used if `requester` is not specified. Defaults to "model".
+        requester (Union[Unset, None, str]): The NFT Id of the requester [OPTIONAL]
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenNameResponse]
+        Response[List[Dict[str, Any]]]
     """
 
     kwargs = _get_kwargs(
-        chain_id=chain_id,
-        token_address=token_address,
         client=client,
-        block_number=block_number,
-        timestamp=timestamp,
+        days=days,
+        group_by=group_by,
+        requester=requester,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    chain_id: float,
-    token_address: str,
     *,
-    block_number: Union[Unset, None, float] = UNSET,
-    timestamp: Union[Unset, None, float] = UNSET,
+    days: Union[Unset, None, float] = UNSET,
+    group_by: Union[Unset, None, str] = UNSET,
+    requester: Union[Unset, None, str] = UNSET,
     client: "Credmark",
-) -> TokenNameResponse:
-    """Get token name
+) -> List[Dict[str, Any]]:
+    """Model Request statistics
 
-     Returns name of a token.
+     Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        block_number (Union[Unset, None, float]):
-        timestamp (Union[Unset, None, float]):
+        days (Union[Unset, None, float]): Size of window in days [OPTIONAL]. Defaults to 90.
+        group_by (Union[Unset, None, str]): Group results by "model", "requester-model",
+            "requester" [OPTIONAL]. Only used if `requester` is not specified. Defaults to "model".
+        requester (Union[Unset, None, str]): The NFT Id of the requester [OPTIONAL]
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenNameResponse]
+        Response[List[Dict[str, Any]]]
     """
 
     return (
         await asyncio_detailed(
-            chain_id=chain_id,
-            token_address=token_address,
             client=client,
-            block_number=block_number,
-            timestamp=timestamp,
+            days=days,
+            group_by=group_by,
+            requester=requester,
         )
     ).parsed
```

### Comparing `credmark-1.2.0/credmark/api/token_api/get_token_volume_historical.py` & `credmark-1.3.0/credmark/api/token_api/get_token_volume.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,32 +6,30 @@
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
-from ...models.token_volume_historical_response import TokenVolumeHistoricalResponse
+from ...models.token_volume_response import TokenVolumeResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/volume/historical".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/volume".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -41,257 +39,265 @@
 
     params["endBlockNumber"] = end_block_number
 
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
-    params["blockInterval"] = block_interval
-
-    params["timeInterval"] = time_interval
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenVolumeHistoricalResponse:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenVolumeResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenVolumeHistoricalResponse.from_dict(response.json())
+        response_200 = TokenVolumeResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
         raise errors.CredmarkError(response.status_code, response.content, response_400)
     raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenVolumeHistoricalResponse]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenVolumeResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[TokenVolumeHistoricalResponse]:
-    """Get historical volume
+) -> Response[TokenVolumeResponse]:
+    """Get token volume
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
-        start_block_number (Union[Unset, None, float]):
-        end_block_number (Union[Unset, None, float]):
-        start_timestamp (Union[Unset, None, float]):
-        end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        scaled (Union[Unset, None, bool]): Scale volume by token decimals. Defaults to `true`.
+            Default: True.
+        start_block_number (Union[Unset, None, float]): Start block number of duration for which
+            token volume will be computed.
+        end_block_number (Union[Unset, None, float]): Start block number of duration for which
+            token volume will be computed. Defaults to the latest block.
+        start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+            specified instead of start block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+            specified instead of end block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenVolumeHistoricalResponse]
+        Response[TokenVolumeResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
-        block_interval=block_interval,
-        time_interval=time_interval,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> TokenVolumeHistoricalResponse:
-    """Get historical volume
+) -> TokenVolumeResponse:
+    """Get token volume
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
-        start_block_number (Union[Unset, None, float]):
-        end_block_number (Union[Unset, None, float]):
-        start_timestamp (Union[Unset, None, float]):
-        end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        scaled (Union[Unset, None, bool]): Scale volume by token decimals. Defaults to `true`.
+            Default: True.
+        start_block_number (Union[Unset, None, float]): Start block number of duration for which
+            token volume will be computed.
+        end_block_number (Union[Unset, None, float]): Start block number of duration for which
+            token volume will be computed. Defaults to the latest block.
+        start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+            specified instead of start block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+            specified instead of end block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenVolumeHistoricalResponse]
+        Response[TokenVolumeResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
-        block_interval=block_interval,
-        time_interval=time_interval,
     ).parsed
 
 
 async def asyncio_detailed(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[TokenVolumeHistoricalResponse]:
-    """Get historical volume
+) -> Response[TokenVolumeResponse]:
+    """Get token volume
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
-        start_block_number (Union[Unset, None, float]):
-        end_block_number (Union[Unset, None, float]):
-        start_timestamp (Union[Unset, None, float]):
-        end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        scaled (Union[Unset, None, bool]): Scale volume by token decimals. Defaults to `true`.
+            Default: True.
+        start_block_number (Union[Unset, None, float]): Start block number of duration for which
+            token volume will be computed.
+        end_block_number (Union[Unset, None, float]): Start block number of duration for which
+            token volume will be computed. Defaults to the latest block.
+        start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+            specified instead of start block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+            specified instead of end block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenVolumeHistoricalResponse]
+        Response[TokenVolumeResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
-        block_interval=block_interval,
-        time_interval=time_interval,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    chain_id: float,
+    chain_id: int,
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> TokenVolumeHistoricalResponse:
-    """Get historical volume
+) -> TokenVolumeResponse:
+    """Get token volume
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
-        chain_id (float):
-        token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
-        start_block_number (Union[Unset, None, float]):
-        end_block_number (Union[Unset, None, float]):
-        start_timestamp (Union[Unset, None, float]):
-        end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
+        chain_id (int): Chain identifier. This endpoint supports the following chains
+
+            `1` - Mainnet
+        token_address (str): The address of the token requested.
+        scaled (Union[Unset, None, bool]): Scale volume by token decimals. Defaults to `true`.
+            Default: True.
+        start_block_number (Union[Unset, None, float]): Start block number of duration for which
+            token volume will be computed.
+        end_block_number (Union[Unset, None, float]): Start block number of duration for which
+            token volume will be computed. Defaults to the latest block.
+        start_timestamp (Union[Unset, None, float]): Start timestamp of a block number can be
+            specified instead of start block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
+        end_timestamp (Union[Unset, None, float]): End timestamp of a block number can be
+            specified instead of end block number. Finds a block at or before the number of seconds
+            since January 1, 1970.
 
     Raises:
         errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[TokenVolumeHistoricalResponse]
+        Response[TokenVolumeResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
             scaled=scaled,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
-            block_interval=block_interval,
-            time_interval=time_interval,
         )
     ).parsed
```

### Comparing `credmark-1.2.0/credmark/api/utilities/__init__.py` & `credmark-1.3.0/credmark/api/utilities/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,17 +57,18 @@
         requester: Union[Unset, None, str] = UNSET,
     ) -> List[Dict[str, Any]]:
         """Model Request statistics
 
          Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
         Args:
-            days (Union[Unset, None, float]):
-            group_by (Union[Unset, None, str]):
-            requester (Union[Unset, None, str]):
+            days (Union[Unset, None, float]): Size of window in days [OPTIONAL]. Defaults to 90.
+            group_by (Union[Unset, None, str]): Group results by "model", "requester-model",
+                "requester" [OPTIONAL]. Only used if `requester` is not specified. Defaults to "model".
+            requester (Union[Unset, None, str]): The NFT Id of the requester [OPTIONAL]
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List[Dict[str, Any]]]
@@ -88,17 +89,18 @@
         requester: Union[Unset, None, str] = UNSET,
     ) -> List[Dict[str, Any]]:
         """Model Request statistics
 
          Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
         Args:
-            days (Union[Unset, None, float]):
-            group_by (Union[Unset, None, str]):
-            requester (Union[Unset, None, str]):
+            days (Union[Unset, None, float]): Size of window in days [OPTIONAL]. Defaults to 90.
+            group_by (Union[Unset, None, str]): Group results by "model", "requester-model",
+                "requester" [OPTIONAL]. Only used if `requester` is not specified. Defaults to "model".
+            requester (Union[Unset, None, str]): The NFT Id of the requester [OPTIONAL]
 
         Raises:
             errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List[Dict[str, Any]]]
```

### Comparing `credmark-1.2.0/credmark/api/utilities/check_health.py` & `credmark-1.3.0/credmark/api/utilities/check_health.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/api/utilities/get_top_models.py` & `credmark-1.3.0/credmark/api/utilities/get_top_models.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/api/utilities/get_total_model_usage.py` & `credmark-1.3.0/credmark/api/utilities/get_total_model_usage.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/client.py` & `credmark-1.3.0/credmark/client.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/DefiApi.md` & `credmark-1.3.0/credmark/docs/DefiApi.md`

 * *Files 8% similar despite different names*

```diff
@@ -72,19 +72,19 @@
  Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
 and get results, use `POST /v1/model/run`.
 
 
 ### Parameters:
 Name | Type | Description
 ------------ | ------------- | -------------
-slug | str | None
-sort | str | None
-order | GetCachedModelResultsOrder | None
-limit | float | None
-offset | float | None
+slug | str | Model slug
+sort | str | Field to sort results by: 'time', 'runtime'. Defaults to 'time'.
+order | GetCachedModelResultsOrder | "asc" ascending order or "desc" descending order. Default is "desc".
+limit | float | Maximum number of results to return. Defaults to 100.
+offset | float | Offset index of results to return for pagination. Defaults to 0.
 
 
 ### Response Type
 ModelRuntimeStatsResponse
 
 # **run_model**
```

### Comparing `credmark-1.2.0/credmark/docs/ModelMetadata.md` & `credmark-1.3.0/credmark/docs/ModelMetadata.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/ModelRunResponse.md` & `credmark-1.3.0/credmark/docs/ModelRunResponse.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 ## Properties
 Name | Type | Description
 ------------ | ------------- | -------------
 slug | str | Short identifying name for the model
 version | str | Version of the model
 chain_id | float | Chain id
 block_number | float | Block number
+block_timestamp | float | Block timestamp
 dependencies | Dict[str, Any] | Dictionary of model dependencies, model name to version or version list.
 cached | bool | Whether it is a cached result
 runtime | float | Running time of the model in milliseconds.
 output | Union[Unset, Dict[str, Any]] | Data generated by the model. An object, the contents of which are specific to the model. If the model run generated an error, this output property will not exist and an error property will exist.
 error | Union[Unset, ModelRunResponseError] |
```

### Comparing `credmark-1.2.0/credmark/docs/ModelRunResponseError.md` & `credmark-1.3.0/credmark/docs/ModelRunResponseError.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/TokenAbiResponse.md` & `credmark-1.3.0/credmark/docs/TokenAbiResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/TokenBalanceHistoricalResponse.md` & `credmark-1.3.0/credmark/docs/TokenBalanceHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/TokenBalanceResponse.md` & `credmark-1.3.0/credmark/docs/TokenBalanceResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/TokenHistoricalHoldersCountResponse.md` & `credmark-1.3.0/credmark/docs/TokenHistoricalHoldersCountResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/TokenHoldersHistoricalResponse.md` & `credmark-1.3.0/credmark/docs/TokenPriceHistoricalResponse.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# TokenHoldersHistoricalResponse
+# TokenPriceHistoricalResponse
 
 
 ## Properties
 Name | Type | Description
 ------------ | ------------- | -------------
 chain_id | float | Chain ID.
 start_block_number | float | Start block number.
 end_block_number | float | End block number.
 start_timestamp | float | Start timestamp. Number of seconds since January 1, 1970.
 end_timestamp | float | End timestamp. Number of seconds since January 1, 1970.
 token_address | str | Token address for the price.
-scaled | bool | If the holding is scaled by token decimals.
 quote_address | str | Quote address is the token/currency of the price units.
-data | List['TokenHoldersHistoricalItem'] | None
+data | List['TokenPriceHistoricalItem'] | None
```

### Comparing `credmark-1.2.0/credmark/docs/TokenHoldersResponse.md` & `credmark-1.3.0/credmark/docs/TokenHoldersResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/TokenPriceHistoricalResponse.md` & `credmark-1.3.0/credmark/docs/TokenVolumeResponse.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# TokenPriceHistoricalResponse
+# TokenVolumeResponse
 
 
 ## Properties
 Name | Type | Description
 ------------ | ------------- | -------------
 chain_id | float | Chain ID.
 start_block_number | float | Start block number.
 end_block_number | float | End block number.
 start_timestamp | float | Start timestamp. Number of seconds since January 1, 1970.
 end_timestamp | float | End timestamp. Number of seconds since January 1, 1970.
 token_address | str | Token address for the price.
-quote_address | str | Quote address is the token/currency of the price units.
-data | List['TokenPriceHistoricalItem'] | None
+scaled | bool | If the volume is scaled by token decimals.
+volume | float | Token volume
```

### Comparing `credmark-1.2.0/credmark/docs/TokenPriceResponse.md` & `credmark-1.3.0/credmark/docs/TokenPriceResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md` & `credmark-1.3.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/TokenVolumeHistoricalResponse.md` & `credmark-1.3.0/credmark/docs/TokenVolumeHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/docs/Utilities.md` & `credmark-1.3.0/credmark/docs/Utilities.md`

 * *Files 27% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
  Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
 
 ### Parameters:
 Name | Type | Description
 ------------ | ------------- | -------------
-days | float | None
-group_by | str | None
-requester | str | None
+days | float | Size of window in days [OPTIONAL]. Defaults to 90.
+group_by | str | Group results by "model", "requester-model", "requester" [OPTIONAL]. Only used if `requester` is not specified. Defaults to "model".
+requester | str | The NFT Id of the requester [OPTIONAL]
 
 
 ### Response Type
 List[Dict[str, Any]]
 
 # **get_top_models**
```

### Comparing `credmark-1.2.0/credmark/errors.py` & `credmark-1.3.0/credmark/errors.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/__init__.py` & `credmark-1.3.0/credmark/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from .check_health_response_503_details import CheckHealthResponse503Details
 from .check_health_response_503_details_additional_property import CheckHealthResponse503DetailsAdditionalProperty
 from .check_health_response_503_error import CheckHealthResponse503Error
 from .check_health_response_503_error_additional_property import CheckHealthResponse503ErrorAdditionalProperty
 from .check_health_response_503_info import CheckHealthResponse503Info
 from .check_health_response_503_info_additional_property import CheckHealthResponse503InfoAdditionalProperty
 from .get_cached_model_results_order import GetCachedModelResultsOrder
-from .get_token_price_align import GetTokenPriceAlign
 from .get_token_price_historical_src import GetTokenPriceHistoricalSrc
 from .get_token_price_src import GetTokenPriceSrc
 from .model_call_stack_entry import ModelCallStackEntry
 from .model_deployment import ModelDeployment
 from .model_metadata import ModelMetadata
 from .model_run_response import ModelRunResponse
 from .model_run_response_error import ModelRunResponseError
@@ -34,16 +33,14 @@
 from .token_creation_block_response import TokenCreationBlockResponse
 from .token_decimals_response import TokenDecimalsResponse
 from .token_error_response import TokenErrorResponse
 from .token_historical_holders_count_response import TokenHistoricalHoldersCountResponse
 from .token_holder import TokenHolder
 from .token_holders_count_historical_item import TokenHoldersCountHistoricalItem
 from .token_holders_count_response import TokenHoldersCountResponse
-from .token_holders_historical_item import TokenHoldersHistoricalItem
-from .token_holders_historical_response import TokenHoldersHistoricalResponse
 from .token_holders_response import TokenHoldersResponse
 from .token_logo_response import TokenLogoResponse
 from .token_metadata_response import TokenMetadataResponse
 from .token_name_response import TokenNameResponse
 from .token_price_historical_item import TokenPriceHistoricalItem
 from .token_price_historical_response import TokenPriceHistoricalResponse
 from .token_price_response import TokenPriceResponse
@@ -67,15 +64,14 @@
     "CheckHealthResponse503Details",
     "CheckHealthResponse503DetailsAdditionalProperty",
     "CheckHealthResponse503Error",
     "CheckHealthResponse503ErrorAdditionalProperty",
     "CheckHealthResponse503Info",
     "CheckHealthResponse503InfoAdditionalProperty",
     "GetCachedModelResultsOrder",
-    "GetTokenPriceAlign",
     "GetTokenPriceHistoricalSrc",
     "GetTokenPriceSrc",
     "ModelCallStackEntry",
     "ModelDeployment",
     "ModelMetadata",
     "ModelRunResponse",
     "ModelRunResponseError",
@@ -90,16 +86,14 @@
     "TokenCreationBlockResponse",
     "TokenDecimalsResponse",
     "TokenErrorResponse",
     "TokenHistoricalHoldersCountResponse",
     "TokenHolder",
     "TokenHoldersCountHistoricalItem",
     "TokenHoldersCountResponse",
-    "TokenHoldersHistoricalItem",
-    "TokenHoldersHistoricalResponse",
     "TokenHoldersResponse",
     "TokenLogoResponse",
     "TokenMetadataResponse",
     "TokenNameResponse",
     "TokenPriceHistoricalItem",
     "TokenPriceHistoricalResponse",
     "TokenPriceResponse",
```

### Comparing `credmark-1.2.0/credmark/models/check_health_response_200.py` & `credmark-1.3.0/credmark/models/check_health_response_200.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_200_details.py` & `credmark-1.3.0/credmark/models/check_health_response_200_details.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_200_details_additional_property.py` & `credmark-1.3.0/credmark/models/check_health_response_200_details_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_200_error.py` & `credmark-1.3.0/credmark/models/check_health_response_200_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_200_error_additional_property.py` & `credmark-1.3.0/credmark/models/check_health_response_200_error_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_200_info.py` & `credmark-1.3.0/credmark/models/check_health_response_200_info.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_200_info_additional_property.py` & `credmark-1.3.0/credmark/models/check_health_response_200_info_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_503.py` & `credmark-1.3.0/credmark/models/check_health_response_503.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_503_details.py` & `credmark-1.3.0/credmark/models/check_health_response_503_details.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_503_details_additional_property.py` & `credmark-1.3.0/credmark/models/check_health_response_503_details_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_503_error.py` & `credmark-1.3.0/credmark/models/check_health_response_503_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_503_error_additional_property.py` & `credmark-1.3.0/credmark/models/check_health_response_503_error_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_503_info.py` & `credmark-1.3.0/credmark/models/check_health_response_503_info.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/check_health_response_503_info_additional_property.py` & `credmark-1.3.0/credmark/models/check_health_response_503_info_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/model_call_stack_entry.py` & `credmark-1.3.0/credmark/models/model_call_stack_entry.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/model_deployment.py` & `credmark-1.3.0/credmark/models/model_deployment.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/model_metadata.py` & `credmark-1.3.0/credmark/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/model_run_response.py` & `credmark-1.3.0/credmark/models/model_run_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,40 +15,43 @@
 class ModelRunResponse:
     """
     Attributes:
         slug (str): Short identifying name for the model Example: var.
         version (str): Version of the model Example: 1.0.
         chain_id (float): Chain id
         block_number (float): Block number
+        block_timestamp (float): Block timestamp
         dependencies (Dict[str, Any]): Dictionary of model dependencies, model name to version or version list. Example:
             {"x": "1.0", "y": ["2.0", "2.1"]}.
         cached (bool): Whether it is a cached result Example: True.
         runtime (float): Running time of the model in milliseconds. Example: 5100.
         output (Union[Unset, Dict[str, Any]]): Data generated by the model. An object, the contents of which are
             specific to the model. If the model run generated an error, this output property will not exist and an error
             property will exist. Example: { ... }.
         error (Union[Unset, ModelRunResponseError]):
     """
 
     slug: str
     version: str
     chain_id: float
     block_number: float
+    block_timestamp: float
     dependencies: Dict[str, Any]
     cached: bool
     runtime: float
     output: Union[Unset, Dict[str, Any]] = UNSET
     error: Union[Unset, "ModelRunResponseError"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         slug = self.slug
         version = self.version
         chain_id = self.chain_id
         block_number = self.block_number
+        block_timestamp = self.block_timestamp
         dependencies = self.dependencies
         cached = self.cached
         runtime = self.runtime
         output = self.output
         error: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.error, Unset):
             error = self.error.to_dict()
@@ -57,14 +60,15 @@
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "slug": slug,
                 "version": version,
                 "chainId": chain_id,
                 "blockNumber": block_number,
+                "blockTimestamp": block_timestamp,
                 "dependencies": dependencies,
                 "cached": cached,
                 "runtime": runtime,
             }
         )
         if output is not UNSET:
             field_dict["output"] = output
@@ -82,14 +86,16 @@
 
         version = d.pop("version")
 
         chain_id = d.pop("chainId")
 
         block_number = d.pop("blockNumber")
 
+        block_timestamp = d.pop("blockTimestamp")
+
         dependencies = d.pop("dependencies")
 
         cached = d.pop("cached")
 
         runtime = d.pop("runtime")
 
         output = d.pop("output", UNSET)
@@ -102,14 +108,15 @@
             error = ModelRunResponseError.from_dict(_error)
 
         model_run_response = cls(
             slug=slug,
             version=version,
             chain_id=chain_id,
             block_number=block_number,
+            block_timestamp=block_timestamp,
             dependencies=dependencies,
             cached=cached,
             runtime=runtime,
             output=output,
             error=error,
         )
```

### Comparing `credmark-1.2.0/credmark/models/model_run_response_error.py` & `credmark-1.3.0/credmark/models/model_run_response_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/model_runtime_statistics.py` & `credmark-1.3.0/credmark/models/model_runtime_statistics.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/model_runtime_stats_response.py` & `credmark-1.3.0/credmark/models/model_runtime_stats_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/run_model_dto.py` & `credmark-1.3.0/credmark/models/run_model_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 @attr.s(auto_attribs=True)
 class RunModelDto:
     """
     Attributes:
         slug (str): slug of the model to run
         chain_id (int): chainId number, for example 1 for mainnet Default: 1.
         block_number (Union[RunModelDtoBlockNumberType1, int]): blockNumber is a number or a string with a number,
-            'latest', 'earliest', or 'pending'
+            'latest', 'earliest'
         input (Dict[str, Any]): Model input data
         version (Union[Unset, str]): Typically not required but you may specify version of the model to run
     """
 
     slug: str
     block_number: Union[RunModelDtoBlockNumberType1, int]
     input: Dict[str, Any]
```

### Comparing `credmark-1.2.0/credmark/models/token_abi_response.py` & `credmark-1.3.0/credmark/models/token_abi_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_balance_historical_item.py` & `credmark-1.3.0/credmark/models/token_balance_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_balance_historical_response.py` & `credmark-1.3.0/credmark/models/token_balance_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_balance_response.py` & `credmark-1.3.0/credmark/models/token_balance_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_creation_block_response.py` & `credmark-1.3.0/credmark/models/token_creation_block_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_decimals_response.py` & `credmark-1.3.0/credmark/models/token_decimals_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_error_response.py` & `credmark-1.3.0/credmark/models/token_error_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_historical_holders_count_response.py` & `credmark-1.3.0/credmark/models/token_historical_holders_count_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_holder.py` & `credmark-1.3.0/credmark/models/token_holder.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_holders_count_historical_item.py` & `credmark-1.3.0/credmark/models/token_holders_count_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_holders_count_response.py` & `credmark-1.3.0/credmark/models/token_holders_count_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_holders_historical_item.py` & `credmark-1.3.0/credmark/models/token_logo_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,77 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.token_holder import TokenHolder
-
-
-T = TypeVar("T", bound="TokenHoldersHistoricalItem")
+T = TypeVar("T", bound="TokenLogoResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenHoldersHistoricalItem:
+class TokenLogoResponse:
     """
     Attributes:
+        chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
-        data (List['TokenHolder']): List of holders from the top
-        total (float): Total number of holders Example: 10.
+        token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
+        logo_url (str): Token logo url Example: https://raw.githubusercontent.com/trustwallet/assets/master/blockchains/
+            ethereum/assets/0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9/logo.png.
     """
 
+    chain_id: float
     block_number: float
     block_timestamp: float
-    data: List["TokenHolder"]
-    total: float
+    token_address: str
+    logo_url: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
-        data = []
-        for data_item_data in self.data:
-            data_item = data_item_data.to_dict()
-
-            data.append(data_item)
-
-        total = self.total
+        token_address = self.token_address
+        logo_url = self.logo_url
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
-                "data": data,
-                "total": total,
+                "tokenAddress": token_address,
+                "logoUrl": logo_url,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.token_holder import TokenHolder
-
         d = src_dict.copy()
+        chain_id = d.pop("chainId")
+
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
-        data = []
-        _data = d.pop("data")
-        for data_item_data in _data:
-            data_item = TokenHolder.from_dict(data_item_data)
-
-            data.append(data_item)
+        token_address = d.pop("tokenAddress")
 
-        total = d.pop("total")
+        logo_url = d.pop("logoUrl")
 
-        token_holders_historical_item = cls(
+        token_logo_response = cls(
+            chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
-            data=data,
-            total=total,
+            token_address=token_address,
+            logo_url=logo_url,
         )
 
-        token_holders_historical_item.additional_properties = d
-        return token_holders_historical_item
+        token_logo_response.additional_properties = d
+        return token_logo_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `credmark-1.2.0/credmark/models/token_holders_historical_response.py` & `credmark-1.3.0/credmark/models/token_price_historical_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
 if TYPE_CHECKING:
-    from ..models.token_holders_historical_item import TokenHoldersHistoricalItem
+    from ..models.token_price_historical_item import TokenPriceHistoricalItem
 
 
-T = TypeVar("T", bound="TokenHoldersHistoricalResponse")
+T = TypeVar("T", bound="TokenPriceHistoricalResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenHoldersHistoricalResponse:
+class TokenPriceHistoricalResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         start_block_number (float): Start block number. Example: 15384120.
         end_block_number (float): End block number. Example: 15581908.
         start_timestamp (float): Start timestamp. Number of seconds since January 1, 1970. Example: 1661086905.
         end_timestamp (float): End timestamp. Number of seconds since January 1, 1970. Example: 1663765199.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        scaled (bool): If the holding is scaled by token decimals. Example: True.
         quote_address (str): Quote address is the token/currency of the price units. Example:
             0x0000000000000000000000000000000000000348.
-        data (List['TokenHoldersHistoricalItem']):
+        data (List['TokenPriceHistoricalItem']):
     """
 
     chain_id: float
     start_block_number: float
     end_block_number: float
     start_timestamp: float
     end_timestamp: float
     token_address: str
-    scaled: bool
     quote_address: str
-    data: List["TokenHoldersHistoricalItem"]
+    data: List["TokenPriceHistoricalItem"]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         start_block_number = self.start_block_number
         end_block_number = self.end_block_number
         start_timestamp = self.start_timestamp
         end_timestamp = self.end_timestamp
         token_address = self.token_address
-        scaled = self.scaled
         quote_address = self.quote_address
         data = []
         for data_item_data in self.data:
             data_item = data_item_data.to_dict()
 
             data.append(data_item)
 
@@ -57,64 +54,60 @@
             {
                 "chainId": chain_id,
                 "startBlockNumber": start_block_number,
                 "endBlockNumber": end_block_number,
                 "startTimestamp": start_timestamp,
                 "endTimestamp": end_timestamp,
                 "tokenAddress": token_address,
-                "scaled": scaled,
                 "quoteAddress": quote_address,
                 "data": data,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.token_holders_historical_item import TokenHoldersHistoricalItem
+        from ..models.token_price_historical_item import TokenPriceHistoricalItem
 
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
         start_block_number = d.pop("startBlockNumber")
 
         end_block_number = d.pop("endBlockNumber")
 
         start_timestamp = d.pop("startTimestamp")
 
         end_timestamp = d.pop("endTimestamp")
 
         token_address = d.pop("tokenAddress")
 
-        scaled = d.pop("scaled")
-
         quote_address = d.pop("quoteAddress")
 
         data = []
         _data = d.pop("data")
         for data_item_data in _data:
-            data_item = TokenHoldersHistoricalItem.from_dict(data_item_data)
+            data_item = TokenPriceHistoricalItem.from_dict(data_item_data)
 
             data.append(data_item)
 
-        token_holders_historical_response = cls(
+        token_price_historical_response = cls(
             chain_id=chain_id,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             token_address=token_address,
-            scaled=scaled,
             quote_address=quote_address,
             data=data,
         )
 
-        token_holders_historical_response.additional_properties = d
-        return token_holders_historical_response
+        token_price_historical_response.additional_properties = d
+        return token_price_historical_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `credmark-1.2.0/credmark/models/token_holders_response.py` & `credmark-1.3.0/credmark/models/token_holders_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_logo_response.py` & `credmark-1.3.0/credmark/models/token_metadata_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenLogoResponse")
+T = TypeVar("T", bound="TokenMetadataResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenLogoResponse:
+class TokenMetadataResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        logo_url (str): Token logo url Example: https://raw.githubusercontent.com/trustwallet/assets/master/blockchains/
-            ethereum/assets/0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9/logo.png.
+        name (str): Token name Example: Aave Token.
+        symbol (str): Token symbol Example: AAVE.
+        decimals (float): Token decimals Example: 18.
     """
 
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
-    logo_url: str
+    name: str
+    symbol: str
+    decimals: float
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
         token_address = self.token_address
-        logo_url = self.logo_url
+        name = self.name
+        symbol = self.symbol
+        decimals = self.decimals
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
                 "tokenAddress": token_address,
-                "logoUrl": logo_url,
+                "name": name,
+                "symbol": symbol,
+                "decimals": decimals,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -52,26 +59,32 @@
 
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
         token_address = d.pop("tokenAddress")
 
-        logo_url = d.pop("logoUrl")
+        name = d.pop("name")
 
-        token_logo_response = cls(
+        symbol = d.pop("symbol")
+
+        decimals = d.pop("decimals")
+
+        token_metadata_response = cls(
             chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
             token_address=token_address,
-            logo_url=logo_url,
+            name=name,
+            symbol=symbol,
+            decimals=decimals,
         )
 
-        token_logo_response.additional_properties = d
-        return token_logo_response
+        token_metadata_response.additional_properties = d
+        return token_metadata_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `credmark-1.2.0/credmark/models/token_metadata_response.py` & `credmark-1.3.0/credmark/models/token_symbol_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenMetadataResponse")
+T = TypeVar("T", bound="TokenSymbolResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenMetadataResponse:
+class TokenSymbolResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        name (str): Token name Example: Aave Token.
         symbol (str): Token symbol Example: AAVE.
-        decimals (float): Token decimals Example: 18.
     """
 
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
-    name: str
     symbol: str
-    decimals: float
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
         token_address = self.token_address
-        name = self.name
         symbol = self.symbol
-        decimals = self.decimals
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
                 "tokenAddress": token_address,
-                "name": name,
                 "symbol": symbol,
-                "decimals": decimals,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -59,32 +51,26 @@
 
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
         token_address = d.pop("tokenAddress")
 
-        name = d.pop("name")
-
         symbol = d.pop("symbol")
 
-        decimals = d.pop("decimals")
-
-        token_metadata_response = cls(
+        token_symbol_response = cls(
             chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
             token_address=token_address,
-            name=name,
             symbol=symbol,
-            decimals=decimals,
         )
 
-        token_metadata_response.additional_properties = d
-        return token_metadata_response
+        token_symbol_response.additional_properties = d
+        return token_symbol_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `credmark-1.2.0/credmark/models/token_name_response.py` & `credmark-1.3.0/credmark/models/token_name_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_price_historical_item.py` & `credmark-1.3.0/credmark/models/token_price_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_price_historical_response.py` & `credmark-1.3.0/credmark/models/token_total_supply_historical_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
 if TYPE_CHECKING:
-    from ..models.token_price_historical_item import TokenPriceHistoricalItem
+    from ..models.token_total_supply_historical_item import TokenTotalSupplyHistoricalItem
 
 
-T = TypeVar("T", bound="TokenPriceHistoricalResponse")
+T = TypeVar("T", bound="TokenTotalSupplyHistoricalResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenPriceHistoricalResponse:
+class TokenTotalSupplyHistoricalResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         start_block_number (float): Start block number. Example: 15384120.
         end_block_number (float): End block number. Example: 15581908.
         start_timestamp (float): Start timestamp. Number of seconds since January 1, 1970. Example: 1661086905.
         end_timestamp (float): End timestamp. Number of seconds since January 1, 1970. Example: 1663765199.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        quote_address (str): Quote address is the token/currency of the price units. Example:
-            0x0000000000000000000000000000000000000348.
-        data (List['TokenPriceHistoricalItem']):
+        scaled (bool): If the total supply is scaled by token decimals. Example: True.
+        data (List['TokenTotalSupplyHistoricalItem']):
     """
 
     chain_id: float
     start_block_number: float
     end_block_number: float
     start_timestamp: float
     end_timestamp: float
     token_address: str
-    quote_address: str
-    data: List["TokenPriceHistoricalItem"]
+    scaled: bool
+    data: List["TokenTotalSupplyHistoricalItem"]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         start_block_number = self.start_block_number
         end_block_number = self.end_block_number
         start_timestamp = self.start_timestamp
         end_timestamp = self.end_timestamp
         token_address = self.token_address
-        quote_address = self.quote_address
+        scaled = self.scaled
         data = []
         for data_item_data in self.data:
             data_item = data_item_data.to_dict()
 
             data.append(data_item)
 
         field_dict: Dict[str, Any] = {}
@@ -54,60 +53,60 @@
             {
                 "chainId": chain_id,
                 "startBlockNumber": start_block_number,
                 "endBlockNumber": end_block_number,
                 "startTimestamp": start_timestamp,
                 "endTimestamp": end_timestamp,
                 "tokenAddress": token_address,
-                "quoteAddress": quote_address,
+                "scaled": scaled,
                 "data": data,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.token_price_historical_item import TokenPriceHistoricalItem
+        from ..models.token_total_supply_historical_item import TokenTotalSupplyHistoricalItem
 
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
         start_block_number = d.pop("startBlockNumber")
 
         end_block_number = d.pop("endBlockNumber")
 
         start_timestamp = d.pop("startTimestamp")
 
         end_timestamp = d.pop("endTimestamp")
 
         token_address = d.pop("tokenAddress")
 
-        quote_address = d.pop("quoteAddress")
+        scaled = d.pop("scaled")
 
         data = []
         _data = d.pop("data")
         for data_item_data in _data:
-            data_item = TokenPriceHistoricalItem.from_dict(data_item_data)
+            data_item = TokenTotalSupplyHistoricalItem.from_dict(data_item_data)
 
             data.append(data_item)
 
-        token_price_historical_response = cls(
+        token_total_supply_historical_response = cls(
             chain_id=chain_id,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             token_address=token_address,
-            quote_address=quote_address,
+            scaled=scaled,
             data=data,
         )
 
-        token_price_historical_response.additional_properties = d
-        return token_price_historical_response
+        token_total_supply_historical_response.additional_properties = d
+        return token_total_supply_historical_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `credmark-1.2.0/credmark/models/token_price_response.py` & `credmark-1.3.0/credmark/models/token_price_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_symbol_response.py` & `credmark-1.3.0/credmark/models/token_volume_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,97 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenSymbolResponse")
+T = TypeVar("T", bound="TokenVolumeResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenSymbolResponse:
+class TokenVolumeResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
-        block_number (float): Block number. Example: 15490034.
-        block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
+        start_block_number (float): Start block number. Example: 15384120.
+        end_block_number (float): End block number. Example: 15581908.
+        start_timestamp (float): Start timestamp. Number of seconds since January 1, 1970. Example: 1661086905.
+        end_timestamp (float): End timestamp. Number of seconds since January 1, 1970. Example: 1663765199.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        symbol (str): Token symbol Example: AAVE.
+        scaled (bool): If the volume is scaled by token decimals. Example: True.
+        volume (float): Token volume Example: 16173531.8220335.
     """
 
     chain_id: float
-    block_number: float
-    block_timestamp: float
+    start_block_number: float
+    end_block_number: float
+    start_timestamp: float
+    end_timestamp: float
     token_address: str
-    symbol: str
+    scaled: bool
+    volume: float
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
-        block_number = self.block_number
-        block_timestamp = self.block_timestamp
+        start_block_number = self.start_block_number
+        end_block_number = self.end_block_number
+        start_timestamp = self.start_timestamp
+        end_timestamp = self.end_timestamp
         token_address = self.token_address
-        symbol = self.symbol
+        scaled = self.scaled
+        volume = self.volume
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
-                "blockNumber": block_number,
-                "blockTimestamp": block_timestamp,
+                "startBlockNumber": start_block_number,
+                "endBlockNumber": end_block_number,
+                "startTimestamp": start_timestamp,
+                "endTimestamp": end_timestamp,
                 "tokenAddress": token_address,
-                "symbol": symbol,
+                "scaled": scaled,
+                "volume": volume,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
-        block_number = d.pop("blockNumber")
+        start_block_number = d.pop("startBlockNumber")
 
-        block_timestamp = d.pop("blockTimestamp")
+        end_block_number = d.pop("endBlockNumber")
+
+        start_timestamp = d.pop("startTimestamp")
+
+        end_timestamp = d.pop("endTimestamp")
 
         token_address = d.pop("tokenAddress")
 
-        symbol = d.pop("symbol")
+        scaled = d.pop("scaled")
+
+        volume = d.pop("volume")
 
-        token_symbol_response = cls(
+        token_volume_response = cls(
             chain_id=chain_id,
-            block_number=block_number,
-            block_timestamp=block_timestamp,
+            start_block_number=start_block_number,
+            end_block_number=end_block_number,
+            start_timestamp=start_timestamp,
+            end_timestamp=end_timestamp,
             token_address=token_address,
-            symbol=symbol,
+            scaled=scaled,
+            volume=volume,
         )
 
-        token_symbol_response.additional_properties = d
-        return token_symbol_response
+        token_volume_response.additional_properties = d
+        return token_volume_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `credmark-1.2.0/credmark/models/token_total_supply_historical_item.py` & `credmark-1.3.0/credmark/models/token_total_supply_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_total_supply_historical_response.py` & `credmark-1.3.0/credmark/models/token_volume_historical_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
 if TYPE_CHECKING:
-    from ..models.token_total_supply_historical_item import TokenTotalSupplyHistoricalItem
+    from ..models.token_volume_historical_item import TokenVolumeHistoricalItem
 
 
-T = TypeVar("T", bound="TokenTotalSupplyHistoricalResponse")
+T = TypeVar("T", bound="TokenVolumeHistoricalResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenTotalSupplyHistoricalResponse:
+class TokenVolumeHistoricalResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         start_block_number (float): Start block number. Example: 15384120.
         end_block_number (float): End block number. Example: 15581908.
         start_timestamp (float): Start timestamp. Number of seconds since January 1, 1970. Example: 1661086905.
         end_timestamp (float): End timestamp. Number of seconds since January 1, 1970. Example: 1663765199.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        scaled (bool): If the total supply is scaled by token decimals. Example: True.
-        data (List['TokenTotalSupplyHistoricalItem']):
+        scaled (bool): If the volume is scaled by token decimals. Example: True.
+        data (List['TokenVolumeHistoricalItem']):
     """
 
     chain_id: float
     start_block_number: float
     end_block_number: float
     start_timestamp: float
     end_timestamp: float
     token_address: str
     scaled: bool
-    data: List["TokenTotalSupplyHistoricalItem"]
+    data: List["TokenVolumeHistoricalItem"]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         start_block_number = self.start_block_number
         end_block_number = self.end_block_number
         start_timestamp = self.start_timestamp
@@ -62,15 +62,15 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.token_total_supply_historical_item import TokenTotalSupplyHistoricalItem
+        from ..models.token_volume_historical_item import TokenVolumeHistoricalItem
 
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
         start_block_number = d.pop("startBlockNumber")
 
         end_block_number = d.pop("endBlockNumber")
@@ -82,31 +82,31 @@
         token_address = d.pop("tokenAddress")
 
         scaled = d.pop("scaled")
 
         data = []
         _data = d.pop("data")
         for data_item_data in _data:
-            data_item = TokenTotalSupplyHistoricalItem.from_dict(data_item_data)
+            data_item = TokenVolumeHistoricalItem.from_dict(data_item_data)
 
             data.append(data_item)
 
-        token_total_supply_historical_response = cls(
+        token_volume_historical_response = cls(
             chain_id=chain_id,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             token_address=token_address,
             scaled=scaled,
             data=data,
         )
 
-        token_total_supply_historical_response.additional_properties = d
-        return token_total_supply_historical_response
+        token_volume_historical_response.additional_properties = d
+        return token_volume_historical_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `credmark-1.2.0/credmark/models/token_total_supply_response.py` & `credmark-1.3.0/credmark/models/token_total_supply_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/models/token_volume_historical_item.py` & `credmark-1.3.0/credmark/models/token_volume_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/credmark/types.py` & `credmark-1.3.0/credmark/types.py`

 * *Files identical despite different names*

### Comparing `credmark-1.2.0/pyproject.toml` & `credmark-1.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "credmark"
-version = "1.2.0"
+version = "1.3.0"
 description = "A client library for accessing Credmark Gateway"
 license = "MIT"
 
 authors = [
   "Credmark <info@credmark.com>",
 ]
```

### Comparing `credmark-1.2.0/PKG-INFO` & `credmark-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credmark
-Version: 1.2.0
+Version: 1.3.0
 Summary: A client library for accessing Credmark Gateway
 Home-page: https://credmark.com
 License: MIT
 Author: Credmark
 Author-email: info@credmark.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

