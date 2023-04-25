# Comparing `tmp/signal-ocean-5.0.0.tar.gz` & `tmp/signal-ocean-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-ocean-5.0.0.tar", last modified: Fri Apr  7 11:45:04 2023, max compression
+gzip compressed data, was "signal-ocean-5.1.0.tar", last modified: Tue Apr 25 11:14:18 2023, max compression
```

## Comparing `signal-ocean-5.0.0.tar` & `signal-ocean-5.1.0.tar`

### file list

```diff
@@ -1,145 +1,146 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.788798 signal-ocean-5.0.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2175 2023-04-07 11:45:04.788798 signal-ocean-5.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1184 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-07 11:45:04.792799 signal-ocean-5.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1524 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.776798 signal-ocean-5.0.0/signal_ocean/
--rw-r--r--   0 root         (0) root         (0)     1151 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/_internals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.776798 signal-ocean-5.0.0/signal_ocean/companies/
--rw-r--r--   0 root         (0) root         (0)      236 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/companies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/companies/companies_api.py
--rw-r--r--   0 root         (0) root         (0)     3020 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/companies/models.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.780798 signal-ocean-5.0.0/signal_ocean/distances/
--rw-r--r--   0 root         (0) root         (0)     1210 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/distances/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/distances/_distances_json.py
--rw-r--r--   0 root         (0) root         (0)    11714 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/distances/distances_api.py
--rw-r--r--   0 root         (0) root         (0)      287 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/distances/loading_condition.py
--rw-r--r--   0 root         (0) root         (0)     4589 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/distances/models.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/distances/port.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/distances/port_filter.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/distances/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/distances/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.780798 signal-ocean-5.0.0/signal_ocean/freight_pricing/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/_freight_pricing_json.py
--rw-r--r--   0 root         (0) root         (0)     4766 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/freight_pricing_api.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/models.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/port.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/port_filter.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/vessel_class_filter.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/vessel_subclass.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/vessel_type.py
--rw-r--r--   0 root         (0) root         (0)      877 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_pricing/vessel_type_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.780798 signal-ocean-5.0.0/signal_ocean/freight_rates/
--rw-r--r--   0 root         (0) root         (0)      565 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_rates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_rates/_freight_rates_json.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_rates/enums.py
--rw-r--r--   0 root         (0) root         (0)     3750 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_rates/freight_rates_api.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_rates/models.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_rates/port_filter.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/freight_rates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.780798 signal-ocean-5.0.0/signal_ocean/geos/
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/geos/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4286 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/geos/geos_api.py
--rw-r--r--   0 root         (0) root         (0)     5991 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/geos/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.784798 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/
--rw-r--r--   0 root         (0) root         (0)     2261 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/area.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/column.py
--rw-r--r--   0 root         (0) root         (0)      675 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/commercial_status.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/fixture_type.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
--rw-r--r--   0 root         (0) root         (0)     4968 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/index_level.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/location_taxonomy.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/market_deployment.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/operational_status.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/push_type.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/tonnage_list.py
--rw-r--r--   0 root         (0) root         (0)     5517 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/vessel.py
--rw-r--r--   0 root         (0) root         (0)     6831 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/vessel_filter.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/vessel_subclass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.784798 signal-ocean-5.0.0/signal_ocean/market_rates/
--rw-r--r--   0 root         (0) root         (0)      536 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/market_rates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/market_rates/_market_rates_json.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/market_rates/enums.py
--rw-r--r--   0 root         (0) root         (0)     4006 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/market_rates/market_rates_api.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/market_rates/models.py
--rw-r--r--   0 root         (0) root         (0)      773 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/market_rates/utils.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/market_rates/vessel_classes.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/plots.py
--rw-r--r--   0 root         (0) root         (0)      578 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.784798 signal-ocean-5.0.0/signal_ocean/port_congestion/
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_congestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_congestion/models.py
--rw-r--r--   0 root         (0) root         (0)    18934 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_congestion/port_congestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.784798 signal-ocean-5.0.0/signal_ocean/port_expenses/
--rw-r--r--   0 root         (0) root         (0)     1026 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_expenses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_expenses/_port_expenses_json.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_expenses/enums.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_expenses/models.py
--rw-r--r--   0 root         (0) root         (0)     8626 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_expenses/port_expenses_api.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_expenses/port_filter.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/port_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.784798 signal-ocean-5.0.0/signal_ocean/scraped_cargoes/
--rw-r--r--   0 root         (0) root         (0)      277 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_cargoes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26586 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_cargoes/models.py
--rw-r--r--   0 root         (0) root         (0)     5363 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.784798 signal-ocean-5.0.0/signal_ocean/scraped_data/
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4560 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_data/scraped_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.784798 signal-ocean-5.0.0/signal_ocean/scraped_fixtures/
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32666 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_fixtures/models.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.784798 signal-ocean-5.0.0/signal_ocean/scraped_lineups/
--rw-r--r--   0 root         (0) root         (0)      281 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_lineups/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21114 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_lineups/models.py
--rw-r--r--   0 root         (0) root         (0)     5968 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_lineups/scraped_lineups_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.788798 signal-ocean-5.0.0/signal_ocean/scraped_positions/
--rw-r--r--   0 root         (0) root         (0)      301 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_positions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16973 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_positions/models.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/scraped_positions/scraped_positions_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.788798 signal-ocean-5.0.0/signal_ocean/tonnage_list/
--rw-r--r--   0 root         (0) root         (0)      879 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/tonnage_list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/tonnage_list/_json.py
--rw-r--r--   0 root         (0) root         (0)     6084 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/tonnage_list/api.py
--rw-r--r--   0 root         (0) root         (0)     7229 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/tonnage_list/data_frame.py
--rw-r--r--   0 root         (0) root         (0)    26447 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/tonnage_list/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.788798 signal-ocean-5.0.0/signal_ocean/util/
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6480 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/util/parsing_helpers.py
--rw-r--r--   0 root         (0) root         (0)     6529 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/util/request_helpers.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessel_class_api.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.788798 signal-ocean-5.0.0/signal_ocean/vessel_valuations/
--rw-r--r--   0 root         (0) root         (0)      298 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessel_valuations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessel_valuations/_valuation_json.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessel_valuations/models.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessel_valuations/vessel_valuations_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.788798 signal-ocean-5.0.0/signal_ocean/vessels/
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessels/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16264 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessels/models.py
--rw-r--r--   0 root         (0) root         (0)     3207 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/vessels/vessels_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.788798 signal-ocean-5.0.0/signal_ocean/voyages/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/voyages/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46003 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/voyages/models.py
--rw-r--r--   0 root         (0) root         (0)    44702 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/voyages/voyages_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.788798 signal-ocean-5.0.0/signal_ocean/voyages_market_data/
--rw-r--r--   0 root         (0) root         (0)      539 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/voyages_market_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15350 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/voyages_market_data/models.py
--rw-r--r--   0 root         (0) root         (0)    15865 2023-04-07 11:44:12.000000 signal-ocean-5.0.0/signal_ocean/voyages_market_data/voyages_market_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:45:04.776798 signal-ocean-5.0.0/signal_ocean.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2175 2023-04-07 11:45:04.000000 signal-ocean-5.0.0/signal_ocean.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4893 2023-04-07 11:45:04.000000 signal-ocean-5.0.0/signal_ocean.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 11:45:04.000000 signal-ocean-5.0.0/signal_ocean.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-04-07 11:45:04.000000 signal-ocean-5.0.0/signal_ocean.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 11:45:04.000000 signal-ocean-5.0.0/signal_ocean.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.253399 signal-ocean-5.1.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-04-25 11:14:18.253399 signal-ocean-5.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 11:14:18.253399 signal-ocean-5.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.241398 signal-ocean-5.1.0/signal_ocean/
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/_internals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.241398 signal-ocean-5.1.0/signal_ocean/companies/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/companies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/companies/companies_api.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/companies/models.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.241398 signal-ocean-5.1.0/signal_ocean/distances/
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/distances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/distances/_distances_json.py
+-rw-r--r--   0 root         (0) root         (0)    11714 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/distances/distances_api.py
+-rw-r--r--   0 root         (0) root         (0)      287 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/distances/loading_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4589 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/distances/models.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/distances/port.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/distances/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/distances/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/distances/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.241398 signal-ocean-5.1.0/signal_ocean/freight_pricing/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/_freight_pricing_json.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/freight_pricing_api.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/models.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/port.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/vessel_class_filter.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/vessel_subclass.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/vessel_type.py
+-rw-r--r--   0 root         (0) root         (0)      877 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_pricing/vessel_type_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.241398 signal-ocean-5.1.0/signal_ocean/freight_rates/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_rates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_rates/_freight_rates_json.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_rates/enums.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_rates/freight_rates_api.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_rates/models.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_rates/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/freight_rates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.245398 signal-ocean-5.1.0/signal_ocean/geos/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/geos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/geos/geos_api.py
+-rw-r--r--   0 root         (0) root         (0)     5991 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/geos/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.245398 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
+-rw-r--r--   0 root         (0) root         (0)      331 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/area.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/column.py
+-rw-r--r--   0 root         (0) root         (0)      675 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/commercial_status.py
+-rw-r--r--   0 root         (0) root         (0)      235 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/fixture_type.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
+-rw-r--r--   0 root         (0) root         (0)     4968 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/index_level.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/location_taxonomy.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/market_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/operational_status.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/push_type.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/tonnage_list.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/vessel.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/vessel_filter.py
+-rw-r--r--   0 root         (0) root         (0)      632 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/vessel_subclass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.245398 signal-ocean-5.1.0/signal_ocean/market_rates/
+-rw-r--r--   0 root         (0) root         (0)      536 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/market_rates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/market_rates/_market_rates_json.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/market_rates/enums.py
+-rw-r--r--   0 root         (0) root         (0)     4006 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/market_rates/market_rates_api.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/market_rates/models.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/market_rates/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/market_rates/vessel_classes.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/plots.py
+-rw-r--r--   0 root         (0) root         (0)      578 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.245398 signal-ocean-5.1.0/signal_ocean/port_congestion/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_congestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_congestion/models.py
+-rw-r--r--   0 root         (0) root         (0)    19251 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_congestion/port_congestion.py
+-rw-r--r--   0 root         (0) root         (0)     4656 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_congestion/port_congestion_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.245398 signal-ocean-5.1.0/signal_ocean/port_expenses/
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_expenses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_expenses/_port_expenses_json.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_expenses/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_expenses/models.py
+-rw-r--r--   0 root         (0) root         (0)     8626 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_expenses/port_expenses_api.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_expenses/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/port_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/scraped_cargoes/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_cargoes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26586 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_cargoes/models.py
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/scraped_data/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_data/scraped_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/scraped_fixtures/
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32666 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_fixtures/models.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/scraped_lineups/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_lineups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21114 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_lineups/models.py
+-rw-r--r--   0 root         (0) root         (0)     5968 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_lineups/scraped_lineups_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/scraped_positions/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_positions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16973 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_positions/models.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/scraped_positions/scraped_positions_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/tonnage_list/
+-rw-r--r--   0 root         (0) root         (0)      879 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/tonnage_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/tonnage_list/_json.py
+-rw-r--r--   0 root         (0) root         (0)     6084 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/tonnage_list/api.py
+-rw-r--r--   0 root         (0) root         (0)     7229 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/tonnage_list/data_frame.py
+-rw-r--r--   0 root         (0) root         (0)    26447 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/tonnage_list/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/util/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6505 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/util/parsing_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6529 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/util/request_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      647 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessel_class_api.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/vessel_valuations/
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessel_valuations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessel_valuations/_valuation_json.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessel_valuations/models.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessel_valuations/vessel_valuations_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/vessels/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16264 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessels/models.py
+-rw-r--r--   0 root         (0) root         (0)     3207 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/vessels/vessels_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.249398 signal-ocean-5.1.0/signal_ocean/voyages/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/voyages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46003 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/voyages/models.py
+-rw-r--r--   0 root         (0) root         (0)    44702 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/voyages/voyages_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.253399 signal-ocean-5.1.0/signal_ocean/voyages_market_data/
+-rw-r--r--   0 root         (0) root         (0)      539 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/voyages_market_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15350 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/voyages_market_data/models.py
+-rw-r--r--   0 root         (0) root         (0)    15865 2023-04-25 11:13:07.000000 signal-ocean-5.1.0/signal_ocean/voyages_market_data/voyages_market_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:14:18.241398 signal-ocean-5.1.0/signal_ocean.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-04-25 11:14:18.000000 signal-ocean-5.1.0/signal_ocean.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-04-25 11:14:18.000000 signal-ocean-5.1.0/signal_ocean.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:14:18.000000 signal-ocean-5.1.0/signal_ocean.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2023-04-25 11:14:18.000000 signal-ocean-5.1.0/signal_ocean.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 11:14:18.000000 signal-ocean-5.1.0/signal_ocean.egg-info/top_level.txt
```

### Comparing `signal-ocean-5.0.0/LICENSE` & `signal-ocean-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/PKG-INFO` & `signal-ocean-5.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 5.0.0
+Version: 5.1.0
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-5.0.0/README.md` & `signal-ocean-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/setup.py` & `signal-ocean-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/__init__.py` & `signal-ocean-5.1.0/signal_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/_internals.py` & `signal-ocean-5.1.0/signal_ocean/_internals.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/companies/companies_api.py` & `signal-ocean-5.1.0/signal_ocean/companies/companies_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/companies/models.py` & `signal-ocean-5.1.0/signal_ocean/companies/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/connection.py` & `signal-ocean-5.1.0/signal_ocean/connection.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/distances/__init__.py` & `signal-ocean-5.1.0/signal_ocean/distances/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/distances/_distances_json.py` & `signal-ocean-5.1.0/signal_ocean/distances/_distances_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/distances/distances_api.py` & `signal-ocean-5.1.0/signal_ocean/distances/distances_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/distances/models.py` & `signal-ocean-5.1.0/signal_ocean/distances/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/distances/port_filter.py` & `signal-ocean-5.1.0/signal_ocean/distances/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/distances/vessel_class_filter.py` & `signal-ocean-5.1.0/signal_ocean/distances/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_pricing/__init__.py` & `signal-ocean-5.1.0/signal_ocean/freight_pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_pricing/_freight_pricing_json.py` & `signal-ocean-5.1.0/signal_ocean/freight_pricing/_freight_pricing_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_pricing/freight_pricing_api.py` & `signal-ocean-5.1.0/signal_ocean/freight_pricing/freight_pricing_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_pricing/models.py` & `signal-ocean-5.1.0/signal_ocean/freight_pricing/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_pricing/port_filter.py` & `signal-ocean-5.1.0/signal_ocean/freight_pricing/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_pricing/vessel_class_filter.py` & `signal-ocean-5.1.0/signal_ocean/freight_pricing/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_pricing/vessel_type_filter.py` & `signal-ocean-5.1.0/signal_ocean/freight_pricing/vessel_type_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_rates/__init__.py` & `signal-ocean-5.1.0/signal_ocean/freight_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_rates/_freight_rates_json.py` & `signal-ocean-5.1.0/signal_ocean/freight_rates/_freight_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_rates/enums.py` & `signal-ocean-5.1.0/signal_ocean/freight_rates/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_rates/freight_rates_api.py` & `signal-ocean-5.1.0/signal_ocean/freight_rates/freight_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_rates/models.py` & `signal-ocean-5.1.0/signal_ocean/freight_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_rates/port_filter.py` & `signal-ocean-5.1.0/signal_ocean/freight_rates/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/freight_rates/utils.py` & `signal-ocean-5.1.0/signal_ocean/freight_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/geos/geos_api.py` & `signal-ocean-5.1.0/signal_ocean/geos/geos_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/geos/models.py` & `signal-ocean-5.1.0/signal_ocean/geos/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/__init__.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/column.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/column.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/commercial_status.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/commercial_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/market_deployment.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/market_deployment.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/operational_status.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/operational_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/tonnage_list.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/vessel.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/vessel.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/vessel_filter.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/vessel_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/historical_tonnage_list/vessel_subclass.py` & `signal-ocean-5.1.0/signal_ocean/historical_tonnage_list/vessel_subclass.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/market_rates/__init__.py` & `signal-ocean-5.1.0/signal_ocean/market_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/market_rates/_market_rates_json.py` & `signal-ocean-5.1.0/signal_ocean/market_rates/_market_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/market_rates/market_rates_api.py` & `signal-ocean-5.1.0/signal_ocean/market_rates/market_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/market_rates/models.py` & `signal-ocean-5.1.0/signal_ocean/market_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/market_rates/utils.py` & `signal-ocean-5.1.0/signal_ocean/market_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/market_rates/vessel_classes.py` & `signal-ocean-5.1.0/signal_ocean/market_rates/vessel_classes.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/plots.py` & `signal-ocean-5.1.0/signal_ocean/plots.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/port.py` & `signal-ocean-5.1.0/signal_ocean/port.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/port_api.py` & `signal-ocean-5.1.0/signal_ocean/port_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/port_congestion/port_congestion.py` & `signal-ocean-5.1.0/signal_ocean/port_congestion/port_congestion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import date, datetime, timedelta
 from dateutil.relativedelta import relativedelta
 from typing import Optional, Tuple, List, cast
 from strictly_typed_pandas.dataset import DataSet
 from functools import reduce
 
 from signal_ocean import Connection
