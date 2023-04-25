# Comparing `tmp/kyoslib_py-4.0.2.tar.gz` & `tmp/kyoslib_py-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyoslib_py-4.0.2.tar", max compression
+gzip compressed data, was "kyoslib_py-4.1.0.tar", max compression
```

## Comparing `kyoslib_py-4.0.2.tar` & `kyoslib_py-4.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2022-12-19 13:58:05.790437 kyoslib_py-4.0.2/LICENSE.txt
--rw-r--r--   0        0        0      988 2022-12-19 13:58:05.790437 kyoslib_py-4.0.2/README.md
--rw-r--r--   0        0        0        0 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/__init__.py
--rw-r--r--   0        0        0     8800 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/forward_curve.py
--rw-r--r--   0        0        0    15633 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/front_end.py
--rw-r--r--   0        0        0    24393 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/historical_price.py
--rw-r--r--   0        0        0     3458 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/kyos_api.py
--rw-r--r--   0        0        0     4298 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/kyos_utils.py
--rw-r--r--   0        0        0    45259 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/settings.py
--rw-r--r--   0        0        0    85676 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/simulation.py
--rw-r--r--   0        0        0    21363 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/tradable_product.py
--rw-r--r--   0        0        0    36053 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/kyoslib_py/valuation_interface.py
--rw-r--r--   0        0        0     1029 2022-12-19 13:58:05.794437 kyoslib_py-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 kyoslib_py-4.0.2/setup.py
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 kyoslib_py-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-25 07:30:03.825109 kyoslib_py-4.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      944 2023-04-25 07:30:03.825109 kyoslib_py-4.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 07:30:03.829109 kyoslib_py-4.1.0/kyoslib_py/__init__.py
+-rw-r--r--   0        0        0     8805 2023-04-25 07:30:03.829109 kyoslib_py-4.1.0/kyoslib_py/forward_curve.py
+-rw-r--r--   0        0        0    15638 2023-04-25 07:30:03.829109 kyoslib_py-4.1.0/kyoslib_py/front_end.py
+-rw-r--r--   0        0        0    24395 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/historical_price.py
+-rw-r--r--   0        0        0     3459 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/kyos_api.py
+-rw-r--r--   0        0        0     4233 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/kyos_utils.py
+-rw-r--r--   0        0        0    45293 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/settings.py
+-rw-r--r--   0        0        0    92410 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/simulation.py
+-rw-r--r--   0        0        0    21363 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/tradable_product.py
+-rw-r--r--   0        0        0    36060 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/valuation_interface.py
+-rw-r--r--   0        0        0     1061 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 kyoslib_py-4.1.0/setup.py
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 kyoslib_py-4.1.0/PKG-INFO
```

### Comparing `kyoslib_py-4.0.2/LICENSE.txt` & `kyoslib_py-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.0.2/README.md` & `kyoslib_py-4.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```python
 from kyoslib_py.simulation import Simulation
 simulation_set = Simulation()
 ```
 
 ## Installation
 
-```pip install kyoslib_py -extra-index-url https://pypi.fury.io/kyos/```
+```pip install kyoslib_py```
 
 ## Dependencies
 
 Python 3.7+
 
 ## Development
```

### Comparing `kyoslib_py-4.0.2/kyoslib_py/forward_curve.py` & `kyoslib_py-4.1.0/kyoslib_py/forward_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         delTypes (list): baseload:1, peak:2, offpeak:3
         grID (int): granularity id of the requested forward curve(e.g. half-hour:1, hour:2, day:3, month:5)
         fullFileName (str): full path of the file(e.g. "./ForwardCurves/ForwardCurveDaily_2_20200101")
 
     Note:
         The current implementation allows to store only data based on monthly granularity.
 
-    Example:
+    Examples:
         >>> from kyoslib_py.forward_curve import write_curve_to_csv
         >>> curves = {}
         >>> data = {}
         >>> month = {}
         >>> baseload = [{'date':'2020-01-01', 'value':20.2}, {'date':'2020-02-01', 'value':30.3}]
         >>> month['baseload'] = baseload
         >>> data['month'] = month
@@ -38,15 +38,14 @@
     elif grID == 5:  # monthly
         curves_df = pd.DataFrame()
         numDelType = len(delTypes)
         # read dates from base load and store in the table, column name should be "0" for the date column
         curves_df['0'] = [x['date'] for x in curves['data']['month']['baseload']]
 
         for i in range(numDelType):
-
             if delTypes[i] == 1:
                 curves_df[str(delTypes[i])] = [
                     x['value'] for x in curves['data']['month']['baseload']
                 ]
             elif delTypes[i] == 2:
                 curves_df[str(delTypes[i])] = [
                     x['value'] for x in curves['data']['month']['peakload']
@@ -57,34 +56,35 @@
                 ]
         # write monthly curves to csv
         curves_df.to_csv(fullFileName, index=False)
     return
 
 
 def get_curve_api(fwdCurveID, granularityID, deliveryTypes, tradingDates, isCSVWrite):
-    """Performs API requests to KYOS API and stores the curve inputs in a generalized format in CSV files or
+    """
+    Performs API requests to KYOS API and stores the curve inputs in a generalized format in CSV files or
     returns a pandas.DataFrame
 
     Args:
         fwdCurveID (int): id of the curve profile
         granularityID (int): half-hour:1, hour:2, day:3, month:5
-        deliveryTypes (list or int): list of delivery type ids(int array), base load:1, peak:2, off-peak:3
+        deliveryTypes (list|int): list of delivery type ids(int array), base load:1, peak:2, off-peak:3
         tradingDates (list): list of trading dates(string array) e.g. ['2019-01-01', '2019-01-02', '2019-01-03']
-        isCSVWrite (bool): indicator of creating csv files, 0 or 1, we will provide  a DataFrame in case of zero.
+        isCSVWrite (bool): indicator of creating csv files, 0 or 1, we will provide a DataFrame in case of zero.
 
     Returns:
         (pandas.DataFrame): Contains all requested curves. If isCSVWrite equals 1 then the dataframe will be empty and
-        the curves will be saved as CSV files on the disk in directory ./ForwardCurves.
+            the curves will be saved as CSV files on the disk in directory ./ForwardCurves.
 
     Note:
         The current implementation allows to read only data based on monthly granularity.
         KYOS API provides the curves with the daylight saving switches for the half-hourly and hourly curves.
         KYOS API supports base load, peak and off-peak delivery types.
 
-    Example:
+    Examples:
         >>> from kyoslib_py.forward_curve import get_curve_api
         >>> arg = {'fwdCurveID': 4, 'granularityID': 5, 'deliveryTypes': [1, 2, 3],
         >>>        'tradingDates': ['2019-01-01', '2019-01-02'], 'isCSVWrite': 1}
         >>> curves_df = get_curve_api(**arg)
         >>> arg = {'fwdCurveID': 4, 'granularityID': 5, 'deliveryTypes': 1 ,
         >>>        'tradingDates': '2019-01-01', 'isCSVWrite': 1}
         >>> curves_df2 = get_curve_api(**arg)
@@ -167,15 +167,14 @@
                     curves_df_i['trading_dates'] = [tradingDate_i for _ in range(numMonths)]
 
                     # read dates from base load and store in the table as delivery dates
                     curves_df_i['delivery_dates'] = [
                         x['date'] for x in data['data']['month']['baseload']
                     ]
                     for i in range(numDelType):
