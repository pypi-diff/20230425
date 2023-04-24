# Comparing `tmp/pyweatherflowudp-1.4.1.tar.gz` & `tmp/pyweatherflowudp-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherflowudp-1.4.1.tar", max compression
+gzip compressed data, was "pyweatherflowudp-1.4.2.tar", max compression
```

## Comparing `pyweatherflowudp-1.4.1.tar` & `pyweatherflowudp-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1081 2021-12-01 08:09:40.000000 pyweatherflowudp-1.4.1/LICENSE
--rw-r--r--   0        0        0    13411 2022-07-11 18:41:47.370939 pyweatherflowudp-1.4.1/README.md
--rw-r--r--   0        0        0      898 2022-07-11 18:47:29.347113 pyweatherflowudp-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      103 2022-07-11 18:44:04.104519 pyweatherflowudp-1.4.1/pyweatherflowudp/__init__.py
--rw-r--r--   0        0        0     6623 2022-06-10 18:53:43.202493 pyweatherflowudp-1.4.1/pyweatherflowudp/aioudp.py
--rw-r--r--   0        0        0     6450 2022-07-11 18:41:47.371191 pyweatherflowudp-1.4.1/pyweatherflowudp/calc.py
--rw-r--r--   0        0        0     4361 2022-06-10 18:54:25.661894 pyweatherflowudp-1.4.1/pyweatherflowudp/client.py
--rw-r--r--   0        0        0     1373 2022-06-10 18:53:43.203601 pyweatherflowudp-1.4.1/pyweatherflowudp/const.py
--rw-r--r--   0        0        0    16322 2022-06-10 18:54:25.662424 pyweatherflowudp-1.4.1/pyweatherflowudp/device.py
--rw-r--r--   0        0        0      801 2022-06-10 18:45:11.571902 pyweatherflowudp-1.4.1/pyweatherflowudp/enums.py
--rw-r--r--   0        0        0      430 2021-12-01 08:09:40.000000 pyweatherflowudp-1.4.1/pyweatherflowudp/errors.py
--rw-r--r--   0        0        0     2584 2022-06-10 18:53:43.204225 pyweatherflowudp-1.4.1/pyweatherflowudp/event.py
--rw-r--r--   0        0        0     1662 2022-06-10 18:53:43.204513 pyweatherflowudp-1.4.1/pyweatherflowudp/helpers.py
--rw-r--r--   0        0        0    12818 2022-07-11 18:41:47.371435 pyweatherflowudp-1.4.1/pyweatherflowudp/mixins.py
--rw-r--r--   0        0        0    14420 2022-07-11 18:47:40.287052 pyweatherflowudp-1.4.1/setup.py
--rw-r--r--   0        0        0    14259 2022-07-11 18:47:40.288312 pyweatherflowudp-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2021-12-01 08:09:40.000000 pyweatherflowudp-1.4.2/LICENSE
+-rw-r--r--   0        0        0    13411 2022-07-11 18:41:47.370939 pyweatherflowudp-1.4.2/README.md
+-rw-r--r--   0        0        0      925 2023-04-24 22:13:36.921417 pyweatherflowudp-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-04-24 22:13:36.921720 pyweatherflowudp-1.4.2/pyweatherflowudp/__init__.py
+-rw-r--r--   0        0        0     6623 2022-06-10 18:53:43.202493 pyweatherflowudp-1.4.2/pyweatherflowudp/aioudp.py
+-rw-r--r--   0        0        0     6400 2023-04-24 22:02:08.547134 pyweatherflowudp-1.4.2/pyweatherflowudp/calc.py
+-rw-r--r--   0        0        0     4361 2022-06-10 18:54:25.661894 pyweatherflowudp-1.4.2/pyweatherflowudp/client.py
+-rw-r--r--   0        0        0     1373 2022-06-10 18:53:43.203601 pyweatherflowudp-1.4.2/pyweatherflowudp/const.py
+-rw-r--r--   0        0        0    16437 2023-04-24 22:02:08.547355 pyweatherflowudp-1.4.2/pyweatherflowudp/device.py
+-rw-r--r--   0        0        0      816 2023-04-24 22:02:08.547550 pyweatherflowudp-1.4.2/pyweatherflowudp/enums.py
+-rw-r--r--   0        0        0      430 2021-12-01 08:09:40.000000 pyweatherflowudp-1.4.2/pyweatherflowudp/errors.py
+-rw-r--r--   0        0        0     2584 2022-06-10 18:53:43.204225 pyweatherflowudp-1.4.2/pyweatherflowudp/event.py
+-rw-r--r--   0        0        0     1653 2023-04-24 22:02:08.547726 pyweatherflowudp-1.4.2/pyweatherflowudp/helpers.py
+-rw-r--r--   0        0        0    12818 2023-04-24 21:59:34.543377 pyweatherflowudp-1.4.2/pyweatherflowudp/mixins.py
+-rw-r--r--   0        0        0    14424 1970-01-01 00:00:00.000000 pyweatherflowudp-1.4.2/setup.py
+-rw-r--r--   0        0        0    14310 1970-01-01 00:00:00.000000 pyweatherflowudp-1.4.2/PKG-INFO
```

### Comparing `pyweatherflowudp-1.4.1/LICENSE` & `pyweatherflowudp-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyweatherflowudp-1.4.1/README.md` & `pyweatherflowudp-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherflowudp-1.4.1/pyweatherflowudp/aioudp.py` & `pyweatherflowudp-1.4.2/pyweatherflowudp/aioudp.py`

 * *Files identical despite different names*

### Comparing `pyweatherflowudp-1.4.1/pyweatherflowudp/calc.py` & `pyweatherflowudp-1.4.2/pyweatherflowudp/calc.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,29 @@
                 else 1
             ),
         )
         * UNIT_DEGREES_CELSIUS
     ).to(air_temperature.u)
 
 
