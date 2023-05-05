# Comparing `tmp/fds.sdk.OverviewReportBuilder-1.0.1-py3-none-any.whl.zip` & `tmp/fds.sdk.OverviewReportBuilder-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,76 +1,130 @@
-Zip file size: 195761 bytes, number of entries: 74
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-24 17:23 fds/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-24 17:23 fds/sdk/__init__.py
--rw-r--r--  2.0 unx      914 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/__init__.py
--rw-r--r--  2.0 unx    39867 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/api_client.py
--rw-r--r--  2.0 unx    17749 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/configuration.py
--rw-r--r--  2.0 unx     5116 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/exceptions.py
--rw-r--r--  2.0 unx    82199 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model_utils.py
--rw-r--r--  2.0 unx    14255 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/rest.py
--rw-r--r--  2.0 unx      233 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/api/__init__.py
--rw-r--r--  2.0 unx    55244 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/api/company_api.py
--rw-r--r--  2.0 unx      482 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/apis/__init__.py
--rw-r--r--  2.0 unx      348 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/__init__.py
--rw-r--r--  2.0 unx    11342 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/category.py
--rw-r--r--  2.0 unx    11407 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/category_category.py
--rw-r--r--  2.0 unx    11436 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/currency_code.py
--rw-r--r--  2.0 unx    11132 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/currency_code_currency_code.py
--rw-r--r--  2.0 unx    11480 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/currency_symbol.py
--rw-r--r--  2.0 unx    11144 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/currency_symbol_currency_symbol.py
--rw-r--r--  2.0 unx    14071 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/data_point_meta.py
--rw-r--r--  2.0 unx    11876 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/data_point_meta_any_of.py
--rw-r--r--  2.0 unx    11408 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/description.py
--rw-r--r--  2.0 unx    11126 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/description_description.py
--rw-r--r--  2.0 unx    12429 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/error_object.py
--rw-r--r--  2.0 unx    11108 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/error_object_links.py
--rw-r--r--  2.0 unx    11131 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/error_object_source.py
--rw-r--r--  2.0 unx    11590 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/error_response.py
--rw-r--r--  2.0 unx    11364 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/frequency.py
--rw-r--r--  2.0 unx    11583 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/frequency_frequency.py
--rw-r--r--  2.0 unx    10832 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/meta.py
--rw-r--r--  2.0 unx    19219 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/metadata_entry.py
--rw-r--r--  2.0 unx    11298 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/metric.py
--rw-r--r--  2.0 unx    11181 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/metric_metric.py
--rw-r--r--  2.0 unx    11301 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/peer_list_data.py
--rw-r--r--  2.0 unx    11372 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/peer_list_object.py
--rw-r--r--  2.0 unx    11605 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/peer_list_response.py
--rw-r--r--  2.0 unx    12600 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data.py
--rw-r--r--  2.0 unx    14007 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_business.py
--rw-r--r--  2.0 unx    11421 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_business_crunchbase_categories.py
--rw-r--r--  2.0 unx    11394 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_business_crunchbase_url.py
--rw-r--r--  2.0 unx    11409 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_business_description.py
--rw-r--r--  2.0 unx    11222 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_business_industry.py
--rw-r--r--  2.0 unx    13957 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_contact.py
--rw-r--r--  2.0 unx    12004 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_contact_people.py
--rw-r--r--  2.0 unx    12633 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_size.py
--rw-r--r--  2.0 unx    11234 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_size_employee_number.py
--rw-r--r--  2.0 unx    11599 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_size_ev.py
--rw-r--r--  2.0 unx    11848 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_size_revenue.py
--rw-r--r--  2.0 unx    18231 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_stage.py
--rw-r--r--  2.0 unx    11394 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_stage_crunchbase_rank.py
--rw-r--r--  2.0 unx    11216 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_stage_pe_active_firm_number.py
--rw-r--r--  2.0 unx    11506 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_stage_pe_active_firms.py
--rw-r--r--  2.0 unx    11973 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_stage_pevc_latest_post_money_valuation.py
--rw-r--r--  2.0 unx    11717 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_data_stage_trade_date_range.py
--rw-r--r--  2.0 unx    11580 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/profile_response.py
--rw-r--r--  2.0 unx    11458 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/relevance_type.py
--rw-r--r--  2.0 unx    12285 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type.py
--rw-r--r--  2.0 unx    11267 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type_c.py
--rw-r--r--  2.0 unx    11265 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type_p.py
--rw-r--r--  2.0 unx    11267 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type_s.py
--rw-r--r--  2.0 unx    11276 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/scale.py
--rw-r--r--  2.0 unx    11090 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/scale_scale.py
--rw-r--r--  2.0 unx    11702 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/stach_table_response.py
--rw-r--r--  2.0 unx    11458 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/transaction_id.py
--rw-r--r--  2.0 unx    11138 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/transaction_id_transaction_id.py
--rw-r--r--  2.0 unx    11502 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/transaction_type.py
--rw-r--r--  2.0 unx    11271 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/transaction_type_transaction_type.py
--rw-r--r--  2.0 unx    11370 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/value_type.py
--rw-r--r--  2.0 unx    11277 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/model/value_type_value_type.py
--rw-r--r--  2.0 unx     5461 b- defN 23-Feb-24 17:23 fds/sdk/OverviewReportBuilder/models/__init__.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Feb-24 17:24 fds.sdk.OverviewReportBuilder-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    11533 b- defN 23-Feb-24 17:24 fds.sdk.OverviewReportBuilder-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-24 17:24 fds.sdk.OverviewReportBuilder-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Feb-24 17:24 fds.sdk.OverviewReportBuilder-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8385 b- defN 23-Feb-24 17:24 fds.sdk.OverviewReportBuilder-1.0.1.dist-info/RECORD
-74 files, 918246 bytes uncompressed, 181769 bytes compressed:  80.2%
+Zip file size: 352375 bytes, number of entries: 128
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 08:54 fds/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 08:54 fds/sdk/__init__.py
+-rw-r--r--  2.0 unx      928 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/__init__.py
+-rw-r--r--  2.0 unx    39881 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/api_client.py
+-rw-r--r--  2.0 unx    17763 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/configuration.py
+-rw-r--r--  2.0 unx     5130 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/exceptions.py
+-rw-r--r--  2.0 unx    82213 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model_utils.py
+-rw-r--r--  2.0 unx    14269 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/rest.py
+-rw-r--r--  2.0 unx      233 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/api/__init__.py
+-rw-r--r--  2.0 unx    67039 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/api/company_api.py
+-rw-r--r--  2.0 unx      482 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/apis/__init__.py
+-rw-r--r--  2.0 unx      348 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/__init__.py
+-rw-r--r--  2.0 unx    11356 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/category.py
+-rw-r--r--  2.0 unx    11421 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/category_category.py
+-rw-r--r--  2.0 unx    11450 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/currency_code.py
+-rw-r--r--  2.0 unx    11146 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/currency_code_currency_code.py
+-rw-r--r--  2.0 unx    11494 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/currency_symbol.py
+-rw-r--r--  2.0 unx    11158 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/currency_symbol_currency_symbol.py
+-rw-r--r--  2.0 unx    14085 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/data_point_meta.py
+-rw-r--r--  2.0 unx    11890 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/data_point_meta_any_of.py
+-rw-r--r--  2.0 unx    11422 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/description.py
+-rw-r--r--  2.0 unx    11140 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/description_description.py
+-rw-r--r--  2.0 unx    12443 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/error_object.py
+-rw-r--r--  2.0 unx    11122 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/error_object_links.py
+-rw-r--r--  2.0 unx    11145 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/error_object_source.py
+-rw-r--r--  2.0 unx    11604 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/error_response.py
+-rw-r--r--  2.0 unx    11378 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/frequency.py
+-rw-r--r--  2.0 unx    11597 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/frequency_frequency.py
+-rw-r--r--  2.0 unx    28232 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object.py
+-rw-r--r--  2.0 unx    12169 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_active_investors.py
+-rw-r--r--  2.0 unx    12169 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_average_daily_vol.py
+-rw-r--r--  2.0 unx    11248 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_average_daily_vol_value.py
+-rw-r--r--  2.0 unx    11909 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_average_rating.py
+-rw-r--r--  2.0 unx    12157 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_basic_shares.py
+-rw-r--r--  2.0 unx    11894 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_branches.py
+-rw-r--r--  2.0 unx    12178 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_broker_contributors.py
+-rw-r--r--  2.0 unx    12172 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_diluted_market_cap.py
+-rw-r--r--  2.0 unx    12163 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_diluted_shares.py
+-rw-r--r--  2.0 unx    12163 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_dividend_yield.py
+-rw-r--r--  2.0 unx    12675 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_employees.py
+-rw-r--r--  2.0 unx    12169 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_enterprise_value.py
+-rw-r--r--  2.0 unx    11921 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_estimated_vc_raised.py
+-rw-r--r--  2.0 unx    12108 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_first_date.py
+-rw-r--r--  2.0 unx    11285 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_first_date_value.py
+-rw-r--r--  2.0 unx    12117 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_first_funding.py
+-rw-r--r--  2.0 unx    12139 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_float.py
+-rw-r--r--  2.0 unx    12163 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_funding_rounds.py
+-rw-r--r--  2.0 unx    11903 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_gross_assets.py
+-rw-r--r--  2.0 unx    11909 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_gross_premiums.py
+-rw-r--r--  2.0 unx    12163 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_institutional.py
+-rw-r--r--  2.0 unx    12114 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_last_funding.py
+-rw-r--r--  2.0 unx    12466 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_latest_post_money_valuation.py
+-rw-r--r--  2.0 unx    12160 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_lt_growth_rate.py
+-rw-r--r--  2.0 unx    12151 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_market_cap.py
+-rw-r--r--  2.0 unx    11508 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_meta.py
+-rw-r--r--  2.0 unx    11173 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_meta_sources.py
+-rw-r--r--  2.0 unx    11921 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_net_interest_income.py
+-rw-r--r--  2.0 unx    11894 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_premiums.py
+-rw-r--r--  2.0 unx    11903 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_range52_week.py
+-rw-r--r--  2.0 unx    11230 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_range52_week_value.py
+-rw-r--r--  2.0 unx    12415 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_revenue.py
+-rw-r--r--  2.0 unx    11230 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_revenue_as_of_date.py
+-rw-r--r--  2.0 unx    11903 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_target_price.py
+-rw-r--r--  2.0 unx    12199 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_top10_institutional_holders.py
+-rw-r--r--  2.0 unx    11909 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_total_deposits.py
+-rw-r--r--  2.0 unx    12166 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_total_investors.py
+-rw-r--r--  2.0 unx    12136 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_wacc.py
+-rw-r--r--  2.0 unx    19428 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object.py
+-rw-r--r--  2.0 unx    12154 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_aum_fund_month.py
+-rw-r--r--  2.0 unx    12157 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_aum_share_daily.py
+-rw-r--r--  2.0 unx    11912 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_available_for_sale.py
+-rw-r--r--  2.0 unx    12121 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_average_spread.py
+-rw-r--r--  2.0 unx    11897 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_currency_iso.py
+-rw-r--r--  2.0 unx    12163 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_daily_trading_vol.py
+-rw-r--r--  2.0 unx    12133 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_distribution_yield.py
+-rw-r--r--  2.0 unx    11903 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_esg_compliance.py
+-rw-r--r--  2.0 unx    12118 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_expense_ratio.py
+-rw-r--r--  2.0 unx    11266 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_expense_ratio_value.py
+-rw-r--r--  2.0 unx    12117 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_first_nav_record.py
+-rw-r--r--  2.0 unx    12151 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_fund_flow_ytd.py
+-rw-r--r--  2.0 unx    12126 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_inception_date_fund.py
+-rw-r--r--  2.0 unx    12129 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_inception_date_share.py
+-rw-r--r--  2.0 unx    11991 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_meta.py
+-rw-r--r--  2.0 unx    11173 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_meta_as_of_date.py
+-rw-r--r--  2.0 unx    12166 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_outstanding_share.py
+-rw-r--r--  2.0 unx    11918 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_sfdr_classification.py
+-rw-r--r--  2.0 unx    38556 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_object.py
+-rw-r--r--  2.0 unx    11619 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/key_stats_response.py
+-rw-r--r--  2.0 unx    10846 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/meta.py
+-rw-r--r--  2.0 unx    18913 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/metadata_entry.py
+-rw-r--r--  2.0 unx    11312 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/metric.py
+-rw-r--r--  2.0 unx    11195 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/metric_metric.py
+-rw-r--r--  2.0 unx    11683 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/peer_list_data.py
+-rw-r--r--  2.0 unx    11802 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/peer_list_object.py
+-rw-r--r--  2.0 unx    11619 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/peer_list_response.py
+-rw-r--r--  2.0 unx    13030 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data.py
+-rw-r--r--  2.0 unx    14021 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_business.py
+-rw-r--r--  2.0 unx    11435 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_business_crunchbase_categories.py
+-rw-r--r--  2.0 unx    11408 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_business_crunchbase_url.py
+-rw-r--r--  2.0 unx    11423 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_business_description.py
+-rw-r--r--  2.0 unx    11236 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_business_industry.py
+-rw-r--r--  2.0 unx    13971 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_contact.py
+-rw-r--r--  2.0 unx    12018 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_contact_people.py
+-rw-r--r--  2.0 unx    12691 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_size.py
+-rw-r--r--  2.0 unx    11613 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_size_ev.py
+-rw-r--r--  2.0 unx    11862 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_size_revenue.py
+-rw-r--r--  2.0 unx    18324 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_stage.py
+-rw-r--r--  2.0 unx    11408 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_stage_crunchbase_rank.py
+-rw-r--r--  2.0 unx    11520 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_stage_pe_active_firms.py
+-rw-r--r--  2.0 unx    11987 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_stage_pevc_latest_post_money_valuation.py
+-rw-r--r--  2.0 unx    11731 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_data_stage_trade_date_range.py
+-rw-r--r--  2.0 unx    11594 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/profile_response.py
+-rw-r--r--  2.0 unx    11290 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/scale.py
+-rw-r--r--  2.0 unx    11104 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/scale_scale.py
+-rw-r--r--  2.0 unx    11101 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/sources.py
+-rw-r--r--  2.0 unx    11716 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/stach_table_response.py
+-rw-r--r--  2.0 unx    11472 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/transaction_id.py
+-rw-r--r--  2.0 unx    11152 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/transaction_id_transaction_id.py
+-rw-r--r--  2.0 unx    11516 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/transaction_type.py
+-rw-r--r--  2.0 unx    11285 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/transaction_type_transaction_type.py
+-rw-r--r--  2.0 unx    11384 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/value_type.py
+-rw-r--r--  2.0 unx    11291 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/model/value_type_value_type.py
+-rw-r--r--  2.0 unx    11861 b- defN 23-May-05 08:54 fds/sdk/OverviewReportBuilder/models/__init__.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-May-05 08:55 fds.sdk.OverviewReportBuilder-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    16019 b- defN 23-May-05 08:55 fds.sdk.OverviewReportBuilder-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 08:55 fds.sdk.OverviewReportBuilder-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-May-05 08:55 fds.sdk.OverviewReportBuilder-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    15614 b- defN 23-May-05 08:55 fds.sdk.OverviewReportBuilder-1.1.0.dist-info/RECORD
+128 files, 1649720 bytes uncompressed, 326087 bytes compressed:  80.2%
```

## zipnote {}

```diff
@@ -78,14 +78,194 @@
 
 Filename: fds/sdk/OverviewReportBuilder/model/frequency.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/frequency_frequency.py
 Comment: 
 
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_active_investors.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_average_daily_vol.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_average_daily_vol_value.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_average_rating.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_basic_shares.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_branches.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_broker_contributors.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_diluted_market_cap.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_diluted_shares.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_dividend_yield.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_employees.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_enterprise_value.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_estimated_vc_raised.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_first_date.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_first_date_value.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_first_funding.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_float.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_funding_rounds.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_gross_assets.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_gross_premiums.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_institutional.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_last_funding.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_latest_post_money_valuation.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_lt_growth_rate.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_market_cap.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_meta.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_meta_sources.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_net_interest_income.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_premiums.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_range52_week.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_range52_week_value.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_revenue.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_revenue_as_of_date.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_target_price.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_top10_institutional_holders.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_total_deposits.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_total_investors.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_wacc.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_aum_fund_month.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_aum_share_daily.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_available_for_sale.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_average_spread.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_currency_iso.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_daily_trading_vol.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_distribution_yield.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_esg_compliance.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_expense_ratio.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_expense_ratio_value.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_first_nav_record.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_fund_flow_ytd.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_inception_date_fund.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_inception_date_share.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_meta.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_meta_as_of_date.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_outstanding_share.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_sfdr_classification.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_object.py
+Comment: 
+
+Filename: fds/sdk/OverviewReportBuilder/model/key_stats_response.py
+Comment: 
+
 Filename: fds/sdk/OverviewReportBuilder/model/meta.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/metadata_entry.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/metric.py