-
                         if deliveryTypes[i] == 1:
                             curves_df_i['baseload'] = [
                                 x['value'] for x in data['data']['month']['baseload']
                             ]
                         elif deliveryTypes[i] == 2:
                             curves_df_i['peak'] = [
                                 x['value'] for x in data['data']['month']['peakload']
```

### Comparing `kyoslib_py-4.0.2/kyoslib_py/front_end.py` & `kyoslib_py-4.1.0/kyoslib_py/front_end.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             yanchor (str) : (Optional) One of ( "auto" | "top" | "middle" | "bottom" ) Sets the title's vertical
                 alignment with respect to its y position. "top" means that the title's cap line is at y. Default:"bottom"
             orientation (str) : (Optional) one of ( "v" | "h" ). Sets the orientation of the legend. Default:"h"
             x (float): (Optional) number between or equal to -2 and 3 Sets the x position (in normalized coordinates)
                 of the legend. KYOS Platform Defaults to 0.1
             y (float): (Optional) number between or equal to -2 and 3 Sets the y position (in normalized coordinates)
                 of the legend. KYOS Platform Defaults to -0.075
-        Example:
+        Examples:
             >>> graph_object = PlatformGraphs()
             >>> fig = px.histogram()
             >>> graph_object.save2disk(fig, filename="001_option_value")
         """
         # legend style same over the whole platform
         # -> styling can be moved to a separate method
         fig.update_layout(
@@ -90,15 +90,15 @@
         bold_row_name (bool): Display the row name in bold font when showing it in the platform front-end
         bold_column_name (bool): Display the column name in bold font when showing it in the platform front-end
         columns_names (None|list): None: use the column names of the dataframe | list of list: user defined columns names (should include name for the row index as well)
 
     Notes:
         The data in the dataframe saved in a csv file in the desired format.
 
-    Example:
+    Examples:
         >>> make_platform_table(data_df, '001_Option_Value', bold_column_name=True)
     """
     current_dir = os.path.dirname(os.path.realpath('__file__'))
     # create output directory
     output_dir = os.path.join(current_dir, 'Output/PlatformDisplay/')
     os.makedirs(output_dir, exist_ok=True)
 
@@ -181,15 +181,15 @@
         output_filename (string): beginning of the name of the output json file. It can be used to order how graphs are
             displayed in the platform. Graph with start of the name "001_" will be displayed first.
 
 
     Note:
         The histogram graph is build using the "Highcharts" package. For more info refer to [HighCharts](https://www.highcharts.com/demo/column-basic)
 
-    Example:
+    Examples:
         >>> make_platform_histogram(values=values, values_names=['Value'],
         >>>                         title='Total Option Value (EUR)',
         >>>                         n_bins=20, output_filename='001_option_value')
     """
     # find bin edges based on all value series.
     bin_edges = np.histogram_bin_edges(values, bins=n_bins, range=None, weights=None)
     bin_means = list()
@@ -273,15 +273,15 @@
 
         unit_name (string): unit name of the values
 
     Note:
         The histogram graph is build using the "Highcharts" package. For more info refer to
         [HighCharts](https://www.highcharts.com/demo/column-basic)
 
-    Example:
+    Examples:
         >>> make_bar_column_chart(values=np.zeros((2,2)), values_names=['series_1', 'series_2'],is_stacked=True,
         >>> x_axis=['2019-01-01', '2019-01-02'], title='Daily Positions', y_axis_title='Positions',
         >>> output_filename='001_option_value', unit_name='Lots')
     """
 
     if x_axis is None:
         x_axis = []
@@ -354,15 +354,15 @@
 
         unit_name (string): unit name of the values
 
     Note:
         The histogram graph is build using the "Highcharts" package. For more info refer to
          [HighCharts](https://www.highcharts.com/demo/column-basic)
 
-    Example:
+    Examples:
         >>> make_basic_line_chart(values=np.zeros((2,2)), values_names=['series_1', 'series_2'],
         >>> x_axis=['2019-01-01', '2019-01-02'], title='Daily Positions', y_axis_title=' ',
         >>> output_filename='001_option_value', unit_name='Lots')
     """
 
     if x_axis is None:
         x_axis = []
```

### Comparing `kyoslib_py-4.0.2/kyoslib_py/historical_price.py` & `kyoslib_py-4.1.0/kyoslib_py/historical_price.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         prices (DataFrame): Pandas dataframe containing the price data. Empty list until loaded with a method (see below).
 
     Notes:
         All historical price profiles contained with the json file in the HistoricalData directory are loaded at the same
         time and stored within the class variable all_price_sources. The path of the subdirectory is also saved as a class
         variable (price_path).
 
-    Example:
+    Examples:
         >>> from kyoslib_py.historical_price import HistoricalPrice
         >>> HistoricalPrice()
         >>> HistoricalPrice.all_price_sources[0].id
         >>> 33
     """
 
     all_price_sources = []
@@ -81,15 +81,15 @@
         """
         Method to load all price data in the associated csv file for a given price source id and store it as a
         DataFrame within the object.
 
         Returns:
             (HistoricalPrice): Instance of the HistoricalPrice class with prices field populated with a DataFrame; date columns are sent as type DateTime.
 
-        Example:
+        Examples:
             >>> from kyoslib_py.historical_price import HistoricalPrice
             >>> HistoricalPrice()
             >>> HistoricalPrice.all_price_sources[0].load_all_prices()
         """
 
         csv_name = 'historical_data_' + str(self.id) + '.csv'
         full_path = self.price_path / csv_name
@@ -129,15 +129,15 @@
                 delivery periods returned if not provided.
             maturity (list, optional): List of maturities for which to return historical prices. Only relevant for forward prices. All
                 maturities returned if not provided
 
         Returns:
             (prices_out): DataFrame of the relevant price data. Returned in same format as the input data, which depends on the data being of type 'forward' or 'spot'.
 
-        Example:
+        Examples:
             --------
             >>> from kyoslib_py.historical_price import HistoricalPrice
             >>> HistoricalPrice()
             >>> HistoricalPrice.all_price_sources[0].get_historical_prices()
             >>> HistoricalPrice.all_price_sources[0].get_historical_prices(start_date=dt.datetime(2019,1,1),
                 delivery_period_id = [1 2])
         """
@@ -218,15 +218,15 @@
             maturity (int, optional): Maturity of requested data. Relevant for forward data only. Can only be used in
                 combination with one product and cannot be used with maturity.
 
         Returns:
             (prices_df): DataFrame of the relevant price data in specific format which varies depending on the data being
                 spot or forward.
 
-        Example:
+        Examples:
             --------
             >>> from kyoslib_py.historical_price import HistoricalPrice as Hp
             >>> prices = Hp.get_historical_prices_api(profile_id=15, price_type='spot')
             >>> prices = Hp.get_historical_prices_api(profile_id=27, price_type='forward', csv_write=True)
             >>> prices = Hp.get_historical_prices_api(profile_id=15, price_type='spot', start_date='2020-07-20',
             >>>                                       end_date='2020-08-01')
 
@@ -256,15 +256,14 @@
 
                 # Combine and store in dataframe
                 spot_data = {'start_delivery': start_del_dates, 'price': spot_prices}
                 final_df = pd.DataFrame(spot_data, columns=['start_delivery', 'price'])
 
             # Forward data
             elif str.casefold(price_type) == 'forward':
-
                 nr_delivery_types = len(input_dict.get('delivery_types'))
                 if nr_delivery_types > 0:
                     del_type_dict = input_dict.get('delivery_types')[
                         0
                     ]  # Dict with high level info
                     fwd_del_type_id = del_type_dict.get('delivery_type_id')
                     dates_list = del_type_dict.get('dates')  # List of dicts
@@ -360,15 +359,14 @@
             elif start and not end:
                 url_options = f'{start}'
             elif not start and end:
                 url_options = f'{end}'
 
         # Filters for forward products
         if str.casefold(price_type) == 'forward':
-
             # Products filter
             if products is not None:
                 prod_str = f'{products[0].lower()}'
                 for p, q in enumerate(products):
                     if p == 0:
                         continue
                     else:
```

### Comparing `kyoslib_py-4.0.2/kyoslib_py/kyos_api.py` & `kyoslib_py-4.1.0/kyoslib_py/kyos_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         When job is running from inside a production container, these variables will be automatically set.
 
         In case of debugging, these need to be set from PyCharm's active configuration, or by executing:
 
         - `$ export EXECUTOR_HASH=8I2817LTWFBKVOPNRI4G7D6TXKGJJHA5XWDDG5CL`
         - `$ export PLATFORM_HOSTNAME=client.kyos.com`
 
-    Example:
+    Examples:
         >>> from kyoslib_py.kyos_api import call_kyos_api_v1
         >>> status, data = call_kyos_api_v1("/commodities?ids=1")
         >>> if 200 >= status < 300:
         >>>     print(data)
         >>> else:
         >>>     print("An error was encountered: ", data)
         '{'data': [{'id': 1, 'name': 'Dutch power'}], 'includes': [], 'relationships': []}'
```

### Comparing `kyoslib_py-4.0.2/kyoslib_py/kyos_utils.py` & `kyoslib_py-4.1.0/kyoslib_py/kyos_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 def dict_merge(initial_dict, *args, overwrite_existing=False):
     """instead of updating only top-level keys, dict_merge recurses down into dicts nested
     to an arbitrary depth, updating keys. The ``merge_dct`` is merged into ``dct``.
 
     Args:
         initial_dict (dict): dict onto which the merge is executed
-        *args: Any number of dictonaries to be merged into initial_dict
+        *args (dict): Any number of dictonaries to be merged into initial_dict
         overwrite_existing (bool): Display the column name in bold font when showing it in the platform front-end
 
     Returns:
         rtn_dct (dict): merged dictonary
 
-    Example:
+    Examples:
         >>> initial = {"accumulator": {"knock_out_price": 150, "trigger_price": 130, "accumulation_price": 110}}
         >>> new_key_dict = {"accumulator": {"sim": {"id": 10}}}
         >>> final = dict_merge(initial, new_key_dict)
         {"accumulator": {"knock_out_price": 150, "trigger_price": 130, "accumulation_price": 110, "sim": {"id": 10}}}
     """
     assert (
         initial_dict is not None and len(args) >= 1
@@ -50,17 +50,18 @@
                     rtn_dct[k] = v
     return rtn_dct
 
 
 def matlab_datenum_to_datetime(datenums) -> list:
     """
     Args:
-        datenums (list or 1d np.array): Vector of matlab datenums
-    Return:
-        (list):
+        datenums (list or 1d np.array): Vector of matlab datenums.
+
+    Returns:
+        (list): List of dates in datetime format.
     """
 
     def datenum_to_datetime_scalar(datenum: float) -> datetime:
         """
         Convert Matlab datenum into Python datetime.
         Args:
              datenum (float): Date in datenum format
@@ -93,24 +94,21 @@
 
 def date_to_mc(date):
     return (date.year - 2000) * 12 + date.month
 
 
 def stop_model(msg):
     """
-    'stop_model' function is used when some problem is encountered and the model should not proceed further
-       because results will be meaningless and computational time wasted.
-    It returns a Status.txt file with the error message. This file can then be picked up by
-       php. The message will be then be displayed in the job status in the platform.
+    Used when a problem is encountered and the model should not proceed further because results
+    will be meaningless and computational time wasted.
+    The function creates a Status.txt file containing the error message. This file is then
+    picked up by PHP to display the error message in the front end.
 
     Args:
         msg (str): Message that defines the error.
-
-    Returns:
-        Status.txt: saves the Status.txt file.
     """
 
     with open('Status.txt', 'w') as fid:
         fid.write(msg)
         fid.close()
 
     print(msg)
```

### Comparing `kyoslib_py-4.0.2/kyoslib_py/settings.py` & `kyoslib_py-4.1.0/kyoslib_py/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class CurrencySet:
     """
     This is the manager object of the currency class. This class loads the set of all available currencies.
     Attributes:
         currencies (list): list of objects
 
-    Example:
+    Examples:
         >>> from kyoslib_py.settings import CurrencySet
         >>> currency_set = CurrencySet.from_csv()
         >>> currency = currency_set.get_currency(1)
         >>> currency.get_name()
         'EUR'
     """
 
@@ -156,15 +156,15 @@
         currency_dir (str): path to the directory
     Return:
         (list):  List of currency objects
 
     Note:
         CSV file called currency.csv must exist within the current working (project) directory. This file contains the relevant currency data.
 
-    Example:
+    Examples:
         >>> from kyoslib_py.settings import make_currency
         >>> currencies = make_currency()
         >>> currencies[0].name
         'EUR'
         >>> next((x for x in currencies if x.get_id() == 2), None)
     """
     # create path to csv file
@@ -183,15 +183,14 @@
 
     Attributes:
            commodities (list): list of objects
 
     """
 
     def __init__(self, dst_file_path: str = './Input/dst_switches.csv'):
-
         dst_file_path = Path(dst_file_path)
         if dst_file_path.exists() and os.stat(dst_file_path).st_size > 0:
             dst_switches_table = pd.read_csv(dst_file_path).values
 
             dst_switches_per_timezone = []
             unique_timezone_ids = np.unique(dst_switches_table[:, 0])
 
@@ -212,15 +211,14 @@
                 dst_switch_values = dst_switches_table[index, 6]
 
                 dst = pd.Series(dst_switch_values)
                 dst.index = dst_moments
 
                 dst_switches_per_timezone.append({"timezone_id": timezone_id, "dst_series": dst})
         else:
-
             dst_switches_per_timezone = [{"timezone_id": 0, "dst_series": pd.Series([])}]
 
         self.dst_switches_per_timezone = dst_switches_per_timezone
 
     def get_dst_moments(self, timezone_id: int) -> pd.Series:
         """
         This method gets the time dependent DST series.
@@ -246,15 +244,15 @@
 class CommoditySet:
     """
     This is the manager object of the commodity class. This class loads the set of all available commodites.
 
     Attributes:
            commodities (list): list of objects
 
-    Example:
+    Examples:
         >>> from kyoslib_py.settings import CommoditySet
         >>> commodity_set = CommoditySet.from_xml()
         >>> commodity = commodity_set.get_commodity(5)
         >>> commodity.get_name()
         'TTF'
     """
 
@@ -289,14 +287,15 @@
     ) -> object:
         """
         This method builds the CommoditySet object from a xml file.
         Args:
             xml_path: path to the xml file with commodity information
             currency_set: kyoslib.CurrencySet object
             calendar_set: kyoslib.CalendarSet object
+            dst_switches_set: object
 
         Returns:
             kyoslib.CommoditySet object
 
         """
         if currency_set is None:
             currency_set = CurrencySet.from_csv()
@@ -459,15 +458,14 @@
         IsDefaultGroupUnit: bool,
         CarbonContent: float,
         TimezoneId: int,
         TimezoneOffsetMinutes: int,
         TradablePeriod: int,
         dst_switches: pd.Series,
     ):
-
         self.id = ID
         self.name = Name
         self.is_cent = IsCent
         self.currency = currency
         self.unit_id = UnitID
         self.energy_content = Energy  # measured in Joules
         self.group_id = GroupID
@@ -788,30 +786,29 @@
 def make_commodity(
     xml_folder: str = None,
     xml_path: str = 'PrototypeSettings.xml',
     currencies: list = None,
     json_path: str = None,
     commodity_info_list: list = None,
 ) -> list:
-
     """
     Returns a list of all available commodity objects in the input xml file generated by the KYOS platform
 
     Parameters:
         xml_path (str): Full path to xml file including name
 
     Return:
         (list): List of commodity objects
 
     Note:
         XML settings file called KyPythonSettings.xml must exist within the current working (project) directory. This file
         contains the commodity information.
         The make_currency function should be run before make_commodity
 
-    Example:
+    Examples:
         >>> from kyoslib_py.settings import make_commodity
         >>> commodity_set = make_commodity()
         >>> commodity_set[0].group_name
         'power'
         >>> next((x for x in commodity_set if x.id == 5), None)
     """
     # create path to xml file
@@ -837,15 +834,14 @@
         >>> from kyoslib_py.settings import DeliveryTypeSet
         >>> delivery_types = DeliveryTypeSet.from_xml(xml_node=commodity_node, calendar_set=calendar_set)
         >>> baseload = delivery_types.get_delivery_type(1)
 
     """
 
     def __init__(self, delivery_type_info_list: list = None) -> object:
-
         if delivery_type_info_list is None:
             # to be done, raise error
             return
 
         self.delivery_types = [
             DeliveryType(**delivery_type_info) for delivery_type_info in delivery_type_info_list
         ]
@@ -881,15 +877,14 @@
         return DeliveryTypeSet(delivery_type_info_list)
 
     @staticmethod
     def from_json(json_key: dict = None, calendar_set: object = None):
         all_delivery_types = json_key
         delivery_type_info_list = []
         for delivery_type_dict in all_delivery_types:
-
             delivery_moments = delivery_type_dict['Days']
 
             delivery_type_info = dict()
             delivery_type_info['ID'] = delivery_type_dict['ID']
             calendar_id = delivery_type_dict['CalendarID']
 
             delivery_type_info['Calendar'] = None
@@ -1112,15 +1107,14 @@
         >>> calendar_set = CalendarSet.from_xml()
         >>> calendar = calendar_set.get_calendar(1)
         >>> calendar.get_name()
         'NL'
     """
 
     def __init__(self, calendar_info_list: list = None):
-
         if calendar_info_list is None:
             # to be done raise error
             return
 
         self.calendars = [Calendar(**calendar_info) for calendar_info in calendar_info_list]
 
     # from {data_type} methods
```

### Comparing `kyoslib_py-4.0.2/kyoslib_py/simulation.py` & `kyoslib_py-4.1.0/kyoslib_py/simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class SimulationError(Exception):
     """Capture errors which occurred using the kyoslib_py.simulation module.
 
     Attributes:
         message (str): explanation of the error
 
-    Example:
+    Examples:
         >>> raise SimulationError(message='Error reading currencies!')
         >>>
         >>> try:
                 simulation_spot_daily = simulation_obj.get_spot(comm_name='TTF')
             except SimulationError as err:
                 print(err)
             finally:
@@ -50,15 +50,15 @@
         commodities (list): List of all the relevant Commodity objects associated with this simulation job
         model_currency (Currency): the KySim model currency
         base_currency (Currency): the base currency of the Kyos Platfom
         spot_folder (str): Path to the folder containing the spot simulation outputs of the KySim job
         forward_folder (str): Path to the folder containing the forward simulation outputs of the KySim job
         power_spot_granul (int): Integer representing the granularity of spot simulations (daily only, hourly, half-hourly or quarter-hourly)
 
-    Example:
+    Examples:
         >>> from kyoslib_py.simulation import Simulation
         >>> simulation_obj = Simulation.from_xml()
         >>> simulation_obj.get_nr_simulations()
         100
         >>> simulation_obj.model_currency.get_name()
         'GBP'
     """
@@ -71,15 +71,15 @@
             kysim_info (dict): dictionary with all the simulations properties expected keys: \n
                 -> SpotSimFolder(str): Path to the folder containing the spot simulation outputs of the KySim job \n
                 -> FwdSimFolder(str): Path to the folder containing the forward simulation outputs of the KySim job \n
                 -> OtherSimFolder(str): Path to the folder containing the other simulation outputs of the KySim job \n
                 -> TradingDate(datetime): Datetime object of the trading date on which the simulation job was based \n
                 -> PowerSpotGranularity(int): Integer representing the granularity of spot simulations (daily only, hourly, half-hourly or quarter-hourly) \n
                 -> EndDate(datetime): Datetime object of the end date of the simulations \n
-                -> NrSimulations(int):  Number of simulations \n
+                -> NrSimulations(int): Number of simulations \n
                 -> ModelCurrency(kyoslib_py.settings.Currency object): The KySim model currency \n
                 -> BaseCurrency(kyoslib_py.settings.Currency): The base currency of the Kyos Platform \n
                 -> curve_info (dict): with commodity_id, fwd_curve_id, spot_source_id per simulated commodity \n
             currency_set (CurrencySet): available currencies; the set should contain at least all currencies related to
                 the simulation profile
             commodity_set (CommoditySet): available commodities; the set should contain at least all simulated commodities.
         """
@@ -121,21 +121,22 @@
     def from_xml(
         xml_path='./PrototypeSettings.xml', currency_set=None, commodity_set=None
     ) -> object:
         """
         This static method builds de simulation class object from a xml file.
 
         Args:
-            xml_path: path to the xml file with KySimInfo
-            currency_set: kyoslib_py.CurrencySet object
-            commodity_set: kyoslib_py.Commodity object
+            xml_path (str): Path to the xml file with KySimInfo
+            currency_set (CurrencySet): Contains all relevant information relative to currencies
+                and currency conversions.
+            commodity_set (CommoditySet): Contains all relevant information relative to
+                commodity settings.
 
         Returns:
-            kyoslib_py.Simulation object
-
+            (Simulation): kyoslib_py.Simulation object
         """
         if currency_set is None:
             currency_set = CurrencySet.from_csv()
 
         if commodity_set is None:
             commodity_set = CommoditySet.from_xml(currency_set=currency_set)
 
@@ -319,15 +320,15 @@
                 retrieved if the requested commodity belongs to the 'carbon' group. Defaults to true.
 
         Returns:
             (pandas.DataFrame): Dataframe containing the individual simulations per column where each row represents a unique time period
             e.g. day or hour. If the granularity is below daily, then the first column represents the average across the
             simulations.
 
-        Example:
+        Examples:
             >>> from kyoslib_py.simulation import Simulation
             >>> simulation_obj = Simulation()
             >>> simulation_spot_daily = simulation_obj.get_spot(commodity_name='NBP', delivery_period_name='daily',
                                                     start_date=dt.datetime(2020, 1, 1), end_date=dt.datetime(2020, 1, 31),
                                                 currency_name = 'EUR', del_type_id = 1, carbon_floor = False)
             >>> simulation_spot_daily = simulation_obj.get_spot(commodity_name='TTF')
             >>> implied_forward_curve = simulation_spot_daily.mean(axis =1)
@@ -567,15 +568,15 @@
 
             carbon_floor (bool, optional): Indicates whether the carbon floor adjusted spot simulations should be
                 retrieved if the requested commodity belongs to the 'carbon' group.
 
         Returns:
             pandas.DataFrame: Dataframe containing the individual simulations per column where each row represents a unique day.
 
-        Example:
+        Examples:
             >>> from kyoslib_py.simulation import Simulation
             >>> simulation_obj = Simulation()
             >>> monthly_forward_prices = simulation_obj.get_fwd_product(commodity_name = 'TTF', fwd_year = 2020, fwd_month = 11,
                                                                         start_date=dt.datetime(2020, 1, 1), end_date =
                                                                         dt.datetime(2020, 10, 31), currency_name = 'EUR',
                                                                         del_type_id=1, carbon_floor=False)
             >>> monthly_forward_prices = simulation_obj.get_fwd_product(commodity_name = 'TTF', fwd_year = 2020, fwd_month = 11)
@@ -623,15 +624,14 @@
             )
         elif delivery_period_id == 4 or (
             delivery_period_id == 5
             and fwd_year == valuation_date.year
             and fwd_month == valuation_date.month
             and (group_name.lower() == 'power' or group_name.lower() == 'gas')
         ):
-
             if delivery_type_name == '':
                 file_path = sim_spot_dir.joinpath("BOM_" + commodity_name + ".mat")
             else:
                 file_path = sim_spot_dir.joinpath(
                     "BOM_" + commodity_name + '_' + delivery_type_name + ".mat"
                 )
 
@@ -653,15 +653,14 @@
             trading_date = pd.to_datetime(bom_prices[:, 0] - 719529, unit='D')
             index = (simulated_trading_dates[0] <= trading_date) & (
                 trading_date <= simulated_trading_dates[-1]
             )
             fwd_sims = bom_prices[index, 3:]
 
         else:
-
             product_start_mc = (fwd_year - 2000) * 12 + fwd_month
             if delivery_period_id == 5:  # month
                 product_end_mc = product_start_mc
             elif delivery_period_id == 6:  # quarter
                 product_end_mc = product_start_mc + 2
             elif delivery_period_id == 7:  # season
                 product_end_mc = product_start_mc + 5
@@ -868,15 +867,14 @@
             fwd_sims = prices[index, 3:]
 
         elif delivery_period_id == 4 or (
             delivery_period_id == 5
             and maturity == 0
             and (group_name.lower() == 'power' or group_name.lower() == 'gas')
         ):
-
             if delivery_type_name == '':
                 file_path = sim_spot_dir.joinpath("BOM_" + commodity_name + ".mat")
             else:
                 file_path = sim_spot_dir.joinpath(
                     "BOM_" + commodity_name + '_' + delivery_type_name + ".mat"
                 )
 
@@ -1060,29 +1058,29 @@
         dst: bool = True,
     ) -> pd.DataFrame:
         """
         A Simulation class method to import forward curves used in the simulations.
 
         Args:
             commodity_name (str): Name of the commodity for which the forward curve it to be imported, as matching that given in the XML settings file.
-            delivery_period_name (str): Curve granularity requested. hourly,daily and monthly supported.
+            delivery_period_name (str): Curve granularity requested. half-hourly, hourly, daily and monthly supported.
             start_date (datetime, optional): Start date from which to begin the imported forward curve.
             end_date (datetime, optional): Date at which the imported forward curve will end (inclusive of this date).
             del_type_id (int, optional): ID number of the delivery type of the required forward curve as defined on the KYOS platform i.e. 1 = baseload, 2 = peakload, 3 = offpeak. Only available for monthly curves.
             dst (bool, optional): Returns an hourly curve with Daylight Savings Time switches included (with missing hour and/or averaged double hour) if True, otherwise non-DST curve is outputted. Defaults to true; only meaningful with hourly (power) curves.
 
         Returns:
             pandas.DataFrame: Dataframe containing the forward curve prices, where each row represents a new time period corresponding to
             the granularity supplied.
 
         Note:
             Forward curve are always imported in the currency of the commodity (which may be different from the model
             currency)
 
-        Example:
+        Examples:
             >>> from kyoslib_py.simulation import Simulation
             >>> simulation_obj = Simulation()
             >>> hourly_fwd_curve = simulation_obj.get_fwd_curve(commodity_name = 'UK Power', delivery_period_name = 'hourly',
                                         start_date = None, end_date = None, del_type_id = 1, dst = True)
             >>> daily_fwd_curve = simulation_obj.get_fwd_curve(commodity_name = 'TTF', delivery_period_name = 'daily')
         """
 
@@ -1138,14 +1136,118 @@
 
         if del_type_id != 1 and commodity_group != 'power':
             raise SimulationError(
                 message='Delivery type specified not available for this commodity type. '
                 'Curve with standard (baseload) delivery will be returned'
             )
 
+        if delivery_period_name == 'quarter-hour' and dst is True:
+            curve_file_name = 'ForwardCurveQuarterHourlyDST' + filename_end + '.csv'
+            fwd_curve_path = subfolder_fwd_curve_path.joinpath(curve_file_name)
+            try:
+                forward_curve_csv = pd.read_csv(
+                    fwd_curve_path, sep=';', header=None, names=['date', 'quarter-hour', 'value']
+                )
+            except:
+                raise SimulationError(
+                    message='Curve requested not found. Please check the path and trading date to confirm the requested curve'
+                    ' exists'
+                )
+
+            forward_curve_csv.index.name = 'date'
+            melted_curve = forward_curve_csv.reset_index().melt(
+                id_vars='date', var_name='quarter_hour', value_name='value'
+            )
+            melted_curve = melted_curve.set_index("date")
+            melted_curve['datetime'] = pd.to_datetime(melted_curve.index) + pd.to_timedelta(
+                melted_curve["quarter_hour"] * 15, unit='m'
+            )
+            melted_curve = melted_curve.set_index('datetime')['value'].sort_index()
+            forward_curve_df = pd.DataFrame(melted_curve.loc[start_date:end_date])
+
+        if delivery_period_name == 'quarter-hour' and dst is False:
+            curve_file_name = 'ForwardCurveQuarterHourlyNoDST' + filename_end + '.csv'
+            fwd_curve_path = subfolder_fwd_curve_path.joinpath(curve_file_name)
+            try:
+                forward_curve_csv = pd.read_csv(fwd_curve_path, sep=';', header=None)
+            except:
+                raise SimulationError(
+                    message="Curve requested not found. Please check the path and trading date to confirm the requested curve exists"
+                )
+
+            curve_array = forward_curve_csv.to_numpy()
+            first_date = dt.datetime.strptime(curve_array[0, 0], "%Y-%m-%d")
+            last_date = dt.datetime.strptime(curve_array[-1, 0], "%Y-%m-%d")
+            # Creating timedeltas with a stepsize of 15 minutes
+            date_list = [
+                first_date + dt.timedelta(minutes=15 * x)
+                for x in range(0, ((last_date - first_date).days * 24 + 24) * 4)
+            ]
+            date_list = pd.DataFrame(date_list)
+            quarter_hourly_prices = pd.DataFrame(forward_curve_csv[2])
+            data_for_concat = [date_list, quarter_hourly_prices]
+            forward_curve_csv = pd.concat(
+                data_for_concat, axis=1
+            )  # Concatenate date_list and quarter_hour_prices
+            forward_curve_csv.columns = ['date', 'values']
+            forward_curve_csv.set_index(forward_curve_csv['date'], inplace=True)
+            forward_curve_csv.drop(columns=['date'], inplace=True)
+            forward_curve_df = pd.DataFrame(forward_curve_csv.loc[start_date:end_date])
+
+        if delivery_period_name == 'halfhourly' and dst is True:
+            curve_file_name = 'ForwardCurveHalfHourly' + filename_end + '.csv'
+            fwd_curve_path = subfolder_fwd_curve_path.joinpath(curve_file_name)
+            try:
+                forward_curve_csv = pd.read_csv(fwd_curve_path, sep=';', header=None, index_col=0)
+            except:
+                raise SimulationError(
+                    message='Curve requested not found. Please check the path and trading date to confirm the requested curve'
+                    ' exists'
+                )
+
+            forward_curve_csv.index.name = 'date'
+            melted_curve = forward_curve_csv.reset_index().melt(
+                id_vars='date', var_name='half_hour', value_name='value'
+            )
+            melted_curve = melted_curve.set_index("date")
+            melted_curve['datetime'] = pd.to_datetime(melted_curve.index) + pd.to_timedelta(
+                melted_curve["half_hour"] * 30, unit='m'
+            )
+            melted_curve = melted_curve.set_index('datetime')['value'].sort_index()
+
+            forward_curve_df = pd.DataFrame(melted_curve.loc[start_date:end_date])
+
+        if delivery_period_name == 'halfhourly' and dst is False:
+            curve_file_name = 'ForwardCurveHalfHourlyNoDST' + filename_end + '.csv'
+            fwd_curve_path = subfolder_fwd_curve_path.joinpath(curve_file_name)
+            try:
+                forward_curve_csv = pd.read_csv(fwd_curve_path, sep=';', header=None)
+            except:
+                raise SimulationError(
+                    message="Curve requested not found. Please check the path and trading date to confirm the requested curve exists"
+                )
+            curve_array = forward_curve_csv.to_numpy()
+            first_date = dt.datetime.strptime(curve_array[0, 0], "%Y-%m-%d")
+            last_date = dt.datetime.strptime(curve_array[-1, 0], "%Y-%m-%d")
+            # Creating timedeltas with a stepsize of 30 minutes
+            date_list = [
+                first_date + dt.timedelta(minutes=30 * x)
+                for x in range(0, ((last_date - first_date).days * 24 + 24) * 2)
+            ]
+            date_list = pd.DataFrame(date_list)
+            half_hourly_prices = pd.DataFrame(forward_curve_csv[2])
+            data_for_concat = [date_list, half_hourly_prices]
+            forward_curve_csv = pd.concat(
+                data_for_concat, axis=1
+            )  # Concatenate date_list and hourly_prices
+            forward_curve_csv.columns = ['date', 'values']
+            forward_curve_csv.set_index(forward_curve_csv['date'], inplace=True)
+            forward_curve_csv.drop(columns=['date'], inplace=True)
+            forward_curve_df = pd.DataFrame(forward_curve_csv.loc[start_date:end_date])
+
         if delivery_period_name == 'hourly' and dst is True:
             curve_file_name = 'ForwardCurveHourlyDST' + filename_end + '.csv'
             fwd_curve_path = subfolder_fwd_curve_path.joinpath(curve_file_name)
             try:
                 forward_curve_csv = pd.read_csv(
                     fwd_curve_path, sep=';', header=None, names=['date', 'hour', 'value']
                 )
@@ -1156,14 +1258,15 @@
                 )
             hours_delta = pd.to_timedelta(forward_curve_csv.iloc[:, 1].values, unit='h')
             forward_curve_csv.iloc[:, 0] = pd.to_datetime(forward_curve_csv.iloc[:, 0])
             forward_curve_csv.iloc[:, 0] = forward_curve_csv.iloc[:, 0] + hours_delta
             forward_curve_csv.set_index(forward_curve_csv['date'], inplace=True)
             forward_curve_csv.drop(columns=['date', 'hour'], inplace=True)
             forward_curve_df = pd.DataFrame(forward_curve_csv.loc[start_date:end_date])
