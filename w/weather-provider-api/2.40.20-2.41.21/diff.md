# Comparing `tmp/weather_provider_api-2.40.20.tar.gz` & `tmp/weather_provider_api-2.41.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_provider_api-2.40.20.tar", max compression
+gzip compressed data, was "weather_provider_api-2.41.21.tar", max compression
```

## Comparing `weather_provider_api-2.40.20.tar` & `weather_provider_api-2.41.21.tar`

### file list

```diff
@@ -1,81 +1,80 @@
--rw-r--r--   0        0        0    17098 2023-02-15 11:06:49.177032 weather_provider_api-2.40.20/LICENSE
-drwxr-xr-x   0        0        0        0 2023-02-15 11:06:49.177032 weather_provider_api-2.40.20/LICENSES/
--rw-r--r--   0        0        0    11816 2023-02-15 11:06:49.177032 weather_provider_api-2.40.20/README.md
--rw-r--r--   0        0        0     1882 2023-02-15 11:07:41.045421 weather_provider_api-2.40.20/pyproject.toml
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.181032 weather_provider_api-2.40.20/weather_provider_api/__init__.py
--rw-r--r--   0        0        0     3704 2023-02-15 11:06:49.181032 weather_provider_api-2.40.20/weather_provider_api/app_config.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/__init__.py
--rw-r--r--   0        0        0      280 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/base_model.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/errors/__init__.py
--rw-r--r--   0        0        0      268 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/errors/additional_responses.py
--rw-r--r--   0        0        0      278 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/errors/api_models.py
--rw-r--r--   0        0        0      503 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/errors/exceptions.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/initializers/__init__.py
--rw-r--r--   0        0        0      975 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/initializers/error_handling.py
--rw-r--r--   0        0        0     1375 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/initializers/headers.py
--rw-r--r--   0        0        0     2174 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/initializers/logging.py
--rw-r--r--   0        0        0      790 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/initializers/monitoring.py
--rw-r--r--   0        0        0      924 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/initializers/mounting.py
--rw-r--r--   0        0        0      303 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/initializers/rate_limiter.py
--rw-r--r--   0        0        0      988 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/initializers/validation.py
--rw-r--r--   0        0        0      274 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/core/views.py
--rw-r--r--   0        0        0     2815 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/main.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/__init__.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/__init__.py
--rw-r--r--   0        0        0     6430 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/api_models.py
--rw-r--r--   0        0        0     5806 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/api_view_v1.py
--rw-r--r--   0        0        0     9450 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/api_view_v2.py
--rw-r--r--   0        0        0       91 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/base_models/__init__.py
--rw-r--r--   0        0        0     5846 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/base_models/model.py
--rw-r--r--   0        0        0     1141 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/base_models/source.py
--rw-r--r--   0        0        0     6686 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/controller.py
--rw-r--r--   0        0        0      726 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/exceptions.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/repository/__init__.py
--rw-r--r--   0        0        0    14715 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/repository/repository.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/__init__.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/__init__.py
--rw-r--r--   0        0        0      656 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/cds.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/client/__init__.py
--rw-r--r--   0        0        0    13650 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/client/downloader.py
--rw-r--r--   0        0        0     6490 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
--rw-r--r--   0        0        0     6932 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
--rw-r--r--   0        0        0    15478 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
--rw-r--r--   0        0        0      591 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/factors.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/models/__init__.py
--rw-r--r--   0        0        0     8855 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/models/era5land.py
--rw-r--r--   0        0        0     7972 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/__init__.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
--rw-r--r--   0        0        0    24157 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
--rw-r--r--   0        0        0     9343 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
--rw-r--r--   0        0        0     1258 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/knmi.py
--rw-r--r--   0        0        0      415 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
--rw-r--r--   0        0        0    10462 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
--rw-r--r--   0        0        0    15043 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
--rw-r--r--   0        0        0     4265 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
--rw-r--r--   0        0        0    11316 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
--rw-r--r--   0        0        0    13406 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
--rw-r--r--   0        0        0    19917 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/stations.py
--rw-r--r--   0        0        0     2085 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/utils.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
--rw-r--r--   0        0        0     5148 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/__init__.py
--rw-r--r--   0        0        0     4240 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/date_helpers.py
--rw-r--r--   0        0        0     1472 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/file_helpers.py
--rw-r--r--   0        0        0     5742 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/geo_position.py
--rw-r--r--   0        0        0     1791 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/grid_helpers.py
--rw-r--r--   0        0        0      447 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/pandas_helpers.py
--rw-r--r--   0        0        0     5052 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/serializers.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/scripts/__init__.py
--rw-r--r--   0        0        0      393 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/scripts/erase_arome_repository.py
--rw-r--r--   0        0        0      413 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/scripts/erase_era5land_repository.py
--rw-r--r--   0        0        0      381 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/scripts/erase_era5sl_repository.py
--rw-r--r--   0        0        0      383 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/scripts/update_arome_repository.py
--rw-r--r--   0        0        0      401 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/scripts/update_era5land_repository.py
--rw-r--r--   0        0        0      371 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/scripts/update_era5sl_repository.py
--rw-r--r--   0        0        0      140 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/versions/__init__.py
--rw-r--r--   0        0        0      469 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/versions/v1.py
--rw-r--r--   0        0        0      469 2023-02-15 11:06:49.185032 weather_provider_api-2.40.20/weather_provider_api/versions/v2.py
--rw-r--r--   0        0        0    14762 1970-01-01 00:00:00.000000 weather_provider_api-2.40.20/setup.py
--rw-r--r--   0        0        0    13006 1970-01-01 00:00:00.000000 weather_provider_api-2.40.20/PKG-INFO
+-rw-r--r--   0        0        0    17098 2023-04-25 06:11:11.020151 weather_provider_api-2.41.21/LICENSE
+drwxr-xr-x   0        0        0        0 2023-04-25 06:11:11.020151 weather_provider_api-2.41.21/LICENSES/
+-rw-r--r--   0        0        0    11816 2023-04-25 06:11:11.024152 weather_provider_api-2.41.21/README.md
+-rw-r--r--   0        0        0     1905 2023-04-25 06:11:39.924658 weather_provider_api-2.41.21/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/__init__.py
+-rw-r--r--   0        0        0     3704 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/app_config.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/__init__.py
+-rw-r--r--   0        0        0      280 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/base_model.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/errors/__init__.py
+-rw-r--r--   0        0        0      268 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/errors/additional_responses.py
+-rw-r--r--   0        0        0      278 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/errors/api_models.py
+-rw-r--r--   0        0        0      503 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/errors/exceptions.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/__init__.py
+-rw-r--r--   0        0        0      975 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/error_handling.py
+-rw-r--r--   0        0        0     1375 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/headers.py
+-rw-r--r--   0        0        0     2174 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/logging.py
+-rw-r--r--   0        0        0      790 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/monitoring.py
+-rw-r--r--   0        0        0      924 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/mounting.py
+-rw-r--r--   0        0        0      303 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/rate_limiter.py
+-rw-r--r--   0        0        0      988 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/initializers/validation.py
+-rw-r--r--   0        0        0      274 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/core/views.py
+-rw-r--r--   0        0        0     2815 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/main.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/__init__.py
+-rw-r--r--   0        0        0     6492 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_models.py
+-rw-r--r--   0        0        0     5806 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_view_v1.py
+-rw-r--r--   0        0        0     9693 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_view_v2.py
+-rw-r--r--   0        0        0       91 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/__init__.py
+-rw-r--r--   0        0        0     5846 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/model.py
+-rw-r--r--   0        0        0     1141 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/source.py
+-rw-r--r--   0        0        0     6686 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/controller.py
+-rw-r--r--   0        0        0      726 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/exceptions.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/repository/__init__.py
+-rw-r--r--   0        0        0    14715 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/repository/repository.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/__init__.py
+-rw-r--r--   0        0        0      656 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/cds.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/__init__.py
+-rw-r--r--   0        0        0    13650 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/downloader.py
+-rw-r--r--   0        0        0     6490 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
+-rw-r--r--   0        0        0     6932 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
+-rw-r--r--   0        0        0    15478 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
+-rw-r--r--   0        0        0      591 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/factors.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/__init__.py
+-rw-r--r--   0        0        0     8855 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/era5land.py
+-rw-r--r--   0        0        0     7972 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
+-rw-r--r--   0        0        0    24157 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
+-rw-r--r--   0        0        0     9343 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
+-rw-r--r--   0        0        0     1258 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/knmi.py
+-rw-r--r--   0        0        0      415 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
+-rw-r--r--   0        0        0    10462 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
+-rw-r--r--   0        0        0    15043 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
+-rw-r--r--   0        0        0     4265 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
+-rw-r--r--   0        0        0    11316 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
+-rw-r--r--   0        0        0    13406 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
+-rw-r--r--   0        0        0    19917 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/stations.py
+-rw-r--r--   0        0        0     2085 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/utils.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
+-rw-r--r--   0        0        0     5148 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.028154 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/__init__.py
+-rw-r--r--   0        0        0     4240 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/date_helpers.py
+-rw-r--r--   0        0        0     1472 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/file_helpers.py
+-rw-r--r--   0        0        0     5742 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/geo_position.py
+-rw-r--r--   0        0        0     1791 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/grid_helpers.py
+-rw-r--r--   0        0        0      447 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/pandas_helpers.py
+-rw-r--r--   0        0        0     5052 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/serializers.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/__init__.py
+-rw-r--r--   0        0        0      393 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/erase_arome_repository.py
+-rw-r--r--   0        0        0      413 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/erase_era5land_repository.py
+-rw-r--r--   0        0        0      381 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/erase_era5sl_repository.py
+-rw-r--r--   0        0        0      383 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/update_arome_repository.py
+-rw-r--r--   0        0        0      401 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/update_era5land_repository.py
+-rw-r--r--   0        0        0      371 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/scripts/update_era5sl_repository.py
+-rw-r--r--   0        0        0      140 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/versions/__init__.py
+-rw-r--r--   0        0        0      469 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/versions/v1.py
+-rw-r--r--   0        0        0      469 2023-04-25 06:11:11.032155 weather_provider_api-2.41.21/weather_provider_api/versions/v2.py
+-rw-r--r--   0        0        0    13036 1970-01-01 00:00:00.000000 weather_provider_api-2.41.21/PKG-INFO
```

### Comparing `weather_provider_api-2.40.20/LICENSE` & `weather_provider_api-2.41.21/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/README.md` & `weather_provider_api-2.41.21/README.md`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/pyproject.toml` & `weather_provider_api-2.41.21/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 [tool.poetry]
 name = "weather_provider_api"
-version = "2.40.020"
+version = "2.41.021"
 description = "Weather Provider Libraries and API"
 authors = ["Verbindingsteam", "Raoul Linnenbank <58594297+rflinnenbank@users.noreply.github.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository="https://github.com/alliander-opensource/wpla/"
 include = [
     {path = "var_maps/*.json", format = "wheel"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-fastapi = "^0.88.0"
+fastapi = "^0.95.1"
 requests = "^2.28.1"
 geopy = "^2.3.0"
 numpy = "^1.23.5"
-structlog = "^22.3.0"
+structlog = "^23.1.0"
 gunicorn = "^20.1.0"
 eccodes = "^1.5.0"
 accept-types = "^0.4.1"
 lxml = "^4.9.1"
 starlette-prometheus = "^0.9.0"
 beautifulsoup4 = "^4.11.1"
 netcdf4 = "^1.6.2"
-ecmwflibs = "^0.5.0"
 tomli = "^2.0.1"
-pandas = "^1.5.2"
+pandas = "1.5.3"
 xarray = "^2022.12.0"
 cfgrib = "^0.9.10.3"
-uvicorn = "^0.20.0"
+uvicorn = "^0.21.1"
 slowapi = "^0.1.7"
+ecmwflibs = "0.5.1"
+starlette = "^0.26.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 coverage = "^6.5.0"
 pytest-cov = "^4.0.0"
 isort = "^5.10.1"
 black = "^22.10.0"
@@ -59,7 +60,8 @@
 
 [tool.pylint]
 max-line-length = 120
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `weather_provider_api-2.40.20/weather_provider_api/app_config.py` & `weather_provider_api-2.41.21/weather_provider_api/app_config.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/core/initializers/error_handling.py` & `weather_provider_api-2.41.21/weather_provider_api/core/initializers/error_handling.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/core/initializers/headers.py` & `weather_provider_api-2.41.21/weather_provider_api/core/initializers/headers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/core/initializers/logging.py` & `weather_provider_api-2.41.21/weather_provider_api/core/initializers/logging.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/core/initializers/monitoring.py` & `weather_provider_api-2.41.21/weather_provider_api/core/initializers/monitoring.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/core/initializers/mounting.py` & `weather_provider_api-2.41.21/weather_provider_api/core/initializers/mounting.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/core/initializers/validation.py` & `weather_provider_api-2.41.21/weather_provider_api/core/initializers/validation.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/main.py` & `weather_provider_api-2.41.21/weather_provider_api/main.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/api_models.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         description="Response format (overrides mime-types from Accept HTTP header)",
     )
 
 
 # Note: I'd love to combine the (almost) duplicate entries below, but the hybrid solutions don't work in FastAPI 0.30.
 @dataclass
 class WeatherContentRequestQuery:
+    # TODO: Change Example value to current date base values
     begin: str = Query(None, description="From date and time", example="2019-01-01 00:00")
     end: str = Query(None, description="To date and time", example="2019-01-31 23:59")
     lat: float = Query(..., description="GPS Latitude or RD x-coordinate", example=52.10)
     lon: float = Query(..., description="GPS Longitude or RD y-coordinate", example=5.18)
     factors: List[str] = Query(None, description="Only return these weather factors (default: all factors)")
```

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/api_view_v1.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_view_v1.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/api_view_v2.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/api_view_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,17 @@
     source_id: str,
     model_id: str,
     cleanup_tasks: BackgroundTasks,
     ret_args: WeatherContentRequestMultiLocationQuery = Depends(),
     fmt_args: WeatherFormattingRequestQuery = Depends(),
     accept: str = Depends(header_accept_type),
 ):  # pragma: no cover
+    starting_time = datetime.utcnow()
+    logger.info(f"WeatherRequest({starting_time}): {request.url}", datetime=datetime.utcnow())
+
     source_id = source_id.lower()
     model_id = model_id.lower()
 
     coords = controller.str_to_coords(ret_args.locations)
 
     begin = parse_datetime(ret_args.begin, raise_errors=True, loc=["query", "begin"])
     end = parse_datetime(
@@ -234,9 +237,9 @@
     for coord in coords:
         new_coords.append(coord[0])
 
     response, optional_file_path = serializers.file_or_text_response(
         converted_weather_data, response_format, source_id, model_id, ret_args, coords
     )
     cleanup_tasks.add_task(remove_file, optional_file_path)
-
+    logger.info(f"WeatherRequest({starting_time}) data preparation finished.", datetime=datetime.utcnow())
     return response
```

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/base_models/model.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/model.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/base_models/source.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/base_models/source.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/controller.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/controller.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/exceptions.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/exceptions.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/repository/repository.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/repository/repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/cds.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/cds.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/client/downloader.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/downloader.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/factors.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/factors.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/models/era5land.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/era5land.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/cds/models/era5sl.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/cds/models/era5sl.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/knmi.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/knmi.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/pluim.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/pluim.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/stations.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/stations.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/knmi/utils.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/knmi/utils.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/date_helpers.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/date_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/file_helpers.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/geo_position.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/geo_position.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/grid_helpers.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/grid_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/weather_provider_api/routers/weather/utils/serializers.py` & `weather_provider_api-2.41.21/weather_provider_api/routers/weather/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.40.20/setup.py` & `weather_provider_api-2.41.21/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,236 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: weather-provider-api
+Version: 2.41.21
+Summary: Weather Provider Libraries and API
+Home-page: https://github.com/alliander-opensource/wpla/
+License: MPL-2.0
+Author: Verbindingsteam
+Requires-Python: >=3.8,<3.11
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: accept-types (>=0.4.1,<0.5.0)
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: cfgrib (>=0.9.10.3,<0.10.0.0)
+Requires-Dist: eccodes (>=1.5.0,<2.0.0)
+Requires-Dist: ecmwflibs (==0.5.1)
+Requires-Dist: fastapi (>=0.95.1,<0.96.0)
+Requires-Dist: geopy (>=2.3.0,<3.0.0)
+Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
+Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Requires-Dist: netcdf4 (>=1.6.2,<2.0.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: slowapi (>=0.1.7,<0.2.0)
+Requires-Dist: starlette (>=0.26.1,<0.27.0)
+Requires-Dist: starlette-prometheus (>=0.9.0,<0.10.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
+Requires-Dist: xarray (>=2022.12.0,<2023.0.0)
+Project-URL: Repository, https://github.com/alliander-opensource/wpla/
+Description-Content-Type: text/markdown
+
+<!--
+SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
+SPDX-License-Identifier: MPL-2.0
+-->
+[![License: MIT](https://img.shields.io/badge/License-MPL2.0-informational.svg)](https://github.com/alliander-opensource/weather-provider-api/blob/master/LICENSE)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=alert_status)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=security_rating)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)
+[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=bugs)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)
+<!--[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=coverage)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)-->
+
+# Weather Provider Library and API
+
+This API is intended to help you fetch weather data from different data sources in an efficient and uniform way.
+By just supplying a list of locations and a time window you can get data for a specific source immediately.
+
+This project can currently be found on the following location:
+https://github.com/alliander-opensource/Weather-Provider-API
+
+For more information also check out this webinar:
+
+[![Webinar Weather Provider API](https://img.youtube.com/vi/pjE0DZmSphQ/0.jpg)](https://www.youtube.com/watch?v=pjE0DZmSphQ)
+
+
+The project uses a number of data sources for the acquisition of weather data. Currently being supported by this API 
+are the following weather data sources:
+
+**DATA SOURCE #1: KNMI Historical data per day / hour**
+
+Consists of the data from 35 weather stations for temperature, sun, cloud, air pressure, wind and precipitation.
+
+A full description of available weather variables is available for the data per day:
+http://projects.knmi.nl/klimatologie/daggegevens/selectie.cgi
+
+A full description for the data per hour consists only of a subset of the previous list:
+http://projects.knmi.nl/klimatologie/uurgegevens/selectie.cgi
+
+**DATA SOURCE #2: KNMI prediction data (14 day prediction, per block of 6 hours)**
+
+Prediction data for weather stations:
+De Bilt, Den Helder(De Kooy), Groningen(Eelde), Leeuwarden, Maastricht(Beek), Schiphol, Twente en Vlissingen
+
+Available weather variables are temperature, wind, precipitation, cape for summer, and snow for winter.
+
+An interactive graph can be found at:<BR>
+https://www.knmi.nl/nederland-nu/weer/waarschuwingen-en-verwachtingen/weer-en-klimaatpluim
+
+**DATA SOURCE #3: KNMI prediction data (48 hour, per hour prediction)**
+
+Prediction data is updated every 6 hours (00, 06, 12 and 18 UTC+00) based on the HARMONIE AROME model of KNMI.
+
+Geographical resolution is 0.037 grades west-east and 0.023 grades north-south.
+
+A full description of available weather variables is available at:
+https://www.knmidata.nl/data-services/knmi-producten-overzicht/atmosfeer-modeldata/data-product-1
+
+**DATA SOURCE #4: KNMI current weather data()**
+>> Actuele waarnemingen
+
+**DATA SOURCE #5: CDS (Climate Data Store) hourly data from 1979 to present**
+
+ERA5 is the fifth generation ECMWF (European Centre for Medium Range Weather Forecast)
+atmospheric reanalysis of the global climate.
+ERA5 data released so far covers the period from 1979 to 2-3 months before the present.
+ERA5 provides worldwide data for temperature and pressure, wind (at 100 meter height),
+radiation and heat, clouds, evaporation and runoff, precipitation and rain, snow, soil, etc.
+The spatial resolution of the data set is approximately 80 km.
+
+A full description of available weather variables is available at:
+https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=overview
+
+NOTE: The Weather Provider Library and API currently only stores only a selection of the available variables
+in its archives.
+
+## Input parameters to use the API
+
+### General input parameters
+
+- coords: nested 3-layer list representing a list of polygon.
+In case of points, they are treated as one-point polygon
+- start: start time of output data, for prediction data this is not needed
+- end: end time of output data, for prediction data this is not needed
+- data_time: history or prediction data
+- data_source: KNMI, Climate Data Store(CDS, not available yet), DarkSky (not available yet)
+- data_timestep: day, hour, or day_part (6 hour)
+- weather_factors: list of weather factors,
+            default is all available weather factors
+- output_unit: org (original), human_readable or SI (International System of Units),
+            default is the original names and units in data sources.
+### Case specific input parameters
+#### Choosing (a group of) weather variables for historical data from KNMI
+For historical data from KNMI the value for ``` weather_factors ``` in input can be a list of desired variables in random order,
+indicated by their acronyms separated by ':',
+for example ``` TG: TN: EV24 ```.
+
+The following acronyms are defined to indicate groups of variables:
+* **WIND = DDVEC:FG:FHX:FHX:FX** - *wind*
+* **TEMP = TG:TN:TX:T10N** - *temperature*
+* **SUNR = SQ:SP:Q** - *sunshine duration and global radiation*
+* **PRCP = DR:RH:EV24** - *precipitation and evaporation*
+* **PRES = PG:PGX** - *pressure at sea level*
+* **VICL = VVN:VVX:NG** - *visibility and clouds*
+* **MSTR = UG:UX:UN** - *humidity*
+* **ALL** - *all variables (default)*
+
+#### Choosing the name and unit for output
+The output data from the four data sources of KNMI may have different names and units for the same weather variable,
+which may not easy to use in analytics.
+
+This API provides an option to chose a standard name/unit for the mostly used weather variables, see table below.
+The value of  ``` output_unit ``` in input can be set to:
+* ``` org ```: to keep the originally used names and units
+* ``` SI ```: to convert the variable-names into SI/human readable name,
+and convert the units into SI units
+* ``` human ```: to convert the variable-names into SI/human readable name,
+and convert the units into human-readable units.
+
+
+| Hist day name | Hist day unit | Hist hour name | Hist hour unit | Forecast 14d name | Forecast 14d unit | Forecast 48h name | Forecast 48h unit | SI/Human readable name |    SI unit    | Human readable unit |
+| :-----------: |:-------------:| :-------------:| :------------: |:-----------------:| :----------------:| :---------------- |:-----------------:| :---------------------:| :-----------: |:-------------------:|
+| FG            | 0.1 m/s       | FH             | 0.1 m/s        | wind_speed        | km/uur            |                   |                   | wind_speed             | m/s           | m/s                 |
+| FHX           | 0.1 m/s       | FX             | 0.1 m/s        |                   |                   |                   |                   | wind_speed_max         | m/s           | m/s                 |
+| TG            | 0.1 celsius   | T              | 0.1 celsius    | temperature       | celsius           | 2T                | K                 | temperature            | K             | celsius             |
+| Q             | J/cm2         | Q              | J/cm2          |                   |                   | GRAD              | J m**-2           | global_radiation       | J/m2          | J/m2                |
+| RH            | 0.1 mm        | RH             | 0.1 mm         | precipitation     | mm                |                   |                   | precipitation          | m             | mm                  |
+| PG            | 0.1 hPa       | P              | 0.1 hPa        |                   |                   | LSP               | Pa                | air_pressure           | Pa            | Pa                  |
+| NG            | [1,2…9]      | N              | [1,2…9]       |                   |                   |                   |                   | cloud_cover            | [1,2…9]      | [1,2…9]             |
+| UG            | %             | U              | %              |                   |                   |                   |                   | humidity               | %             | %                   |
+
+The CDS data uses only SI units, and as such there is no distinction between ``` org ``` and ``` si ``` .
+
+## Getting started - using as a package/project
+### Prerequisites
+
+This package is supported from Python 3.8 or later. See '''requirements.txt''' for a list of dependencies.
+This package works under at least Linux and Windows environments. (Other Operating Systems not tested)
+
+### Installing
+
+1. Clone the repo
+2. Navigate to root
+3. Install the dependencies using conda/pip or both, depending on your environment
+```
+conda install --file requirements.txt
+```
+```
+pip install -r requirements.txt
+```
+4. Ready for use!
+
+### Using as a full project
+The full API can now be run by executing:
+```main.py```
+With the exception of ERA5 Single Levels and Harmonie Arome data, every data source can now be accessed
+using either the created end points or the API docs interface at the running location.
+(127.0.0.1:8080 when running locally)
+
+Specific calls can now be run by executing the proper command. For examples, check out the **\bin** folder.
+
+### Using as a wheel
+Install the wheel into your project environment and import the required classes.
+Usually this will be either a specific Weather Model or the Weather Controller.
+
+## Contributing
+
+Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
+
+## Contact
+To contact the project owners directly please e-mail us at [weather.provider@alliander.com](mailto://weather.provider@alliander.com)
+            
+## Authors
+
+This project was initially created by:
+
+* **Tongyou Gu** - *Original API development*
+* **Jeroen van de Logt** - *Functions in utilities*
+* **Bas Niesink** - *Implementation weather REST API*
+* **Raoul Linnenbank** - *Active API Development, Geo positioning, CDS ERA5, caching, remodeling, Harmonie Arome and optimisation*
+
+Currently, this project is governed in an open source fashion, this is documented in [PROJECT_GOVERNANCE](PROJECT_GOVERNANCE.md).
+
+## License
+
+This project is licensed under the Mozilla Public License, version 2.0 - see LICENSE for details
+
+## Licenses third-party code
+
+This project includes third-party code, which is licensed under their own respective Open-Source licenses. SPDX-License-Identifier headers are used to show which license is applicable. The concerning license files can be found in the LICENSES directory. 
+
+## Acknowledgments
 
-packages = \
-['weather_provider_api',
- 'weather_provider_api.core',
- 'weather_provider_api.core.errors',
- 'weather_provider_api.core.initializers',
- 'weather_provider_api.routers',
- 'weather_provider_api.routers.weather',
- 'weather_provider_api.routers.weather.base_models',
- 'weather_provider_api.routers.weather.repository',
- 'weather_provider_api.routers.weather.sources',
- 'weather_provider_api.routers.weather.sources.cds',
- 'weather_provider_api.routers.weather.sources.cds.client',
- 'weather_provider_api.routers.weather.sources.cds.models',
- 'weather_provider_api.routers.weather.sources.knmi',
- 'weather_provider_api.routers.weather.sources.knmi.client',
- 'weather_provider_api.routers.weather.sources.knmi.models',
- 'weather_provider_api.routers.weather.sources.weather_alert',
- 'weather_provider_api.routers.weather.utils',
- 'weather_provider_api.scripts',
- 'weather_provider_api.versions']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['accept-types>=0.4.1,<0.5.0',
- 'beautifulsoup4>=4.11.1,<5.0.0',
- 'cfgrib>=0.9.10.3,<0.10.0.0',
- 'eccodes>=1.5.0,<2.0.0',
- 'ecmwflibs>=0.5.0,<0.6.0',
- 'fastapi>=0.88.0,<0.89.0',
- 'geopy>=2.3.0,<3.0.0',
- 'gunicorn>=20.1.0,<21.0.0',
- 'lxml>=4.9.1,<5.0.0',
- 'netcdf4>=1.6.2,<2.0.0',
- 'numpy>=1.23.5,<2.0.0',
- 'pandas>=1.5.2,<2.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'slowapi>=0.1.7,<0.2.0',
- 'starlette-prometheus>=0.9.0,<0.10.0',
- 'structlog>=22.3.0,<23.0.0',
- 'tomli>=2.0.1,<3.0.0',
- 'uvicorn>=0.20.0,<0.21.0',
- 'xarray>=2022.12.0,<2023.0.0']
-
-entry_points = \
-{'console_scripts': ['wpla_clear_arome = '
-                     'weather_provider_api.scripts.erase_arome_repository:main',
-                     'wpla_clear_era5land = '
-                     'weather_provider_api.scripts.erase_era5land_repository:main',
-                     'wpla_clear_era5sl = '
-                     'weather_provider_api.scripts.erase_era5sl_repository:main',
-                     'wpla_run_api = weather_provider_api.main:main',
-                     'wpla_update_arome = '
-                     'weather_provider_api.scripts.update_arome_repository:main',
-                     'wpla_update_era5land = '
-                     'weather_provider_api.scripts.update_era5land_repository:main',
-                     'wpla_update_era5sl = '
-                     'weather_provider_api.scripts.update_era5sl_repository:main']}
-
-setup_kwargs = {
-    'name': 'weather-provider-api',
-    'version': '2.40.20',
-    'description': 'Weather Provider Libraries and API',
-    'long_description': "<!--\nSPDX-FileCopyrightText: 2019-2022 Alliander N.V.\nSPDX-License-Identifier: MPL-2.0\n-->\n[![License: MIT](https://img.shields.io/badge/License-MPL2.0-informational.svg)](https://github.com/alliander-opensource/weather-provider-api/blob/master/LICENSE)\n[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=alert_status)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)\n[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)\n[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=security_rating)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)\n[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)\n[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=bugs)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)\n<!--[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=alliander-opensource_weather-provider-api&metric=coverage)](https://sonarcloud.io/dashboard?id=alliander-opensource_Weather-Provider-API)-->\n\n# Weather Provider Library and API\n\nThis API is intended to help you fetch weather data from different data sources in an efficient and uniform way.\nBy just supplying a list of locations and a time window you can get data for a specific source immediately.\n\nThis project can currently be found on the following location:\nhttps://github.com/alliander-opensource/Weather-Provider-API\n\nFor more information also check out this webinar:\n\n[![Webinar Weather Provider API](https://img.youtube.com/vi/pjE0DZmSphQ/0.jpg)](https://www.youtube.com/watch?v=pjE0DZmSphQ)\n\n\nThe project uses a number of data sources for the acquisition of weather data. Currently being supported by this API \nare the following weather data sources:\n\n**DATA SOURCE #1: KNMI Historical data per day / hour**\n\nConsists of the data from 35 weather stations for temperature, sun, cloud, air pressure, wind and precipitation.\n\nA full description of available weather variables is available for the data per day:\nhttp://projects.knmi.nl/klimatologie/daggegevens/selectie.cgi\n\nA full description for the data per hour consists only of a subset of the previous list:\nhttp://projects.knmi.nl/klimatologie/uurgegevens/selectie.cgi\n\n**DATA SOURCE #2: KNMI prediction data (14 day prediction, per block of 6 hours)**\n\nPrediction data for weather stations:\nDe Bilt, Den Helder(De Kooy), Groningen(Eelde), Leeuwarden, Maastricht(Beek), Schiphol, Twente en Vlissingen\n\nAvailable weather variables are temperature, wind, precipitation, cape for summer, and snow for winter.\n\nAn interactive graph can be found at:<BR>\nhttps://www.knmi.nl/nederland-nu/weer/waarschuwingen-en-verwachtingen/weer-en-klimaatpluim\n\n**DATA SOURCE #3: KNMI prediction data (48 hour, per hour prediction)**\n\nPrediction data is updated every 6 hours (00, 06, 12 and 18 UTC+00) based on the HARMONIE AROME model of KNMI.\n\nGeographical resolution is 0.037 grades west-east and 0.023 grades north-south.\n\nA full description of available weather variables is available at:\nhttps://www.knmidata.nl/data-services/knmi-producten-overzicht/atmosfeer-modeldata/data-product-1\n\n**DATA SOURCE #4: KNMI current weather data()**\n>> Actuele waarnemingen\n\n**DATA SOURCE #5: CDS (Climate Data Store) hourly data from 1979 to present**\n\nERA5 is the fifth generation ECMWF (European Centre for Medium Range Weather Forecast)\natmospheric reanalysis of the global climate.\nERA5 data released so far covers the period from 1979 to 2-3 months before the present.\nERA5 provides worldwide data for temperature and pressure, wind (at 100 meter height),\nradiation and heat, clouds, evaporation and runoff, precipitation and rain, snow, soil, etc.\nThe spatial resolution of the data set is approximately 80 km.\n\nA full description of available weather variables is available at:\nhttps://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=overview\n\nNOTE: The Weather Provider Library and API currently only stores only a selection of the available variables\nin its archives.\n\n## Input parameters to use the API\n\n### General input parameters\n\n- coords: nested 3-layer list representing a list of polygon.\nIn case of points, they are treated as one-point polygon\n- start: start time of output data, for prediction data this is not needed\n- end: end time of output data, for prediction data this is not needed\n- data_time: history or prediction data\n- data_source: KNMI, Climate Data Store(CDS, not available yet), DarkSky (not available yet)\n- data_timestep: day, hour, or day_part (6 hour)\n- weather_factors: list of weather factors,\n            default is all available weather factors\n- output_unit: org (original), human_readable or SI (International System of Units),\n            default is the original names and units in data sources.\n### Case specific input parameters\n#### Choosing (a group of) weather variables for historical data from KNMI\nFor historical data from KNMI the value for ``` weather_factors ``` in input can be a list of desired variables in random order,\nindicated by their acronyms separated by ':',\nfor example ``` TG: TN: EV24 ```.\n\nThe following acronyms are defined to indicate groups of variables:\n* **WIND = DDVEC:FG:FHX:FHX:FX** - *wind*\n* **TEMP = TG:TN:TX:T10N** - *temperature*\n* **SUNR = SQ:SP:Q** - *sunshine duration and global radiation*\n* **PRCP = DR:RH:EV24** - *precipitation and evaporation*\n* **PRES = PG:PGX** - *pressure at sea level*\n* **VICL = VVN:VVX:NG** - *visibility and clouds*\n* **MSTR = UG:UX:UN** - *humidity*\n* **ALL** - *all variables (default)*\n\n#### Choosing the name and unit for output\nThe output data from the four data sources of KNMI may have different names and units for the same weather variable,\nwhich may not easy to use in analytics.\n\nThis API provides an option to chose a standard name/unit for the mostly used weather variables, see table below.\nThe value of  ``` output_unit ``` in input can be set to:\n* ``` org ```: to keep the originally used names and units\n* ``` SI ```: to convert the variable-names into SI/human readable name,\nand convert the units into SI units\n* ``` human ```: to convert the variable-names into SI/human readable name,\nand convert the units into human-readable units.\n\n\n| Hist day name | Hist day unit | Hist hour name | Hist hour unit | Forecast 14d name | Forecast 14d unit | Forecast 48h name | Forecast 48h unit | SI/Human readable name |    SI unit    | Human readable unit |\n| :-----------: |:-------------:| :-------------:| :------------: |:-----------------:| :----------------:| :---------------- |:-----------------:| :---------------------:| :-----------: |:-------------------:|\n| FG            | 0.1 m/s       | FH             | 0.1 m/s        | wind_speed        | km/uur            |                   |                   | wind_speed             | m/s           | m/s                 |\n| FHX           | 0.1 m/s       | FX             | 0.1 m/s        |                   |                   |                   |                   | wind_speed_max         | m/s           | m/s                 |\n| TG            | 0.1 celsius   | T              | 0.1 celsius    | temperature       | celsius           | 2T                | K                 | temperature            | K             | celsius             |\n| Q             | J/cm2         | Q              | J/cm2          |                   |                   | GRAD              | J m**-2           | global_radiation       | J/m2          | J/m2                |\n| RH            | 0.1 mm        | RH             | 0.1 mm         | precipitation     | mm                |                   |                   | precipitation          | m             | mm                  |\n| PG            | 0.1 hPa       | P              | 0.1 hPa        |                   |                   | LSP               | Pa                | air_pressure           | Pa            | Pa                  |\n| NG            | [1,2…9]      | N              | [1,2…9]       |                   |                   |                   |                   | cloud_cover            | [1,2…9]      | [1,2…9]             |\n| UG            | %             | U              | %              |                   |                   |                   |                   | humidity               | %             | %                   |\n\nThe CDS data uses only SI units, and as such there is no distinction between ``` org ``` and ``` si ``` .\n\n## Getting started - using as a package/project\n### Prerequisites\n\nThis package is supported from Python 3.8 or later. See '''requirements.txt''' for a list of dependencies.\nThis package works under at least Linux and Windows environments. (Other Operating Systems not tested)\n\n### Installing\n\n1. Clone the repo\n2. Navigate to root\n3. Install the dependencies using conda/pip or both, depending on your environment\n```\nconda install --file requirements.txt\n```\n```\npip install -r requirements.txt\n```\n4. Ready for use!\n\n### Using as a full project\nThe full API can now be run by executing:\n```main.py```\nWith the exception of ERA5 Single Levels and Harmonie Arome data, every data source can now be accessed\nusing either the created end points or the API docs interface at the running location.\n(127.0.0.1:8080 when running locally)\n\nSpecific calls can now be run by executing the proper command. For examples, check out the **\\bin** folder.\n\n### Using as a wheel\nInstall the wheel into your project environment and import the required classes.\nUsually this will be either a specific Weather Model or the Weather Controller.\n\n## Contributing\n\nPlease read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.\n\n## Contact\nTo contact the project owners directly please e-mail us at [weather.provider@alliander.com](mailto://weather.provider@alliander.com)\n            \n## Authors\n\nThis project was initially created by:\n\n* **Tongyou Gu** - *Original API development*\n* **Jeroen van de Logt** - *Functions in utilities*\n* **Bas Niesink** - *Implementation weather REST API*\n* **Raoul Linnenbank** - *Active API Development, Geo positioning, CDS ERA5, caching, remodeling, Harmonie Arome and optimisation*\n\nCurrently, this project is governed in an open source fashion, this is documented in [PROJECT_GOVERNANCE](PROJECT_GOVERNANCE.md).\n\n## License\n\nThis project is licensed under the Mozilla Public License, version 2.0 - see LICENSE for details\n\n## Licenses third-party code\n\nThis project includes third-party code, which is licensed under their own respective Open-Source licenses. SPDX-License-Identifier headers are used to show which license is applicable. The concerning license files can be found in the LICENSES directory. \n\n## Acknowledgments\n\nThanks to team Inzicht & Analytics and Strategie & Innovatie to\nmake this project possible.\n\nA big thanks as well to Alliander for being the main sponsor for this open source project.  \n\nAnd of course a big thanks to the guys of IT New Business & R&D to provide\nsuch an easy-to-use Python environment in the cloud.\n",
-    'author': 'Verbindingsteam',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/alliander-opensource/wpla/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
-}
+Thanks to team Inzicht & Analytics and Strategie & Innovatie to
+make this project possible.
 
+A big thanks as well to Alliander for being the main sponsor for this open source project.  
+
+And of course a big thanks to the guys of IT New Business & R&D to provide
+such an easy-to-use Python environment in the cloud.
 
-setup(**setup_kwargs)
```