@@ -126,65 +306,47 @@
 
 Filename: fds/sdk/OverviewReportBuilder/model/profile_data_contact_people.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/profile_data_size.py
 Comment: 
 
-Filename: fds/sdk/OverviewReportBuilder/model/profile_data_size_employee_number.py
-Comment: 
-
 Filename: fds/sdk/OverviewReportBuilder/model/profile_data_size_ev.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/profile_data_size_revenue.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/profile_data_stage.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/profile_data_stage_crunchbase_rank.py
 Comment: 
 
-Filename: fds/sdk/OverviewReportBuilder/model/profile_data_stage_pe_active_firm_number.py
-Comment: 
-
 Filename: fds/sdk/OverviewReportBuilder/model/profile_data_stage_pe_active_firms.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/profile_data_stage_pevc_latest_post_money_valuation.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/profile_data_stage_trade_date_range.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/profile_response.py
 Comment: 
 
-Filename: fds/sdk/OverviewReportBuilder/model/relevance_type.py
-Comment: 
-
-Filename: fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type.py
-Comment: 
-
-Filename: fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type_c.py
-Comment: 
-
-Filename: fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type_p.py
-Comment: 
-
-Filename: fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type_s.py
-Comment: 
-
 Filename: fds/sdk/OverviewReportBuilder/model/scale.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/scale_scale.py
 Comment: 
 