+
         if delivery_period_name == 'hourly' and dst is False:
             curve_file_name = 'ForwardCurveHourly' + filename_end + '.csv'
             fwd_curve_path = subfolder_fwd_curve_path.joinpath(curve_file_name)
             try:
                 forward_curve_csv = pd.read_csv(fwd_curve_path, sep=';', header=None)
             except:
                 raise SimulationError(
@@ -1200,14 +1303,29 @@
                 SimulationError(
                     message="Curve requested not found. Please check the path and trading date to confirm the requested curve exists"
                 )
             forward_curve_csv.iloc[:, 0] = pd.to_datetime(forward_curve_csv.iloc[:, 0])
             forward_curve_csv.set_index(forward_curve_csv.iloc[:, 0], inplace=True)
             forward_curve_csv.drop(columns=['date'], inplace=True)
             forward_curve_df = pd.DataFrame(forward_curve_csv.loc[start_date:end_date])
+        if delivery_period_name == 'daily':
+            curve_file_name = 'ForwardCurveDaily' + filename_end + '.csv'
+            fwd_curve_path = subfolder_fwd_curve_path.joinpath(curve_file_name)
+            try:
+                forward_curve_csv = pd.read_csv(
+                    fwd_curve_path, sep=';', header=None, names=['date', 'value']
+                )
+            except:
+                SimulationError(
+                    message="Curve requested not found. Please check the path and trading date to confirm the requested curve exists"
+                )
+            forward_curve_csv.iloc[:, 0] = pd.to_datetime(forward_curve_csv.iloc[:, 0])
+            forward_curve_csv.set_index(forward_curve_csv.iloc[:, 0], inplace=True)
+            forward_curve_csv.drop(columns=['date'], inplace=True)
+            forward_curve_df = pd.DataFrame(forward_curve_csv.loc[start_date:end_date])
         if delivery_period_name == 'monthly':
             curve_file_name = 'ForwardCurveMonthly' + filename_end + '.csv'
             fwd_curve_path = subfolder_fwd_curve_path.joinpath(curve_file_name)
             if commodity_group == 'power':
                 try:
                     forward_curve_csv = pd.read_csv(
                         fwd_curve_path, sep=';', header=None, names=['date', '1', '2', '3']
@@ -1239,28 +1357,27 @@
     def get_fx(
         self,
         term_currency_id: int,
         base_currency_id: int = None,
         start_date: datetime = None,
         end_date: datetime = None,
     ) -> pd.DataFrame:
-
         """
         Get the daily FX simulated prices in a given period. The FX base currency is by default the KySim model currency,
             but can be adjusted via the base_currency_id argument.
 
         Args:
             term_currency_id: The currency id to which you want to convert the prices.
             base_currency_id (optional, int): id of the base currency. By default, this is the model currency id
             start_date (datetime, optional): Start date from which to begin importing the fx simulations.
             end_date (datetime, optional): End date until which the simulated fx prices are to be imported.
         Returns:
             pd.DataFrame: Dataframe containing the daily simulated prices, datetime as index and the fx per simulation in the columns.
 
-        Example:
+        Examples:
                    >>> from kyoslib_py.simulation import Simulation
                    >>> simulation_obj = Simulation()
                    >>> fx_sims = simulation_set.get_fx(2)
         """
         model_currency = self.get_model_currency()
         model_currency_id = model_currency.get_id()
         if base_currency_id is None:
@@ -1312,15 +1429,14 @@
                     + ' could not be loaded!'
                 )
                 raise SimulationError(message=msg)
             # [matlab datenum, sim_1, sim_2, ...]
             return fx_matrix
 
         if base_currency_id == model_currency_id:
-
             fx_matrix = load_fx(forward_folder_path, model_currency_name, term_currency_name)
         elif term_currency_id == model_currency_id:
             fx_matrix = load_fx(forward_folder_path, term_currency_name, base_currency_name)
             fx_matrix[:, 1:] = 1 / fx_matrix[:, 1:]
 
         else:
             # we need to get two fx and compute the requested fx
@@ -1372,15 +1488,15 @@
             pandas.DataFrame: Dataframe containing the simulated prices, where each row represents a time period corresponding to
             the delivery_period supplied.
 
         Assumption:
           - All "values" are consecutive (no gaps in time steps).
           - Currently, the method can convert only from/to the KySim model currency
 
-        Example:
+        Examples:
             >>> from kyoslib_py.simulation import Simulation
             >>> simulation_obj = Simulation()
             >>> fwd_sims = simulation_set.get_fwd_product(commodity_name='TTF', fwd_year=2021, fwd_month=5)
             >>> simulation_set.convert_fx(simulation_prices=fwd_sims, delivery_period_name='monthly', from_currency_id=1, to_currency_id=2)
         """
         # copy the pd.dataframe, so that will not manipulate the input data
         simulation_prices = simulation_prices.copy()
@@ -1456,28 +1572,28 @@
         """
         A Simulation class method to import weather/volume/renewable simulations.
 
         Args:
             series_type (srting - choice between "weather" / "volume" / "renewable"): Type of the simulations.
                 Volume and Weather simulations supported. Renewable is also a volume sim, it comes from recently introduced
                 Renewable Asset object, which is a wrapper for holding more information related to Weather & Volume.
-            series_identifier (int/string):
+            series_identifier (int|string):
                 if series_type = "weather" => (int) the id of the historical weather time-series used by KySim
                 if series_type = "volume" => (string) the user defined (in KySim) of the simulated volume simulations
                 if series_type = "renewable" => (int) the user defined (in KySim) Renewable Asset id
             delivery_period_name (str): Curve delivery_period requested. Hourly and Daily supported.
             start_date (datetime, optional): Start date from which to begin the imported weather/volume simulations.
             end_date (datetime, optional): End date at which the imported weather/volume simulations will end (inclusive of this date).
 
         Returns:
             pandas.DataFrame: ``(weather_volume_simulations) Size: (start_date:end_date, NumSim+1)``
                 Containing the individual simulations per column where each row
                 represents a unique day/hour. The first column represents the average of the weather/volume simulations
 
-        Example:
+        Examples:
             >>> from kyoslib_py.simulation import Simulation
             >>> import datetime as dt
             >>> simulation_obj = Simulation()
             >>> start_date = dt.datetime(2020, 3, 24)
             >>> end_date = dt.datetime(2020, 12, 31, 23)
             >>> volume_simulations = simulation_obj.get_weather_volume_sim(series_identifier = "Dutch_Offshore",
             >>>                                                            delivery_period_name = 'Hourly', series_type = 'Volume',
@@ -1533,15 +1649,14 @@
                 if delivery_period_name.lower() == 'hourly':
                     # Declare input file name and the path
                     inputFilePath = sim_other_dir.joinpath(
                         'WeatherSimsHourly_' + 'Series' + str(series_identifier) + '.mat'
                     )
                     # Import Hourly Weather Simulations
                     try:
-
                         f = h5py.File(inputFilePath, 'r')
                         raw_data = f['WeatherSimsHourly'][()].T
                         raw_data = pd.DataFrame(raw_data)
                     except:
                         raise SimulationError(
                             message='Hourly weather simulations for the requested series id could not'
                             ' be found'
@@ -1549,15 +1664,14 @@
                 elif delivery_period_name.lower() == 'daily':
                     # Declare input file name and the path
                     inputFilePath = sim_other_dir.joinpath(
                         'WeatherSimsDaily_' + 'Series' + str(series_identifier) + '.mat'
                     )
                     # Import Daily Weather Simulations
                     try:
-
                         f = h5py.File(inputFilePath, 'r')
                         raw_data = f['WeatherSimsDaily'][()].T
                         raw_data = pd.DataFrame(raw_data)
                     except:
                         raise SimulationError(
                             message='Daily weather simulations for the requested series id could not'
                             ' be found'
@@ -1708,15 +1822,14 @@
             start_delivery_mc (np.array): vector of month codes of the start delivery month
             end_delivery_mc (np.array): vector of month codes of the end delivery month
             month_codes (np.array): vector of month codes
             month_sims (np.array): three-dimensional array with
 
         Returns:
             fwd_sims (np.array):  2d vector (days, simulations) of days on the rows and simulations in the columns
-
         """
 
         @jit(nopython=True, parallel=True)
         def weight_sims_by_hours(nr_months, month_sims, hours_delivery_month):
             for i in range(nr_months):
                 month_sims[:, :, i] = month_sims[:, :, i] * hours_delivery_month[i]
             return month_sims
```

### Comparing `kyoslib_py-4.0.2/kyoslib_py/tradable_product.py` & `kyoslib_py-4.1.0/kyoslib_py/tradable_product.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.0.2/kyoslib_py/valuation_interface.py` & `kyoslib_py-4.1.0/kyoslib_py/valuation_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         values (numpy array): 2D numpy array containing the data values
         simulations (list): A list of instances of the SimulationData class, which contain specifically simulation data.
 
     Note:
         Note that only the parameters of the constructor are assigned to the object when called, and the other attributes
         are populated using the set_data method.
 
-    Example:
+    Examples:
         >>> from kyoslib_py.valuation_interface
         >>> this_comm_data = CommData(commodity_id=2, forward_curve_id=33, currency_id=1,
                                 granularity=5)
         >>> this_comm_data.commodity_id =
         2
     """
 
@@ -144,15 +144,15 @@
         dates (numpy array): 1D numpy array containing the dates of the data values
         values (numpy array): 2D numpy array containing the data values
 
     Note:
         Note that only the parameters of the constructor are assigned to the object when called, and the other attributes
         are populated using the set_data method.
 
-    Example:
+    Examples:
         >>> from kyoslib_py.valuation_interface
         >>> this_sim_data = SimulationData(csv_filename='example.csv', type_output=['simulation'],
             type_calculation = ['simulation'] , dates=date_array, values=simulation_array)
     """
 
     def __init__(self, csv_filename, type_output, type_calculation, dates=None, values=None):
         """
@@ -185,15 +185,15 @@
         data (list): List which holds instances of the CommData class
         extra_model_data (dict): model specific information
 
     Note:
         Only one DataInterface can be constructed at a time. Each new instance of the class is appended to the list class
         variable all_interfaces
 
-    Example:
+    Examples:
         >>> from kyoslib_py.valuation_interface import ValuationInterface
         >>> import datetime as dt
         >>> contract_output = ValuationInterface(model_name='Accumulator',
         >>>                                      trading_date=dt.datetime(2020, 1, 1),
         >>>                                      folder ='/Output', profile_id=13))
         >>> print(contract_output.model_name)
         >>> 'Accumulator'
@@ -260,15 +260,15 @@
             type_calculation (list): List with length one containing a string indicating the type of calculations associated with the simulations
             dates (numpy array, optional): 1D numpy array containing the dates of the data values
             values (numpy array, optional): 2D numpy array containing the data values
 
         Returns:
             (ValuationInterface): Instance of the ValuationInterface class object with CommData and/or SimulationData class instances appended
 
-        Example:
+        Examples:
             >>> import numpy as np
             >>> import datetime as dt
             >>> from kyoslib_py.valuation_interface import ValuationInterface
             >>> contract_output = ValuationInterface(model_name='Accumulator',
             >>>                                      trading_date=dt.datetime(2020, 1, 1),
             >>>                                      folder ='/Output', profile_id=13))
             >>> volume_dates = np.array([dt.datetime(2020,1,1), dt.datetime(2020,2,1),
@@ -506,15 +506,15 @@
         The export_data method exports data for the relevant commodity into csv files and a single JSON files that
         describes the relevant data.
 
         Args:
             commodity_id (int, optional):
                 Commodity ID of the data to be exported. If not provided, all data is exported to csv and JSON.
 
-        Example:
+        Examples:
             >>> import numpy as np
             >>> import datetime as dt
             >>> from kyoslib_py.valuation_interface import ValuationInterface
             >>> contract_output = ValuationInterface(model_name='Accumulator',
             >>>                                      trading_date=dt.datetime(2020, 1, 1),
             >>>                                      folder ='/Output', profile_id=13))
             >>> volume_dates = np.array([dt.datetime(2020,1,1), dt.datetime(2020,2,1),
@@ -637,15 +637,15 @@
         The metadata is saved ina file called 'metadata.json'.
         The metadata has a specific format, and it is used to pass extra data identifying an asset.
         Please contact KYOS for more information on the metadata.
 
         Args:
             input_folder (str): Full path of directory where the metadata.json file is located, without trailing file separator
 
-        Example:
+        Examples:
             >>> from kyoslib_py.valuation_interface import ValuationInterface
             >>> contract_output = ValuationInterface(model_name='Accumulator',
             >>>                                      trading_date=dt.datetime(2020, 1, 1),
             >>>                                      folder ='/Output', profile_id=13))
             >>> contract_output.set_metadata('/metadata_folder')
         """
 
@@ -705,15 +705,15 @@
         Args:
             data (dict):  a dictinary which conatins model specific information. e.g. accumulator object
             overwrite (bool): True, clear the dictonariy and append the new input,
                               False, append new input to the existing dictonary
         Returns:
             (ValuationInterface): Instance of the ValuationInterface class object with extra model data
 
-        Example:
+        Examples:
             >>> import datetime as dt
             >>> from kyoslib_py.valuation_interface import ValuationInterface
             >>> contract_output = ValuationInterface(model_name='KyAccumulator',
             >>>                                      trading_date=dt.datetime(2020, 1, 1),
             >>>                                      folder ='/Output', profile_id=13)
             >>> extraInfo = {"accumulator": {"knock_out_price" : 150, "trigger_price": 130, "accumulation_price": 110}}
             >>> contract_output.set_extra_model_data(data=extraInfo)
```

### Comparing `kyoslib_py-4.0.2/pyproject.toml` & `kyoslib_py-4.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.poetry]
 name = "kyoslib_py"
-version = "4.0.2"
+version = "4.1.0"
 description = "KYOS shared lib code as python package"
 authors = ["KYOS <support@kyos.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/kyosenergy/kyoslib_py"
 documentation = "https://kyosenergy.github.io/kyoslib_py/"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.10"
 numpy = "<1.22.1"
-pandas = "<1.5.3"
+pandas = "<1.5.4"
 requests = "^2.28.1"
 h5py = "^3.6.0"
 numba = "0.56.4"
 plotly = "^5.7.0"
+mkdocstrings-python = "^0.8.2"
 
 [tool.poetry.dev-dependencies]
-invoke = "^1.7.1"
-pytest = "^7.2"
+invoke = "^2.0.0"
+pytest = "^7.3"
 pytest-cov = "^4.0.0"
-black = "^22.12"
+black = "^23.3.0"
 isort = "^5.8.0"
 safety = "^2.0.0"
-mkdocs-material = "^8.3.2"
-mkdocstrings = "^0.18.1"
+mkdocs-material = "^9.1.6"
+mkdocstrings = "^0.19.1"
 darglint = "^1.8.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `kyoslib_py-4.0.2/setup.py` & `kyoslib_py-4.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 ['kyoslib_py']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['h5py>=3.6.0,<4.0.0',
+ 'mkdocstrings-python>=0.8.2,<0.9.0',
  'numba==0.56.4',
  'numpy<1.22.1',
- 'pandas<1.5.3',
+ 'pandas<1.5.4',
  'plotly>=5.7.0,<6.0.0',
  'requests>=2.28.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['run_model = src.entry:main']}
 
 setup_kwargs = {
     'name': 'kyoslib-py',
-    'version': '4.0.2',
+    'version': '4.1.0',
     'description': 'KYOS shared lib code as python package',
-    'long_description': "# kyoslib_py\n\n## Usage\n\nExample code:\n\n```python\nfrom kyoslib_py.simulation import Simulation\nsimulation_set = Simulation()\n```\n\n## Installation\n\n```pip install kyoslib_py -extra-index-url https://pypi.fury.io/kyos/```\n\n## Dependencies\n\nPython 3.7+\n\n## Development\n\nThis project is executing CI checks using **GitHub actions**.\n\nIt will run `pytest` and `black`.\n\n### Invoking development tasks\n\n[Invoke](https://www.pyinvoke.org/) is used for development tasks.\n\nTasks are stored in `tasks.py` and are executable using the `inv[oke]` command line tool.\n\nTo see the list of tasks, you can type:\n\n```bash\ninv --list\n```\n\nFor example, before your commits, you should run\n```bash\ninv format\n```\nto format your code.\n\n## Documentation\n\nThe package documentation is generated by MkDocs. The correct version can be installed in the project's virtual environment by:\n\n```bash\npoetry install\n```\n\nThen the documentation can be built, and a server to view it started by:\n\n```bash\nmkdocs serve\n```\n",
+    'long_description': "# kyoslib_py\n\n## Usage\n\nExample code:\n\n```python\nfrom kyoslib_py.simulation import Simulation\nsimulation_set = Simulation()\n```\n\n## Installation\n\n```pip install kyoslib_py```\n\n## Dependencies\n\nPython 3.7+\n\n## Development\n\nThis project is executing CI checks using **GitHub actions**.\n\nIt will run `pytest` and `black`.\n\n### Invoking development tasks\n\n[Invoke](https://www.pyinvoke.org/) is used for development tasks.\n\nTasks are stored in `tasks.py` and are executable using the `inv[oke]` command line tool.\n\nTo see the list of tasks, you can type:\n\n```bash\ninv --list\n```\n\nFor example, before your commits, you should run\n```bash\ninv format\n```\nto format your code.\n\n## Documentation\n\nThe package documentation is generated by MkDocs. The correct version can be installed in the project's virtual environment by:\n\n```bash\npoetry install\n```\n\nThen the documentation can be built, and a server to view it started by:\n\n```bash\nmkdocs serve\n```\n",
     'author': 'KYOS',
     'author_email': 'support@kyos.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://github.com/kyosenergy/kyoslib_py',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `kyoslib_py-4.0.2/PKG-INFO` & `kyoslib_py-4.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: kyoslib-py
-Version: 4.0.2
+Version: 4.1.0
 Summary: KYOS shared lib code as python package
 Home-page: http://github.com/kyosenergy/kyoslib_py
 License: MIT
 Author: KYOS
 Author-email: support@kyos.com
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: h5py (>=3.6.0,<4.0.0)
+Requires-Dist: mkdocstrings-python (>=0.8.2,<0.9.0)
 Requires-Dist: numba (==0.56.4)
 Requires-Dist: numpy (<1.22.1)
-Requires-Dist: pandas (<1.5.3)
+Requires-Dist: pandas (<1.5.4)
 Requires-Dist: plotly (>=5.7.0,<6.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://kyosenergy.github.io/kyoslib_py/
 Project-URL: Repository, http://github.com/kyosenergy/kyoslib_py
 Description-Content-Type: text/markdown
 
 # kyoslib_py
@@ -31,15 +32,15 @@
 ```python
 from kyoslib_py.simulation import Simulation
 simulation_set = Simulation()
 ```
 
 ## Installation
 
-```pip install kyoslib_py -extra-index-url https://pypi.fury.io/kyos/```
+```pip install kyoslib_py```
 
 ## Dependencies
 
 Python 3.7+
 
 ## Development
```