+def feels_like_temperature(
+    air_temperature: Quantity[float],
+    relative_humidity: Quantity[float],
+    wind_speed: Quantity[float],
+) -> Quantity[float] | None:
+    """Calculate the "feels like" temperature."""
+    # fmt: off
+    if (temp := heat_index(air_temperature=air_temperature, relative_humidity=relative_humidity)) is not None:
+        return temp
+    if (temp := wind_chill(air_temperature=air_temperature, wind_speed=wind_speed)) is not None:
+        return temp
+    # fmt: on
+    return air_temperature
+
+
 def freezing_level(
     air_temperature: Quantity[float], altitude: Quantity[float]
 ) -> Quantity[float]:
     """Calculate the estimated altitude above mean sea level (AMSL) where the temperature is at the freezing point (0°C/32°F).
 
     References:
         https://github.com/briis/hass-weatherflow2mqtt/issues/131
@@ -84,46 +99,35 @@
 
 
 def heat_index(
     air_temperature: Quantity[float], relative_humidity: Quantity[float]
 ) -> Quantity[float] | None:
     """Calculate the heat index.
 
-    Only temperatures >= 80°F (26.66°C) have a heat index.
+    Only temperatures >= 80°F (26.66°C) and relative humidity >= 40% have a heat index.
     """
     temp_fahrenheit = air_temperature.to("degF").m
-
-    if temp_fahrenheit < 80:
-        return None
-
     rh_percent = relative_humidity.m * (
         1 if relative_humidity.u == UNIT_PERCENT or relative_humidity.m > 1 else 100
     )
+    if temp_fahrenheit < 80 or rh_percent < 40:
+        return None
 
-    heat_idx = 0.5 * (
-        temp_fahrenheit + 61.0 + ((temp_fahrenheit - 68.0) * 1.2) + (rh_percent * 0.094)
+    heat_idx = (
+        -42.379
+        + 2.04901523 * temp_fahrenheit
+        + 10.14333127 * rh_percent
+        - 0.22475541 * temp_fahrenheit * rh_percent
+        - 0.00683783 * temp_fahrenheit**2
+        - 0.05481717 * rh_percent**2
+        + 0.00122874 * temp_fahrenheit**2 * rh_percent
+        + 0.00085282 * temp_fahrenheit * rh_percent**2
+        - 0.00000199 * temp_fahrenheit**2 * rh_percent**2
     )
-    if (heat_idx + temp_fahrenheit) / 2 >= 80:
-        heat_idx = (
-            -42.379
-            + 2.04901523 * temp_fahrenheit
-            + 10.14333127 * rh_percent
-            - 0.22475541 * temp_fahrenheit * rh_percent
-            - 0.00683783 * temp_fahrenheit * temp_fahrenheit
-            - 0.05481717 * rh_percent * rh_percent
-            + 0.00122874 * temp_fahrenheit * temp_fahrenheit * rh_percent
-            + 0.00085282 * temp_fahrenheit * rh_percent * rh_percent
-            - 0.00000199 * temp_fahrenheit * temp_fahrenheit * rh_percent * rh_percent
-        )
-        if rh_percent < 13 and (80 <= temp_fahrenheit <= 112):
-            heat_idx -= ((13 - rh_percent) / 4) * (
-                (17 - abs(temp_fahrenheit - 95.0)) / 17
-            ) ** 0.5
-        elif rh_percent > 85 and (80 <= temp_fahrenheit <= 87):
-            heat_idx += ((rh_percent - 85) / 10) * ((87 - temp_fahrenheit) / 5)
+
     return (heat_idx * units.degF).to(air_temperature.u)
 
 
 @units.wraps(units.millibar, (units.millibar, units.meter))
 def sea_level_pressure(
     station_pressure: Quantity[float], altitude: Quantity[float]
 ) -> Quantity[float]:
@@ -183,15 +187,14 @@
 ) -> Quantity[float] | None:
     """Calculate the wind chill temperature.
 
     Only temperatures <= 50°F (10°C) and winds >= 3mph (1.34112 m/s) have a wind chill.
     """
     temp_fahrenheit = air_temperature.to("degF").m
     wind_mph = wind_speed.to("mph").m
-
     if temp_fahrenheit > 50 or wind_mph < 3:
         return None
 
     return (
         (
             35.74
             + (0.6215 * temp_fahrenheit)
```

### Comparing `pyweatherflowudp-1.4.1/pyweatherflowudp/client.py` & `pyweatherflowudp-1.4.2/pyweatherflowudp/client.py`

 * *Files identical despite different names*

### Comparing `pyweatherflowudp-1.4.1/pyweatherflowudp/const.py` & `pyweatherflowudp-1.4.2/pyweatherflowudp/const.py`

 * *Files identical despite different names*

### Comparing `pyweatherflowudp-1.4.1/pyweatherflowudp/device.py` & `pyweatherflowudp-1.4.2/pyweatherflowudp/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import logging
 from datetime import datetime
 from typing import Any, Callable, final
 
 from pint import Quantity
 
-from .calc import wind_chill
+from .calc import feels_like_temperature, wind_chill
 from .const import (
     EVENT_OBSERVATION_AIR,
     EVENT_OBSERVATION_SKY,
     EVENT_OBSERVATION_TEMPEST,
     EVENT_RAIN_START,
     EVENT_RAPID_WIND,
     EVENT_STATUS_DEVICE,
@@ -471,19 +471,21 @@
     }
 
     # Derived metrics
 
     @property
     def feels_like_temperature(self) -> Quantity[float] | None:
         """Return the feels like temperature in degrees Celsius (°C)."""
-        if self.heat_index is not None:
-            return self.heat_index
-        if self.wind_chill_temperature is not None:
-            return self.wind_chill_temperature
-        return self.air_temperature
+        if None in (self.air_temperature, self.relative_humidity, self.wind_speed):
+            return None
+        return feels_like_temperature(
+            air_temperature=self.air_temperature,
+            relative_humidity=self.relative_humidity,
+            wind_speed=self.wind_speed,
+        )
 
     @property
     def wind_chill_temperature(self) -> Quantity[float] | None:
         """Return the calculated wind chill temperature in degrees Celsius (°C)."""
         if None in (self.air_temperature, self.wind_speed):
             return None
         return wind_chill(self.air_temperature, self.wind_speed)
```

### Comparing `pyweatherflowudp-1.4.1/pyweatherflowudp/enums.py` & `pyweatherflowudp-1.4.2/pyweatherflowudp/enums.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """Precipitation types."""
 
     NONE = 0
     RAIN = 1
     HAIL = 2
     RAIN_HAIL = 3
 
-    # Handle unknown/future fan modes
+    # Handle unknown/future precipitation types
     UNKNOWN = -1
 
     @classmethod
     def _missing_(cls, _: object) -> PrecipitationType:  # pragma: no cover
         """Return default if not found."""
         return cls.UNKNOWN
 
@@ -27,14 +27,14 @@
     """Radio statuses."""
 
     RADIO_OFF = 0
     RADIO_ON = 1
     RADIO_ACTIVE = 3
     BLE_CONNECTED = 7
 
-    # Handle unknown/future fan modes
+    # Handle unknown/future radio statuses
     UNKNOWN = -1
 
     @classmethod
     def _missing_(cls, _: object) -> RadioStatus:  # pragma: no cover
         """Return a default if not found."""
         return cls.UNKNOWN
```

### Comparing `pyweatherflowudp-1.4.1/pyweatherflowudp/event.py` & `pyweatherflowudp-1.4.2/pyweatherflowudp/event.py`

 * *Files identical despite different names*

### Comparing `pyweatherflowudp-1.4.1/pyweatherflowudp/helpers.py` & `pyweatherflowudp-1.4.2/pyweatherflowudp/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Helper functions."""
 from __future__ import annotations
 
 from datetime import datetime, timezone