+Filename: fds/sdk/OverviewReportBuilder/model/sources.py
+Comment: 
+
 Filename: fds/sdk/OverviewReportBuilder/model/stach_table_response.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/transaction_id.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/model/transaction_id_transaction_id.py
@@ -201,23 +363,23 @@
 
 Filename: fds/sdk/OverviewReportBuilder/model/value_type_value_type.py
 Comment: 
 
 Filename: fds/sdk/OverviewReportBuilder/models/__init__.py
 Comment: 
 
-Filename: fds.sdk.OverviewReportBuilder-1.0.1.dist-info/LICENSE
+Filename: fds.sdk.OverviewReportBuilder-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: fds.sdk.OverviewReportBuilder-1.0.1.dist-info/METADATA
+Filename: fds.sdk.OverviewReportBuilder-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: fds.sdk.OverviewReportBuilder-1.0.1.dist-info/WHEEL
+Filename: fds.sdk.OverviewReportBuilder-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: fds.sdk.OverviewReportBuilder-1.0.1.dist-info/top_level.txt
+Filename: fds.sdk.OverviewReportBuilder-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fds.sdk.OverviewReportBuilder-1.0.1.dist-info/RECORD
+Filename: fds.sdk.OverviewReportBuilder-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fds/sdk/OverviewReportBuilder/__init__.py

```diff
@@ -1,20 +1,21 @@
 # flake8: noqa
 
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 
 # import ApiClient
 from fds.sdk.OverviewReportBuilder.api_client import ApiClient
 
 # import Configuration
 from fds.sdk.OverviewReportBuilder.configuration import Configuration
```

## fds/sdk/OverviewReportBuilder/api_client.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -101,15 +102,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'fds-sdk/python/OverviewReportBuilder/1.0.1'
+        self.user_agent = 'fds-sdk/python/OverviewReportBuilder/1.1.0'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

## fds/sdk/OverviewReportBuilder/configuration.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -416,16 +417,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.1".\
+               "Version of the API: 1.2.0\n"\
+               "SDK Package Version: 1.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

## fds/sdk/OverviewReportBuilder/exceptions.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

## fds/sdk/OverviewReportBuilder/model_utils.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

## fds/sdk/OverviewReportBuilder/rest.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

## fds/sdk/OverviewReportBuilder/api/company_api.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 from multiprocessing.pool import ApplyResult
@@ -21,14 +22,15 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiException
 from fds.sdk.OverviewReportBuilder.model.error_response import ErrorResponse
+from fds.sdk.OverviewReportBuilder.model.key_stats_response import KeyStatsResponse
 from fds.sdk.OverviewReportBuilder.model.peer_list_response import PeerListResponse
 from fds.sdk.OverviewReportBuilder.model.profile_response import ProfileResponse
 from fds.sdk.OverviewReportBuilder.model.stach_table_response import StachTableResponse
 
 
 
 
@@ -115,14 +117,16 @@
                 'operation_id': 'financial_highlights_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