+from signal_ocean.port_congestion.port_congestion_api import PortCongestionAPI
 from signal_ocean.voyages import VoyagesAPI
 from signal_ocean.voyages.models import (
     Voyage,
     VoyageEvent,
     VoyageEventDetail,
     VoyageGeo,
     VoyagesFlat,
@@ -32,19 +33,18 @@
         """Initializes PortCongestion.
 
         Args:
             connection: API connection configuration. If not provided, the
                 default connection method is used.
         """
         self.__connection = connection or Connection()
+        self._port_congestion_api = PortCongestionAPI(self.__connection)
 
     def _get_voyages_data(
-        self,
-        voyages_start_date: date,
-        vessel_class_id: int,
+        self, voyages_start_date: date, vessel_class_id: int,
     ) -> Tuple[
         DataSet[Voyage],
         DataSet[VoyageEvent],
         DataSet[VoyageEventDetail],
         DataSet[VoyageGeo],
     ]:
         """Get Voyages Data to calculate port congestion.
@@ -154,17 +154,16 @@
             ports_filter = voyages_extd.port_name_geos.isin(ports)
             _filter = _filter & ports_filter
         elif areas and not ports:
             areas_filter = voyages_extd.area_name_level0_geos.isin(areas)
             _filter = _filter & areas_filter
         elif areas and ports:
             areas_ports_filter = (
-                (voyages_extd.area_name_level0_geos.isin(areas)) |
-                (voyages_extd.port_name_geos.isin(ports))
-            )
+                voyages_extd.area_name_level0_geos.isin(areas)
+            ) | (voyages_extd.port_name_geos.isin(ports))
             _filter = _filter & areas_ports_filter
         else:
             pass
 
         voyages_extd = voyages_extd[
             (voyages_extd["purpose"].isin(["Load", "Discharge"]))
             & (voyages_extd["event_detail_type"] != "StS")
@@ -372,17 +371,16 @@
             "mode",
             "geo_asset_name",
             "latitude",
             "longitude",
             "arrival_date",
         ]
 
-        vessels_congestion_data_datetimetz = (
-            vessels_congestion_data.select_dtypes("datetimetz")
-        )
+        vessels_congestion_data_datetimetz = vessels_congestion_data.\
+            select_dtypes("datetimetz")
         vessels_congestion_data[
             vessels_congestion_data_datetimetz.columns
         ] = vessels_congestion_data_datetimetz.apply(
             lambda x: x.dt.tz_convert(None), axis=0
         )
 
         vessels_congestion_data = cast(
@@ -391,15 +389,15 @@
                 vessels_congestion_data[
                     vessels_congestion_data.day_date.dt.date.between(
                         congestion_start_date, date.today()
                     )
                 ]
             )[wanted_columns]
             .copy()
-            .reset_index(drop=True)
+            .reset_index(drop=True),
         )
 
         return vessels_congestion_data
 
     def _calculate_number_of_vessels_over_time(
         self, vessels_congestion_data: DataSet[VesselsCongestionData]
     ) -> DataSet[NumberOfVesselsOverTime]:
@@ -408,72 +406,81 @@
         Args:
             VesselsCongestionData: The Dataset over which
                 port congestion will be calculated.
 
         Returns:
             NumberOfVesselsOverTime.
         """
-        num_of_vessels_time_series = cast(DataSet[NumberOfVesselsOverTime], (
-            vessels_congestion_data.groupby("day_date")["imo"]
-            .nunique()
-            .reset_index()
-        ))
+        num_of_vessels_time_series = cast(
+            DataSet[NumberOfVesselsOverTime],
+            (
+                vessels_congestion_data.groupby("day_date")["imo"]
+                .nunique()
+                .reset_index()
+            ),
+        )
 
         num_of_vessels_time_series.columns = ["date", "vessels"]  # type:ignore
 
         return num_of_vessels_time_series
 
-    def _calculate_waiting_time_over_time(
-        self, vessels_congestion_data: DataSet[VesselsCongestionData]
+    def _get_waiting_time_over_time(
+        self,
+        congestion_start_date: date,
+        vessel_class_id: int,
+        ports: Optional[List[str]] = None,
+        areas: Optional[List[str]] = None,
     ) -> DataSet[WaitingTimeOverTime]:
         """Generate waiting time time series.
 
         Args:
             VesselsCongestionData: The Dataset over which
                 port congestion will be calculated.
 
+        Raises:
+            RuntimeError: In case of Port Congestion API call failure.
+
         Returns:
             WaitingTimeOverTime.
         """
-        waiting_vessels = vessels_congestion_data[
-            (vessels_congestion_data["mode"] == "Waiting")
-            & (
-                vessels_congestion_data.waiting_time_start.dt.date
-                != vessels_congestion_data.day_date.dt.date
+        try:
+            ts_df = pd.DataFrame(
+                self._port_congestion_api.query_port_congestion(
+                    date_from=congestion_start_date,
+                    vessel_class_ids=[vessel_class_id],
+                    ports=ports,
+                    level_0_areas=areas,
+                )
             )
-        ].copy()
-
-        waiting_vessels["waiting_time"] = (
-            waiting_vessels["day_date"]  # .dt.tz_localize(None)
-            - waiting_vessels["waiting_time_start"]  # .dt.tz_localize(None)
-        ).dt.total_seconds() / (60 * 60 * 24.0)
+        except RuntimeError as exc:
+            raise exc
 
         waiting_time_df = (
-            waiting_vessels[
-                (waiting_vessels.waiting_time < 60)
-                & (waiting_vessels.day_date.dt.date != date.today())
-            ]
-            .groupby("day_date")["waiting_time"]
+            ts_df.rename(
+                columns={
+                    "observation_date": "date",
+                    "avg_wait_estimate": "avg_waiting_time",
+                }
+            )
+            .groupby("date")
             .mean()
             .reset_index()
-            .rename(columns={"waiting_time": "avg_waiting_time"})
-            .set_index("day_date")
+            .set_index("date")
         )
-
-        waiting_time_df.avg_waiting_time = (
-            waiting_time_df.avg_waiting_time.round(1)
+        waiting_time_df.avg_waiting_time = waiting_time_df.\
+            avg_waiting_time.round(1)
+        waiting_time_df.index = cast(
+            pd.Index, pd.to_datetime(waiting_time_df.index).tz_convert(None)
         )
+        waiting_time_df = waiting_time_df.reset_index()
 
-        all_days = pd.date_range(
-            waiting_time_df.index.min(), waiting_time_df.index.max(), freq="D"
+        return cast(
+            DataSet[WaitingTimeOverTime],
+            waiting_time_df[["date", "avg_waiting_time"]],
         )
-        waiting_time_df = waiting_time_df.reindex(all_days).reset_index()
-        waiting_time_df.columns = ['date', 'avg_waiting_time']
-
-        return cast(DataSet[WaitingTimeOverTime], waiting_time_df)
 
     def _calculate_live_port_congestion(
         self, vessels_congestion_data: DataSet[VesselsCongestionData]
     ) -> DataSet[LiveCongestion]:
         """Generate live port congestion DataFrame.
 
         Args:
@@ -491,21 +498,20 @@
             vessels_at_port_df.day_date - vessels_at_port_df["arrival_date"]
         ).dt.total_seconds() / (60 * 60 * 24.0)
 
         vessels_at_port_df.loc[
             vessels_at_port_df.days_at_port < 0, "days_at_port"
         ] = None
         return cast(
-            DataSet[LiveCongestion],
-            vessels_at_port_df.reset_index(drop=True)
+            DataSet[LiveCongestion], vessels_at_port_df.reset_index(drop=True)
         )
 
     def get_port_congestion(
         self,
-        congestion_start_date: datetime,
+        congestion_start_date: date,
         vessel_class_id: int,
         ports: Optional[List[str]] = None,
         areas: Optional[List[str]] = None,
     ) -> Tuple[
         DataSet[NumberOfVesselsOverTime],
         DataSet[WaitingTimeOverTime],
         DataSet[LiveCongestion],
@@ -542,27 +548,31 @@
             events_details_df,
             geos_df,
             congestion_start_date,
             ports,
             areas,
         )
 
-        number_of_vessels_over_time = (
-            self._calculate_number_of_vessels_over_time(
-                vessels_congestion_data
-            )
-        )
-
-        waiting_time_over_time = self._calculate_waiting_time_over_time(
+        num_of_vessels_over_time = self._calculate_number_of_vessels_over_time(
             vessels_congestion_data
         )
 
+        try:
+            waiting_time_over_time = self._get_waiting_time_over_time(
+                congestion_start_date, vessel_class_id, ports, areas
+            )
+        except RuntimeError:
+            waiting_time_over_time = cast(
+                DataSet[WaitingTimeOverTime],
+                {"date": congestion_start_date, "avg_waiting_time": 0.0}
+            )
+
         live_port_congestion = self._calculate_live_port_congestion(
             vessels_congestion_data
         )
 
         return (
-            number_of_vessels_over_time,
+            num_of_vessels_over_time,
             waiting_time_over_time,
             live_port_congestion,
             vessels_congestion_data,
         )
```

### Comparing `signal-ocean-5.0.0/signal_ocean/port_expenses/__init__.py` & `signal-ocean-5.1.0/signal_ocean/port_expenses/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/port_expenses/_port_expenses_json.py` & `signal-ocean-5.1.0/signal_ocean/port_expenses/_port_expenses_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/port_expenses/enums.py` & `signal-ocean-5.1.0/signal_ocean/port_expenses/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/port_expenses/models.py` & `signal-ocean-5.1.0/signal_ocean/port_expenses/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/port_expenses/port_expenses_api.py` & `signal-ocean-5.1.0/signal_ocean/port_expenses/port_expenses_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/port_expenses/port_filter.py` & `signal-ocean-5.1.0/signal_ocean/port_expenses/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/port_filter.py` & `signal-ocean-5.1.0/signal_ocean/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/scraped_cargoes/models.py` & `signal-ocean-5.1.0/signal_ocean/scraped_cargoes/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py` & `signal-ocean-5.1.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/scraped_data/scraped_data_api.py` & `signal-ocean-5.1.0/signal_ocean/scraped_data/scraped_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/scraped_fixtures/models.py` & `signal-ocean-5.1.0/signal_ocean/scraped_fixtures/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py` & `signal-ocean-5.1.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/scraped_lineups/models.py` & `signal-ocean-5.1.0/signal_ocean/scraped_lineups/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/scraped_lineups/scraped_lineups_api.py` & `signal-ocean-5.1.0/signal_ocean/scraped_lineups/scraped_lineups_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/scraped_positions/models.py` & `signal-ocean-5.1.0/signal_ocean/scraped_positions/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/scraped_positions/scraped_positions_api.py` & `signal-ocean-5.1.0/signal_ocean/scraped_positions/scraped_positions_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/tonnage_list/__init__.py` & `signal-ocean-5.1.0/signal_ocean/tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/tonnage_list/_json.py` & `signal-ocean-5.1.0/signal_ocean/tonnage_list/_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/tonnage_list/api.py` & `signal-ocean-5.1.0/signal_ocean/tonnage_list/api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/tonnage_list/data_frame.py` & `signal-ocean-5.1.0/signal_ocean/tonnage_list/data_frame.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/tonnage_list/models.py` & `signal-ocean-5.1.0/signal_ocean/tonnage_list/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/util/parsing_helpers.py` & `signal-ocean-5.1.0/signal_ocean/util/parsing_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,16 +160,16 @@
 
     if field_type_origin is Union:
         for candidate_cls in getattr(cls, '__args__', []):
             try:
                 return parse_model(
                     data, candidate_cls, rename_keys=rename_keys
                 )
-            except (TypeError, ValueError):
-                pass
+            except (TypeError, ValueError, NotImplementedError):
+                continue
 
         raise ValueError(f'Cannot parse value {data} as {cls}')
 
     if field_type_origin is list and isinstance(data, Iterable):
         list_field_type = getattr(cls, '__args__', [])[0]
         if type(list_field_type) is TypeVar:
             return list(data)
```

### Comparing `signal-ocean-5.0.0/signal_ocean/util/request_helpers.py` & `signal-ocean-5.1.0/signal_ocean/util/request_helpers.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/vessel_class.py` & `signal-ocean-5.1.0/signal_ocean/vessel_class.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/vessel_class_api.py` & `signal-ocean-5.1.0/signal_ocean/vessel_class_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/vessel_class_filter.py` & `signal-ocean-5.1.0/signal_ocean/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/vessel_valuations/_valuation_json.py` & `signal-ocean-5.1.0/signal_ocean/vessel_valuations/_valuation_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/vessel_valuations/models.py` & `signal-ocean-5.1.0/signal_ocean/vessel_valuations/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/vessel_valuations/vessel_valuations_api.py` & `signal-ocean-5.1.0/signal_ocean/vessel_valuations/vessel_valuations_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/vessels/models.py` & `signal-ocean-5.1.0/signal_ocean/vessels/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/vessels/vessels_api.py` & `signal-ocean-5.1.0/signal_ocean/vessels/vessels_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/voyages/__init__.py` & `signal-ocean-5.1.0/signal_ocean/voyages/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/voyages/models.py` & `signal-ocean-5.1.0/signal_ocean/voyages/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/voyages/voyages_api.py` & `signal-ocean-5.1.0/signal_ocean/voyages/voyages_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/voyages_market_data/__init__.py` & `signal-ocean-5.1.0/signal_ocean/voyages_market_data/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/voyages_market_data/models.py` & `signal-ocean-5.1.0/signal_ocean/voyages_market_data/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean/voyages_market_data/voyages_market_data_api.py` & `signal-ocean-5.1.0/signal_ocean/voyages_market_data/voyages_market_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-5.0.0/signal_ocean.egg-info/PKG-INFO` & `signal-ocean-5.1.0/signal_ocean.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 5.0.0
+Version: 5.1.0
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-5.0.0/signal_ocean.egg-info/SOURCES.txt` & `signal-ocean-5.1.0/signal_ocean.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 signal_ocean/market_rates/market_rates_api.py
 signal_ocean/market_rates/models.py
 signal_ocean/market_rates/utils.py
 signal_ocean/market_rates/vessel_classes.py
 signal_ocean/port_congestion/__init__.py
 signal_ocean/port_congestion/models.py
 signal_ocean/port_congestion/port_congestion.py
+signal_ocean/port_congestion/port_congestion_api.py
 signal_ocean/port_expenses/__init__.py
 signal_ocean/port_expenses/_port_expenses_json.py
 signal_ocean/port_expenses/enums.py
 signal_ocean/port_expenses/models.py
 signal_ocean/port_expenses/port_expenses_api.py
 signal_ocean/port_expenses/port_filter.py
 signal_ocean/scraped_cargoes/__init__.py
```