-from typing import Any, TypeVar
+from typing import Any, TypeVar, cast
 
 from pint import Quantity
 from pint.unit import Unit
 
 DIRECTIONS = [
     "N",
     "NNE",
@@ -21,27 +21,23 @@
     "SW",
     "WSW",
     "W",
     "WNW",
     "NW",
     "NNW",
 ]
+DIRECTIONS_COUNT = len(DIRECTIONS)
 T = TypeVar("T")  # pylint: disable=invalid-name
 UTC = timezone.utc
 
 
 def degrees_to_cardinal(degree: float | Quantity[float]) -> str:
     """Convert degrees to a cardinal direction."""
-    return DIRECTIONS[
-        round(
-            (degree.m if isinstance(degree, Quantity) else degree)
-            / (360.0 / (directions_count := len(DIRECTIONS)))
-        )
-        % directions_count
-    ]
+    _deg = cast(float, degree.m if isinstance(degree, Quantity) else degree)
+    return DIRECTIONS[round(_deg / (360.0 / DIRECTIONS_COUNT)) % DIRECTIONS_COUNT]
 
 
 def nvl(value: T | None, default: T) -> T:
     """Return default if value is None, else value."""
     return default if value is None else value
```

### Comparing `pyweatherflowudp-1.4.1/pyweatherflowudp/mixins.py` & `pyweatherflowudp-1.4.2/pyweatherflowudp/mixins.py`

 * *Files identical despite different names*

### Comparing `pyweatherflowudp-1.4.1/setup.py` & `pyweatherflowudp-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['Pint>=0.19,<0.20', 'PsychroLib>=2.5.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'pyweatherflowudp',
-    'version': '1.4.1',
+    'version': '1.4.2',
     'description': 'An event-based asynchronous library to read UDP packets from Weatherflow weather systems on a local network without any reliance on the cloud.',
     'long_description': '[![pypi](https://img.shields.io/pypi/v/pyweatherflowudp?style=for-the-badge)](https://pypi.org/project/pyweatherflowudp)\n[![downloads](https://img.shields.io/pypi/dm/pyweatherflowudp?style=for-the-badge)](https://pypi.org/project/pyweatherflowudp)\n[![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)\n\n# pyweatherflowudp\n\nAn event-based asynchronous library to read UDP packets from Weatherflow weather systems on a local network without any reliance on the cloud.\n\nThe atomic data provided by WeatherFlow sensors is all natively metric. To help facilitate transformations to other units or to perform calculations and comparisons, this module utilizes [Pint](https://pint.readthedocs.io/en/stable/)\'s Quantity class as the type of most properties which have a unit of measurement. See the [Quantity](#Quantity) section below for more details.\n\nThis module utilizes [PsychroLib](https://github.com/psychrometrics/psychrolib) to help with additional weather calculations that are derived from the various data points provided by the actual WeatherFlow sensors. While WeatherFlow has these additional data points available via the app and rest API, they are unavailable via the low-level UDP packet data. And while a list of [derived metrics](https://weatherflow.github.io/Tempest/api/derived-metric-formulas.html) and the associated equations has been posted, they can be quite complex to implement, such as calculating wet bulb temperature. As such, PsychroLib is an invaluable resource since the work has already been done and it eliminates the need to write all the equations in this module (and potentially get them wrong). You may notice that some of these values aren\'t an exact match with what is shown in the WeatherFlow app because there are different formulas (some simpler, some more complex) to calculate derived weather metrics. This is because WeatherFlow and PsychroLib may have chosen one of the sometimes many different formulas to get the result desired. They should still be relatively close, however.\n\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.01137/status.svg)](https://doi.org/10.21105/joss.01137) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2537945.svg)](https://doi.org/10.5281/zenodo.2537945)\n\n## Supported Devices\n\n- Tempest\n- Air (untested)\n- Sky (untested)\n\n## Usage\n\nThe primary way of interacting with this module, and the devices that are found with it, is via event subscriptions.\n\nThe classes and events which they currently support are outlined below, but you can also see an example tying this altogether in [demo.py](/demo.py).\n\n### Client\n\n#### `WeatherFlowListener`\n\n- EVENT_DEVICE_DISCOVERED - emitted when a new device (Hub, Air, Sky or Tempest) is disovered for the first time\n\nThe classes and events in this section can be imported from `pyweatherflowudp.client`.\n\n### Devices\n\n#### `HubDevice`\n\n- EVENT_LOAD_COMPLETE - emitted once when the hub has finished parsing a status update for the first time\n- EVENT_STATUS_UPDATE - emitted each time a status update has been parsed by the hub, including immediately following an EVENT_LOAD_COMPLETE\n\n#### `WeatherFlowSensorDevice` (base class for `AirDevice`, `SkyDevice` and `TempestDevice`)\n\n- EVENT_LOAD_COMPLETE - emitted once when the sensor has finished parsing one status update and one observation for the first time\n- EVENT_OBSERVATION - emitted each time an observation has been parsed by the sensor\n- EVENT_STATUS_UPDATE - emitted each time a status update has been parsed by the sensor\n\n#### `AirSensorType` (`AirDevice` / `TempestDevice`)\n\n- EVENT_STRIKE - emitted when a lightning strike has been detected\n\n#### `SkySensorType` (`SkyDevice` / `TempestDevice`)\n\n- EVENT_RAIN_START - emitted when rain has been detected\n- EVENT_RAPID_WIND - emitted every 3 seconds (or less frequently depending on battery voltage) to inform about current wind condtions\n\nThe classes and events in this section can be imported from `pyweatherflowudp.device`.\n\n## Properties and Methods\n\n### WeatherFlowListener\n\n| property     | type | description                                                                              |\n| ------------ | ---- | ---------------------------------------------------------------------------------------- |\n| devices      | list | The known devices.                                                                       |\n| hubs         | list | The known hubs.                                                                          |\n| is_listening | bool | `True` if the listener is currently monitoring UDP packets on the network, else `False`. |\n| sensors      | list | The known sensors.                                                                       |\n\n### WeatherFlowDevice\n\nBase for hubs and sensors.\n\n| property          | type     | description                                                         |\n| ----------------- | -------- | ------------------------------------------------------------------- |\n| firmware_revision | str      | The current firmware revision of the device.                        |\n| load_complete     | bool     | `True` if the device has parsed all initial updates, else `False`.  |\n| model             | str      | The model of the device ("Hub", "Air", "Sky", "Tempest").           |\n| rssi              | Quantity | The signal strength of the device in decibels.                      |\n| serial_number     | str      | The serial number of the device.                                    |\n| timestamp         | datetime | The UTC timestamp from the last status update.                      |\n| up_since          | datetime | The UTC timestamp the device started up and has since been running. |\n| uptime            | int      | The number of seconds the device has been up and running.           |\n\n### HubDevice\n\n| property    | type | description                         |\n| ----------- | ---- | ----------------------------------- |\n| reset_flags | list | The current reset flags of the hub. |\n\n### WeatherFlowSensorDevice\n\nBase for sensors.\n\n| property        | type     | description                                           |\n| --------------- | -------- | ----------------------------------------------------- |\n| battery         | Quantity | The current battery voltage.                          |\n| hub_rssi        | Quantity | The signal strength of the hub in decibels.           |\n| hub_sn          | str      | The serial number of the hub the sensor belongs to.   |\n| last_report     | datetime | The UTC timestamp from the last observation.          |\n| sensor_status   | list     | The list of issues the sensor is currently reporting. |\n| report_interval | Quantity | The report interval in minutes.                       |\n| reset_flags     | list     | The current reset flags of the hub.                   |\n\n### AirSensorType\n\nBase for "air" sensor measurements (Air/Tempest).\n\n| property                          | type                 | description                                               |\n| --------------------------------- | -------------------- | --------------------------------------------------------- |\n| air_temperature                   | Quantity             | The current air temperature in degrees Celsius.           |\n| last_lightning_strike_event       | LightningStrikeEvent | The last lightning strike event.                          |\n| lightning_strike_average_distance | Quantity             | The average distance for lightning strikes in kilometers. |\n| lightning_strike_count            | int                  | The number of lightning strikes.                          |\n| relative_humidity                 | Quantity             | The relative humidity percentage.                         |\n| station_pressure                  | Quantity             | The observed station pressure in millibars.               |\n| air_density\\*                     | Quantity             | The calculated air density in kilograms per cubic meter.  |\n| delta_t\\*                         | Quantity             | The calculated Delta T in delta degrees Celsius.          |\n| dew_point_temperature\\*           | Quantity             | The calculated dew point temperature in degrees Celsius.  |\n| heat_index\\*                      | Quantity             | The calculated heat index in degrees Celsius.             |\n| vapor_pressure\\*                  | Quantity             | The calculated vapor pressure in millibars.               |\n| wet_bulb_temperature\\*            | Quantity             | The calculated wet bulb temperature in degrees Celsius.   |\n\n\\* Indicates derived properties\n\n| method                       | input (type)        | return   | description                                                                                                             |\n| ---------------------------- | ------------------- | -------- | ----------------------------------------------------------------------------------------------------------------------- |\n| calculate_cloud_base         | altitude (Quantity) | Quantity | Calculate the estimated altitude above mean sea level (AMSL) to the cloud base.                                         |\n| calculate_freezing_level     | altitude (Quantity) | Quantity | Calculate the estimated altitude above mean sea level (AMSL) where the temperature is at the freezing point (0°C/32°F). |\n| calculate_sea_level_pressure | altitude (Quantity) | Quantity | Calculate the sea level pressure in millibars (mbar).                                                                   |\n\n### SkySensorType\n\nBase for "sky" sensor measurements (Sky/Tempest).\n\n| property                          | type              | description                                                                        |\n| --------------------------------- | ----------------- | ---------------------------------------------------------------------------------- |\n| illuminance                       | Quantity          | The current illuminance in Lux.                                                    |\n| last_rain_start_event             | RainStartEvent    | The last rain start event.                                                         |\n| last_wind_event                   | WindEvent         | The last wind event.                                                               |\n| precipitation_type                | PrecipitationType | The current precipitation type: (NONE, RAIN, HAIL or RAIN_HAIL).                   |\n| rain_accumulation_previous_minute | Quantity          | The rain accumulation from the previous minute in millimeters.                     |\n| rain_rate\\*                       | Quantity          | The rain rate in millimeters per hour (based on the previous minute accumulation). |\n| solar_radiation                   | Quantity          | The solar radiation in Watts per cubic meter.                                      |\n| uv                                | int               | The current UV index.                                                              |\n| wind_average                      | Quantity          | The wind speed average over the report interval in meters per second.              |\n| wind_direction                    | Quantity          | The wind direction over the report interval in degrees.                            |\n| wind_direction_cardinal           | string            | The wind direction cardinal (16-wind compass rose).                                |\n| wind_gust                         | Quantity          | The wind gust (maximum 3 second sample) in meters per second.                      |\n| wind_lull                         | Quantity          | The wind lull (minimum 3 second sample) in meters per second.                      |\n| wind_sample_interval              | Quantity          | The wind sample interval in seconds.                                               |\n| wind_speed                        | Quantity          | The wind speed in meters per second.                                               |\n\n\\* Indicates derived properties\n\n### TempestDevice\n\n| property                 | type     | description                                                 |\n| ------------------------ | -------- | ----------------------------------------------------------- |\n| feels_like_temperature\\* | Quantity | The calculated "feels like" temperature in degrees Celsius. |\n| wind_chill_temperature\\* | Quantity | The calculated wind chill temperature in degrees Celsius.   |\n\n\\* Indicates derived properties\n\n### Quantity\n\nThe `pint.Quantity` class has been utilized for device properties which are associated with a unit of measurement. This allows a conversion from the native metric unit to another of the user\'s choice such as degrees Celsius to degrees Fahrenheit, which produces another `pint.Quantity`:\n\n```python\ndevice.air_temperature.to("degF")\n```\n\nTo retrieve only the numeric value of a property, you can just append a `.magnitude` (or `.m` short form) like:\n\n```python\ndevice.air_temperature.m\n```\n\nYou can also retrieve only the units portion of a property with `.units` (or `.u` short form) like:\n\n```python\ndevice.air_temperature.u\n```\n\nCheck out the [Pint docs](https://pint.readthedocs.io/en/stable/#user-guide) for more tips.\n',
     'author': 'Nathan Spencer',
     'author_email': 'natekspencer@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/briis/pyweatherflowudp',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `pyweatherflowudp-1.4.1/PKG-INFO` & `pyweatherflowudp-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyweatherflowudp
-Version: 1.4.1
+Version: 1.4.2
 Summary: An event-based asynchronous library to read UDP packets from Weatherflow weather systems on a local network without any reliance on the cloud.
 Home-page: https://github.com/briis/pyweatherflowudp
 License: MIT
 Keywords: WeatherFlow,UDP,asynchronous,local
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pint (>=0.19,<0.20)
 Requires-Dist: PsychroLib (>=2.5.0,<3.0.0)
 Project-URL: Repository, https://github.com/briis/pyweatherflowudp
 Description-Content-Type: text/markdown
 
 [![pypi](https://img.shields.io/pypi/v/pyweatherflowudp?style=for-the-badge)](https://pypi.org/project/pyweatherflowudp)
 [![downloads](https://img.shields.io/pypi/dm/pyweatherflowudp?style=for-the-badge)](https://pypi.org/project/pyweatherflowudp)
```