+                    'actual',
+                    'estimate',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -134,20 +138,28 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
+                    'actual':
+                        (int,),
+                    'estimate':
+                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
+                    'actual': 'actual',
+                    'estimate': 'estimate',
                 },
                 'location_map': {
                     'id': 'query',
+                    'actual': 'query',
+                    'estimate': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -209,14 +221,70 @@
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
+        self.key_stats_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (
+                  { 200: (KeyStatsResponse,), 400: (ErrorResponse,), 404: (ErrorResponse,),  },
+                  None
+                ),
+                'auth': [
+                    'FactSetApiKey',
+                    'FactSetOAuth2'
+                ],
+                'endpoint_path': '/key-stats',
+                'operation_id': 'key_stats_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
         self.peer_list_get_endpoint = _Endpoint(
             settings={
                 'response_type': (
                   { 200: (PeerListResponse,), 400: (ErrorResponse,), 404: (ErrorResponse,),  },
                   None
                 ),
                 'auth': [
@@ -318,15 +386,17 @@
                         "MINORITY_STAKE": "MINORITY_STAKE",
                         "SPINOFF": "SPINOFF",
                         "IPO": "IPO",
                         "FOLLOW_ON": "FOLLOW_ON",
                         "ST_DEBT": "ST_DEBT",
                         "NOTES_BONDS": "NOTES_BONDS",
                         "REVOLVING_CREDIT": "REVOLVING_CREDIT",
-                        "TERM_LOANS": "TERM_LOANS"
+                        "TERM_LOANS": "TERM_LOANS",
+                        "PEVC_INVESTMENTS": "PEVC_INVESTMENTS",
+                        "FUNDING": "FUNDING"
                     },
                     ('financing_type',): {
 
                         "DEBT": "DEBT",
                         "EQUITY": "EQUITY"
                     },
                 },
@@ -566,14 +636,16 @@
 
         This method makes a synchronous HTTP request. Returns the http data only
 
         Args:
             id (str): Company ticker
 
         Keyword Args:
+            actual (int): The number of actual data periods to be returned. Must be greater than 0. [optional] if omitted the server will use the default value of 4
+            estimate (int): The number of estimate data periods to be returned. Must be greater than 0. [optional] if omitted the server will use the default value of 1
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -611,14 +683,16 @@
 
         This method makes a synchronous HTTP request. Returns http data, http status and headers
 
         Args:
             id (str): Company ticker
 
         Keyword Args:
+            actual (int): The number of actual data periods to be returned. Must be greater than 0. [optional] if omitted the server will use the default value of 4
+            estimate (int): The number of estimate data periods to be returned. Must be greater than 0. [optional] if omitted the server will use the default value of 1
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -660,14 +734,16 @@
 
         This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
 
         Args:
             id (str): Company ticker
 
         Keyword Args:
+            actual (int): The number of actual data periods to be returned. Must be greater than 0. [optional] if omitted the server will use the default value of 4
+            estimate (int): The number of estimate data periods to be returned. Must be greater than 0. [optional] if omitted the server will use the default value of 1
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -704,14 +780,16 @@
 
         This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
 
         Args:
             id (str): Company ticker
 
         Keyword Args:
+            actual (int): The number of actual data periods to be returned. Must be greater than 0. [optional] if omitted the server will use the default value of 4
+            estimate (int): The number of estimate data periods to be returned. Must be greater than 0. [optional] if omitted the server will use the default value of 1
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -919,14 +997,197 @@
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
         kwargs['id'] = \
             id
         return self.get_profile_profile_endpoint.call_with_http_info(**kwargs)
 
 
+    def key_stats_get(
+        self,
+        id,
+        **kwargs
+    ) -> KeyStatsResponse:
+        """Key Stats  # noqa: E501
+
+        This method makes a synchronous HTTP request. Returns the http data only
+
+        Args:
+            id (str): Company ticker
+
+        Keyword Args:
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            KeyStatsResponse
+                Response Object
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
+        kwargs['id'] = \
+            id
+        return self.key_stats_get_endpoint.call_with_http_info(**kwargs)
+
+    def key_stats_get_with_http_info(
+        self,
+        id,
+        **kwargs
+    ) -> typing.Tuple[KeyStatsResponse, int, typing.MutableMapping]:
+        """Key Stats  # noqa: E501
+
+        This method makes a synchronous HTTP request. Returns http data, http status and headers
+
+        Args:
+            id (str): Company ticker
+
+        Keyword Args:
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            KeyStatsResponse
+                Response Object
+            int
+                Http Status Code
+            dict
+                Dictionary of the response headers
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
+        kwargs['id'] = \
+            id
+        return self.key_stats_get_endpoint.call_with_http_info(**kwargs)
+
+    def key_stats_get_async(
+        self,
+        id,
+        **kwargs
+    ) -> "ApplyResult[KeyStatsResponse]":
+        """Key Stats  # noqa: E501
+
+        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
+
+        Args:
+            id (str): Company ticker
+
+        Keyword Args:
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[KeyStatsResponse]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
+        kwargs['id'] = \
+            id
+        return self.key_stats_get_endpoint.call_with_http_info(**kwargs)
+
+    def key_stats_get_with_http_info_async(
+        self,
+        id,
+        **kwargs
+    ) -> "ApplyResult[typing.Tuple[KeyStatsResponse, int, typing.MutableMapping]]":
+        """Key Stats  # noqa: E501
+
+        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
+
+        Args:
+            id (str): Company ticker
+
+        Keyword Args:
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[(KeyStatsResponse, int, typing.Dict)]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
+        kwargs['id'] = \
+            id
+        return self.key_stats_get_endpoint.call_with_http_info(**kwargs)
+
+
     def peer_list_get(
         self,
         id,
         **kwargs
     ) -> PeerListResponse:
         """Peer List  # noqa: E501
```

## fds/sdk/OverviewReportBuilder/model/category.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/category_category.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/currency_code.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/currency_code_currency_code.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/currency_symbol.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/currency_symbol_currency_symbol.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/data_point_meta.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/data_point_meta_any_of.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/description.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/description_description.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/error_object.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/error_object_links.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/error_object_source.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/error_response.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/frequency.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/frequency_frequency.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/meta.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/metadata_entry.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -38,18 +39,17 @@
     from fds.sdk.OverviewReportBuilder.model.currency_symbol_currency_symbol import CurrencySymbolCurrencySymbol
     from fds.sdk.OverviewReportBuilder.model.description import Description
     from fds.sdk.OverviewReportBuilder.model.description_description import DescriptionDescription
     from fds.sdk.OverviewReportBuilder.model.frequency import Frequency
     from fds.sdk.OverviewReportBuilder.model.frequency_frequency import FrequencyFrequency
     from fds.sdk.OverviewReportBuilder.model.metric import Metric
     from fds.sdk.OverviewReportBuilder.model.metric_metric import MetricMetric
-    from fds.sdk.OverviewReportBuilder.model.relevance_type import RelevanceType
-    from fds.sdk.OverviewReportBuilder.model.relevance_type_relevance_type import RelevanceTypeRelevanceType
     from fds.sdk.OverviewReportBuilder.model.scale import Scale
     from fds.sdk.OverviewReportBuilder.model.scale_scale import ScaleScale
+    from fds.sdk.OverviewReportBuilder.model.sources import Sources
     from fds.sdk.OverviewReportBuilder.model.transaction_id import TransactionId
     from fds.sdk.OverviewReportBuilder.model.transaction_id_transaction_id import TransactionIdTransactionId
     from fds.sdk.OverviewReportBuilder.model.transaction_type import TransactionType
     from fds.sdk.OverviewReportBuilder.model.transaction_type_transaction_type import TransactionTypeTransactionType
     from fds.sdk.OverviewReportBuilder.model.value_type import ValueType
     from fds.sdk.OverviewReportBuilder.model.value_type_value_type import ValueTypeValueType
     globals()['Category'] = Category
@@ -60,18 +60,17 @@
     globals()['CurrencySymbolCurrencySymbol'] = CurrencySymbolCurrencySymbol
     globals()['Description'] = Description
     globals()['DescriptionDescription'] = DescriptionDescription
     globals()['Frequency'] = Frequency
     globals()['FrequencyFrequency'] = FrequencyFrequency
     globals()['Metric'] = Metric
     globals()['MetricMetric'] = MetricMetric
-    globals()['RelevanceType'] = RelevanceType
-    globals()['RelevanceTypeRelevanceType'] = RelevanceTypeRelevanceType
     globals()['Scale'] = Scale
     globals()['ScaleScale'] = ScaleScale
+    globals()['Sources'] = Sources
     globals()['TransactionId'] = TransactionId
     globals()['TransactionIdTransactionId'] = TransactionIdTransactionId
     globals()['TransactionType'] = TransactionType
     globals()['TransactionTypeTransactionType'] = TransactionTypeTransactionType
     globals()['ValueType'] = ValueType
     globals()['ValueTypeValueType'] = ValueTypeValueType
 
@@ -131,16 +130,16 @@
         return {
             'category': (CategoryCategory,),  # noqa: E501
             'currency_code': (CurrencyCodeCurrencyCode,),  # noqa: E501
             'currency_symbol': (CurrencySymbolCurrencySymbol,),  # noqa: E501
             'description': (DescriptionDescription,),  # noqa: E501
             'frequency': (FrequencyFrequency,),  # noqa: E501
             'metric': (MetricMetric,),  # noqa: E501
-            'relevance_type': (RelevanceTypeRelevanceType,),  # noqa: E501
             'scale': (ScaleScale,),  # noqa: E501
+            'value': ([str],),  # noqa: E501
             'transaction_id': (TransactionIdTransactionId,),  # noqa: E501
             'transaction_type': (TransactionTypeTransactionType,),  # noqa: E501
             'value_type': (ValueTypeValueType,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -150,16 +149,16 @@
     attribute_map = {
         'category': 'category',  # noqa: E501
         'currency_code': 'currencyCode',  # noqa: E501
         'currency_symbol': 'currencySymbol',  # noqa: E501
         'description': 'description',  # noqa: E501
         'frequency': 'frequency',  # noqa: E501
         'metric': 'metric',  # noqa: E501
-        'relevance_type': 'relevanceType',  # noqa: E501
         'scale': 'scale',  # noqa: E501
+        'value': 'value',  # noqa: E501
         'transaction_id': 'transactionId',  # noqa: E501
         'transaction_type': 'transactionType',  # noqa: E501
         'value_type': 'valueType',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -202,16 +201,16 @@
                                 _visited_composed_classes = (Animal,)
             category (CategoryCategory): [optional]  # noqa: E501
             currency_code (CurrencyCodeCurrencyCode): [optional]  # noqa: E501
             currency_symbol (CurrencySymbolCurrencySymbol): [optional]  # noqa: E501
             description (DescriptionDescription): [optional]  # noqa: E501
             frequency (FrequencyFrequency): [optional]  # noqa: E501
             metric (MetricMetric): [optional]  # noqa: E501
-            relevance_type (RelevanceTypeRelevanceType): [optional]  # noqa: E501
             scale (ScaleScale): [optional]  # noqa: E501
+            value ([str]): [optional]  # noqa: E501
             transaction_id (TransactionIdTransactionId): [optional]  # noqa: E501
             transaction_type (TransactionTypeTransactionType): [optional]  # noqa: E501
             value_type (ValueTypeValueType): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -312,16 +311,16 @@
                                 _visited_composed_classes = (Animal,)
             category (CategoryCategory): [optional]  # noqa: E501
             currency_code (CurrencyCodeCurrencyCode): [optional]  # noqa: E501
             currency_symbol (CurrencySymbolCurrencySymbol): [optional]  # noqa: E501
             description (DescriptionDescription): [optional]  # noqa: E501
             frequency (FrequencyFrequency): [optional]  # noqa: E501
             metric (MetricMetric): [optional]  # noqa: E501
-            relevance_type (RelevanceTypeRelevanceType): [optional]  # noqa: E501
             scale (ScaleScale): [optional]  # noqa: E501
+            value ([str]): [optional]  # noqa: E501
             transaction_id (TransactionIdTransactionId): [optional]  # noqa: E501
             transaction_type (TransactionTypeTransactionType): [optional]  # noqa: E501
             value_type (ValueTypeValueType): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -390,14 +389,14 @@
           'oneOf': [
               Category,
               CurrencyCode,
               CurrencySymbol,
               Description,
               Frequency,
               Metric,
-              RelevanceType,
               Scale,
+              Sources,
               TransactionId,
               TransactionType,
               ValueType,
           ],
         }
```

## fds/sdk/OverviewReportBuilder/model/metric.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/metric_metric.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/peer_list_data.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -79,39 +80,42 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
+            'ticker': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'ticker': 'ticker',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, name, ticker, *args, **kwargs):  # noqa: E501
         """PeerListData - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            id (str): The FactSet Entity ID of the peer
+            name (str): The name of the peer
+            ticker (str): The ticker of the peer
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,14 +169,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.name = name
+        self.ticker = ticker
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,20 +190,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, name, ticker, *args, **kwargs):  # noqa: E501
         """PeerListData - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            id (str): The FactSet Entity ID of the peer
+            name (str): The name of the peer
+            ticker (str): The ticker of the peer
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -250,14 +256,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.name = name
+        self.ticker = ticker
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

## fds/sdk/OverviewReportBuilder/model/peer_list_object.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +27,17 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_meta import KeyStatsEntityObjectMeta
     from fds.sdk.OverviewReportBuilder.model.peer_list_data import PeerListData
+    globals()['KeyStatsEntityObjectMeta'] = KeyStatsEntityObjectMeta
     globals()['PeerListData'] = PeerListData
 
 
 class PeerListObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -84,23 +87,25 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'peers': ([PeerListData],),  # noqa: E501
+            'meta': (KeyStatsEntityObjectMeta,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'peers': 'peers',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -139,14 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            meta (KeyStatsEntityObjectMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -224,14 +230,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            meta (KeyStatsEntityObjectMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/OverviewReportBuilder/model/peer_list_response.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,18 +27,20 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_meta import KeyStatsEntityObjectMeta
     from fds.sdk.OverviewReportBuilder.model.profile_data_business import ProfileDataBusiness
     from fds.sdk.OverviewReportBuilder.model.profile_data_contact import ProfileDataContact
     from fds.sdk.OverviewReportBuilder.model.profile_data_size import ProfileDataSize
     from fds.sdk.OverviewReportBuilder.model.profile_data_stage import ProfileDataStage
+    globals()['KeyStatsEntityObjectMeta'] = KeyStatsEntityObjectMeta
     globals()['ProfileDataBusiness'] = ProfileDataBusiness
     globals()['ProfileDataContact'] = ProfileDataContact
     globals()['ProfileDataSize'] = ProfileDataSize
     globals()['ProfileDataStage'] = ProfileDataStage
 
 
 class ProfileData(ModelNormal):
@@ -93,26 +96,28 @@
         """
         lazy_import()
         return {
             'business': (ProfileDataBusiness,),  # noqa: E501
             'contact': (ProfileDataContact,),  # noqa: E501
             'size': (ProfileDataSize,),  # noqa: E501
             'stage': (ProfileDataStage,),  # noqa: E501
+            'meta': (KeyStatsEntityObjectMeta,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'business': 'business',  # noqa: E501
         'contact': 'contact',  # noqa: E501
         'size': 'size',  # noqa: E501
         'stage': 'stage',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -154,14 +159,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            meta (KeyStatsEntityObjectMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -245,14 +251,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            meta (KeyStatsEntityObjectMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/OverviewReportBuilder/model/profile_data_business.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_business_crunchbase_categories.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_business_crunchbase_url.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_business_description.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_business_industry.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_contact.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_contact_people.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_size.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,18 +27,18 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.OverviewReportBuilder.model.profile_data_size_employee_number import ProfileDataSizeEmployeeNumber
+    from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_expense_ratio_value import KeyStatsFundObjectExpenseRatioValue
     from fds.sdk.OverviewReportBuilder.model.profile_data_size_ev import ProfileDataSizeEv
     from fds.sdk.OverviewReportBuilder.model.profile_data_size_revenue import ProfileDataSizeRevenue
-    globals()['ProfileDataSizeEmployeeNumber'] = ProfileDataSizeEmployeeNumber
+    globals()['KeyStatsFundObjectExpenseRatioValue'] = KeyStatsFundObjectExpenseRatioValue
     globals()['ProfileDataSizeEv'] = ProfileDataSizeEv
     globals()['ProfileDataSizeRevenue'] = ProfileDataSizeRevenue
 
 
 class ProfileDataSize(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -87,15 +88,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'employee_number': (ProfileDataSizeEmployeeNumber,),  # noqa: E501
+            'employee_number': (KeyStatsFundObjectExpenseRatioValue,),  # noqa: E501
             'ev': (ProfileDataSizeEv,),  # noqa: E501
             'mcap': (ProfileDataSizeEv,),  # noqa: E501
             'revenue': (ProfileDataSizeRevenue,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -116,15 +117,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, employee_number, ev, mcap, revenue, *args, **kwargs):  # noqa: E501
         """ProfileDataSize - a model defined in OpenAPI
 
         Args:
-            employee_number (ProfileDataSizeEmployeeNumber):
+            employee_number (KeyStatsFundObjectExpenseRatioValue):
             ev (ProfileDataSizeEv):
             mcap (ProfileDataSizeEv):
             revenue (ProfileDataSizeRevenue):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -207,15 +208,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, employee_number, ev, mcap, revenue, *args, **kwargs):  # noqa: E501
         """ProfileDataSize - a model defined in OpenAPI
 
         Args:
-            employee_number (ProfileDataSizeEmployeeNumber):
+            employee_number (KeyStatsFundObjectExpenseRatioValue):
             ev (ProfileDataSizeEv):
             mcap (ProfileDataSizeEv):
             revenue (ProfileDataSizeRevenue):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
```

## fds/sdk/OverviewReportBuilder/model/profile_data_size_ev.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_size_revenue.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_stage.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,25 +27,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_average_daily_vol_value import KeyStatsEntityObjectAverageDailyVolValue
     from fds.sdk.OverviewReportBuilder.model.profile_data_business_industry import ProfileDataBusinessIndustry
     from fds.sdk.OverviewReportBuilder.model.profile_data_size_ev import ProfileDataSizeEv
     from fds.sdk.OverviewReportBuilder.model.profile_data_stage_crunchbase_rank import ProfileDataStageCrunchbaseRank
-    from fds.sdk.OverviewReportBuilder.model.profile_data_stage_pe_active_firm_number import ProfileDataStagePeActiveFirmNumber
     from fds.sdk.OverviewReportBuilder.model.profile_data_stage_pe_active_firms import ProfileDataStagePeActiveFirms
     from fds.sdk.OverviewReportBuilder.model.profile_data_stage_pevc_latest_post_money_valuation import ProfileDataStagePevcLatestPostMoneyValuation
     from fds.sdk.OverviewReportBuilder.model.profile_data_stage_trade_date_range import ProfileDataStageTradeDateRange
+    globals()['KeyStatsEntityObjectAverageDailyVolValue'] = KeyStatsEntityObjectAverageDailyVolValue
     globals()['ProfileDataBusinessIndustry'] = ProfileDataBusinessIndustry
     globals()['ProfileDataSizeEv'] = ProfileDataSizeEv
     globals()['ProfileDataStageCrunchbaseRank'] = ProfileDataStageCrunchbaseRank
-    globals()['ProfileDataStagePeActiveFirmNumber'] = ProfileDataStagePeActiveFirmNumber
     globals()['ProfileDataStagePeActiveFirms'] = ProfileDataStagePeActiveFirms
     globals()['ProfileDataStagePevcLatestPostMoneyValuation'] = ProfileDataStagePevcLatestPostMoneyValuation
     globals()['ProfileDataStageTradeDateRange'] = ProfileDataStageTradeDateRange
 
 
 class ProfileDataStage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
@@ -100,23 +101,23 @@
         lazy_import()
         return {
             'exchange_primary': (ProfileDataBusinessIndustry,),  # noqa: E501
             'trade_date_range': (ProfileDataStageTradeDateRange,),  # noqa: E501
             'founded_year': (ProfileDataBusinessIndustry,),  # noqa: E501
             'pevc_backing': (ProfileDataBusinessIndustry,),  # noqa: E501
             'pevc_latest_post_money_valuation': (ProfileDataStagePevcLatestPostMoneyValuation,),  # noqa: E501
-            'pe_active_firm_number': (ProfileDataStagePeActiveFirmNumber,),  # noqa: E501
-            'pe_active_investment_number': (ProfileDataStagePeActiveFirmNumber,),  # noqa: E501
+            'pe_active_firm_number': (KeyStatsEntityObjectAverageDailyVolValue,),  # noqa: E501
+            'pe_active_investment_number': (KeyStatsEntityObjectAverageDailyVolValue,),  # noqa: E501
             'pe_last_investment_date': (ProfileDataBusinessIndustry,),  # noqa: E501
             'pe_active_firms': ([ProfileDataStagePeActiveFirms],),  # noqa: E501
             'pe_active_acq_date': (ProfileDataBusinessIndustry,),  # noqa: E501
             'pe_active_acq_amt': (ProfileDataSizeEv,),  # noqa: E501
             'vc_last_round': (ProfileDataBusinessIndustry,),  # noqa: E501
             'vc_last_round_amt': (ProfileDataSizeEv,),  # noqa: E501
-            'vc_last_round_investor_number': (ProfileDataStagePeActiveFirmNumber,),  # noqa: E501
+            'vc_last_round_investor_number': (KeyStatsEntityObjectAverageDailyVolValue,),  # noqa: E501
             'vc_last_round_date': (ProfileDataBusinessIndustry,),  # noqa: E501
             'vc_total_est_raised': (ProfileDataSizeEv,),  # noqa: E501
             'crunchbase_rank': (ProfileDataStageCrunchbaseRank,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -187,23 +188,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             pevc_latest_post_money_valuation (ProfileDataStagePevcLatestPostMoneyValuation): [optional]  # noqa: E501
-            pe_active_firm_number (ProfileDataStagePeActiveFirmNumber): [optional]  # noqa: E501
-            pe_active_investment_number (ProfileDataStagePeActiveFirmNumber): [optional]  # noqa: E501
+            pe_active_firm_number (KeyStatsEntityObjectAverageDailyVolValue): [optional]  # noqa: E501
+            pe_active_investment_number (KeyStatsEntityObjectAverageDailyVolValue): [optional]  # noqa: E501
             pe_last_investment_date (ProfileDataBusinessIndustry): [optional]  # noqa: E501
             pe_active_firms ([ProfileDataStagePeActiveFirms]): [optional]  # noqa: E501
             pe_active_acq_date (ProfileDataBusinessIndustry): [optional]  # noqa: E501
             pe_active_acq_amt (ProfileDataSizeEv): [optional]  # noqa: E501
             vc_last_round (ProfileDataBusinessIndustry): [optional]  # noqa: E501
             vc_last_round_amt (ProfileDataSizeEv): [optional]  # noqa: E501
-            vc_last_round_investor_number (ProfileDataStagePeActiveFirmNumber): [optional]  # noqa: E501
+            vc_last_round_investor_number (KeyStatsEntityObjectAverageDailyVolValue): [optional]  # noqa: E501
             vc_last_round_date (ProfileDataBusinessIndustry): [optional]  # noqa: E501
             vc_total_est_raised (ProfileDataSizeEv): [optional]  # noqa: E501
             crunchbase_rank (ProfileDataStageCrunchbaseRank): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -291,23 +292,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             pevc_latest_post_money_valuation (ProfileDataStagePevcLatestPostMoneyValuation): [optional]  # noqa: E501
-            pe_active_firm_number (ProfileDataStagePeActiveFirmNumber): [optional]  # noqa: E501
-            pe_active_investment_number (ProfileDataStagePeActiveFirmNumber): [optional]  # noqa: E501
+            pe_active_firm_number (KeyStatsEntityObjectAverageDailyVolValue): [optional]  # noqa: E501
+            pe_active_investment_number (KeyStatsEntityObjectAverageDailyVolValue): [optional]  # noqa: E501
             pe_last_investment_date (ProfileDataBusinessIndustry): [optional]  # noqa: E501
             pe_active_firms ([ProfileDataStagePeActiveFirms]): [optional]  # noqa: E501
             pe_active_acq_date (ProfileDataBusinessIndustry): [optional]  # noqa: E501
             pe_active_acq_amt (ProfileDataSizeEv): [optional]  # noqa: E501
             vc_last_round (ProfileDataBusinessIndustry): [optional]  # noqa: E501
             vc_last_round_amt (ProfileDataSizeEv): [optional]  # noqa: E501
-            vc_last_round_investor_number (ProfileDataStagePeActiveFirmNumber): [optional]  # noqa: E501
+            vc_last_round_investor_number (KeyStatsEntityObjectAverageDailyVolValue): [optional]  # noqa: E501
             vc_last_round_date (ProfileDataBusinessIndustry): [optional]  # noqa: E501
             vc_total_est_raised (ProfileDataSizeEv): [optional]  # noqa: E501
             crunchbase_rank (ProfileDataStageCrunchbaseRank): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

## fds/sdk/OverviewReportBuilder/model/profile_data_stage_crunchbase_rank.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_stage_pe_active_firms.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_stage_pevc_latest_post_money_valuation.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_data_stage_trade_date_range.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/profile_response.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/scale.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/scale_scale.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/stach_table_response.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/transaction_id.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/transaction_id_transaction_id.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/transaction_type.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/transaction_type_transaction_type.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/value_type.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/model/value_type_value_type.py

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/OverviewReportBuilder/models/__init__.py

```diff
@@ -21,14 +21,74 @@
 from fds.sdk.OverviewReportBuilder.model.description_description import DescriptionDescription
 from fds.sdk.OverviewReportBuilder.model.error_object import ErrorObject
 from fds.sdk.OverviewReportBuilder.model.error_object_links import ErrorObjectLinks
 from fds.sdk.OverviewReportBuilder.model.error_object_source import ErrorObjectSource
 from fds.sdk.OverviewReportBuilder.model.error_response import ErrorResponse
 from fds.sdk.OverviewReportBuilder.model.frequency import Frequency
 from fds.sdk.OverviewReportBuilder.model.frequency_frequency import FrequencyFrequency
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object import KeyStatsEntityObject
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_active_investors import KeyStatsEntityObjectActiveInvestors
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_average_daily_vol import KeyStatsEntityObjectAverageDailyVol
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_average_daily_vol_value import KeyStatsEntityObjectAverageDailyVolValue
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_average_rating import KeyStatsEntityObjectAverageRating
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_basic_shares import KeyStatsEntityObjectBasicShares
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_branches import KeyStatsEntityObjectBranches
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_broker_contributors import KeyStatsEntityObjectBrokerContributors
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_diluted_market_cap import KeyStatsEntityObjectDilutedMarketCap
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_diluted_shares import KeyStatsEntityObjectDilutedShares
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_dividend_yield import KeyStatsEntityObjectDividendYield
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_employees import KeyStatsEntityObjectEmployees
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_enterprise_value import KeyStatsEntityObjectEnterpriseValue
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_estimated_vc_raised import KeyStatsEntityObjectEstimatedVcRaised
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_first_date import KeyStatsEntityObjectFirstDate
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_first_date_value import KeyStatsEntityObjectFirstDateValue
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_first_funding import KeyStatsEntityObjectFirstFunding
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_float import KeyStatsEntityObjectFloat
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_funding_rounds import KeyStatsEntityObjectFundingRounds
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_gross_assets import KeyStatsEntityObjectGrossAssets
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_gross_premiums import KeyStatsEntityObjectGrossPremiums
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_institutional import KeyStatsEntityObjectInstitutional
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_last_funding import KeyStatsEntityObjectLastFunding
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_latest_post_money_valuation import KeyStatsEntityObjectLatestPostMoneyValuation
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_lt_growth_rate import KeyStatsEntityObjectLtGrowthRate
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_market_cap import KeyStatsEntityObjectMarketCap
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_meta import KeyStatsEntityObjectMeta
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_meta_sources import KeyStatsEntityObjectMetaSources
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_net_interest_income import KeyStatsEntityObjectNetInterestIncome
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_premiums import KeyStatsEntityObjectPremiums
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_range52_week import KeyStatsEntityObjectRange52Week
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_range52_week_value import KeyStatsEntityObjectRange52WeekValue
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_revenue import KeyStatsEntityObjectRevenue
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_revenue_as_of_date import KeyStatsEntityObjectRevenueAsOfDate
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_target_price import KeyStatsEntityObjectTargetPrice
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_top10_institutional_holders import KeyStatsEntityObjectTop10InstitutionalHolders
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_total_deposits import KeyStatsEntityObjectTotalDeposits
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_total_investors import KeyStatsEntityObjectTotalInvestors
+from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_wacc import KeyStatsEntityObjectWacc
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object import KeyStatsFundObject
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_aum_fund_month import KeyStatsFundObjectAumFundMonth
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_aum_share_daily import KeyStatsFundObjectAumShareDaily
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_available_for_sale import KeyStatsFundObjectAvailableForSale
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_average_spread import KeyStatsFundObjectAverageSpread
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_currency_iso import KeyStatsFundObjectCurrencyIso
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_daily_trading_vol import KeyStatsFundObjectDailyTradingVol
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_distribution_yield import KeyStatsFundObjectDistributionYield
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_esg_compliance import KeyStatsFundObjectEsgCompliance
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_expense_ratio import KeyStatsFundObjectExpenseRatio
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_expense_ratio_value import KeyStatsFundObjectExpenseRatioValue
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_first_nav_record import KeyStatsFundObjectFirstNavRecord
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_fund_flow_ytd import KeyStatsFundObjectFundFlowYTD
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_inception_date_fund import KeyStatsFundObjectInceptionDateFund
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_inception_date_share import KeyStatsFundObjectInceptionDateShare
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_meta import KeyStatsFundObjectMeta
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_meta_as_of_date import KeyStatsFundObjectMetaAsOfDate
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_outstanding_share import KeyStatsFundObjectOutstandingShare
+from fds.sdk.OverviewReportBuilder.model.key_stats_fund_object_sfdr_classification import KeyStatsFundObjectSfdrClassification
+from fds.sdk.OverviewReportBuilder.model.key_stats_object import KeyStatsObject
+from fds.sdk.OverviewReportBuilder.model.key_stats_response import KeyStatsResponse
 from fds.sdk.OverviewReportBuilder.model.meta import Meta
 from fds.sdk.OverviewReportBuilder.model.metadata_entry import MetadataEntry
 from fds.sdk.OverviewReportBuilder.model.metric import Metric
 from fds.sdk.OverviewReportBuilder.model.metric_metric import MetricMetric
 from fds.sdk.OverviewReportBuilder.model.peer_list_data import PeerListData
 from fds.sdk.OverviewReportBuilder.model.peer_list_object import PeerListObject
 from fds.sdk.OverviewReportBuilder.model.peer_list_response import PeerListResponse
@@ -37,31 +97,25 @@
 from fds.sdk.OverviewReportBuilder.model.profile_data_business_crunchbase_categories import ProfileDataBusinessCrunchbaseCategories
 from fds.sdk.OverviewReportBuilder.model.profile_data_business_crunchbase_url import ProfileDataBusinessCrunchbaseUrl
 from fds.sdk.OverviewReportBuilder.model.profile_data_business_description import ProfileDataBusinessDescription
 from fds.sdk.OverviewReportBuilder.model.profile_data_business_industry import ProfileDataBusinessIndustry
 from fds.sdk.OverviewReportBuilder.model.profile_data_contact import ProfileDataContact
 from fds.sdk.OverviewReportBuilder.model.profile_data_contact_people import ProfileDataContactPeople
 from fds.sdk.OverviewReportBuilder.model.profile_data_size import ProfileDataSize
-from fds.sdk.OverviewReportBuilder.model.profile_data_size_employee_number import ProfileDataSizeEmployeeNumber
 from fds.sdk.OverviewReportBuilder.model.profile_data_size_ev import ProfileDataSizeEv
 from fds.sdk.OverviewReportBuilder.model.profile_data_size_revenue import ProfileDataSizeRevenue
 from fds.sdk.OverviewReportBuilder.model.profile_data_stage import ProfileDataStage
 from fds.sdk.OverviewReportBuilder.model.profile_data_stage_crunchbase_rank import ProfileDataStageCrunchbaseRank
-from fds.sdk.OverviewReportBuilder.model.profile_data_stage_pe_active_firm_number import ProfileDataStagePeActiveFirmNumber
 from fds.sdk.OverviewReportBuilder.model.profile_data_stage_pe_active_firms import ProfileDataStagePeActiveFirms
 from fds.sdk.OverviewReportBuilder.model.profile_data_stage_pevc_latest_post_money_valuation import ProfileDataStagePevcLatestPostMoneyValuation
 from fds.sdk.OverviewReportBuilder.model.profile_data_stage_trade_date_range import ProfileDataStageTradeDateRange
 from fds.sdk.OverviewReportBuilder.model.profile_response import ProfileResponse
-from fds.sdk.OverviewReportBuilder.model.relevance_type import RelevanceType
-from fds.sdk.OverviewReportBuilder.model.relevance_type_relevance_type import RelevanceTypeRelevanceType
-from fds.sdk.OverviewReportBuilder.model.relevance_type_relevance_type_c import RelevanceTypeRelevanceTypeC
-from fds.sdk.OverviewReportBuilder.model.relevance_type_relevance_type_p import RelevanceTypeRelevanceTypeP
-from fds.sdk.OverviewReportBuilder.model.relevance_type_relevance_type_s import RelevanceTypeRelevanceTypeS
 from fds.sdk.OverviewReportBuilder.model.scale import Scale
 from fds.sdk.OverviewReportBuilder.model.scale_scale import ScaleScale
+from fds.sdk.OverviewReportBuilder.model.sources import Sources
 from fds.sdk.OverviewReportBuilder.model.stach_table_response import StachTableResponse
 from fds.sdk.OverviewReportBuilder.model.transaction_id import TransactionId
 from fds.sdk.OverviewReportBuilder.model.transaction_id_transaction_id import TransactionIdTransactionId
 from fds.sdk.OverviewReportBuilder.model.transaction_type import TransactionType
 from fds.sdk.OverviewReportBuilder.model.transaction_type_transaction_type import TransactionTypeTransactionType
 from fds.sdk.OverviewReportBuilder.model.value_type import ValueType
 from fds.sdk.OverviewReportBuilder.model.value_type_value_type import ValueTypeValueType
```

## Comparing `fds/sdk/OverviewReportBuilder/model/profile_data_size_employee_number.py` & `fds/sdk/OverviewReportBuilder/model/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
 
-class ProfileDataSizeEmployeeNumber(ModelNormal):
+class Sources(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,15 +78,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (float, none_type,),  # noqa: E501
+            'value': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -96,19 +97,16 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, value, *args, **kwargs):  # noqa: E501
-        """ProfileDataSizeEmployeeNumber - a model defined in OpenAPI
-
-        Args:
-            value (float, none_type):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Sources - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,14 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            value ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -160,15 +159,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -181,19 +179,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, value, *args, **kwargs):  # noqa: E501
-        """ProfileDataSizeEmployeeNumber - a model defined in OpenAPI
-
-        Args:
-            value (float, none_type):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Sources - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -218,14 +213,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            value ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -243,15 +239,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

## Comparing `fds/sdk/OverviewReportBuilder/model/profile_data_stage_pe_active_firm_number.py` & `fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_range52_week_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
 
-class ProfileDataStagePeActiveFirmNumber(ModelNormal):
+class KeyStatsEntityObjectRange52WeekValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,15 +78,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (float,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -97,18 +98,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, value, *args, **kwargs):  # noqa: E501
-        """ProfileDataStagePeActiveFirmNumber - a model defined in OpenAPI
+        """KeyStatsEntityObjectRange52WeekValue - a model defined in OpenAPI
 
         Args:
-            value (float):
+            value (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,18 +183,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, value, *args, **kwargs):  # noqa: E501
-        """ProfileDataStagePeActiveFirmNumber - a model defined in OpenAPI
+        """KeyStatsEntityObjectRange52WeekValue - a model defined in OpenAPI
 
         Args:
-            value (float):
+            value (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

## Comparing `fds/sdk/OverviewReportBuilder/model/relevance_type.py` & `fds/sdk/OverviewReportBuilder/model/key_stats_fund_object_meta_as_of_date.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fds.sdk.OverviewReportBuilder.model.relevance_type_relevance_type import RelevanceTypeRelevanceType
-    globals()['RelevanceTypeRelevanceType'] = RelevanceTypeRelevanceType
 
-
-class RelevanceType(ModelNormal):
+class KeyStatsFundObjectMetaAsOfDate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,52 +63,50 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'relevance_type': (RelevanceTypeRelevanceType,),  # noqa: E501
+            'value': ([date],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'relevance_type': 'relevanceType',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelevanceType - a model defined in OpenAPI
+        """KeyStatsFundObjectMetaAsOfDate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            relevance_type (RelevanceTypeRelevanceType): [optional]  # noqa: E501
+            value ([date]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelevanceType - a model defined in OpenAPI
+        """KeyStatsFundObjectMetaAsOfDate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -218,15 +213,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            relevance_type (RelevanceTypeRelevanceType): [optional]  # noqa: E501
+            value ([date]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type.py` & `fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_average_daily_vol_value.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,24 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fds.sdk.OverviewReportBuilder.model.relevance_type_relevance_type_c import RelevanceTypeRelevanceTypeC
-    from fds.sdk.OverviewReportBuilder.model.relevance_type_relevance_type_p import RelevanceTypeRelevanceTypeP
-    from fds.sdk.OverviewReportBuilder.model.relevance_type_relevance_type_s import RelevanceTypeRelevanceTypeS
-    globals()['RelevanceTypeRelevanceTypeC'] = RelevanceTypeRelevanceTypeC
-    globals()['RelevanceTypeRelevanceTypeP'] = RelevanceTypeRelevanceTypeP
-    globals()['RelevanceTypeRelevanceTypeS'] = RelevanceTypeRelevanceTypeS
 
-
-class RelevanceTypeRelevanceType(ModelNormal):
+class KeyStatsEntityObjectAverageDailyVolValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -70,56 +63,53 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'c': (RelevanceTypeRelevanceTypeC,),  # noqa: E501
-            'p': (RelevanceTypeRelevanceTypeP,),  # noqa: E501
-            's': (RelevanceTypeRelevanceTypeS,),  # noqa: E501
+            'value': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'c': 'C',  # noqa: E501
-        'p': 'P',  # noqa: E501
-        's': 'S',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelevanceTypeRelevanceType - a model defined in OpenAPI
+    def _from_openapi_data(cls, value, *args, **kwargs):  # noqa: E501
+        """KeyStatsEntityObjectAverageDailyVolValue - a model defined in OpenAPI
+
+        Args:
+            value (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,17 +134,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            c (RelevanceTypeRelevanceTypeC): [optional]  # noqa: E501
-            p (RelevanceTypeRelevanceTypeP): [optional]  # noqa: E501
-            s (RelevanceTypeRelevanceTypeS): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -174,14 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -194,16 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelevanceTypeRelevanceType - a model defined in OpenAPI
+    def __init__(self, value, *args, **kwargs):  # noqa: E501
+        """KeyStatsEntityObjectAverageDailyVolValue - a model defined in OpenAPI
+
+        Args:
+            value (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +219,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            c (RelevanceTypeRelevanceTypeC): [optional]  # noqa: E501
-            p (RelevanceTypeRelevanceTypeP): [optional]  # noqa: E501
-            s (RelevanceTypeRelevanceTypeS): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,14 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

## Comparing `fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type_c.py` & `fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_revenue_as_of_date.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
 
-class RelevanceTypeRelevanceTypeC(ModelNormal):
+class KeyStatsEntityObjectRevenueAsOfDate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,15 +78,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),  # noqa: E501
+            'value': (date,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -96,16 +97,19 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelevanceTypeRelevanceTypeC - a model defined in OpenAPI
+    def _from_openapi_data(cls, value, *args, **kwargs):  # noqa: E501
+        """KeyStatsEntityObjectRevenueAsOfDate - a model defined in OpenAPI
+
+        Args:
+            value (date):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +134,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str): [optional] if omitted the server will use the default value of "Customer"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -158,14 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -178,16 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelevanceTypeRelevanceTypeC - a model defined in OpenAPI
+    def __init__(self, value, *args, **kwargs):  # noqa: E501
+        """KeyStatsEntityObjectRevenueAsOfDate - a model defined in OpenAPI
+
+        Args:
+            value (date):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -212,15 +219,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str): [optional] if omitted the server will use the default value of "Customer"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -238,14 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

## Comparing `fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type_p.py` & `fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_first_date_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
 
-class RelevanceTypeRelevanceTypeP(ModelNormal):
+class KeyStatsEntityObjectFirstDateValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,15 +78,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),  # noqa: E501
+            'value': (date,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -96,16 +97,19 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelevanceTypeRelevanceTypeP - a model defined in OpenAPI
+    def _from_openapi_data(cls, value, *args, **kwargs):  # noqa: E501
+        """KeyStatsEntityObjectFirstDateValue - a model defined in OpenAPI
+
+        Args:
+            value (date): Date formatted to YYYY-MM-DD
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +134,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str): [optional] if omitted the server will use the default value of "Partner"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -158,14 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -178,16 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelevanceTypeRelevanceTypeP - a model defined in OpenAPI
+    def __init__(self, value, *args, **kwargs):  # noqa: E501
+        """KeyStatsEntityObjectFirstDateValue - a model defined in OpenAPI
+
+        Args:
+            value (date): Date formatted to YYYY-MM-DD
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -212,15 +219,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str): [optional] if omitted the server will use the default value of "Partner"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -238,14 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

## Comparing `fds/sdk/OverviewReportBuilder/model/relevance_type_relevance_type_s.py` & `fds/sdk/OverviewReportBuilder/model/key_stats_entity_object_net_interest_income.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     FactSet Overview Report Builder API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    Get relevant industry-specific data for high level analysis of public and private companies  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.2.0
+    Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.OverviewReportBuilder.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fds.sdk.OverviewReportBuilder.model.key_stats_entity_object_range52_week_value import KeyStatsEntityObjectRange52WeekValue
+    globals()['KeyStatsEntityObjectRange52WeekValue'] = KeyStatsEntityObjectRange52WeekValue
 
-class RelevanceTypeRelevanceTypeS(ModelNormal):
+
+class KeyStatsEntityObjectNetInterestIncome(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,50 +67,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'value': (str,),  # noqa: E501
+            'value': (KeyStatsEntityObjectRange52WeekValue,),  # noqa: E501
+            'label': (KeyStatsEntityObjectRange52WeekValue,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'value': 'value',  # noqa: E501
+        'label': 'label',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelevanceTypeRelevanceTypeS - a model defined in OpenAPI
+    def _from_openapi_data(cls, value, label, *args, **kwargs):  # noqa: E501
+        """KeyStatsEntityObjectNetInterestIncome - a model defined in OpenAPI
+
+        Args:
+            value (KeyStatsEntityObjectRange52WeekValue):
+            label (KeyStatsEntityObjectRange52WeekValue):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +143,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str): [optional] if omitted the server will use the default value of "Supplier"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -158,14 +170,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.value = value
+        self.label = label
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -178,16 +192,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelevanceTypeRelevanceTypeS - a model defined in OpenAPI
+    def __init__(self, value, label, *args, **kwargs):  # noqa: E501
+        """KeyStatsEntityObjectNetInterestIncome - a model defined in OpenAPI
+
+        Args:
+            value (KeyStatsEntityObjectRange52WeekValue):
+            label (KeyStatsEntityObjectRange52WeekValue):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -212,15 +230,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str): [optional] if omitted the server will use the default value of "Supplier"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -238,14 +255,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.value = value
+        self.label = label
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

## Comparing `fds.sdk.OverviewReportBuilder-1.0.1.dist-info/LICENSE` & `fds.sdk.OverviewReportBuilder-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

