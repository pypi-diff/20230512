# Comparing `tmp/pystlouisfed-2.1.0.tar.gz` & `tmp/pystlouisfed-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\tomas.koutek\code\stlouisfed\dist\tmp3_yqeepd\pystlouisfed-2.1.0.tar", last modified: Wed Feb  9 10:44:17 2022, max compression
+gzip compressed data, was "C:\Users\tomas.koutek\code\stlouisfed\dist\.tmp-deq5709_\pystlouisfed-2.1.1.tar", last modified: Fri May 12 09:09:31 2023, max compression
```

## Comparing `pystlouisfed-2.1.0.tar` & `pystlouisfed-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/
--rw-rw-rw-   0        0        0     1087 2022-01-18 20:25:15.000000 pystlouisfed-2.1.0/LICENSE
--rw-rw-rw-   0        0        0    22503 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    20869 2022-02-07 14:47:38.000000 pystlouisfed-2.1.0/README.md
--rw-rw-rw-   0        0        0       91 2022-01-17 20:33:49.000000 pystlouisfed-2.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/pystlouisfed/
--rw-rw-rw-   0        0        0      537 2022-02-09 10:05:12.000000 pystlouisfed-2.1.0/pystlouisfed/__init__.py
--rw-rw-rw-   0        0        0   178876 2022-02-09 10:06:35.000000 pystlouisfed-2.1.0/pystlouisfed/client.py
--rw-rw-rw-   0        0        0    11919 2022-01-20 21:54:24.000000 pystlouisfed-2.1.0/pystlouisfed/enums.py
--rw-rw-rw-   0        0        0     3234 2022-01-17 21:23:59.000000 pystlouisfed-2.1.0/pystlouisfed/models.py
-drwxrwxrwx   0        0        0        0 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/pystlouisfed.egg-info/
--rw-rw-rw-   0        0        0    22503 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/pystlouisfed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/pystlouisfed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/pystlouisfed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/pystlouisfed.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/pystlouisfed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-02-09 10:44:17.000000 pystlouisfed-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2248 2022-02-09 10:05:12.000000 pystlouisfed-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:09:31.000000 pystlouisfed-2.1.1/
+-rw-rw-rw-   0        0        0     1087 2022-01-18 20:25:15.000000 pystlouisfed-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0    22421 2023-05-12 09:09:31.000000 pystlouisfed-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20791 2023-05-12 07:38:47.000000 pystlouisfed-2.1.1/README.md
+-rw-rw-rw-   0        0        0       91 2022-01-17 20:33:49.000000 pystlouisfed-2.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-12 09:09:31.000000 pystlouisfed-2.1.1/pystlouisfed/
+-rw-rw-rw-   0        0        0      537 2023-05-12 08:59:32.000000 pystlouisfed-2.1.1/pystlouisfed/__init__.py
+-rw-rw-rw-   0        0        0   179118 2023-05-12 09:00:17.000000 pystlouisfed-2.1.1/pystlouisfed/client.py
+-rw-rw-rw-   0        0        0    11919 2022-01-20 21:54:24.000000 pystlouisfed-2.1.1/pystlouisfed/enums.py
+-rw-rw-rw-   0        0        0     3282 2022-02-16 16:08:19.000000 pystlouisfed-2.1.1/pystlouisfed/models.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:09:31.000000 pystlouisfed-2.1.1/pystlouisfed.egg-info/
+-rw-rw-rw-   0        0        0    22421 2023-05-12 09:09:30.000000 pystlouisfed-2.1.1/pystlouisfed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-05-12 09:09:31.000000 pystlouisfed-2.1.1/pystlouisfed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 09:09:30.000000 pystlouisfed-2.1.1/pystlouisfed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-05-12 09:09:30.000000 pystlouisfed-2.1.1/pystlouisfed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-12 09:09:30.000000 pystlouisfed-2.1.1/pystlouisfed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 09:09:31.000000 pystlouisfed-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2248 2023-05-12 07:38:47.000000 pystlouisfed-2.1.1/setup.py
```

### Comparing `pystlouisfed-2.1.0/LICENSE` & `pystlouisfed-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pystlouisfed-2.1.0/PKG-INFO` & `pystlouisfed-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystlouisfed
-Version: 2.1.0
+Version: 2.1.1
 Summary: Federal Reserve Bank of St. Louis - FRED, ALFRED, GeoFRED and FRASER
 Home-page: https://github.com/TomasKoutek/pystlouisfed
 Download-URL: https://github.com/TomasKoutek/pystlouisfed.git
 Author: Tomas Koutek
 Author-email: 66636b6f6666@gmail.com
 Maintainer: Tomas Koutek
 License: MIT
@@ -115,15 +115,15 @@
 other methods return `pandas.DataFrame`
 For example method `FRED.category_series` (all series for a specific category)
 
 ```python
 from pystlouisfed import FRED
 
 fred = FRED(api_key='abcdefghijklmnopqrstuvwxyz123456')
-df = fred.category_series(category_id=125).head()
+df = fred.category_series(category_id=125)
 
 print(df.head())
 ```
 
 ```
         realtime_start realtime_end                                              title observation_start observation_end  frequency frequency_short                units units_short      seasonal_adjustment seasonal_adjustment_short              last_updated  popularity  group_popularity                                              notes
 id                                                                                                                                                                                                                                                                                                                                                
@@ -213,28 +213,28 @@
 
 FRED (ALFRED) has many different parameters, which are not the same for each method. So there is no need to remember everything or keep looking at the documentation.
 `pystlouisfed` uses the [Enums](https://tomaskoutek.github.io/pystlouisfed/enums.html) constants. For example, the API endpoint FRED:series_observations (and
 method `FRED.series_observations`) has the optional parameters
 "units", "frequency", "aggregation_method" or "output_type":
 
 ```
-    def series_observations(
-            self,
-            series_id: str,
-            realtime_start: date = date.today(),
-            realtime_end: date = date.today(),
-            sort_order: enums.SortOrder = enums.SortOrder.asc,
-            observation_start: date = date(1776, 7, 4),
-            observation_end: date = date(9999, 12, 31),
-            units: enums.Unit = enums.Unit.lin,
-            frequency: enums.Frequency = None,
-            aggregation_method: enums.AggregationMethod = enums.AggregationMethod.average,
-            output_type: enums.OutputType = enums.OutputType.realtime_period,
-            vintage_dates: List[str] = None
-    ) -> pd.DataFram:
+def series_observations(
+        self,
+        series_id: str,
+        realtime_start: date = None,
+        realtime_end: date = None,
+        sort_order: enums.SortOrder = enums.SortOrder.asc,
+        observation_start: date = date(1776, 7, 4),
+        observation_end: date = date(9999, 12, 31),
+        units: enums.Unit = enums.Unit.lin,
+        frequency: enums.Frequency = None,
+        aggregation_method: enums.AggregationMethod = enums.AggregationMethod.average,
+        output_type: enums.OutputType = enums.OutputType.realtime_period,
+        vintage_dates: List[str] = None
+) -> pd.DataFrame:
 ```
 
 But what should be the value? For example, for the parameter "aggregation_method" it is possible to use `pystlouisfed.AggregationMethod`:
 
 ```python
 from enum import Enum
 
@@ -477,9 +477,7 @@
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 
-
-
```

### Comparing `pystlouisfed-2.1.0/README.md` & `pystlouisfed-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 other methods return `pandas.DataFrame`
 For example method `FRED.category_series` (all series for a specific category)
 
 ```python
 from pystlouisfed import FRED
 
 fred = FRED(api_key='abcdefghijklmnopqrstuvwxyz123456')
-df = fred.category_series(category_id=125).head()
+df = fred.category_series(category_id=125)
 
 print(df.head())
 ```
 
 ```
         realtime_start realtime_end                                              title observation_start observation_end  frequency frequency_short                units units_short      seasonal_adjustment seasonal_adjustment_short              last_updated  popularity  group_popularity                                              notes
 id                                                                                                                                                                                                                                                                                                                                                
@@ -177,28 +177,28 @@
 
 FRED (ALFRED) has many different parameters, which are not the same for each method. So there is no need to remember everything or keep looking at the documentation.
 `pystlouisfed` uses the [Enums](https://tomaskoutek.github.io/pystlouisfed/enums.html) constants. For example, the API endpoint FRED:series_observations (and
 method `FRED.series_observations`) has the optional parameters
 "units", "frequency", "aggregation_method" or "output_type":
 
 ```
-    def series_observations(
-            self,
-            series_id: str,
-            realtime_start: date = date.today(),
-            realtime_end: date = date.today(),
-            sort_order: enums.SortOrder = enums.SortOrder.asc,
-            observation_start: date = date(1776, 7, 4),
-            observation_end: date = date(9999, 12, 31),
-            units: enums.Unit = enums.Unit.lin,
-            frequency: enums.Frequency = None,
-            aggregation_method: enums.AggregationMethod = enums.AggregationMethod.average,
-            output_type: enums.OutputType = enums.OutputType.realtime_period,
-            vintage_dates: List[str] = None
-    ) -> pd.DataFram:
+def series_observations(
+        self,
+        series_id: str,
+        realtime_start: date = None,
+        realtime_end: date = None,
+        sort_order: enums.SortOrder = enums.SortOrder.asc,
+        observation_start: date = date(1776, 7, 4),
+        observation_end: date = date(9999, 12, 31),
+        units: enums.Unit = enums.Unit.lin,
+        frequency: enums.Frequency = None,
+        aggregation_method: enums.AggregationMethod = enums.AggregationMethod.average,
+        output_type: enums.OutputType = enums.OutputType.realtime_period,
+        vintage_dates: List[str] = None
+) -> pd.DataFrame:
 ```
 
 But what should be the value? For example, for the parameter "aggregation_method" it is possible to use `pystlouisfed.AggregationMethod`:
 
 ```python
 from enum import Enum
```

### Comparing `pystlouisfed-2.1.0/pystlouisfed/__init__.py` & `pystlouisfed-2.1.1/pystlouisfed/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 from pystlouisfed.client import FRED, ALFRED, GeoFRED, FRASER
 from pystlouisfed.enums import SortOrder, TagGroupID, FilterVariable, Seasonality, FilterValue, OrderBy, Unit, Frequency, AggregationMethod, OutputType, SearchType, RegionType, ShapeType
 from pystlouisfed.models import Release, Category, Shape, Source, Series, SeriesGroup
 
 __pdoc__ = {
     'client.Client': False,
```

### Comparing `pystlouisfed-2.1.0/pystlouisfed/client.py` & `pystlouisfed-2.1.1/pystlouisfed/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5747,5434 +5747,5449 @@
 00016720: 656d 7074 793a 0d0a 2020 2020 2020 2020  empty:..        
 00016730: 2020 2020 6466 5b64 6174 655f 636f 6c75      df[date_colu
 00016740: 6d6e 735d 203d 2064 665b 6461 7465 5f63  mns] = df[date_c
 00016750: 6f6c 756d 6e73 5d2e 6170 706c 7928 7064  olumns].apply(pd
 00016760: 2e74 6f5f 6461 7465 7469 6d65 2c20 666f  .to_datetime, fo
 00016770: 726d 6174 3d27 2559 2d25 6d2d 2564 2729  rmat='%Y-%m-%d')
 00016780: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00016790: 6466 203d 2064 662e 6173 7479 7065 2864  df = df.astype(d
-000167a0: 7479 7065 3d7b 0d0a 2020 2020 2020 2020  type={..        
-000167b0: 2020 2020 2020 2020 276e 616d 6527 3a20          'name': 
-000167c0: 2773 7472 696e 6727 2c0d 0a20 2020 2020  'string',..     
-000167d0: 2020 2020 2020 2020 2020 2027 6c69 6e6b             'link
-000167e0: 273a 2027 7374 7269 6e67 272c 0d0a 2020  ': 'string',..  
-000167f0: 2020 2020 2020 2020 2020 2020 2020 2770                'p
-00016800: 7265 7373 5f72 656c 6561 7365 273a 2027  ress_release': '
-00016810: 626f 6f6c 270d 0a20 2020 2020 2020 2020  bool'..         
-00016820: 2020 207d 292e 7365 745f 696e 6465 7828     }).set_index(
-00016830: 2769 6427 290d 0a0d 0a20 2020 2020 2020  'id')....       
-00016840: 2072 6574 7572 6e20 6466 0d0a 0d0a 2020   return df....  
-00016850: 2020 6465 6620 7365 7269 6573 5f73 6561    def series_sea
-00016860: 7263 6828 0d0a 2020 2020 2020 2020 2020  rch(..          
-00016870: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-00016880: 2020 2020 2073 6561 7263 685f 7465 7874       search_text
-00016890: 3a20 7374 722c 0d0a 2020 2020 2020 2020  : str,..        
-000168a0: 2020 2020 7365 6172 6368 5f74 7970 653a      search_type:
-000168b0: 2065 6e75 6d73 2e53 6561 7263 6854 7970   enums.SearchTyp
-000168c0: 6520 3d20 656e 756d 732e 5365 6172 6368  e = enums.Search
-000168d0: 5479 7065 2e66 756c 6c5f 7465 7874 2c0d  Type.full_text,.
-000168e0: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
-000168f0: 6c74 696d 655f 7374 6172 743a 2064 6174  ltime_start: dat
-00016900: 6520 3d20 4e6f 6e65 2c0d 0a20 2020 2020  e = None,..     
-00016910: 2020 2020 2020 2072 6561 6c74 696d 655f         realtime_
-00016920: 656e 643a 2064 6174 6520 3d20 4e6f 6e65  end: date = None
-00016930: 2c0d 0a20 2020 2020 2020 2020 2020 206f  ,..            o
-00016940: 7264 6572 5f62 793a 2065 6e75 6d73 2e4f  rder_by: enums.O
-00016950: 7264 6572 4279 203d 204e 6f6e 652c 0d0a  rderBy = None,..
-00016960: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-00016970: 5f6f 7264 6572 3a20 656e 756d 732e 536f  _order: enums.So
-00016980: 7274 4f72 6465 7220 3d20 4e6f 6e65 2c0d  rtOrder = None,.
-00016990: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-000169a0: 7465 725f 7661 7269 6162 6c65 3a20 656e  ter_variable: en
-000169b0: 756d 732e 4669 6c74 6572 5661 7269 6162  ums.FilterVariab
-000169c0: 6c65 203d 204e 6f6e 652c 0d0a 2020 2020  le = None,..    
-000169d0: 2020 2020 2020 2020 6669 6c74 6572 5f76          filter_v
-000169e0: 616c 7565 3a20 656e 756d 732e 4669 6c74  alue: enums.Filt
-000169f0: 6572 5661 6c75 6520 3d20 4e6f 6e65 2c0d  erValue = None,.
-00016a00: 0a20 2020 2020 2020 2020 2020 2074 6167  .            tag
-00016a10: 5f6e 616d 6573 3a20 4c69 7374 5b73 7472  _names: List[str
-00016a20: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-00016a30: 2020 2020 2020 2065 7863 6c75 6465 5f74         exclude_t
-00016a40: 6167 5f6e 616d 6573 3a20 4c69 7374 5b73  ag_names: List[s
-00016a50: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
-00016a60: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
-00016a70: 653a 0d0a 2020 2020 2020 2020 2222 220d  e:..        """.
-00016a80: 0a20 2020 2020 2020 2023 2320 5061 7261  .        ## Para
-00016a90: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
-00016aa0: 6073 6561 7263 685f 7465 7874 600d 0a20  `search_text`.. 
-00016ab0: 2020 2020 2020 2054 6865 2077 6f72 6473         The words
-00016ac0: 2074 6f20 6d61 7463 6820 6167 6169 6e73   to match agains
-00016ad0: 7420 6563 6f6e 6f6d 6963 2064 6174 6120  t economic data 
-00016ae0: 7365 7269 6573 2e0d 0a0d 0a20 2020 2020  series.....     
-00016af0: 2020 2060 7365 6172 6368 5f74 7970 6560     `search_type`
-00016b00: 0d0a 2020 2020 2020 2020 4465 7465 726d  ..        Determ
-00016b10: 696e 6573 2074 6865 2074 7970 6520 6f66  ines the type of
-00016b20: 2073 6561 7263 6820 746f 2070 6572 666f   search to perfo
-00016b30: 726d 2e0d 0a0d 0a20 2020 2020 2020 2060  rm.....        `
-00016b40: 7265 616c 7469 6d65 5f73 7461 7274 600d  realtime_start`.
-00016b50: 0a20 2020 2020 2020 2054 6865 2073 7461  .        The sta
-00016b60: 7274 206f 6620 7468 6520 7265 616c 2d74  rt of the real-t
-00016b70: 696d 6520 7065 7269 6f64 2e20 466f 7220  ime period. For 
-00016b80: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-00016b90: 2c20 7365 6520 5b52 6561 6c2d 5469 6d65  , see [Real-Time
-00016ba0: 2050 6572 696f 6473 5d28 6874 7470 733a   Periods](https:
-00016bb0: 2f2f 6672 6564 2e73 746c 6f75 6973 6665  //fred.stlouisfe
-00016bc0: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
-00016bd0: 7265 642f 7265 616c 7469 6d65 5f70 6572  red/realtime_per
-00016be0: 696f 642e 6874 6d6c 292e 0d0a 0d0a 2020  iod.html).....  
-00016bf0: 2020 2020 2020 6072 6561 6c74 696d 655f        `realtime_
-00016c00: 656e 6460 0d0a 2020 2020 2020 2020 5468  end`..        Th
-00016c10: 6520 656e 6420 6f66 2074 6865 2072 6561  e end of the rea
-00016c20: 6c2d 7469 6d65 2070 6572 696f 642e 2046  l-time period. F
-00016c30: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00016c40: 696f 6e2c 2073 6565 205b 5265 616c 2d54  ion, see [Real-T
-00016c50: 696d 6520 5065 7269 6f64 735d 2868 7474  ime Periods](htt
-00016c60: 7073 3a2f 2f66 7265 642e 7374 6c6f 7569  ps://fred.stloui
-00016c70: 7366 6564 2e6f 7267 2f64 6f63 732f 6170  sfed.org/docs/ap
-00016c80: 692f 6672 6564 2f72 6561 6c74 696d 655f  i/fred/realtime_
-00016c90: 7065 7269 6f64 2e68 746d 6c29 2e0d 0a0d  period.html)....
-00016ca0: 0a20 2020 2020 2020 2060 6f72 6465 725f  .        `order_
-00016cb0: 6279 600d 0a20 2020 2020 2020 204f 7264  by`..        Ord
-00016cc0: 6572 2072 6573 756c 7473 2062 7920 7661  er results by va
-00016cd0: 6c75 6573 206f 6620 7468 6520 7370 6563  lues of the spec
-00016ce0: 6966 6965 6420 6174 7472 6962 7574 652e  ified attribute.
-00016cf0: 0d0a 0d0a 2020 2020 2020 2020 6073 6f72  ....        `sor
-00016d00: 745f 6f72 6465 7260 0d0a 2020 2020 2020  t_order`..      
-00016d10: 2020 536f 7274 2072 6573 756c 7473 2069    Sort results i
-00016d20: 7320 6173 6365 6e64 696e 6720 6f72 2064  s ascending or d
-00016d30: 6573 6365 6e64 696e 6720 6f72 6465 7220  escending order 
-00016d40: 666f 7220 6174 7472 6962 7574 6520 7661  for attribute va
-00016d50: 6c75 6573 2073 7065 6369 6669 6564 2062  lues specified b
-00016d60: 7920 6f72 6465 725f 6279 2e0d 0a0d 0a20  y order_by..... 
-00016d70: 2020 2020 2020 2060 6669 6c74 6572 5f76         `filter_v
-00016d80: 6172 6961 626c 6560 0d0a 2020 2020 2020  ariable`..      
-00016d90: 2020 5468 6520 6174 7472 6962 7574 6520    The attribute 
-00016da0: 746f 2066 696c 7465 7220 7265 7375 6c74  to filter result
-00016db0: 7320 6279 2e0d 0a0d 0a20 2020 2020 2020  s by.....       
-00016dc0: 2060 6669 6c74 6572 5f76 616c 7565 600d   `filter_value`.
-00016dd0: 0a20 2020 2020 2020 2054 6865 2076 616c  .        The val
-00016de0: 7565 206f 6620 7468 6520 6669 6c74 6572  ue of the filter
-00016df0: 5f76 6172 6961 626c 6520 6174 7472 6962  _variable attrib
-00016e00: 7574 6520 746f 2066 696c 7465 7220 7265  ute to filter re
-00016e10: 7375 6c74 7320 6279 2e0d 0a0d 0a20 2020  sults by.....   
-00016e20: 2020 2020 2060 7461 675f 6e61 6d65 7360       `tag_names`
-00016e30: 0d0a 2020 2020 2020 2020 4120 7365 6d69  ..        A semi
-00016e40: 636f 6c6f 6e20 6465 6c69 6d69 7465 6420  colon delimited 
-00016e50: 6c69 7374 206f 6620 7461 6720 6e61 6d65  list of tag name
-00016e60: 7320 7468 6174 2073 6572 6965 7320 6d61  s that series ma
-00016e70: 7463 6820 616c 6c20 6f66 2e0d 0a0d 0a20  tch all of..... 
-00016e80: 2020 2020 2020 2060 6578 636c 7564 655f         `exclude_
-00016e90: 7461 675f 6e61 6d65 7360 0d0a 2020 2020  tag_names`..    
-00016ea0: 2020 2020 4120 7365 6d69 636f 6c6f 6e20      A semicolon 
-00016eb0: 6465 6c69 6d69 7465 6420 6c69 7374 206f  delimited list o
-00016ec0: 6620 7461 6720 6e61 6d65 7320 7468 6174  f tag names that
-00016ed0: 2073 6572 6965 7320 6d61 7463 6820 6e6f   series match no
-00016ee0: 6e65 206f 662e 0d0a 0d0a 2020 2020 2020  ne of.....      
-00016ef0: 2020 2323 2044 6573 6372 6970 7469 6f6e    ## Description
-00016f00: 0d0a 2020 2020 2020 2020 6874 7470 733a  ..        https:
-00016f10: 2f2f 6672 6564 2e73 746c 6f75 6973 6665  //fred.stlouisfe
-00016f20: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
-00016f30: 7265 642f 7365 7269 6573 5f73 6561 7263  red/series_searc
-00016f40: 682e 6874 6d6c 0d0a 0d0a 2020 2020 2020  h.html....      
-00016f50: 2020 4765 7420 6563 6f6e 6f6d 6963 2064    Get economic d
-00016f60: 6174 6120 7365 7269 6573 2074 6861 7420  ata series that 
-00016f70: 6d61 7463 6820 7365 6172 6368 2074 6578  match search tex
-00016f80: 742e 0d0a 0d0a 2020 2020 2020 2020 2323  t.....        ##
-00016f90: 2041 5049 2052 6571 7565 7374 2028 4854   API Request (HT
-00016fa0: 5450 5320 4745 5429 0d0a 2020 2020 2020  TPS GET)..      
-00016fb0: 2020 6874 7470 733a 2f2f 6170 692e 7374    https://api.st
-00016fc0: 6c6f 7569 7366 6564 2e6f 7267 2f66 7265  louisfed.org/fre
-00016fd0: 642f 7365 7269 6573 2f73 6561 7263 683f  d/series/search?
-00016fe0: 7365 6172 6368 5f74 6578 743d 6d6f 6e65  search_text=mone
-00016ff0: 7461 7279 2b73 6572 7669 6365 2b69 6e64  tary+service+ind
-00017000: 6578 2661 7069 5f6b 6579 3d61 6263 6465  ex&api_key=abcde
-00017010: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
-00017020: 7677 7879 7a31 3233 3435 3626 6669 6c65  vwxyz123456&file
-00017030: 5f74 7970 653d 6a73 6f6e 0d0a 0d0a 2020  _type=json....  
-00017040: 2020 2020 2020 2323 2041 5049 2052 6573        ## API Res
-00017050: 706f 6e73 650d 0a20 2020 2020 2020 2060  ponse..        `
-00017060: 6060 6a73 6f6e 0d0a 2020 2020 2020 2020  ``json..        
-00017070: 7b0d 0a20 2020 2020 2020 2020 2022 7265  {..          "re
-00017080: 616c 7469 6d65 5f73 7461 7274 223a 2022  altime_start": "
-00017090: 3230 3137 2d30 382d 3031 222c 0d0a 2020  2017-08-01",..  
-000170a0: 2020 2020 2020 2020 2272 6561 6c74 696d          "realtim
-000170b0: 655f 656e 6422 3a20 2232 3031 372d 3038  e_end": "2017-08
-000170c0: 2d30 3122 2c0d 0a20 2020 2020 2020 2020  -01",..         
-000170d0: 2022 6f72 6465 725f 6279 223a 2022 7365   "order_by": "se
-000170e0: 6172 6368 5f72 616e 6b22 2c0d 0a20 2020  arch_rank",..   
-000170f0: 2020 2020 2020 2022 736f 7274 5f6f 7264         "sort_ord
-00017100: 6572 223a 2022 6465 7363 222c 0d0a 2020  er": "desc",..  
-00017110: 2020 2020 2020 2020 2263 6f75 6e74 223a          "count":
-00017120: 2033 322c 0d0a 2020 2020 2020 2020 2020   32,..          
-00017130: 226f 6666 7365 7422 3a20 302c 0d0a 2020  "offset": 0,..  
-00017140: 2020 2020 2020 2020 226c 696d 6974 223a          "limit":
-00017150: 2031 3030 302c 0d0a 2020 2020 2020 2020   1000,..        
-00017160: 2020 2273 6572 6965 7373 223a 205b 0d0a    "seriess": [..
-00017170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017180: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00017190: 2020 2020 2022 6964 223a 2022 4d53 494d       "id": "MSIM
-000171a0: 3222 2c0d 0a20 2020 2020 2020 2020 2020  2",..           
-000171b0: 2020 2020 2020 2022 7265 616c 7469 6d65         "realtime
-000171c0: 5f73 7461 7274 223a 2022 3230 3137 2d30  _start": "2017-0
-000171d0: 382d 3031 222c 0d0a 2020 2020 2020 2020  8-01",..        
-000171e0: 2020 2020 2020 2020 2020 2272 6561 6c74            "realt
-000171f0: 696d 655f 656e 6422 3a20 2232 3031 372d  ime_end": "2017-
-00017200: 3038 2d30 3122 2c0d 0a20 2020 2020 2020  08-01",..       
-00017210: 2020 2020 2020 2020 2020 2022 7469 746c             "titl
-00017220: 6522 3a20 224d 6f6e 6574 6172 7920 5365  e": "Monetary Se
-00017230: 7276 6963 6573 2049 6e64 6578 3a20 4d32  rvices Index: M2
-00017240: 2028 7072 6566 6572 7265 6429 222c 0d0a   (preferred)",..
-00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017260: 2020 226f 6273 6572 7661 7469 6f6e 5f73    "observation_s
-00017270: 7461 7274 223a 2022 3139 3637 2d30 312d  tart": "1967-01-
-00017280: 3031 222c 0d0a 2020 2020 2020 2020 2020  01",..          
-00017290: 2020 2020 2020 2020 226f 6273 6572 7661          "observa
-000172a0: 7469 6f6e 5f65 6e64 223a 2022 3230 3133  tion_end": "2013
-000172b0: 2d31 322d 3031 222c 0d0a 2020 2020 2020  -12-01",..      
-000172c0: 2020 2020 2020 2020 2020 2020 2266 7265              "fre
-000172d0: 7175 656e 6379 223a 2022 4d6f 6e74 686c  quency": "Monthl
-000172e0: 7922 2c0d 0a20 2020 2020 2020 2020 2020  y",..           
-000172f0: 2020 2020 2020 2022 6672 6571 7565 6e63         "frequenc
-00017300: 795f 7368 6f72 7422 3a20 224d 222c 0d0a  y_short": "M",..
-00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017320: 2020 2275 6e69 7473 223a 2022 4269 6c6c    "units": "Bill
-00017330: 696f 6e73 206f 6620 446f 6c6c 6172 7322  ions of Dollars"
-00017340: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00017350: 2020 2020 2022 756e 6974 735f 7368 6f72       "units_shor
-00017360: 7422 3a20 2242 696c 2e20 6f66 2024 222c  t": "Bil. of $",
-00017370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017380: 2020 2020 2273 6561 736f 6e61 6c5f 6164      "seasonal_ad
-00017390: 6a75 7374 6d65 6e74 223a 2022 5365 6173  justment": "Seas
-000173a0: 6f6e 616c 6c79 2041 646a 7573 7465 6422  onally Adjusted"
-000173b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000173c0: 2020 2020 2022 7365 6173 6f6e 616c 5f61       "seasonal_a
-000173d0: 646a 7573 746d 656e 745f 7368 6f72 7422  djustment_short"
-000173e0: 3a20 2253 4122 2c0d 0a20 2020 2020 2020  : "SA",..       
-000173f0: 2020 2020 2020 2020 2020 2022 6c61 7374             "last
-00017400: 5f75 7064 6174 6564 223a 2022 3230 3134  _updated": "2014
-00017410: 2d30 312d 3137 2030 373a 3136 3a34 342d  -01-17 07:16:44-
-00017420: 3036 222c 0d0a 2020 2020 2020 2020 2020  06",..          
-00017430: 2020 2020 2020 2020 2270 6f70 756c 6172          "popular
-00017440: 6974 7922 3a20 3334 2c0d 0a20 2020 2020  ity": 34,..     
-00017450: 2020 2020 2020 2020 2020 2020 2022 6772               "gr
-00017460: 6f75 705f 706f 7075 6c61 7269 7479 223a  oup_popularity":
-00017470: 2033 332c 0d0a 2020 2020 2020 2020 2020   33,..          
-00017480: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
-00017490: 2022 5468 6520 4d53 4920 6d65 6173 7572   "The MSI measur
-000174a0: 6520 7468 6520 666c 6f77 206f 6620 6d6f  e the flow of mo
-000174b0: 6e65 7461 7279 2073 6572 7669 6365 7320  netary services 
-000174c0: 7265 6365 6976 6564 2065 6163 6820 7065  received each pe
-000174d0: 7269 6f64 2062 7920 686f 7573 6568 6f6c  riod by househol
-000174e0: 6473 2061 6e64 2066 6972 6d73 2066 726f  ds and firms fro
-000174f0: 6d20 7468 6569 7220 686f 6c64 696e 6773  m their holdings
-00017500: 206f 6620 6d6f 6e65 7461 7279 2061 7373   of monetary ass
-00017510: 6574 7320 286c 6576 656c 7320 6f66 2074  ets (levels of t
-00017520: 6865 2069 6e64 6578 6573 2061 7265 2073  he indexes are s
-00017530: 6f6d 6574 696d 6573 2072 6566 6572 7265  ometimes referre
-00017540: 6420 746f 2061 7320 4469 7669 7369 6120  d to as Divisia 
-00017550: 6d6f 6e65 7461 7279 2061 6767 7265 6761  monetary aggrega
-00017560: 7465 7329 2e5c 5c6e 5072 6566 6572 7265  tes).\\nPreferre
-00017570: 6420 6265 6e63 686d 6172 6b20 7261 7465  d benchmark rate
-00017580: 2065 7175 616c 7320 3130 3020 6261 7369   equals 100 basi
-00017590: 7320 706f 696e 7473 2070 6c75 7320 7468  s points plus th
-000175a0: 6520 6c61 7267 6573 7420 7261 7465 2069  e largest rate i
-000175b0: 6e20 7468 6520 7365 7420 6f66 2072 6174  n the set of rat
-000175c0: 6573 2e5c 5c6e 416c 7465 726e 6174 6976  es.\\nAlternativ
-000175d0: 6520 6265 6e63 686d 6172 6b20 7261 7465  e benchmark rate
-000175e0: 2065 7175 616c 7320 7468 6520 6c61 7267   equals the larg
-000175f0: 6572 206f 6620 7468 6520 7072 6566 6572  er of the prefer
-00017600: 7265 6420 6265 6e63 686d 6172 6b20 7261  red benchmark ra
-00017610: 7465 2061 6e64 2074 6865 2042 6161 2063  te and the Baa c
-00017620: 6f72 706f 7261 7465 2062 6f6e 6420 7969  orporate bond yi
-00017630: 656c 642e 5c5c 6e4d 6f72 6520 696e 666f  eld.\\nMore info
-00017640: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
-00017650: 6520 6e65 7720 4d53 4920 6361 6e20 6265  e new MSI can be
-00017660: 2066 6f75 6e64 2061 745c 5c6e 6874 7470   found at\\nhttp
-00017670: 3a2f 2f72 6573 6561 7263 682e 7374 6c6f  ://research.stlo
-00017680: 7569 7366 6564 2e6f 7267 2f6d 7369 2f69  uisfed.org/msi/i
-00017690: 6e64 6578 2e68 746d 6c2e 220d 0a20 2020  ndex.html."..   
-000176a0: 2020 2020 2020 2020 2020 2020 207d 2c0d               },.
-000176b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000176c0: 202e 2e2e 0d0a 2020 2020 2020 2020 2020   .....          
-000176d0: 2020 5d0d 0a20 2020 2020 2020 207d 0d0a    ]..        }..
-000176e0: 2020 2020 2020 2020 6060 600d 0a0d 0a20          ```.... 
-000176f0: 2020 2020 2020 2023 2320 5265 7475 726e         ## Return
-00017700: 730d 0a20 2020 2020 2020 2060 7061 6e64  s..        `pand
-00017710: 6173 2e44 6174 6146 7261 6d65 600d 0a0d  as.DataFrame`...
-00017720: 0a20 2020 2020 2020 2023 2320 4578 616d  .        ## Exam
-00017730: 706c 650d 0a20 2020 2020 2020 2060 6060  ple..        ```
-00017740: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
-00017750: 3e3e 3e20 6672 6564 203d 2046 5245 4428  >>> fred = FRED(
-00017760: 6170 695f 6b65 793d 2761 6263 6465 6667  api_key='abcdefg
-00017770: 6869 6a6b 6c6d 6e6f 7071 7273 7475 7677  hijklmnopqrstuvw
-00017780: 7879 7a31 3233 3435 3627 290d 0a20 2020  xyz123456')..   
-00017790: 2020 2020 203e 3e3e 2066 7265 642e 7365       >>> fred.se
-000177a0: 7269 6573 5f73 6561 7263 6828 7365 6172  ries_search(sear
-000177b0: 6368 5f74 6578 743d 276d 6f6e 6574 6172  ch_text='monetar
-000177c0: 7920 7365 7276 6963 6520 696e 6465 7827  y service index'
-000177d0: 292e 6865 6164 2829 0d0a 2020 2020 2020  ).head()..      
-000177e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000177f0: 616c 7469 6d65 5f73 7461 7274 2072 6561  altime_start rea
-00017800: 6c74 696d 655f 656e 6420 2020 2020 2020  ltime_end       
-00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017830: 2020 2020 2074 6974 6c65 206f 6273 6572       title obser
-00017840: 7661 7469 6f6e 5f73 7461 7274 206f 6273  vation_start obs
-00017850: 6572 7661 7469 6f6e 5f65 6e64 2066 7265  ervation_end fre
-00017860: 7175 656e 6379 2066 7265 7175 656e 6379  quency frequency
-00017870: 5f73 686f 7274 2020 2020 2020 2020 2020  _short          
-00017880: 2020 2020 2020 756e 6974 7320 756e 6974        units unit
-00017890: 735f 7368 6f72 7420 2073 6561 736f 6e61  s_short  seasona
-000178a0: 6c5f 6164 6a75 7374 6d65 6e74 2073 6561  l_adjustment sea
-000178b0: 736f 6e61 6c5f 6164 6a75 7374 6d65 6e74  sonal_adjustment
-000178c0: 5f73 686f 7274 2020 2020 2020 2020 2020  _short          
-000178d0: 2020 2020 6c61 7374 5f75 7064 6174 6564      last_updated
-000178e0: 2020 706f 7075 6c61 7269 7479 2020 6772    popularity  gr
-000178f0: 6f75 705f 706f 7075 6c61 7269 7479 2020  oup_popularity  
+00016790: 2320 6669 7820 6874 7470 733a 2f2f 6769  # fix https://gi
+000167a0: 7468 7562 2e63 6f6d 2f54 6f6d 6173 4b6f  thub.com/TomasKo
+000167b0: 7574 656b 2f70 7973 746c 6f75 6973 6665  utek/pystlouisfe
+000167c0: 642f 6973 7375 6573 2f31 0d0a 2020 2020  d/issues/1..    
+000167d0: 2020 2020 2020 2020 2320 4973 2074 6865          # Is the
+000167e0: 206c 696e 6b20 6f70 7469 6f6e 616c 3f0d   link optional?.
+000167f0: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
+00016800: 6879 2064 6f65 736e 2774 2046 5245 4420  hy doesn't FRED 
+00016810: 7265 7475 726e 2061 6e20 656d 7074 7920  return an empty 
+00016820: 636f 6c75 6d6e 3f0d 0a20 2020 2020 2020  column?..       
+00016830: 2020 2020 2069 6620 276c 696e 6b27 206e       if 'link' n
+00016840: 6f74 2069 6e20 6466 2e63 6f6c 756d 6e73  ot in df.columns
+00016850: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00016860: 2020 2064 665b 276c 696e 6b27 5d20 3d20     df['link'] = 
+00016870: 2727 0d0a 0d0a 2020 2020 2020 2020 2020  ''....          
+00016880: 2020 6466 203d 2064 662e 6173 7479 7065    df = df.astype
+00016890: 2864 7479 7065 3d7b 0d0a 2020 2020 2020  (dtype={..      
+000168a0: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
+000168b0: 3a20 2773 7472 696e 6727 2c0d 0a20 2020  : 'string',..   
+000168c0: 2020 2020 2020 2020 2020 2020 2027 6c69               'li
+000168d0: 6e6b 273a 2027 7374 7269 6e67 272c 0d0a  nk': 'string',..
+000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168f0: 2770 7265 7373 5f72 656c 6561 7365 273a  'press_release':
+00016900: 2027 626f 6f6c 270d 0a20 2020 2020 2020   'bool'..       
+00016910: 2020 2020 207d 292e 7365 745f 696e 6465       }).set_inde
+00016920: 7828 2769 6427 290d 0a0d 0a20 2020 2020  x('id')....     
+00016930: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
+00016940: 2020 2020 6465 6620 7365 7269 6573 5f73      def series_s
+00016950: 6561 7263 6828 0d0a 2020 2020 2020 2020  earch(..        
+00016960: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+00016970: 2020 2020 2020 2073 6561 7263 685f 7465         search_te
+00016980: 7874 3a20 7374 722c 0d0a 2020 2020 2020  xt: str,..      
+00016990: 2020 2020 2020 7365 6172 6368 5f74 7970        search_typ
+000169a0: 653a 2065 6e75 6d73 2e53 6561 7263 6854  e: enums.SearchT
+000169b0: 7970 6520 3d20 656e 756d 732e 5365 6172  ype = enums.Sear
+000169c0: 6368 5479 7065 2e66 756c 6c5f 7465 7874  chType.full_text
+000169d0: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+000169e0: 6561 6c74 696d 655f 7374 6172 743a 2064  ealtime_start: d
+000169f0: 6174 6520 3d20 4e6f 6e65 2c0d 0a20 2020  ate = None,..   
+00016a00: 2020 2020 2020 2020 2072 6561 6c74 696d           realtim
+00016a10: 655f 656e 643a 2064 6174 6520 3d20 4e6f  e_end: date = No
+00016a20: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+00016a30: 206f 7264 6572 5f62 793a 2065 6e75 6d73   order_by: enums
+00016a40: 2e4f 7264 6572 4279 203d 204e 6f6e 652c  .OrderBy = None,
+00016a50: 0d0a 2020 2020 2020 2020 2020 2020 736f  ..            so
+00016a60: 7274 5f6f 7264 6572 3a20 656e 756d 732e  rt_order: enums.
+00016a70: 536f 7274 4f72 6465 7220 3d20 4e6f 6e65  SortOrder = None
+00016a80: 2c0d 0a20 2020 2020 2020 2020 2020 2066  ,..            f
+00016a90: 696c 7465 725f 7661 7269 6162 6c65 3a20  ilter_variable: 
+00016aa0: 656e 756d 732e 4669 6c74 6572 5661 7269  enums.FilterVari
+00016ab0: 6162 6c65 203d 204e 6f6e 652c 0d0a 2020  able = None,..  
+00016ac0: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
+00016ad0: 5f76 616c 7565 3a20 656e 756d 732e 4669  _value: enums.Fi
+00016ae0: 6c74 6572 5661 6c75 6520 3d20 4e6f 6e65  lterValue = None
+00016af0: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00016b00: 6167 5f6e 616d 6573 3a20 4c69 7374 5b73  ag_names: List[s
+00016b10: 7472 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  tr] = None,..   
+00016b20: 2020 2020 2020 2020 2065 7863 6c75 6465           exclude
+00016b30: 5f74 6167 5f6e 616d 6573 3a20 4c69 7374  _tag_names: List
+00016b40: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
+00016b50: 2020 2920 2d3e 2070 642e 4461 7461 4672    ) -> pd.DataFr
+00016b60: 616d 653a 0d0a 2020 2020 2020 2020 2222  ame:..        ""
+00016b70: 220d 0a20 2020 2020 2020 2023 2320 5061  "..        ## Pa
+00016b80: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
+00016b90: 2020 6073 6561 7263 685f 7465 7874 600d    `search_text`.
+00016ba0: 0a20 2020 2020 2020 2054 6865 2077 6f72  .        The wor
+00016bb0: 6473 2074 6f20 6d61 7463 6820 6167 6169  ds to match agai
+00016bc0: 6e73 7420 6563 6f6e 6f6d 6963 2064 6174  nst economic dat
+00016bd0: 6120 7365 7269 6573 2e0d 0a0d 0a20 2020  a series.....   
+00016be0: 2020 2020 2060 7365 6172 6368 5f74 7970       `search_typ
+00016bf0: 6560 0d0a 2020 2020 2020 2020 4465 7465  e`..        Dete
+00016c00: 726d 696e 6573 2074 6865 2074 7970 6520  rmines the type 
+00016c10: 6f66 2073 6561 7263 6820 746f 2070 6572  of search to per
+00016c20: 666f 726d 2e0d 0a0d 0a20 2020 2020 2020  form.....       
+00016c30: 2060 7265 616c 7469 6d65 5f73 7461 7274   `realtime_start
+00016c40: 600d 0a20 2020 2020 2020 2054 6865 2073  `..        The s
+00016c50: 7461 7274 206f 6620 7468 6520 7265 616c  tart of the real
+00016c60: 2d74 696d 6520 7065 7269 6f64 2e20 466f  -time period. Fo
+00016c70: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+00016c80: 6f6e 2c20 7365 6520 5b52 6561 6c2d 5469  on, see [Real-Ti
+00016c90: 6d65 2050 6572 696f 6473 5d28 6874 7470  me Periods](http
+00016ca0: 733a 2f2f 6672 6564 2e73 746c 6f75 6973  s://fred.stlouis
+00016cb0: 6665 642e 6f72 672f 646f 6373 2f61 7069  fed.org/docs/api
+00016cc0: 2f66 7265 642f 7265 616c 7469 6d65 5f70  /fred/realtime_p
+00016cd0: 6572 696f 642e 6874 6d6c 292e 0d0a 0d0a  eriod.html).....
+00016ce0: 2020 2020 2020 2020 6072 6561 6c74 696d          `realtim
+00016cf0: 655f 656e 6460 0d0a 2020 2020 2020 2020  e_end`..        
+00016d00: 5468 6520 656e 6420 6f66 2074 6865 2072  The end of the r
+00016d10: 6561 6c2d 7469 6d65 2070 6572 696f 642e  eal-time period.
+00016d20: 2046 6f72 206d 6f72 6520 696e 666f 726d   For more inform
+00016d30: 6174 696f 6e2c 2073 6565 205b 5265 616c  ation, see [Real
+00016d40: 2d54 696d 6520 5065 7269 6f64 735d 2868  -Time Periods](h
+00016d50: 7474 7073 3a2f 2f66 7265 642e 7374 6c6f  ttps://fred.stlo
+00016d60: 7569 7366 6564 2e6f 7267 2f64 6f63 732f  uisfed.org/docs/
+00016d70: 6170 692f 6672 6564 2f72 6561 6c74 696d  api/fred/realtim
+00016d80: 655f 7065 7269 6f64 2e68 746d 6c29 2e0d  e_period.html)..
+00016d90: 0a0d 0a20 2020 2020 2020 2060 6f72 6465  ...        `orde
+00016da0: 725f 6279 600d 0a20 2020 2020 2020 204f  r_by`..        O
+00016db0: 7264 6572 2072 6573 756c 7473 2062 7920  rder results by 
+00016dc0: 7661 6c75 6573 206f 6620 7468 6520 7370  values of the sp
+00016dd0: 6563 6966 6965 6420 6174 7472 6962 7574  ecified attribut
+00016de0: 652e 0d0a 0d0a 2020 2020 2020 2020 6073  e.....        `s
+00016df0: 6f72 745f 6f72 6465 7260 0d0a 2020 2020  ort_order`..    
+00016e00: 2020 2020 536f 7274 2072 6573 756c 7473      Sort results
+00016e10: 2069 7320 6173 6365 6e64 696e 6720 6f72   is ascending or
+00016e20: 2064 6573 6365 6e64 696e 6720 6f72 6465   descending orde
+00016e30: 7220 666f 7220 6174 7472 6962 7574 6520  r for attribute 
+00016e40: 7661 6c75 6573 2073 7065 6369 6669 6564  values specified
+00016e50: 2062 7920 6f72 6465 725f 6279 2e0d 0a0d   by order_by....
+00016e60: 0a20 2020 2020 2020 2060 6669 6c74 6572  .        `filter
+00016e70: 5f76 6172 6961 626c 6560 0d0a 2020 2020  _variable`..    
+00016e80: 2020 2020 5468 6520 6174 7472 6962 7574      The attribut
+00016e90: 6520 746f 2066 696c 7465 7220 7265 7375  e to filter resu
+00016ea0: 6c74 7320 6279 2e0d 0a0d 0a20 2020 2020  lts by.....     
+00016eb0: 2020 2060 6669 6c74 6572 5f76 616c 7565     `filter_value
+00016ec0: 600d 0a20 2020 2020 2020 2054 6865 2076  `..        The v
+00016ed0: 616c 7565 206f 6620 7468 6520 6669 6c74  alue of the filt
+00016ee0: 6572 5f76 6172 6961 626c 6520 6174 7472  er_variable attr
+00016ef0: 6962 7574 6520 746f 2066 696c 7465 7220  ibute to filter 
+00016f00: 7265 7375 6c74 7320 6279 2e0d 0a0d 0a20  results by..... 
+00016f10: 2020 2020 2020 2060 7461 675f 6e61 6d65         `tag_name
+00016f20: 7360 0d0a 2020 2020 2020 2020 4120 7365  s`..        A se
+00016f30: 6d69 636f 6c6f 6e20 6465 6c69 6d69 7465  micolon delimite
+00016f40: 6420 6c69 7374 206f 6620 7461 6720 6e61  d list of tag na
+00016f50: 6d65 7320 7468 6174 2073 6572 6965 7320  mes that series 
+00016f60: 6d61 7463 6820 616c 6c20 6f66 2e0d 0a0d  match all of....
+00016f70: 0a20 2020 2020 2020 2060 6578 636c 7564  .        `exclud
+00016f80: 655f 7461 675f 6e61 6d65 7360 0d0a 2020  e_tag_names`..  
+00016f90: 2020 2020 2020 4120 7365 6d69 636f 6c6f        A semicolo
+00016fa0: 6e20 6465 6c69 6d69 7465 6420 6c69 7374  n delimited list
+00016fb0: 206f 6620 7461 6720 6e61 6d65 7320 7468   of tag names th
+00016fc0: 6174 2073 6572 6965 7320 6d61 7463 6820  at series match 
+00016fd0: 6e6f 6e65 206f 662e 0d0a 0d0a 2020 2020  none of.....    
+00016fe0: 2020 2020 2323 2044 6573 6372 6970 7469      ## Descripti
+00016ff0: 6f6e 0d0a 2020 2020 2020 2020 6874 7470  on..        http
+00017000: 733a 2f2f 6672 6564 2e73 746c 6f75 6973  s://fred.stlouis
+00017010: 6665 642e 6f72 672f 646f 6373 2f61 7069  fed.org/docs/api
+00017020: 2f66 7265 642f 7365 7269 6573 5f73 6561  /fred/series_sea
+00017030: 7263 682e 6874 6d6c 0d0a 0d0a 2020 2020  rch.html....    
+00017040: 2020 2020 4765 7420 6563 6f6e 6f6d 6963      Get economic
+00017050: 2064 6174 6120 7365 7269 6573 2074 6861   data series tha
+00017060: 7420 6d61 7463 6820 7365 6172 6368 2074  t match search t
+00017070: 6578 742e 0d0a 0d0a 2020 2020 2020 2020  ext.....        
+00017080: 2323 2041 5049 2052 6571 7565 7374 2028  ## API Request (
+00017090: 4854 5450 5320 4745 5429 0d0a 2020 2020  HTTPS GET)..    
+000170a0: 2020 2020 6874 7470 733a 2f2f 6170 692e      https://api.
+000170b0: 7374 6c6f 7569 7366 6564 2e6f 7267 2f66  stlouisfed.org/f
+000170c0: 7265 642f 7365 7269 6573 2f73 6561 7263  red/series/searc
+000170d0: 683f 7365 6172 6368 5f74 6578 743d 6d6f  h?search_text=mo
+000170e0: 6e65 7461 7279 2b73 6572 7669 6365 2b69  netary+service+i
+000170f0: 6e64 6578 2661 7069 5f6b 6579 3d61 6263  ndex&api_key=abc
+00017100: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
+00017110: 7475 7677 7879 7a31 3233 3435 3626 6669  tuvwxyz123456&fi
+00017120: 6c65 5f74 7970 653d 6a73 6f6e 0d0a 0d0a  le_type=json....
+00017130: 2020 2020 2020 2020 2323 2041 5049 2052          ## API R
+00017140: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+00017150: 2060 6060 6a73 6f6e 0d0a 2020 2020 2020   ```json..      
+00017160: 2020 7b0d 0a20 2020 2020 2020 2020 2022    {..          "
+00017170: 7265 616c 7469 6d65 5f73 7461 7274 223a  realtime_start":
+00017180: 2022 3230 3137 2d30 382d 3031 222c 0d0a   "2017-08-01",..
+00017190: 2020 2020 2020 2020 2020 2272 6561 6c74            "realt
+000171a0: 696d 655f 656e 6422 3a20 2232 3031 372d  ime_end": "2017-
+000171b0: 3038 2d30 3122 2c0d 0a20 2020 2020 2020  08-01",..       
+000171c0: 2020 2022 6f72 6465 725f 6279 223a 2022     "order_by": "
+000171d0: 7365 6172 6368 5f72 616e 6b22 2c0d 0a20  search_rank",.. 
+000171e0: 2020 2020 2020 2020 2022 736f 7274 5f6f           "sort_o
+000171f0: 7264 6572 223a 2022 6465 7363 222c 0d0a  rder": "desc",..
+00017200: 2020 2020 2020 2020 2020 2263 6f75 6e74            "count
+00017210: 223a 2033 322c 0d0a 2020 2020 2020 2020  ": 32,..        
+00017220: 2020 226f 6666 7365 7422 3a20 302c 0d0a    "offset": 0,..
+00017230: 2020 2020 2020 2020 2020 226c 696d 6974            "limit
+00017240: 223a 2031 3030 302c 0d0a 2020 2020 2020  ": 1000,..      
+00017250: 2020 2020 2273 6572 6965 7373 223a 205b      "seriess": [
+00017260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017270: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00017280: 2020 2020 2020 2022 6964 223a 2022 4d53         "id": "MS
+00017290: 494d 3222 2c0d 0a20 2020 2020 2020 2020  IM2",..         
+000172a0: 2020 2020 2020 2020 2022 7265 616c 7469           "realti
+000172b0: 6d65 5f73 7461 7274 223a 2022 3230 3137  me_start": "2017
+000172c0: 2d30 382d 3031 222c 0d0a 2020 2020 2020  -08-01",..      
+000172d0: 2020 2020 2020 2020 2020 2020 2272 6561              "rea
+000172e0: 6c74 696d 655f 656e 6422 3a20 2232 3031  ltime_end": "201
+000172f0: 372d 3038 2d30 3122 2c0d 0a20 2020 2020  7-08-01",..     
+00017300: 2020 2020 2020 2020 2020 2020 2022 7469               "ti
+00017310: 746c 6522 3a20 224d 6f6e 6574 6172 7920  tle": "Monetary 
+00017320: 5365 7276 6963 6573 2049 6e64 6578 3a20  Services Index: 
+00017330: 4d32 2028 7072 6566 6572 7265 6429 222c  M2 (preferred)",
+00017340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017350: 2020 2020 226f 6273 6572 7661 7469 6f6e      "observation
+00017360: 5f73 7461 7274 223a 2022 3139 3637 2d30  _start": "1967-0
+00017370: 312d 3031 222c 0d0a 2020 2020 2020 2020  1-01",..        
+00017380: 2020 2020 2020 2020 2020 226f 6273 6572            "obser
+00017390: 7661 7469 6f6e 5f65 6e64 223a 2022 3230  vation_end": "20
+000173a0: 3133 2d31 322d 3031 222c 0d0a 2020 2020  13-12-01",..    
+000173b0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+000173c0: 7265 7175 656e 6379 223a 2022 4d6f 6e74  requency": "Mont
+000173d0: 686c 7922 2c0d 0a20 2020 2020 2020 2020  hly",..         
+000173e0: 2020 2020 2020 2020 2022 6672 6571 7565           "freque
+000173f0: 6e63 795f 7368 6f72 7422 3a20 224d 222c  ncy_short": "M",
+00017400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017410: 2020 2020 2275 6e69 7473 223a 2022 4269      "units": "Bi
+00017420: 6c6c 696f 6e73 206f 6620 446f 6c6c 6172  llions of Dollar
+00017430: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
+00017440: 2020 2020 2020 2022 756e 6974 735f 7368         "units_sh
+00017450: 6f72 7422 3a20 2242 696c 2e20 6f66 2024  ort": "Bil. of $
+00017460: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00017470: 2020 2020 2020 2273 6561 736f 6e61 6c5f        "seasonal_
+00017480: 6164 6a75 7374 6d65 6e74 223a 2022 5365  adjustment": "Se
+00017490: 6173 6f6e 616c 6c79 2041 646a 7573 7465  asonally Adjuste
+000174a0: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
+000174b0: 2020 2020 2020 2022 7365 6173 6f6e 616c         "seasonal
+000174c0: 5f61 646a 7573 746d 656e 745f 7368 6f72  _adjustment_shor
+000174d0: 7422 3a20 2253 4122 2c0d 0a20 2020 2020  t": "SA",..     
+000174e0: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
+000174f0: 7374 5f75 7064 6174 6564 223a 2022 3230  st_updated": "20
+00017500: 3134 2d30 312d 3137 2030 373a 3136 3a34  14-01-17 07:16:4
+00017510: 342d 3036 222c 0d0a 2020 2020 2020 2020  4-06",..        
+00017520: 2020 2020 2020 2020 2020 2270 6f70 756c            "popul
+00017530: 6172 6974 7922 3a20 3334 2c0d 0a20 2020  arity": 34,..   
+00017540: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00017550: 6772 6f75 705f 706f 7075 6c61 7269 7479  group_popularity
+00017560: 223a 2033 332c 0d0a 2020 2020 2020 2020  ": 33,..        
+00017570: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
+00017580: 223a 2022 5468 6520 4d53 4920 6d65 6173  ": "The MSI meas
+00017590: 7572 6520 7468 6520 666c 6f77 206f 6620  ure the flow of 
+000175a0: 6d6f 6e65 7461 7279 2073 6572 7669 6365  monetary service
+000175b0: 7320 7265 6365 6976 6564 2065 6163 6820  s received each 
+000175c0: 7065 7269 6f64 2062 7920 686f 7573 6568  period by househ
+000175d0: 6f6c 6473 2061 6e64 2066 6972 6d73 2066  olds and firms f
+000175e0: 726f 6d20 7468 6569 7220 686f 6c64 696e  rom their holdin
+000175f0: 6773 206f 6620 6d6f 6e65 7461 7279 2061  gs of monetary a
+00017600: 7373 6574 7320 286c 6576 656c 7320 6f66  ssets (levels of
+00017610: 2074 6865 2069 6e64 6578 6573 2061 7265   the indexes are
+00017620: 2073 6f6d 6574 696d 6573 2072 6566 6572   sometimes refer
+00017630: 7265 6420 746f 2061 7320 4469 7669 7369  red to as Divisi
+00017640: 6120 6d6f 6e65 7461 7279 2061 6767 7265  a monetary aggre
+00017650: 6761 7465 7329 2e5c 5c6e 5072 6566 6572  gates).\\nPrefer
+00017660: 7265 6420 6265 6e63 686d 6172 6b20 7261  red benchmark ra
+00017670: 7465 2065 7175 616c 7320 3130 3020 6261  te equals 100 ba
+00017680: 7369 7320 706f 696e 7473 2070 6c75 7320  sis points plus 
+00017690: 7468 6520 6c61 7267 6573 7420 7261 7465  the largest rate
+000176a0: 2069 6e20 7468 6520 7365 7420 6f66 2072   in the set of r
+000176b0: 6174 6573 2e5c 5c6e 416c 7465 726e 6174  ates.\\nAlternat
+000176c0: 6976 6520 6265 6e63 686d 6172 6b20 7261  ive benchmark ra
+000176d0: 7465 2065 7175 616c 7320 7468 6520 6c61  te equals the la
+000176e0: 7267 6572 206f 6620 7468 6520 7072 6566  rger of the pref
+000176f0: 6572 7265 6420 6265 6e63 686d 6172 6b20  erred benchmark 
+00017700: 7261 7465 2061 6e64 2074 6865 2042 6161  rate and the Baa
+00017710: 2063 6f72 706f 7261 7465 2062 6f6e 6420   corporate bond 
+00017720: 7969 656c 642e 5c5c 6e4d 6f72 6520 696e  yield.\\nMore in
+00017730: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+00017740: 7468 6520 6e65 7720 4d53 4920 6361 6e20  the new MSI can 
+00017750: 6265 2066 6f75 6e64 2061 745c 5c6e 6874  be found at\\nht
+00017760: 7470 3a2f 2f72 6573 6561 7263 682e 7374  tp://research.st
+00017770: 6c6f 7569 7366 6564 2e6f 7267 2f6d 7369  louisfed.org/msi
+00017780: 2f69 6e64 6578 2e68 746d 6c2e 220d 0a20  /index.html.".. 
+00017790: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+000177a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000177b0: 2020 202e 2e2e 0d0a 2020 2020 2020 2020     .....        
+000177c0: 2020 2020 5d0d 0a20 2020 2020 2020 207d      ]..        }
+000177d0: 0d0a 2020 2020 2020 2020 6060 600d 0a0d  ..        ```...
+000177e0: 0a20 2020 2020 2020 2023 2320 5265 7475  .        ## Retu
+000177f0: 726e 730d 0a20 2020 2020 2020 2060 7061  rns..        `pa
+00017800: 6e64 6173 2e44 6174 6146 7261 6d65 600d  ndas.DataFrame`.
+00017810: 0a0d 0a20 2020 2020 2020 2023 2320 4578  ...        ## Ex
+00017820: 616d 706c 650d 0a20 2020 2020 2020 2060  ample..        `
+00017830: 6060 7079 7468 6f6e 0d0a 2020 2020 2020  ``python..      
+00017840: 2020 3e3e 3e20 6672 6564 203d 2046 5245    >>> fred = FRE
+00017850: 4428 6170 695f 6b65 793d 2761 6263 6465  D(api_key='abcde
+00017860: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
+00017870: 7677 7879 7a31 3233 3435 3627 290d 0a20  vwxyz123456').. 
+00017880: 2020 2020 2020 203e 3e3e 2066 7265 642e         >>> fred.
+00017890: 7365 7269 6573 5f73 6561 7263 6828 7365  series_search(se
+000178a0: 6172 6368 5f74 6578 743d 276d 6f6e 6574  arch_text='monet
+000178b0: 6172 7920 7365 7276 6963 6520 696e 6465  ary service inde
+000178c0: 7827 292e 6865 6164 2829 0d0a 2020 2020  x').head()..    
+000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178e0: 7265 616c 7469 6d65 5f73 7461 7274 2072  realtime_start r
+000178f0: 6561 6c74 696d 655f 656e 6420 2020 2020  ealtime_end     
 00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017920: 2020 2020 2020 2020 2020 2020 6e6f 7465              note
-00017930: 730d 0a20 2020 2020 2020 2020 2020 2069  s..            i
-00017940: 640d 0a20 2020 2020 2020 2020 2020 204d  d..            M
-00017950: 5349 4d5a 4d50 2020 2020 2032 3032 322d  SIMZMP     2022-
-00017960: 3032 2d30 3520 2020 3230 3232 2d30 322d  02-05   2022-02-
-00017970: 3035 2020 2020 2020 2020 204d 6f6e 6574  05         Monet
-00017980: 6172 7920 5365 7276 6963 6573 2049 6e64  ary Services Ind
-00017990: 6578 3a20 4d5a 4d20 2870 7265 6665 7272  ex: MZM (preferr
-000179a0: 6564 2920 2020 2020 2020 2031 3936 372d  ed)        1967-
-000179b0: 3031 2d30 3120 2020 2020 2032 3031 332d  01-01      2013-
-000179c0: 3132 2d30 3120 2020 4d6f 6e74 686c 7920  12-01   Monthly 
-000179d0: 2020 2020 2020 2020 2020 2020 2020 4d20                M 
-000179e0: 2042 696c 6c69 6f6e 7320 6f66 2044 6f6c   Billions of Dol
-000179f0: 6c61 7273 2020 2042 696c 2e20 6f66 2024  lars   Bil. of $
-00017a00: 2020 5365 6173 6f6e 616c 6c79 2041 646a    Seasonally Adj
-00017a10: 7573 7465 6420 2020 2020 2020 2020 2020  usted           
-00017a20: 2020 2020 2020 2020 2020 2020 2053 4120               SA 
-00017a30: 3230 3134 2d30 312d 3137 2031 333a 3136  2014-01-17 13:16
-00017a40: 3a34 322b 3030 3a30 3020 2020 2020 2020  :42+00:00       
-00017a50: 2020 2032 3020 2020 2020 2020 2020 2020     20           
-00017a60: 2020 2020 2032 3020 2054 6865 204d 5349       20  The MSI
-00017a70: 206d 6561 7375 7265 2074 6865 2066 6c6f   measure the flo
-00017a80: 7720 6f66 206d 6f6e 6574 6172 7920 7365  w of monetary se
-00017a90: 7276 6963 6573 202e 2e2e 0d0a 2020 2020  rvices .....    
-00017aa0: 2020 2020 2020 2020 4d53 494d 3220 2020          MSIM2   
-00017ab0: 2020 2020 3230 3232 2d30 322d 3035 2020      2022-02-05  
-00017ac0: 2032 3032 322d 3032 2d30 3520 2020 2020   2022-02-05     
-00017ad0: 2020 2020 204d 6f6e 6574 6172 7920 5365       Monetary Se
-00017ae0: 7276 6963 6573 2049 6e64 6578 3a20 4d32  rvices Index: M2
-00017af0: 2028 7072 6566 6572 7265 6429 2020 2020   (preferred)    
-00017b00: 2020 2020 3139 3637 2d30 312d 3031 2020      1967-01-01  
-00017b10: 2020 2020 3230 3133 2d31 322d 3031 2020      2013-12-01  
-00017b20: 204d 6f6e 7468 6c79 2020 2020 2020 2020   Monthly        
-00017b30: 2020 2020 2020 204d 2020 4269 6c6c 696f         M  Billio
-00017b40: 6e73 206f 6620 446f 6c6c 6172 7320 2020  ns of Dollars   
-00017b50: 4269 6c2e 206f 6620 2420 2053 6561 736f  Bil. of $  Seaso
-00017b60: 6e61 6c6c 7920 4164 6a75 7374 6564 2020  nally Adjusted  
-00017b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b80: 2020 2020 2020 5341 2032 3031 342d 3031        SA 2014-01
-00017b90: 2d31 3720 3133 3a31 363a 3434 2b30 303a  -17 13:16:44+00:
-00017ba0: 3030 2020 2020 2020 2020 2020 3136 2020  00          16  
-00017bb0: 2020 2020 2020 2020 2020 2020 2020 3136                16
-00017bc0: 2020 5468 6520 4d53 4920 6d65 6173 7572    The MSI measur
-00017bd0: 6520 7468 6520 666c 6f77 206f 6620 6d6f  e the flow of mo
-00017be0: 6e65 7461 7279 2073 6572 7669 6365 7320  netary services 
-00017bf0: 2e2e 2e0d 0a20 2020 2020 2020 2020 2020  .....           
-00017c00: 204d 5349 414c 4c50 2020 2020 2032 3032   MSIALLP     202
-00017c10: 322d 3032 2d30 3520 2020 3230 3232 2d30  2-02-05   2022-0
-00017c20: 322d 3035 2020 4d6f 6e65 7461 7279 2053  2-05  Monetary S
-00017c30: 6572 7669 6365 7320 496e 6465 783a 2041  ervices Index: A
-00017c40: 4c4c 2041 7373 6574 7320 2870 7265 6665  LL Assets (prefe
-00017c50: 7272 6564 2920 2020 2020 2020 2031 3936  rred)        196
-00017c60: 372d 3031 2d30 3120 2020 2020 2032 3031  7-01-01      201
-00017c70: 332d 3132 2d30 3120 2020 4d6f 6e74 686c  3-12-01   Monthl
-00017c80: 7920 2020 2020 2020 2020 2020 2020 2020  y               
-00017c90: 4d20 2042 696c 6c69 6f6e 7320 6f66 2044  M  Billions of D
-00017ca0: 6f6c 6c61 7273 2020 2042 696c 2e20 6f66  ollars   Bil. of
-00017cb0: 2024 2020 5365 6173 6f6e 616c 6c79 2041   $  Seasonally A
-00017cc0: 646a 7573 7465 6420 2020 2020 2020 2020  djusted         
-00017cd0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00017ce0: 4120 3230 3134 2d30 312d 3137 2031 333a  A 2014-01-17 13:
-00017cf0: 3136 3a34 352b 3030 3a30 3020 2020 2020  16:45+00:00     
-00017d00: 2020 2020 2031 3420 2020 2020 2020 2020       14         
-00017d10: 2020 2020 2020 2031 3420 2054 6865 204d         14  The M
-00017d20: 5349 206d 6561 7375 7265 2074 6865 2066  SI measure the f
-00017d30: 6c6f 7720 6f66 206d 6f6e 6574 6172 7920  low of monetary 
-00017d40: 7365 7276 6963 6573 202e 2e2e 0d0a 2020  services .....  
-00017d50: 2020 2020 2020 2020 2020 4d53 494d 3150            MSIM1P
-00017d60: 2020 2020 2020 3230 3232 2d30 322d 3035        2022-02-05
-00017d70: 2020 2032 3032 322d 3032 2d30 3520 2020     2022-02-05   
-00017d80: 2020 2020 2020 204d 6f6e 6574 6172 7920         Monetary 
-00017d90: 5365 7276 6963 6573 2049 6e64 6578 3a20  Services Index: 
-00017da0: 4d31 2028 7072 6566 6572 7265 6429 2020  M1 (preferred)  
-00017db0: 2020 2020 2020 3139 3637 2d30 312d 3031        1967-01-01
-00017dc0: 2020 2020 2020 3230 3133 2d31 322d 3031        2013-12-01
-00017dd0: 2020 204d 6f6e 7468 6c79 2020 2020 2020     Monthly      
-00017de0: 2020 2020 2020 2020 204d 2020 4269 6c6c           M  Bill
-00017df0: 696f 6e73 206f 6620 446f 6c6c 6172 7320  ions of Dollars 
-00017e00: 2020 4269 6c2e 206f 6620 2420 2053 6561    Bil. of $  Sea
-00017e10: 736f 6e61 6c6c 7920 4164 6a75 7374 6564  sonally Adjusted
-00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e30: 2020 2020 2020 2020 5341 2032 3031 342d          SA 2014-
-00017e40: 3031 2d31 3720 3133 3a31 363a 3435 2b30  01-17 13:16:45+0
-00017e50: 303a 3030 2020 2020 2020 2020 2020 2039  0:00           9
-00017e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e70: 2039 2020 5468 6520 4d53 4920 6d65 6173   9  The MSI meas
-00017e80: 7572 6520 7468 6520 666c 6f77 206f 6620  ure the flow of 
-00017e90: 6d6f 6e65 7461 7279 2073 6572 7669 6365  monetary service
-00017ea0: 7320 2e2e 2e0d 0a20 2020 2020 2020 2020  s .....         
-00017eb0: 2020 204d 5349 4d32 4120 2020 2020 2032     MSIM2A      2
-00017ec0: 3032 322d 3032 2d30 3520 2020 3230 3232  022-02-05   2022
-00017ed0: 2d30 322d 3035 2020 2020 2020 2020 4d6f  -02-05        Mo
-00017ee0: 6e65 7461 7279 2053 6572 7669 6365 7320  netary Services 
-00017ef0: 496e 6465 783a 204d 3220 2861 6c74 6572  Index: M2 (alter
-00017f00: 6e61 7469 7665 2920 2020 2020 2020 2031  native)        1
-00017f10: 3936 372d 3031 2d30 3120 2020 2020 2032  967-01-01      2
-00017f20: 3031 332d 3132 2d30 3120 2020 4d6f 6e74  013-12-01   Mont
-00017f30: 686c 7920 2020 2020 2020 2020 2020 2020  hly             
-00017f40: 2020 4d20 2042 696c 6c69 6f6e 7320 6f66    M  Billions of
-00017f50: 2044 6f6c 6c61 7273 2020 2042 696c 2e20   Dollars   Bil. 
-00017f60: 6f66 2024 2020 5365 6173 6f6e 616c 6c79  of $  Seasonally
-00017f70: 2041 646a 7573 7465 6420 2020 2020 2020   Adjusted       
-00017f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f90: 2053 4120 3230 3134 2d30 312d 3137 2031   SA 2014-01-17 1
-00017fa0: 333a 3136 3a34 342b 3030 3a30 3020 2020  3:16:44+00:00   
-00017fb0: 2020 2020 2020 2020 3820 2020 2020 2020          8       
-00017fc0: 2020 2020 2020 2020 2020 3820 2054 6865            8  The
-00017fd0: 204d 5349 206d 6561 7375 7265 2074 6865   MSI measure the
-00017fe0: 2066 6c6f 7720 6f66 206d 6f6e 6574 6172   flow of monetar
-00017ff0: 7920 7365 7276 6963 6573 202e 2e2e 0d0a  y services .....
-00018000: 2020 2020 2020 2020 6060 600d 0a20 2020          ```..   
-00018010: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
-00018020: 2020 2020 616c 6c6f 7765 645f 6f72 6465      allowed_orde
-00018030: 7273 203d 205b 0d0a 2020 2020 2020 2020  rs = [..        
-00018040: 2020 2020 656e 756d 732e 4f72 6465 7242      enums.OrderB
-00018050: 792e 7365 6172 6368 5f72 616e 6b2c 0d0a  y.search_rank,..
-00018060: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-00018070: 732e 4f72 6465 7242 792e 7365 7269 6573  s.OrderBy.series
-00018080: 5f69 642c 0d0a 2020 2020 2020 2020 2020  _id,..          
-00018090: 2020 656e 756d 732e 4f72 6465 7242 792e    enums.OrderBy.
-000180a0: 7469 746c 652c 0d0a 2020 2020 2020 2020  title,..        
-000180b0: 2020 2020 656e 756d 732e 4f72 6465 7242      enums.OrderB
-000180c0: 792e 756e 6974 732c 0d0a 2020 2020 2020  y.units,..      
-000180d0: 2020 2020 2020 656e 756d 732e 4f72 6465        enums.Orde
-000180e0: 7242 792e 6672 6571 7565 6e63 792c 0d0a  rBy.frequency,..
-000180f0: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-00018100: 732e 4f72 6465 7242 792e 7365 6173 6f6e  s.OrderBy.season
-00018110: 616c 5f61 646a 7573 746d 656e 742c 0d0a  al_adjustment,..
-00018120: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-00018130: 732e 4f72 6465 7242 792e 7265 616c 7469  s.OrderBy.realti
-00018140: 6d65 5f73 7461 7274 2c0d 0a20 2020 2020  me_start,..     
-00018150: 2020 2020 2020 2065 6e75 6d73 2e4f 7264         enums.Ord
-00018160: 6572 4279 2e72 6561 6c74 696d 655f 656e  erBy.realtime_en
-00018170: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-00018180: 656e 756d 732e 4f72 6465 7242 792e 6c61  enums.OrderBy.la
-00018190: 7374 5f75 7064 6174 6564 2c0d 0a20 2020  st_updated,..   
-000181a0: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
-000181b0: 7264 6572 4279 2e6f 6273 6572 7661 7469  rderBy.observati
-000181c0: 6f6e 5f73 7461 7274 2c0d 0a20 2020 2020  on_start,..     
-000181d0: 2020 2020 2020 2065 6e75 6d73 2e4f 7264         enums.Ord
-000181e0: 6572 4279 2e6f 6273 6572 7661 7469 6f6e  erBy.observation
-000181f0: 5f65 6e64 2c0d 0a20 2020 2020 2020 2020  _end,..         
-00018200: 2020 2065 6e75 6d73 2e4f 7264 6572 4279     enums.OrderBy
-00018210: 2e70 6f70 756c 6172 6974 792c 0d0a 2020  .popularity,..  
-00018220: 2020 2020 2020 2020 2020 656e 756d 732e            enums.
-00018230: 4f72 6465 7242 792e 6772 6f75 705f 706f  OrderBy.group_po
-00018240: 7075 6c61 7269 7479 0d0a 2020 2020 2020  pularity..      
-00018250: 2020 5d0d 0a0d 0a20 2020 2020 2020 2023    ]....        #
-00018260: 2049 6620 7468 6520 7661 6c75 6520 6f66   If the value of
-00018270: 2073 6561 7263 685f 7479 7065 2069 7320   search_type is 
-00018280: 2766 756c 6c5f 7465 7874 2720 7468 656e  'full_text' then
-00018290: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
-000182a0: 7565 206f 6620 6f72 6465 725f 6279 2069  ue of order_by i
-000182b0: 7320 2773 6561 7263 685f 7261 6e6b 272e  s 'search_rank'.
-000182c0: 0d0a 2020 2020 2020 2020 6966 2073 6561  ..        if sea
-000182d0: 7263 685f 7479 7065 203d 3d20 656e 756d  rch_type == enum
-000182e0: 732e 5365 6172 6368 5479 7065 2e66 756c  s.SearchType.ful
-000182f0: 6c5f 7465 7874 2061 6e64 206f 7264 6572  l_text and order
-00018300: 5f62 7920 6973 204e 6f6e 653a 0d0a 2020  _by is None:..  
-00018310: 2020 2020 2020 2020 2020 6f72 6465 725f            order_
-00018320: 6279 203d 2065 6e75 6d73 2e4f 7264 6572  by = enums.Order
-00018330: 4279 2e73 6561 7263 685f 7261 6e6b 0d0a  By.search_rank..
-00018340: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
-00018350: 2076 616c 7565 206f 6620 7365 6172 6368   value of search
-00018360: 5f74 7970 6520 6973 2027 7365 7269 6573  _type is 'series
-00018370: 5f69 6427 2074 6865 6e20 7468 6520 6465  _id' then the de
-00018380: 6661 756c 7420 7661 6c75 6520 6f66 206f  fault value of o
-00018390: 7264 6572 5f62 7920 6973 2027 7365 7269  rder_by is 'seri
-000183a0: 6573 5f69 6427 2e0d 0a20 2020 2020 2020  es_id'...       
-000183b0: 2065 6c69 6620 7365 6172 6368 5f74 6578   elif search_tex
-000183c0: 7420 3d3d 2065 6e75 6d73 2e53 6561 7263  t == enums.Searc
-000183d0: 6854 7970 652e 7365 7269 6573 5f69 6420  hType.series_id 
-000183e0: 616e 6420 6f72 6465 725f 6279 2069 7320  and order_by is 
-000183f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00018400: 2020 206f 7264 6572 5f62 7920 3d20 656e     order_by = en
-00018410: 756d 732e 4f72 6465 7242 792e 7365 7269  ums.OrderBy.seri
-00018420: 6573 5f69 640d 0a0d 0a20 2020 2020 2020  es_id....       
-00018430: 2023 2049 6620 6f72 6465 725f 6279 2069   # If order_by i
-00018440: 7320 6571 7561 6c20 746f 2027 7365 6172  s equal to 'sear
-00018450: 6368 5f72 616e 6b27 206f 7220 2770 6f70  ch_rank' or 'pop
-00018460: 756c 6172 6974 7927 2c20 7468 656e 2074  ularity', then t
-00018470: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
-00018480: 206f 6620 736f 7274 5f6f 7264 6572 2069   of sort_order i
-00018490: 7320 2764 6573 6327 2e20 4f74 6865 7277  s 'desc'. Otherw
-000184a0: 6973 652c 2074 6865 2064 6566 6175 6c74  ise, the default
-000184b0: 2073 6f72 7420 6f72 6465 7220 6973 2027   sort order is '
-000184c0: 6173 6327 2e0d 0a20 2020 2020 2020 2069  asc'...        i
-000184d0: 6620 6f72 6465 725f 6279 203d 3d20 656e  f order_by == en
-000184e0: 756d 732e 4f72 6465 7242 792e 7365 6172  ums.OrderBy.sear
-000184f0: 6368 5f72 616e 6b20 6f72 206f 7264 6572  ch_rank or order
-00018500: 5f62 7920 3d3d 2065 6e75 6d73 2e4f 7264  _by == enums.Ord
-00018510: 6572 4279 2e70 6f70 756c 6172 6974 7920  erBy.popularity 
-00018520: 616e 6420 736f 7274 5f6f 7264 6572 2069  and sort_order i
-00018530: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00018540: 2020 2020 2073 6f72 745f 6f72 6465 7220       sort_order 
-00018550: 3d20 656e 756d 732e 536f 7274 4f72 6465  = enums.SortOrde
-00018560: 722e 6465 7363 0d0a 2020 2020 2020 2020  r.desc..        
-00018570: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00018580: 2020 2073 6f72 745f 6f72 6465 7220 3d20     sort_order = 
-00018590: 656e 756d 732e 536f 7274 4f72 6465 722e  enums.SortOrder.
-000185a0: 6173 630d 0a0d 0a20 2020 2020 2020 2069  asc....        i
-000185b0: 6620 6f72 6465 725f 6279 206e 6f74 2069  f order_by not i
-000185c0: 6e20 616c 6c6f 7765 645f 6f72 6465 7273  n allowed_orders
-000185d0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000185e0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000185f0: 2756 6172 6961 626c 6520 6f72 6465 725f  'Variable order_
-00018600: 6279 2028 7b7d 2920 6973 206e 6f74 206f  by ({}) is not o
-00018610: 6e65 206f 6620 7468 6520 7661 6c75 6573  ne of the values
-00018620: 3a20 7b7d 272e 666f 726d 6174 286f 7264  : {}'.format(ord
-00018630: 6572 5f62 792c 2027 2c20 272e 6a6f 696e  er_by, ', '.join
-00018640: 286d 6170 2873 7472 2c20 616c 6c6f 7765  (map(str, allowe
-00018650: 645f 6f72 6465 7273 2929 2929 0d0a 0d0a  d_orders))))....
-00018660: 2020 2020 2020 2020 6966 2073 6561 7263          if searc
-00018670: 685f 7479 7065 206e 6f74 2069 6e20 656e  h_type not in en
-00018680: 756d 732e 5365 6172 6368 5479 7065 3a0d  ums.SearchType:.
-00018690: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000186a0: 7365 2056 616c 7565 4572 726f 7228 2756  se ValueError('V
-000186b0: 6172 6961 626c 6520 7365 6172 6368 5f74  ariable search_t
-000186c0: 7970 6520 287b 7d29 2069 7320 6e6f 7420  ype ({}) is not 
-000186d0: 6f6e 6520 6f66 2074 6865 2076 616c 7565  one of the value
-000186e0: 733a 207b 7d27 2e66 6f72 6d61 7428 7365  s: {}'.format(se
-000186f0: 6172 6368 5f74 7970 652c 2027 2c20 272e  arch_type, ', '.
-00018700: 6a6f 696e 286d 6170 2873 7472 2c20 656e  join(map(str, en
-00018710: 756d 732e 5365 6172 6368 5479 7065 2929  ums.SearchType))
-00018720: 2929 0d0a 0d0a 2020 2020 2020 2020 6966  ))....        if
-00018730: 2066 696c 7465 725f 7661 7269 6162 6c65   filter_variable
-00018740: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00018750: 2066 696c 7465 725f 7661 7269 6162 6c65   filter_variable
-00018760: 206e 6f74 2069 6e20 656e 756d 732e 4669   not in enums.Fi
-00018770: 6c74 6572 5661 7269 6162 6c65 3a0d 0a20  lterVariable:.. 
-00018780: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00018790: 2056 616c 7565 4572 726f 7228 2756 6172   ValueError('Var
-000187a0: 6961 626c 6520 6669 6c74 6572 5f76 6172  iable filter_var
-000187b0: 6961 626c 6520 287b 7d29 2069 7320 6e6f  iable ({}) is no
+00017920: 2020 2020 2020 2074 6974 6c65 206f 6273         title obs
+00017930: 6572 7661 7469 6f6e 5f73 7461 7274 206f  ervation_start o
+00017940: 6273 6572 7661 7469 6f6e 5f65 6e64 2066  bservation_end f
+00017950: 7265 7175 656e 6379 2066 7265 7175 656e  requency frequen
+00017960: 6379 5f73 686f 7274 2020 2020 2020 2020  cy_short        
+00017970: 2020 2020 2020 2020 756e 6974 7320 756e          units un
+00017980: 6974 735f 7368 6f72 7420 2073 6561 736f  its_short  seaso
+00017990: 6e61 6c5f 6164 6a75 7374 6d65 6e74 2073  nal_adjustment s
+000179a0: 6561 736f 6e61 6c5f 6164 6a75 7374 6d65  easonal_adjustme
+000179b0: 6e74 5f73 686f 7274 2020 2020 2020 2020  nt_short        
+000179c0: 2020 2020 2020 6c61 7374 5f75 7064 6174        last_updat
+000179d0: 6564 2020 706f 7075 6c61 7269 7479 2020  ed  popularity  
+000179e0: 6772 6f75 705f 706f 7075 6c61 7269 7479  group_popularity
+000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a10: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00017a20: 7465 730d 0a20 2020 2020 2020 2020 2020  tes..           
+00017a30: 2069 640d 0a20 2020 2020 2020 2020 2020   id..           
+00017a40: 204d 5349 4d5a 4d50 2020 2020 2032 3032   MSIMZMP     202
+00017a50: 322d 3032 2d30 3520 2020 3230 3232 2d30  2-02-05   2022-0
+00017a60: 322d 3035 2020 2020 2020 2020 204d 6f6e  2-05         Mon
+00017a70: 6574 6172 7920 5365 7276 6963 6573 2049  etary Services I
+00017a80: 6e64 6578 3a20 4d5a 4d20 2870 7265 6665  ndex: MZM (prefe
+00017a90: 7272 6564 2920 2020 2020 2020 2031 3936  rred)        196
+00017aa0: 372d 3031 2d30 3120 2020 2020 2032 3031  7-01-01      201
+00017ab0: 332d 3132 2d30 3120 2020 4d6f 6e74 686c  3-12-01   Monthl
+00017ac0: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+00017ad0: 4d20 2042 696c 6c69 6f6e 7320 6f66 2044  M  Billions of D
+00017ae0: 6f6c 6c61 7273 2020 2042 696c 2e20 6f66  ollars   Bil. of
+00017af0: 2024 2020 5365 6173 6f6e 616c 6c79 2041   $  Seasonally A
+00017b00: 646a 7573 7465 6420 2020 2020 2020 2020  djusted         
+00017b10: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00017b20: 4120 3230 3134 2d30 312d 3137 2031 333a  A 2014-01-17 13:
+00017b30: 3136 3a34 322b 3030 3a30 3020 2020 2020  16:42+00:00     
+00017b40: 2020 2020 2032 3020 2020 2020 2020 2020       20         
+00017b50: 2020 2020 2020 2032 3020 2054 6865 204d         20  The M
+00017b60: 5349 206d 6561 7375 7265 2074 6865 2066  SI measure the f
+00017b70: 6c6f 7720 6f66 206d 6f6e 6574 6172 7920  low of monetary 
+00017b80: 7365 7276 6963 6573 202e 2e2e 0d0a 2020  services .....  
+00017b90: 2020 2020 2020 2020 2020 4d53 494d 3220            MSIM2 
+00017ba0: 2020 2020 2020 3230 3232 2d30 322d 3035        2022-02-05
+00017bb0: 2020 2032 3032 322d 3032 2d30 3520 2020     2022-02-05   
+00017bc0: 2020 2020 2020 204d 6f6e 6574 6172 7920         Monetary 
+00017bd0: 5365 7276 6963 6573 2049 6e64 6578 3a20  Services Index: 
+00017be0: 4d32 2028 7072 6566 6572 7265 6429 2020  M2 (preferred)  
+00017bf0: 2020 2020 2020 3139 3637 2d30 312d 3031        1967-01-01
+00017c00: 2020 2020 2020 3230 3133 2d31 322d 3031        2013-12-01
+00017c10: 2020 204d 6f6e 7468 6c79 2020 2020 2020     Monthly      
+00017c20: 2020 2020 2020 2020 204d 2020 4269 6c6c           M  Bill
+00017c30: 696f 6e73 206f 6620 446f 6c6c 6172 7320  ions of Dollars 
+00017c40: 2020 4269 6c2e 206f 6620 2420 2053 6561    Bil. of $  Sea
+00017c50: 736f 6e61 6c6c 7920 4164 6a75 7374 6564  sonally Adjusted
+00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c70: 2020 2020 2020 2020 5341 2032 3031 342d          SA 2014-
+00017c80: 3031 2d31 3720 3133 3a31 363a 3434 2b30  01-17 13:16:44+0
+00017c90: 303a 3030 2020 2020 2020 2020 2020 3136  0:00          16
+00017ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cb0: 3136 2020 5468 6520 4d53 4920 6d65 6173  16  The MSI meas
+00017cc0: 7572 6520 7468 6520 666c 6f77 206f 6620  ure the flow of 
+00017cd0: 6d6f 6e65 7461 7279 2073 6572 7669 6365  monetary service
+00017ce0: 7320 2e2e 2e0d 0a20 2020 2020 2020 2020  s .....         
+00017cf0: 2020 204d 5349 414c 4c50 2020 2020 2032     MSIALLP     2
+00017d00: 3032 322d 3032 2d30 3520 2020 3230 3232  022-02-05   2022
+00017d10: 2d30 322d 3035 2020 4d6f 6e65 7461 7279  -02-05  Monetary
+00017d20: 2053 6572 7669 6365 7320 496e 6465 783a   Services Index:
+00017d30: 2041 4c4c 2041 7373 6574 7320 2870 7265   ALL Assets (pre
+00017d40: 6665 7272 6564 2920 2020 2020 2020 2031  ferred)        1
+00017d50: 3936 372d 3031 2d30 3120 2020 2020 2032  967-01-01      2
+00017d60: 3031 332d 3132 2d30 3120 2020 4d6f 6e74  013-12-01   Mont
+00017d70: 686c 7920 2020 2020 2020 2020 2020 2020  hly             
+00017d80: 2020 4d20 2042 696c 6c69 6f6e 7320 6f66    M  Billions of
+00017d90: 2044 6f6c 6c61 7273 2020 2042 696c 2e20   Dollars   Bil. 
+00017da0: 6f66 2024 2020 5365 6173 6f6e 616c 6c79  of $  Seasonally
+00017db0: 2041 646a 7573 7465 6420 2020 2020 2020   Adjusted       
+00017dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017dd0: 2053 4120 3230 3134 2d30 312d 3137 2031   SA 2014-01-17 1
+00017de0: 333a 3136 3a34 352b 3030 3a30 3020 2020  3:16:45+00:00   
+00017df0: 2020 2020 2020 2031 3420 2020 2020 2020         14       
+00017e00: 2020 2020 2020 2020 2031 3420 2054 6865           14  The
+00017e10: 204d 5349 206d 6561 7375 7265 2074 6865   MSI measure the
+00017e20: 2066 6c6f 7720 6f66 206d 6f6e 6574 6172   flow of monetar
+00017e30: 7920 7365 7276 6963 6573 202e 2e2e 0d0a  y services .....
+00017e40: 2020 2020 2020 2020 2020 2020 4d53 494d              MSIM
+00017e50: 3150 2020 2020 2020 3230 3232 2d30 322d  1P      2022-02-
+00017e60: 3035 2020 2032 3032 322d 3032 2d30 3520  05   2022-02-05 
+00017e70: 2020 2020 2020 2020 204d 6f6e 6574 6172           Monetar
+00017e80: 7920 5365 7276 6963 6573 2049 6e64 6578  y Services Index
+00017e90: 3a20 4d31 2028 7072 6566 6572 7265 6429  : M1 (preferred)
+00017ea0: 2020 2020 2020 2020 3139 3637 2d30 312d          1967-01-
+00017eb0: 3031 2020 2020 2020 3230 3133 2d31 322d  01      2013-12-
+00017ec0: 3031 2020 204d 6f6e 7468 6c79 2020 2020  01   Monthly    
+00017ed0: 2020 2020 2020 2020 2020 204d 2020 4269             M  Bi
+00017ee0: 6c6c 696f 6e73 206f 6620 446f 6c6c 6172  llions of Dollar
+00017ef0: 7320 2020 4269 6c2e 206f 6620 2420 2053  s   Bil. of $  S
+00017f00: 6561 736f 6e61 6c6c 7920 4164 6a75 7374  easonally Adjust
+00017f10: 6564 2020 2020 2020 2020 2020 2020 2020  ed              
+00017f20: 2020 2020 2020 2020 2020 5341 2032 3031            SA 201
+00017f30: 342d 3031 2d31 3720 3133 3a31 363a 3435  4-01-17 13:16:45
+00017f40: 2b30 303a 3030 2020 2020 2020 2020 2020  +00:00          
+00017f50: 2039 2020 2020 2020 2020 2020 2020 2020   9              
+00017f60: 2020 2039 2020 5468 6520 4d53 4920 6d65     9  The MSI me
+00017f70: 6173 7572 6520 7468 6520 666c 6f77 206f  asure the flow o
+00017f80: 6620 6d6f 6e65 7461 7279 2073 6572 7669  f monetary servi
+00017f90: 6365 7320 2e2e 2e0d 0a20 2020 2020 2020  ces .....       
+00017fa0: 2020 2020 204d 5349 4d32 4120 2020 2020       MSIM2A     
+00017fb0: 2032 3032 322d 3032 2d30 3520 2020 3230   2022-02-05   20
+00017fc0: 3232 2d30 322d 3035 2020 2020 2020 2020  22-02-05        
+00017fd0: 4d6f 6e65 7461 7279 2053 6572 7669 6365  Monetary Service
+00017fe0: 7320 496e 6465 783a 204d 3220 2861 6c74  s Index: M2 (alt
+00017ff0: 6572 6e61 7469 7665 2920 2020 2020 2020  ernative)       
+00018000: 2031 3936 372d 3031 2d30 3120 2020 2020   1967-01-01     
+00018010: 2032 3031 332d 3132 2d30 3120 2020 4d6f   2013-12-01   Mo
+00018020: 6e74 686c 7920 2020 2020 2020 2020 2020  nthly           
+00018030: 2020 2020 4d20 2042 696c 6c69 6f6e 7320      M  Billions 
+00018040: 6f66 2044 6f6c 6c61 7273 2020 2042 696c  of Dollars   Bil
+00018050: 2e20 6f66 2024 2020 5365 6173 6f6e 616c  . of $  Seasonal
+00018060: 6c79 2041 646a 7573 7465 6420 2020 2020  ly Adjusted     
+00018070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018080: 2020 2053 4120 3230 3134 2d30 312d 3137     SA 2014-01-17
+00018090: 2031 333a 3136 3a34 342b 3030 3a30 3020   13:16:44+00:00 
+000180a0: 2020 2020 2020 2020 2020 3820 2020 2020            8     
+000180b0: 2020 2020 2020 2020 2020 2020 3820 2054              8  T
+000180c0: 6865 204d 5349 206d 6561 7375 7265 2074  he MSI measure t
+000180d0: 6865 2066 6c6f 7720 6f66 206d 6f6e 6574  he flow of monet
+000180e0: 6172 7920 7365 7276 6963 6573 202e 2e2e  ary services ...
+000180f0: 0d0a 2020 2020 2020 2020 6060 600d 0a20  ..        ```.. 
+00018100: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
+00018110: 2020 2020 2020 616c 6c6f 7765 645f 6f72        allowed_or
+00018120: 6465 7273 203d 205b 0d0a 2020 2020 2020  ders = [..      
+00018130: 2020 2020 2020 656e 756d 732e 4f72 6465        enums.Orde
+00018140: 7242 792e 7365 6172 6368 5f72 616e 6b2c  rBy.search_rank,
+00018150: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+00018160: 756d 732e 4f72 6465 7242 792e 7365 7269  ums.OrderBy.seri
+00018170: 6573 5f69 642c 0d0a 2020 2020 2020 2020  es_id,..        
+00018180: 2020 2020 656e 756d 732e 4f72 6465 7242      enums.OrderB
+00018190: 792e 7469 746c 652c 0d0a 2020 2020 2020  y.title,..      
+000181a0: 2020 2020 2020 656e 756d 732e 4f72 6465        enums.Orde
+000181b0: 7242 792e 756e 6974 732c 0d0a 2020 2020  rBy.units,..    
+000181c0: 2020 2020 2020 2020 656e 756d 732e 4f72          enums.Or
+000181d0: 6465 7242 792e 6672 6571 7565 6e63 792c  derBy.frequency,
+000181e0: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+000181f0: 756d 732e 4f72 6465 7242 792e 7365 6173  ums.OrderBy.seas
+00018200: 6f6e 616c 5f61 646a 7573 746d 656e 742c  onal_adjustment,
+00018210: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+00018220: 756d 732e 4f72 6465 7242 792e 7265 616c  ums.OrderBy.real
+00018230: 7469 6d65 5f73 7461 7274 2c0d 0a20 2020  time_start,..   
+00018240: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
+00018250: 7264 6572 4279 2e72 6561 6c74 696d 655f  rderBy.realtime_
+00018260: 656e 642c 0d0a 2020 2020 2020 2020 2020  end,..          
+00018270: 2020 656e 756d 732e 4f72 6465 7242 792e    enums.OrderBy.
+00018280: 6c61 7374 5f75 7064 6174 6564 2c0d 0a20  last_updated,.. 
+00018290: 2020 2020 2020 2020 2020 2065 6e75 6d73             enums
+000182a0: 2e4f 7264 6572 4279 2e6f 6273 6572 7661  .OrderBy.observa
+000182b0: 7469 6f6e 5f73 7461 7274 2c0d 0a20 2020  tion_start,..   
+000182c0: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
+000182d0: 7264 6572 4279 2e6f 6273 6572 7661 7469  rderBy.observati
+000182e0: 6f6e 5f65 6e64 2c0d 0a20 2020 2020 2020  on_end,..       
+000182f0: 2020 2020 2065 6e75 6d73 2e4f 7264 6572       enums.Order
+00018300: 4279 2e70 6f70 756c 6172 6974 792c 0d0a  By.popularity,..
+00018310: 2020 2020 2020 2020 2020 2020 656e 756d              enum
+00018320: 732e 4f72 6465 7242 792e 6772 6f75 705f  s.OrderBy.group_
+00018330: 706f 7075 6c61 7269 7479 0d0a 2020 2020  popularity..    
+00018340: 2020 2020 5d0d 0a0d 0a20 2020 2020 2020      ]....       
+00018350: 2023 2049 6620 7468 6520 7661 6c75 6520   # If the value 
+00018360: 6f66 2073 6561 7263 685f 7479 7065 2069  of search_type i
+00018370: 7320 2766 756c 6c5f 7465 7874 2720 7468  s 'full_text' th
+00018380: 656e 2074 6865 2064 6566 6175 6c74 2076  en the default v
+00018390: 616c 7565 206f 6620 6f72 6465 725f 6279  alue of order_by
+000183a0: 2069 7320 2773 6561 7263 685f 7261 6e6b   is 'search_rank
+000183b0: 272e 0d0a 2020 2020 2020 2020 6966 2073  '...        if s
+000183c0: 6561 7263 685f 7479 7065 203d 3d20 656e  earch_type == en
+000183d0: 756d 732e 5365 6172 6368 5479 7065 2e66  ums.SearchType.f
+000183e0: 756c 6c5f 7465 7874 2061 6e64 206f 7264  ull_text and ord
+000183f0: 6572 5f62 7920 6973 204e 6f6e 653a 0d0a  er_by is None:..
+00018400: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
+00018410: 725f 6279 203d 2065 6e75 6d73 2e4f 7264  r_by = enums.Ord
+00018420: 6572 4279 2e73 6561 7263 685f 7261 6e6b  erBy.search_rank
+00018430: 0d0a 2020 2020 2020 2020 2320 4966 2074  ..        # If t
+00018440: 6865 2076 616c 7565 206f 6620 7365 6172  he value of sear
+00018450: 6368 5f74 7970 6520 6973 2027 7365 7269  ch_type is 'seri
+00018460: 6573 5f69 6427 2074 6865 6e20 7468 6520  es_id' then the 
+00018470: 6465 6661 756c 7420 7661 6c75 6520 6f66  default value of
+00018480: 206f 7264 6572 5f62 7920 6973 2027 7365   order_by is 'se
+00018490: 7269 6573 5f69 6427 2e0d 0a20 2020 2020  ries_id'...     
+000184a0: 2020 2065 6c69 6620 7365 6172 6368 5f74     elif search_t
+000184b0: 6578 7420 3d3d 2065 6e75 6d73 2e53 6561  ext == enums.Sea
+000184c0: 7263 6854 7970 652e 7365 7269 6573 5f69  rchType.series_i
+000184d0: 6420 616e 6420 6f72 6465 725f 6279 2069  d and order_by i
+000184e0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+000184f0: 2020 2020 206f 7264 6572 5f62 7920 3d20       order_by = 
+00018500: 656e 756d 732e 4f72 6465 7242 792e 7365  enums.OrderBy.se
+00018510: 7269 6573 5f69 640d 0a0d 0a20 2020 2020  ries_id....     
+00018520: 2020 2023 2049 6620 6f72 6465 725f 6279     # If order_by
+00018530: 2069 7320 6571 7561 6c20 746f 2027 7365   is equal to 'se
+00018540: 6172 6368 5f72 616e 6b27 206f 7220 2770  arch_rank' or 'p
+00018550: 6f70 756c 6172 6974 7927 2c20 7468 656e  opularity', then
+00018560: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
+00018570: 7565 206f 6620 736f 7274 5f6f 7264 6572  ue of sort_order
+00018580: 2069 7320 2764 6573 6327 2e20 4f74 6865   is 'desc'. Othe
+00018590: 7277 6973 652c 2074 6865 2064 6566 6175  rwise, the defau
+000185a0: 6c74 2073 6f72 7420 6f72 6465 7220 6973  lt sort order is
+000185b0: 2027 6173 6327 2e0d 0a20 2020 2020 2020   'asc'...       
+000185c0: 2069 6620 6f72 6465 725f 6279 203d 3d20   if order_by == 
+000185d0: 656e 756d 732e 4f72 6465 7242 792e 7365  enums.OrderBy.se
+000185e0: 6172 6368 5f72 616e 6b20 6f72 206f 7264  arch_rank or ord
+000185f0: 6572 5f62 7920 3d3d 2065 6e75 6d73 2e4f  er_by == enums.O
+00018600: 7264 6572 4279 2e70 6f70 756c 6172 6974  rderBy.popularit
+00018610: 7920 616e 6420 736f 7274 5f6f 7264 6572  y and sort_order
+00018620: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00018630: 2020 2020 2020 2073 6f72 745f 6f72 6465         sort_orde
+00018640: 7220 3d20 656e 756d 732e 536f 7274 4f72  r = enums.SortOr
+00018650: 6465 722e 6465 7363 0d0a 2020 2020 2020  der.desc..      
+00018660: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00018670: 2020 2020 2073 6f72 745f 6f72 6465 7220       sort_order 
+00018680: 3d20 656e 756d 732e 536f 7274 4f72 6465  = enums.SortOrde
+00018690: 722e 6173 630d 0a0d 0a20 2020 2020 2020  r.asc....       
+000186a0: 2069 6620 6f72 6465 725f 6279 206e 6f74   if order_by not
+000186b0: 2069 6e20 616c 6c6f 7765 645f 6f72 6465   in allowed_orde
+000186c0: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
+000186d0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+000186e0: 7228 2756 6172 6961 626c 6520 6f72 6465  r('Variable orde
+000186f0: 725f 6279 2028 7b7d 2920 6973 206e 6f74  r_by ({}) is not
+00018700: 206f 6e65 206f 6620 7468 6520 7661 6c75   one of the valu
+00018710: 6573 3a20 7b7d 272e 666f 726d 6174 286f  es: {}'.format(o
+00018720: 7264 6572 5f62 792c 2027 2c20 272e 6a6f  rder_by, ', '.jo
+00018730: 696e 286d 6170 2873 7472 2c20 616c 6c6f  in(map(str, allo
+00018740: 7765 645f 6f72 6465 7273 2929 2929 0d0a  wed_orders))))..
+00018750: 0d0a 2020 2020 2020 2020 6966 2073 6561  ..        if sea
+00018760: 7263 685f 7479 7065 206e 6f74 2069 6e20  rch_type not in 
+00018770: 656e 756d 732e 5365 6172 6368 5479 7065  enums.SearchType
+00018780: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00018790: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000187a0: 2756 6172 6961 626c 6520 7365 6172 6368  'Variable search
+000187b0: 5f74 7970 6520 287b 7d29 2069 7320 6e6f  _type ({}) is no
 000187c0: 7420 6f6e 6520 6f66 2074 6865 2076 616c  t one of the val
 000187d0: 7565 733a 207b 7d27 2e66 6f72 6d61 7428  ues: {}'.format(
-000187e0: 6669 6c74 6572 5f76 6172 6961 626c 652c  filter_variable,
-000187f0: 2027 2c20 272e 6a6f 696e 286d 6170 2873   ', '.join(map(s
-00018800: 7472 2c20 656e 756d 732e 4669 6c74 6572  tr, enums.Filter
-00018810: 5661 7269 6162 6c65 2929 2929 0d0a 0d0a  Variable))))....
-00018820: 2020 2020 2020 2020 6966 2072 6561 6c74          if realt
-00018830: 696d 655f 7374 6172 7420 6973 206e 6f74  ime_start is not
-00018840: 204e 6f6e 6520 616e 6420 7265 616c 7469   None and realti
-00018850: 6d65 5f73 7461 7274 203c 2064 6174 6528  me_start < date(
-00018860: 3137 3736 2c20 372c 2034 293a 0d0a 2020  1776, 7, 4):..  
-00018870: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00018880: 5661 6c75 6545 7272 6f72 2827 5661 7269  ValueError('Vari
-00018890: 6162 6c65 2072 6561 6c74 696d 655f 7374  able realtime_st
-000188a0: 6172 7420 2822 7b7d 2229 2069 7320 6265  art ("{}") is be
-000188b0: 666f 7265 206d 696e 2064 6174 6520 3137  fore min date 17
-000188c0: 3736 2d30 372d 3034 2e27 2e66 6f72 6d61  76-07-04.'.forma
-000188d0: 7428 7265 616c 7469 6d65 5f73 7461 7274  t(realtime_start
-000188e0: 2929 0d0a 0d0a 2020 2020 2020 2020 6966  ))....        if
-000188f0: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
-00018900: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-00018910: 7265 616c 7469 6d65 5f65 6e64 2069 7320  realtime_end is 
-00018920: 6e6f 7420 4e6f 6e65 2061 6e64 2072 6561  not None and rea
-00018930: 6c74 696d 655f 7374 6172 7420 3e20 7265  ltime_start > re
-00018940: 616c 7469 6d65 5f65 6e64 3a0d 0a20 2020  altime_end:..   
-00018950: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00018960: 616c 7565 4572 726f 7228 2754 6865 2064  alueError('The d
-00018970: 6174 6520 7365 7420 6279 2076 6172 6961  ate set by varia
-00018980: 626c 6520 7265 616c 7469 6d65 5f73 7461  ble realtime_sta
-00018990: 7274 2028 227b 7d22 2920 6361 6e20 6e6f  rt ("{}") can no
-000189a0: 7420 6265 2061 6674 6572 2074 6865 2064  t be after the d
-000189b0: 6174 6520 7365 7420 6279 2076 6172 6961  ate set by varia
-000189c0: 626c 6520 7265 616c 7469 6d65 5f65 6e64  ble realtime_end
-000189d0: 2028 227b 7d22 292e 272e 666f 726d 6174   ("{}").'.format
-000189e0: 2872 6561 6c74 696d 655f 7374 6172 742c  (realtime_start,
-000189f0: 2072 6561 6c74 696d 655f 656e 6429 290d   realtime_end)).
-00018a00: 0a0d 0a20 2020 2020 2020 2064 6620 3d20  ...        df = 
-00018a10: 7064 2e44 6174 6146 7261 6d65 280d 0a20  pd.DataFrame(.. 
-00018a20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018a30: 5f63 6c69 656e 742e 6765 7428 0d0a 2020  _client.get(..  
-00018a40: 2020 2020 2020 2020 2020 2020 2020 272f                '/
-00018a50: 6672 6564 2f73 6572 6965 732f 7365 6172  fred/series/sear
-00018a60: 6368 272c 0d0a 2020 2020 2020 2020 2020  ch',..          
-00018a70: 2020 2020 2020 2773 6572 6965 7373 272c        'seriess',
-00018a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018a90: 2020 6c69 6d69 743d 3130 3030 2c0d 0a20    limit=1000,.. 
-00018aa0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018ab0: 6561 7263 685f 7465 7874 3d73 6561 7263  earch_text=searc
-00018ac0: 685f 7465 7874 2c0d 0a20 2020 2020 2020  h_text,..       
-00018ad0: 2020 2020 2020 2020 2073 6561 7263 685f           search_
-00018ae0: 7479 7065 3d73 6561 7263 685f 7479 7065  type=search_type
-00018af0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00018b00: 2020 2072 6561 6c74 696d 655f 7374 6172     realtime_star
-00018b10: 743d 7265 616c 7469 6d65 5f73 7461 7274  t=realtime_start
-00018b20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00018b30: 2020 2072 6561 6c74 696d 655f 656e 643d     realtime_end=
-00018b40: 7265 616c 7469 6d65 5f65 6e64 2c0d 0a20  realtime_end,.. 
-00018b50: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00018b60: 7264 6572 5f62 793d 6f72 6465 725f 6279  rder_by=order_by
-00018b70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00018b80: 2020 2073 6f72 745f 6f72 6465 723d 736f     sort_order=so
-00018b90: 7274 5f6f 7264 6572 2c0d 0a20 2020 2020  rt_order,..     
-00018ba0: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-00018bb0: 725f 7661 7269 6162 6c65 3d66 696c 7465  r_variable=filte
-00018bc0: 725f 7661 7269 6162 6c65 2c0d 0a20 2020  r_variable,..   
-00018bd0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00018be0: 7465 725f 7661 6c75 653d 6669 6c74 6572  ter_value=filter
-00018bf0: 5f76 616c 7565 2c0d 0a20 2020 2020 2020  _value,..       
-00018c00: 2020 2020 2020 2020 2074 6167 5f6e 616d           tag_nam
-00018c10: 6573 3d74 6167 5f6e 616d 6573 2c0d 0a20  es=tag_names,.. 
-00018c20: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00018c30: 7863 6c75 6465 5f74 6167 5f6e 616d 6573  xclude_tag_names
-00018c40: 3d65 7863 6c75 6465 5f74 6167 5f6e 616d  =exclude_tag_nam
-00018c50: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
-00018c60: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
-00018c70: 2020 2020 2020 2020 6461 7465 5f63 6f6c          date_col
-00018c80: 756d 6e73 203d 205b 0d0a 2020 2020 2020  umns = [..      
-00018c90: 2020 2020 2020 2772 6561 6c74 696d 655f        'realtime_
-00018ca0: 7374 6172 7427 2c20 2772 6561 6c74 696d  start', 'realtim
-00018cb0: 655f 656e 6427 2c0d 0a20 2020 2020 2020  e_end',..       
-00018cc0: 2020 2020 2027 6f62 7365 7276 6174 696f       'observatio
-00018cd0: 6e5f 7374 6172 7427 2c20 276f 6273 6572  n_start', 'obser
-00018ce0: 7661 7469 6f6e 5f65 6e64 272c 0d0a 2020  vation_end',..  
-00018cf0: 2020 2020 2020 5d0d 0a0d 0a20 2020 2020        ]....     
-00018d00: 2020 2069 6620 6e6f 7420 6466 2e65 6d70     if not df.emp
-00018d10: 7479 3a0d 0a20 2020 2020 2020 2020 2020  ty:..           
-00018d20: 2064 665b 6461 7465 5f63 6f6c 756d 6e73   df[date_columns
-00018d30: 5d20 3d20 6466 5b64 6174 655f 636f 6c75  ] = df[date_colu
-00018d40: 6d6e 735d 2e61 7070 6c79 2870 642e 746f  mns].apply(pd.to
-00018d50: 5f64 6174 6574 696d 652c 2066 6f72 6d61  _datetime, forma
-00018d60: 743d 2725 592d 256d 2d25 6427 290d 0a20  t='%Y-%m-%d').. 
-00018d70: 2020 2020 2020 2020 2020 2064 662e 6c61             df.la
-00018d80: 7374 5f75 7064 6174 6564 203d 2070 642e  st_updated = pd.
-00018d90: 746f 5f64 6174 6574 696d 6528 6466 2e6c  to_datetime(df.l
-00018da0: 6173 745f 7570 6461 7465 6420 2b20 2730  ast_updated + '0
-00018db0: 3027 2c20 7574 633d 5472 7565 2c20 666f  0', utc=True, fo
-00018dc0: 726d 6174 3d27 2559 2d25 6d2d 2564 2025  rmat='%Y-%m-%d %
-00018dd0: 483a 254d 3a25 5325 7a27 290d 0a0d 0a20  H:%M:%S%z').... 
-00018de0: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
-00018df0: 6466 2e61 7374 7970 6528 6474 7970 653d  df.astype(dtype=
-00018e00: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00018e10: 2020 2027 6964 273a 2027 7374 7269 6e67     'id': 'string
-00018e20: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00018e30: 2020 2020 2774 6974 6c65 273a 2027 7374      'title': 'st
-00018e40: 7269 6e67 272c 0d0a 2020 2020 2020 2020  ring',..        
-00018e50: 2020 2020 2020 2020 276e 6f74 6573 273a          'notes':
-00018e60: 2027 7374 7269 6e67 272c 0d0a 2020 2020   'string',..    
-00018e70: 2020 2020 2020 2020 2020 2020 2766 7265              'fre
-00018e80: 7175 656e 6379 273a 2027 6361 7465 676f  quency': 'catego
-00018e90: 7279 272c 0d0a 2020 2020 2020 2020 2020  ry',..          
-00018ea0: 2020 2020 2020 2766 7265 7175 656e 6379        'frequency
-00018eb0: 5f73 686f 7274 273a 2027 6361 7465 676f  _short': 'catego
-00018ec0: 7279 272c 0d0a 2020 2020 2020 2020 2020  ry',..          
-00018ed0: 2020 2020 2020 2775 6e69 7473 5f73 686f        'units_sho
-00018ee0: 7274 273a 2027 6361 7465 676f 7279 272c  rt': 'category',
-00018ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018f00: 2020 2775 6e69 7473 273a 2027 6361 7465    'units': 'cate
-00018f10: 676f 7279 272c 0d0a 2020 2020 2020 2020  gory',..        
-00018f20: 2020 2020 2020 2020 2773 6561 736f 6e61          'seasona
-00018f30: 6c5f 6164 6a75 7374 6d65 6e74 273a 2027  l_adjustment': '
-00018f40: 6361 7465 676f 7279 272c 0d0a 2020 2020  category',..    
-00018f50: 2020 2020 2020 2020 2020 2020 2773 6561              'sea
-00018f60: 736f 6e61 6c5f 6164 6a75 7374 6d65 6e74  sonal_adjustment
-00018f70: 5f73 686f 7274 273a 2027 6361 7465 676f  _short': 'catego
-00018f80: 7279 270d 0a20 2020 2020 2020 2020 2020  ry'..           
-00018f90: 207d 292e 7365 745f 696e 6465 7828 2769   }).set_index('i
-00018fa0: 6427 290d 0a0d 0a20 2020 2020 2020 2072  d')....        r
-00018fb0: 6574 7572 6e20 6466 0d0a 0d0a 2020 2020  eturn df....    
-00018fc0: 6465 6620 7365 7269 6573 5f73 6561 7263  def series_searc
-00018fd0: 685f 7461 6773 280d 0a20 2020 2020 2020  h_tags(..       
-00018fe0: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-00018ff0: 2020 2020 2020 2020 7365 7269 6573 5f73          series_s
-00019000: 6561 7263 685f 7465 7874 3a20 7374 722c  earch_text: str,
-00019010: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00019020: 616c 7469 6d65 5f73 7461 7274 3a20 6461  altime_start: da
-00019030: 7465 203d 204e 6f6e 652c 0d0a 2020 2020  te = None,..    
-00019040: 2020 2020 2020 2020 7265 616c 7469 6d65          realtime
-00019050: 5f65 6e64 3a20 6461 7465 203d 204e 6f6e  _end: date = Non
-00019060: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00019070: 7461 675f 6e61 6d65 733a 204c 6973 745b  tag_names: List[
-00019080: 7374 725d 203d 204e 6f6e 652c 0d0a 2020  str] = None,..  
-00019090: 2020 2020 2020 2020 2020 7461 675f 6772            tag_gr
-000190a0: 6f75 705f 6964 3a20 656e 756d 732e 5461  oup_id: enums.Ta
-000190b0: 6747 726f 7570 4944 203d 204e 6f6e 652c  gGroupID = None,
-000190c0: 0d0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
-000190d0: 675f 7365 6172 6368 5f74 6578 743a 2073  g_search_text: s
-000190e0: 7472 203d 204e 6f6e 652c 0d0a 2020 2020  tr = None,..    
-000190f0: 2020 2020 2020 2020 6f72 6465 725f 6279          order_by
-00019100: 3a20 656e 756d 732e 4f72 6465 7242 7920  : enums.OrderBy 
-00019110: 3d20 656e 756d 732e 4f72 6465 7242 792e  = enums.OrderBy.
-00019120: 7365 7269 6573 5f63 6f75 6e74 2c0d 0a20  series_count,.. 
-00019130: 2020 2020 2020 2020 2020 2073 6f72 745f             sort_
-00019140: 6f72 6465 723a 2065 6e75 6d73 2e53 6f72  order: enums.Sor
-00019150: 744f 7264 6572 203d 2065 6e75 6d73 2e53  tOrder = enums.S
-00019160: 6f72 744f 7264 6572 2e61 7363 0d0a 2020  ortOrder.asc..  
-00019170: 2020 2920 2d3e 2070 642e 4461 7461 4672    ) -> pd.DataFr
-00019180: 616d 653a 0d0a 2020 2020 2020 2020 2222  ame:..        ""
-00019190: 220d 0a20 2020 2020 2020 2023 2320 5061  "..        ## Pa
-000191a0: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-000191b0: 2020 6073 6572 6965 735f 7365 6172 6368    `series_search
-000191c0: 5f74 6578 7460 0d0a 2020 2020 2020 2020  _text`..        
-000191d0: 5468 6520 776f 7264 7320 746f 206d 6174  The words to mat
-000191e0: 6368 2061 6761 696e 7374 2065 636f 6e6f  ch against econo
-000191f0: 6d69 6320 6461 7461 2073 6572 6965 732e  mic data series.
-00019200: 0d0a 0d0a 2020 2020 2020 2020 6072 6561  ....        `rea
-00019210: 6c74 696d 655f 7374 6172 7460 0d0a 2020  ltime_start`..  
-00019220: 2020 2020 2020 5468 6520 7374 6172 7420        The start 
-00019230: 6f66 2074 6865 2072 6561 6c2d 7469 6d65  of the real-time
-00019240: 2070 6572 696f 642e 2046 6f72 206d 6f72   period. For mor
-00019250: 6520 696e 666f 726d 6174 696f 6e2c 2073  e information, s
-00019260: 6565 205b 5265 616c 2d54 696d 6520 5065  ee [Real-Time Pe
-00019270: 7269 6f64 735d 2868 7474 7073 3a2f 2f66  riods](https://f
-00019280: 7265 642e 7374 6c6f 7569 7366 6564 2e6f  red.stlouisfed.o
-00019290: 7267 2f64 6f63 732f 6170 692f 6672 6564  rg/docs/api/fred
-000192a0: 2f72 6561 6c74 696d 655f 7065 7269 6f64  /realtime_period
-000192b0: 2e68 746d 6c29 2e0d 0a0d 0a20 2020 2020  .html).....     
-000192c0: 2020 2060 7265 616c 7469 6d65 5f65 6e64     `realtime_end
-000192d0: 600d 0a20 2020 2020 2020 2054 6865 2065  `..        The e
-000192e0: 6e64 206f 6620 7468 6520 7265 616c 2d74  nd of the real-t
-000192f0: 696d 6520 7065 7269 6f64 2e20 466f 7220  ime period. For 
-00019300: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-00019310: 2c20 7365 6520 5b52 6561 6c2d 5469 6d65  , see [Real-Time
-00019320: 2050 6572 696f 6473 5d28 6874 7470 733a   Periods](https:
-00019330: 2f2f 6672 6564 2e73 746c 6f75 6973 6665  //fred.stlouisfe
-00019340: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
-00019350: 7265 642f 7265 616c 7469 6d65 5f70 6572  red/realtime_per
-00019360: 696f 642e 6874 6d6c 292e 0d0a 0d0a 2020  iod.html).....  
-00019370: 2020 2020 2020 6074 6167 5f6e 616d 6573        `tag_names
-00019380: 600d 0a20 2020 2020 2020 2041 2073 656d  `..        A sem
-00019390: 6963 6f6c 6f6e 2064 656c 696d 6974 6564  icolon delimited
-000193a0: 206c 6973 7420 6f66 2074 6167 206e 616d   list of tag nam
-000193b0: 6573 2074 6f20 6f6e 6c79 2069 6e63 6c75  es to only inclu
-000193c0: 6465 2069 6e20 7468 6520 7265 7370 6f6e  de in the respon
-000193d0: 7365 2e20 5365 6520 7468 6520 7265 6c61  se. See the rela
-000193e0: 7465 6420 7265 7175 6573 7420 6672 6564  ted request fred
-000193f0: 2f73 6572 6965 732f 7365 6172 6368 2f72  /series/search/r
-00019400: 656c 6174 6564 5f74 6167 732e 0d0a 0d0a  elated_tags.....
-00019410: 2020 2020 2020 2020 6074 6167 5f67 726f          `tag_gro
-00019420: 7570 5f69 6460 0d0a 2020 2020 2020 2020  up_id`..        
-00019430: 4120 7461 6720 6772 6f75 7020 6964 2074  A tag group id t
-00019440: 6f20 6669 6c74 6572 2074 6167 7320 6279  o filter tags by
-00019450: 2074 7970 652e 0d0a 0d0a 2020 2020 2020   type.....      
-00019460: 2020 6074 6167 5f73 6561 7263 685f 7465    `tag_search_te
-00019470: 7874 600d 0a20 2020 2020 2020 2054 6865  xt`..        The
-00019480: 2077 6f72 6473 2074 6f20 6669 6e64 206d   words to find m
-00019490: 6174 6368 696e 6720 7461 6773 2077 6974  atching tags wit
-000194a0: 682e 0d0a 0d0a 2020 2020 2020 2020 606f  h.....        `o
-000194b0: 7264 6572 5f62 7960 0d0a 2020 2020 2020  rder_by`..      
-000194c0: 2020 4f72 6465 7220 7265 7375 6c74 7320    Order results 
-000194d0: 6279 2076 616c 7565 7320 6f66 2074 6865  by values of the
-000194e0: 2073 7065 6369 6669 6564 2061 7474 7269   specified attri
-000194f0: 6275 7465 2e0d 0a0d 0a20 2020 2020 2020  bute.....       
-00019500: 2060 736f 7274 5f6f 7264 6572 600d 0a20   `sort_order`.. 
-00019510: 2020 2020 2020 2053 6f72 7420 7265 7375         Sort resu
-00019520: 6c74 7320 6973 2061 7363 656e 6469 6e67  lts is ascending
-00019530: 206f 7220 6465 7363 656e 6469 6e67 206f   or descending o
-00019540: 7264 6572 2066 6f72 2061 7474 7269 6275  rder for attribu
-00019550: 7465 2076 616c 7565 7320 7370 6563 6966  te values specif
-00019560: 6965 6420 6279 206f 7264 6572 5f62 792e  ied by order_by.
-00019570: 0d0a 0d0a 2020 2020 2020 2020 2323 2044  ....        ## D
-00019580: 6573 6372 6970 7469 6f6e 0d0a 2020 2020  escription..    
-00019590: 2020 2020 6874 7470 733a 2f2f 6672 6564      https://fred
-000195a0: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
-000195b0: 646f 6373 2f61 7069 2f66 7265 642f 7365  docs/api/fred/se
-000195c0: 7269 6573 5f73 6561 7263 685f 7461 6773  ries_search_tags
-000195d0: 2e68 746d 6c0d 0a0d 0a20 2020 2020 2020  .html....       
-000195e0: 2047 6574 2074 6865 2046 5245 4420 7461   Get the FRED ta
-000195f0: 6773 2066 6f72 2061 2073 6572 6965 7320  gs for a series 
-00019600: 7365 6172 6368 2e20 4f70 7469 6f6e 616c  search. Optional
-00019610: 6c79 2c20 6669 6c74 6572 2072 6573 756c  ly, filter resul
-00019620: 7473 2062 7920 7461 6720 6e61 6d65 2c20  ts by tag name, 
-00019630: 7461 6720 6772 6f75 702c 206f 7220 7461  tag group, or ta
-00019640: 6720 7365 6172 6368 2e20 5365 6520 7468  g search. See th
-00019650: 6520 7265 6c61 7465 6420 7265 7175 6573  e related reques
-00019660: 7420 6672 6564 2f73 6572 6965 732f 7365  t fred/series/se
-00019670: 6172 6368 2f72 656c 6174 6564 5f74 6167  arch/related_tag
-00019680: 732e 0d0a 0d0a 2020 2020 2020 2020 2323  s.....        ##
-00019690: 2041 5049 2052 6571 7565 7374 2028 4854   API Request (HT
-000196a0: 5450 5320 4745 5429 0d0a 2020 2020 2020  TPS GET)..      
-000196b0: 2020 6874 7470 733a 2f2f 6170 692e 7374    https://api.st
-000196c0: 6c6f 7569 7366 6564 2e6f 7267 2f66 7265  louisfed.org/fre
-000196d0: 642f 7365 7269 6573 2f73 6561 7263 682f  d/series/search/
-000196e0: 7461 6773 3f73 6572 6965 735f 7365 6172  tags?series_sear
-000196f0: 6368 5f74 6578 743d 6d6f 6e65 7461 7279  ch_text=monetary
-00019700: 2b73 6572 7669 6365 2b69 6e64 6578 2661  +service+index&a
-00019710: 7069 5f6b 6579 3d61 6263 6465 6667 6869  pi_key=abcdefghi
-00019720: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
-00019730: 7a31 3233 3435 3626 6669 6c65 5f74 7970  z123456&file_typ
-00019740: 653d 6a73 6f6e 0d0a 0d0a 2020 2020 2020  e=json....      
-00019750: 2020 2323 2041 5049 2052 6573 706f 6e73    ## API Respons
-00019760: 650d 0a20 2020 2020 2020 2060 6060 6a73  e..        ```js
-00019770: 6f6e 0d0a 2020 2020 2020 2020 7b0d 0a20  on..        {.. 
-00019780: 2020 2020 2020 2020 2020 2022 7265 616c             "real
-00019790: 7469 6d65 5f73 7461 7274 223a 2022 3230  time_start": "20
-000197a0: 3133 2d30 382d 3134 222c 0d0a 2020 2020  13-08-14",..    
-000197b0: 2020 2020 2020 2020 2272 6561 6c74 696d          "realtim
-000197c0: 655f 656e 6422 3a20 2232 3031 332d 3038  e_end": "2013-08
-000197d0: 2d31 3422 2c0d 0a20 2020 2020 2020 2020  -14",..         
-000197e0: 2020 2022 6f72 6465 725f 6279 223a 2022     "order_by": "
-000197f0: 7365 7269 6573 5f63 6f75 6e74 222c 0d0a  series_count",..
-00019800: 2020 2020 2020 2020 2020 2020 2273 6f72              "sor
-00019810: 745f 6f72 6465 7222 3a20 2264 6573 6322  t_order": "desc"
-00019820: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00019830: 636f 756e 7422 3a20 3138 2c0d 0a20 2020  count": 18,..   
-00019840: 2020 2020 2020 2020 2022 6f66 6673 6574           "offset
-00019850: 223a 2030 2c0d 0a20 2020 2020 2020 2020  ": 0,..         
-00019860: 2020 2022 6c69 6d69 7422 3a20 3130 3030     "limit": 1000
-00019870: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00019880: 7461 6773 223a 205b 0d0a 2020 2020 2020  tags": [..      
-00019890: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
-000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198b0: 2022 6e61 6d65 223a 2022 6163 6164 656d   "name": "academ
-000198c0: 6963 2064 6174 6122 2c0d 0a20 2020 2020  ic data",..     
-000198d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000198e0: 6772 6f75 705f 6964 223a 2022 6765 6e22  group_id": "gen"
-000198f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00019900: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
-00019910: 2254 696d 6520 7365 7269 6573 2064 6174  "Time series dat
-00019920: 6120 6372 6561 7465 6420 6d61 696e 6c79  a created mainly
-00019930: 2062 7920 6163 6164 656d 6961 2074 6f20   by academia to 
-00019940: 6164 6472 6573 7320 6772 6f77 696e 6720  address growing 
-00019950: 6465 6d61 6e64 2069 6e20 756e 6465 7273  demand in unders
-00019960: 7461 6e64 696e 6720 7370 6563 6966 6963  tanding specific
-00019970: 2063 6f6e 6365 726e 7320 696e 2074 6865   concerns in the
-00019980: 2065 636f 6e6f 6d79 2074 6861 7420 6172   economy that ar
-00019990: 6520 6e6f 7420 7765 6c6c 206d 6f64 656c  e not well model
-000199a0: 6564 2062 7920 6f72 6469 6e61 7279 2073  ed by ordinary s
-000199b0: 7461 7469 7374 6963 616c 2061 6765 6e63  tatistical agenc
-000199c0: 6965 732e 222c 0d0a 2020 2020 2020 2020  ies.",..        
-000199d0: 2020 2020 2020 2020 2020 2020 2263 7265              "cre
-000199e0: 6174 6564 223a 2022 3230 3132 2d30 382d  ated": "2012-08-
-000199f0: 3239 2031 303a 3232 3a31 392d 3035 222c  29 10:22:19-05",
-00019a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019a10: 2020 2020 2020 2270 6f70 756c 6172 6974        "popularit
-00019a20: 7922 3a20 3632 2c0d 0a20 2020 2020 2020  y": 62,..       
-00019a30: 2020 2020 2020 2020 2020 2020 2022 7365               "se
-00019a40: 7269 6573 5f63 6f75 6e74 223a 2032 350d  ries_count": 25.
-00019a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019a60: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
-00019a70: 2020 2020 202e 2e2e 0d0a 2020 2020 2020       .....      
-00019a80: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
-00019a90: 207d 0d0a 2020 2020 2020 2020 6060 600d   }..        ```.
-00019aa0: 0a0d 0a20 2020 2020 2020 2023 2320 5265  ...        ## Re
-00019ab0: 7475 726e 730d 0a20 2020 2020 2020 2060  turns..        `
-00019ac0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
-00019ad0: 600d 0a0d 0a20 2020 2020 2020 2023 2320  `....        ## 
-00019ae0: 4578 616d 706c 650d 0a20 2020 2020 2020  Example..       
-00019af0: 2060 6060 7079 7468 6f6e 0d0a 2020 2020   ```python..    
-00019b00: 2020 2020 3e3e 3e20 6672 6564 203d 2046      >>> fred = F
-00019b10: 5245 4428 6170 695f 6b65 793d 2761 6263  RED(api_key='abc
-00019b20: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
-00019b30: 7475 7677 7879 7a31 3233 3435 3627 290d  tuvwxyz123456').
-00019b40: 0a20 2020 2020 2020 203e 3e3e 2066 7265  .        >>> fre
-00019b50: 642e 7365 7269 6573 5f73 6561 7263 685f  d.series_search_
-00019b60: 7461 6773 2873 6572 6965 735f 7365 6172  tags(series_sear
-00019b70: 6368 5f74 6578 743d 276d 6f6e 6574 6172  ch_text='monetar
-00019b80: 7920 7365 7276 6963 6520 696e 6465 7827  y service index'
-00019b90: 292e 6865 6164 2829 0d0a 2020 2020 2020  ).head()..      
-00019ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bb0: 2020 2020 6772 6f75 705f 6964 2020 2020      group_id    
-00019bc0: 2020 2020 2020 2020 6e6f 7465 7320 2020          notes   
-00019bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019be0: 6372 6561 7465 6420 2070 6f70 756c 6172  created  popular
-00019bf0: 6974 7920 2073 6572 6965 735f 636f 756e  ity  series_coun
-00019c00: 740d 0a20 2020 2020 2020 2020 2020 206e  t..            n
-00019c10: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
-00019c20: 2061 6363 6f75 6e74 696e 6720 2020 2020   accounting     
-00019c30: 2020 2020 6765 6e20 2020 2020 2020 2020      gen         
-00019c40: 2020 2020 2020 2020 2032 3031 322d 3032           2012-02
-00019c50: 2d32 3720 3136 3a31 383a 3139 2b30 303a  -27 16:18:19+00:
-00019c60: 3030 2020 2020 2020 2020 2020 3433 2020  00          43  
-00019c70: 2020 2020 2020 2020 2020 2032 0d0a 2020             2..  
-00019c80: 2020 2020 2020 2020 2020 6164 7665 7274            advert
-00019c90: 6973 656d 656e 7420 2020 2020 2067 656e  isement      gen
-00019ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019cb0: 2020 3230 3132 2d30 382d 3036 2031 393a    2012-08-06 19:
-00019cc0: 3530 3a30 372b 3030 3a30 3020 2020 2020  50:07+00:00     
-00019cd0: 2020 2020 2031 3720 2020 2020 2020 2020       17         
-00019ce0: 2020 2020 320d 0a20 2020 2020 2020 2020      2..         
-00019cf0: 2020 2061 7373 6574 7320 2020 2020 2020     assets       
-00019d00: 2020 2020 2020 6765 6e20 2020 2020 2020        gen       
-00019d10: 2020 2020 2020 2020 2020 2032 3031 322d             2012-
-00019d20: 3032 2d32 3720 3136 3a31 383a 3139 2b30  02-27 16:18:19+0
-00019d30: 303a 3030 2020 2020 2020 2020 2020 3634  0:00          64
-00019d40: 2020 2020 2020 2020 2020 2020 2032 0d0a               2..
-00019d50: 2020 2020 2020 2020 2020 2020 626f 6520              boe 
-00019d60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019d70: 7263 2020 4261 6e6b 206f 6620 456e 676c  rc  Bank of Engl
-00019d80: 616e 6420 3230 3133 2d30 322d 3235 2032  and 2013-02-25 2
-00019d90: 323a 3231 3a31 392b 3030 3a30 3020 2020  2:21:19+00:00   
-00019da0: 2020 2020 2020 2034 3220 2020 2020 2020         42       
-00019db0: 2020 2020 2020 320d 0a20 2020 2020 2020        2..       
-00019dc0: 2020 2020 2063 6f6d 6d75 6e69 6361 7469       communicati
-00019dd0: 6f6e 2020 2020 2020 6765 6e20 2020 2020  on      gen     
-00019de0: 2020 2020 2020 2020 2020 2020 2032 3031               201
-00019df0: 322d 3032 2d32 3720 3136 3a31 383a 3139  2-02-27 16:18:19
-00019e00: 2b30 303a 3030 2020 2020 2020 2020 2020  +00:00          
-00019e10: 3232 2020 2020 2020 2020 2020 2020 2032  22             2
-00019e20: 0d0a 2020 2020 2020 2020 6060 600d 0a20  ..        ```.. 
-00019e30: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00019e40: 2020 2020 616c 6c6f 7765 645f 6f72 6465      allowed_orde
-00019e50: 7273 203d 205b 0d0a 2020 2020 2020 2020  rs = [..        
-00019e60: 2020 2020 656e 756d 732e 4f72 6465 7242      enums.OrderB
-00019e70: 792e 7365 7269 6573 5f63 6f75 6e74 2c0d  y.series_count,.
-00019e80: 0a20 2020 2020 2020 2020 2020 2065 6e75  .            enu
-00019e90: 6d73 2e4f 7264 6572 4279 2e70 6f70 756c  ms.OrderBy.popul
-00019ea0: 6172 6974 792c 0d0a 2020 2020 2020 2020  arity,..        
-00019eb0: 2020 2020 656e 756d 732e 4f72 6465 7242      enums.OrderB
-00019ec0: 792e 6372 6561 7465 642c 0d0a 2020 2020  y.created,..    
-00019ed0: 2020 2020 2020 2020 656e 756d 732e 4f72          enums.Or
-00019ee0: 6465 7242 792e 6e61 6d65 2c0d 0a20 2020  derBy.name,..   
-00019ef0: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
-00019f00: 7264 6572 4279 2e67 726f 7570 5f69 642c  rderBy.group_id,
-00019f10: 0d0a 2020 2020 2020 2020 5d0d 0a0d 0a20  ..        ].... 
-00019f20: 2020 2020 2020 2069 6620 6f72 6465 725f         if order_
-00019f30: 6279 206e 6f74 2069 6e20 616c 6c6f 7765  by not in allowe
-00019f40: 645f 6f72 6465 7273 3a0d 0a20 2020 2020  d_orders:..     
-00019f50: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00019f60: 7565 4572 726f 7228 2756 6172 6961 626c  ueError('Variabl
-00019f70: 6520 6f72 6465 725f 6279 2028 7b7d 2920  e order_by ({}) 
-00019f80: 6973 206e 6f74 206f 6e65 206f 6620 7468  is not one of th
-00019f90: 6520 7661 6c75 6573 3a20 7b7d 272e 666f  e values: {}'.fo
-00019fa0: 726d 6174 286f 7264 6572 5f62 792c 2027  rmat(order_by, '
-00019fb0: 2c20 272e 6a6f 696e 286d 6170 2873 7472  , '.join(map(str
-00019fc0: 2c20 616c 6c6f 7765 645f 6f72 6465 7273  , allowed_orders
-00019fd0: 2929 2929 0d0a 0d0a 2020 2020 2020 2020  ))))....        
-00019fe0: 6966 2072 6561 6c74 696d 655f 7374 6172  if realtime_star
-00019ff0: 7420 6973 206e 6f74 204e 6f6e 6520 616e  t is not None an
-0001a000: 6420 7265 616c 7469 6d65 5f73 7461 7274  d realtime_start
-0001a010: 203c 2064 6174 6528 3137 3736 2c20 372c   < date(1776, 7,
-0001a020: 2034 293a 0d0a 2020 2020 2020 2020 2020   4):..          
-0001a030: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0001a040: 6f72 2827 5661 7269 6162 6c65 2072 6561  or('Variable rea
-0001a050: 6c74 696d 655f 7374 6172 7420 2822 7b7d  ltime_start ("{}
-0001a060: 2229 2069 7320 6265 666f 7265 206d 696e  ") is before min
-0001a070: 2064 6174 6520 3137 3736 2d30 372d 3034   date 1776-07-04
-0001a080: 2e27 2e66 6f72 6d61 7428 7265 616c 7469  .'.format(realti
-0001a090: 6d65 5f73 7461 7274 2929 0d0a 0d0a 2020  me_start))....  
-0001a0a0: 2020 2020 2020 6966 2072 6561 6c74 696d        if realtim
-0001a0b0: 655f 7374 6172 7420 6973 206e 6f74 204e  e_start is not N
-0001a0c0: 6f6e 6520 616e 6420 7265 616c 7469 6d65  one and realtime
-0001a0d0: 5f65 6e64 2069 7320 6e6f 7420 4e6f 6e65  _end is not None
-0001a0e0: 2061 6e64 2072 6561 6c74 696d 655f 7374   and realtime_st
-0001a0f0: 6172 7420 3e20 7265 616c 7469 6d65 5f65  art > realtime_e
-0001a100: 6e64 3a0d 0a20 2020 2020 2020 2020 2020  nd:..           
-0001a110: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0001a120: 7228 2754 6865 2064 6174 6520 7365 7420  r('The date set 
-0001a130: 6279 2076 6172 6961 626c 6520 7265 616c  by variable real
-0001a140: 7469 6d65 5f73 7461 7274 2028 227b 7d22  time_start ("{}"
-0001a150: 2920 6361 6e20 6e6f 7420 6265 2061 6674  ) can not be aft
-0001a160: 6572 2074 6865 2064 6174 6520 7365 7420  er the date set 
-0001a170: 6279 2076 6172 6961 626c 6520 7265 616c  by variable real
-0001a180: 7469 6d65 5f65 6e64 2028 227b 7d22 292e  time_end ("{}").
-0001a190: 272e 666f 726d 6174 2872 6561 6c74 696d  '.format(realtim
-0001a1a0: 655f 7374 6172 742c 2072 6561 6c74 696d  e_start, realtim
-0001a1b0: 655f 656e 6429 290d 0a0d 0a20 2020 2020  e_end))....     
-0001a1c0: 2020 2064 6620 3d20 7064 2e44 6174 6146     df = pd.DataF
-0001a1d0: 7261 6d65 280d 0a20 2020 2020 2020 2020  rame(..         
-0001a1e0: 2020 2073 656c 662e 5f63 6c69 656e 742e     self._client.
-0001a1f0: 6765 7428 0d0a 2020 2020 2020 2020 2020  get(..          
-0001a200: 2020 2020 2020 272f 6672 6564 2f73 6572        '/fred/ser
-0001a210: 6965 732f 7365 6172 6368 2f74 6167 7327  ies/search/tags'
-0001a220: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001a230: 2020 2027 7461 6773 272c 0d0a 2020 2020     'tags',..    
-0001a240: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
-0001a250: 743d 3130 3030 2c0d 0a20 2020 2020 2020  t=1000,..       
-0001a260: 2020 2020 2020 2020 2073 6572 6965 735f           series_
-0001a270: 7365 6172 6368 5f74 6578 743d 7365 7269  search_text=seri
-0001a280: 6573 5f73 6561 7263 685f 7465 7874 2c0d  es_search_text,.
-0001a290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a2a0: 2072 6561 6c74 696d 655f 7374 6172 743d   realtime_start=
-0001a2b0: 7265 616c 7469 6d65 5f73 7461 7274 2c0d  realtime_start,.
-0001a2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a2d0: 2072 6561 6c74 696d 655f 656e 643d 7265   realtime_end=re
-0001a2e0: 616c 7469 6d65 5f65 6e64 2c0d 0a20 2020  altime_end,..   
-0001a2f0: 2020 2020 2020 2020 2020 2020 2074 6167               tag
-0001a300: 5f6e 616d 6573 3d74 6167 5f6e 616d 6573  _names=tag_names
-0001a310: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001a320: 2020 2074 6167 5f67 726f 7570 5f69 643d     tag_group_id=
-0001a330: 7461 675f 6772 6f75 705f 6964 2c0d 0a20  tag_group_id,.. 
-0001a340: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001a350: 6167 5f73 6561 7263 685f 7465 7874 3d74  ag_search_text=t
-0001a360: 6167 5f73 6561 7263 685f 7465 7874 2c0d  ag_search_text,.
-0001a370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a380: 206f 7264 6572 5f62 793d 6f72 6465 725f   order_by=order_
-0001a390: 6279 2c0d 0a20 2020 2020 2020 2020 2020  by,..           
-0001a3a0: 2020 2020 2073 6f72 745f 6f72 6465 723d       sort_order=
-0001a3b0: 736f 7274 5f6f 7264 6572 0d0a 2020 2020  sort_order..    
-0001a3c0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001a3d0: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
-0001a3e0: 6966 206e 6f74 2064 662e 656d 7074 793a  if not df.empty:
-0001a3f0: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-0001a400: 2e63 7265 6174 6564 203d 2070 642e 746f  .created = pd.to
-0001a410: 5f64 6174 6574 696d 6528 6466 2e63 7265  _datetime(df.cre
-0001a420: 6174 6564 202b 2027 3030 272c 2075 7463  ated + '00', utc
-0001a430: 3d54 7275 652c 2066 6f72 6d61 743d 2725  =True, format='%
-0001a440: 592d 256d 2d25 6420 2548 3a25 4d3a 2553  Y-%m-%d %H:%M:%S
-0001a450: 257a 2729 0d0a 0d0a 2020 2020 2020 2020  %z')....        
-0001a460: 2020 2020 6466 203d 2064 662e 6173 7479      df = df.asty
-0001a470: 7065 2864 7479 7065 3d7b 0d0a 2020 2020  pe(dtype={..    
-0001a480: 2020 2020 2020 2020 2020 2020 276e 616d              'nam
-0001a490: 6527 3a20 2773 7472 696e 6727 2c0d 0a20  e': 'string',.. 
-0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001a4b0: 6e6f 7465 7327 3a20 2773 7472 696e 6727  notes': 'string'
-0001a4c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001a4d0: 2020 2027 6772 6f75 705f 6964 273a 2027     'group_id': '
-0001a4e0: 6361 7465 676f 7279 270d 0a20 2020 2020  category'..     
-0001a4f0: 2020 2020 2020 207d 292e 7365 745f 696e         }).set_in
-0001a500: 6465 7828 276e 616d 6527 290d 0a0d 0a20  dex('name').... 
-0001a510: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
-0001a520: 0d0a 0d0a 2020 2020 6465 6620 7365 7269  ....    def seri
-0001a530: 6573 5f73 6561 7263 685f 7265 6c61 7465  es_search_relate
-0001a540: 645f 7461 6773 280d 0a20 2020 2020 2020  d_tags(..       
-0001a550: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-0001a560: 2020 2020 2020 2020 7365 7269 6573 5f73          series_s
-0001a570: 6561 7263 685f 7465 7874 3a20 7374 722c  earch_text: str,
-0001a580: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001a590: 616c 7469 6d65 5f73 7461 7274 3a20 6461  altime_start: da
-0001a5a0: 7465 203d 204e 6f6e 652c 0d0a 2020 2020  te = None,..    
-0001a5b0: 2020 2020 2020 2020 7265 616c 7469 6d65          realtime
-0001a5c0: 5f65 6e64 3a20 6461 7465 203d 204e 6f6e  _end: date = Non
-0001a5d0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0001a5e0: 7461 675f 6e61 6d65 733a 204c 6973 745b  tag_names: List[
-0001a5f0: 7374 725d 203d 204e 6f6e 652c 0d0a 2020  str] = None,..  
-0001a600: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
-0001a610: 655f 7461 675f 6e61 6d65 733a 204c 6973  e_tag_names: Lis
-0001a620: 745b 7374 725d 203d 204e 6f6e 652c 0d0a  t[str] = None,..
-0001a630: 2020 2020 2020 2020 2020 2020 7461 675f              tag_
-0001a640: 6772 6f75 705f 6964 3a20 656e 756d 732e  group_id: enums.
-0001a650: 5461 6747 726f 7570 4944 203d 204e 6f6e  TagGroupID = Non
-0001a660: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0001a670: 7461 675f 7365 6172 6368 5f74 6578 743a  tag_search_text:
-0001a680: 2073 7472 203d 204e 6f6e 652c 0d0a 2020   str = None,..  
-0001a690: 2020 2020 2020 2020 2020 6f72 6465 725f            order_
-0001a6a0: 6279 3a20 656e 756d 732e 4f72 6465 7242  by: enums.OrderB
-0001a6b0: 7920 3d20 656e 756d 732e 4f72 6465 7242  y = enums.OrderB
-0001a6c0: 792e 7365 7269 6573 5f63 6f75 6e74 2c0d  y.series_count,.
-0001a6d0: 0a20 2020 2020 2020 2020 2020 2073 6f72  .            sor
-0001a6e0: 745f 6f72 6465 723a 2065 6e75 6d73 2e53  t_order: enums.S
-0001a6f0: 6f72 744f 7264 6572 203d 2065 6e75 6d73  ortOrder = enums
-0001a700: 2e53 6f72 744f 7264 6572 2e61 7363 0d0a  .SortOrder.asc..
-0001a710: 2020 2020 2920 2d3e 2070 642e 4461 7461      ) -> pd.Data
-0001a720: 4672 616d 653a 0d0a 2020 2020 2020 2020  Frame:..        
-0001a730: 2222 220d 0a20 2020 2020 2020 2023 2320  """..        ## 
-0001a740: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-0001a750: 2020 2020 6073 6572 6965 735f 7365 6172      `series_sear
-0001a760: 6368 5f74 6578 7460 0d0a 2020 2020 2020  ch_text`..      
-0001a770: 2020 5468 6520 776f 7264 7320 746f 206d    The words to m
-0001a780: 6174 6368 2061 6761 696e 7374 2065 636f  atch against eco
-0001a790: 6e6f 6d69 6320 6461 7461 2073 6572 6965  nomic data serie
-0001a7a0: 732e 0d0a 0d0a 2020 2020 2020 2020 6072  s.....        `r
-0001a7b0: 6561 6c74 696d 655f 7374 6172 7460 0d0a  ealtime_start`..
-0001a7c0: 2020 2020 2020 2020 5468 6520 7374 6172          The star
-0001a7d0: 7420 6f66 2074 6865 2072 6561 6c2d 7469  t of the real-ti
-0001a7e0: 6d65 2070 6572 696f 642e 2046 6f72 206d  me period. For m
-0001a7f0: 6f72 6520 696e 666f 726d 6174 696f 6e2c  ore information,
-0001a800: 2073 6565 205b 5265 616c 2d54 696d 6520   see [Real-Time 
-0001a810: 5065 7269 6f64 735d 2868 7474 7073 3a2f  Periods](https:/
-0001a820: 2f66 7265 642e 7374 6c6f 7569 7366 6564  /fred.stlouisfed
-0001a830: 2e6f 7267 2f64 6f63 732f 6170 692f 6672  .org/docs/api/fr
-0001a840: 6564 2f72 6561 6c74 696d 655f 7065 7269  ed/realtime_peri
-0001a850: 6f64 2e68 746d 6c29 2e0d 0a0d 0a20 2020  od.html).....   
-0001a860: 2020 2020 2060 7265 616c 7469 6d65 5f65       `realtime_e
-0001a870: 6e64 600d 0a20 2020 2020 2020 2054 6865  nd`..        The
-0001a880: 2065 6e64 206f 6620 7468 6520 7265 616c   end of the real
-0001a890: 2d74 696d 6520 7065 7269 6f64 2e20 466f  -time period. Fo
-0001a8a0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-0001a8b0: 6f6e 2c20 7365 6520 5b52 6561 6c2d 5469  on, see [Real-Ti
-0001a8c0: 6d65 2050 6572 696f 6473 5d28 6874 7470  me Periods](http
-0001a8d0: 733a 2f2f 6672 6564 2e73 746c 6f75 6973  s://fred.stlouis
-0001a8e0: 6665 642e 6f72 672f 646f 6373 2f61 7069  fed.org/docs/api
-0001a8f0: 2f66 7265 642f 7265 616c 7469 6d65 5f70  /fred/realtime_p
-0001a900: 6572 696f 642e 6874 6d6c 292e 0d0a 0d0a  eriod.html).....
-0001a910: 2020 2020 2020 2020 6074 6167 5f6e 616d          `tag_nam
-0001a920: 6573 600d 0a20 2020 2020 2020 2041 2073  es`..        A s
-0001a930: 656d 6963 6f6c 6f6e 2064 656c 696d 6974  emicolon delimit
-0001a940: 6564 206c 6973 7420 6f66 2074 6167 206e  ed list of tag n
-0001a950: 616d 6573 2074 6f20 6f6e 6c79 2069 6e63  ames to only inc
-0001a960: 6c75 6465 2069 6e20 7468 6520 7265 7370  lude in the resp
-0001a970: 6f6e 7365 2e20 5365 6520 7468 6520 7265  onse. See the re
-0001a980: 6c61 7465 6420 7265 7175 6573 7420 6672  lated request fr
-0001a990: 6564 2f73 6572 6965 732f 7365 6172 6368  ed/series/search
-0001a9a0: 2f72 656c 6174 6564 5f74 6167 732e 0d0a  /related_tags...
-0001a9b0: 0d0a 2020 2020 2020 2020 6065 7863 6c75  ..        `exclu
-0001a9c0: 6465 5f74 6167 5f6e 616d 6573 600d 0a20  de_tag_names`.. 
-0001a9d0: 2020 2020 2020 2054 7570 6c65 206f 6620         Tuple of 
-0001a9e0: 7461 6720 6e61 6d65 7320 7468 6174 2073  tag names that s
-0001a9f0: 6572 6965 7320 6d61 7463 6820 6e6f 6e65  eries match none
-0001aa00: 206f 662e 0d0a 0d0a 2020 2020 2020 2020   of.....        
-0001aa10: 6074 6167 5f67 726f 7570 5f69 6460 0d0a  `tag_group_id`..
-0001aa20: 2020 2020 2020 2020 4120 7461 6720 6772          A tag gr
-0001aa30: 6f75 7020 6964 2074 6f20 6669 6c74 6572  oup id to filter
-0001aa40: 2074 6167 7320 6279 2074 7970 652e 0d0a   tags by type...
-0001aa50: 0d0a 2020 2020 2020 2020 6074 6167 5f73  ..        `tag_s
-0001aa60: 6561 7263 685f 7465 7874 600d 0a20 2020  earch_text`..   
-0001aa70: 2020 2020 2054 6865 2077 6f72 6473 2074       The words t
-0001aa80: 6f20 6669 6e64 206d 6174 6368 696e 6720  o find matching 
-0001aa90: 7461 6773 2077 6974 682e 0d0a 0d0a 2020  tags with.....  
-0001aaa0: 2020 2020 2020 606f 7264 6572 5f62 7960        `order_by`
-0001aab0: 0d0a 2020 2020 2020 2020 4f72 6465 7220  ..        Order 
-0001aac0: 7265 7375 6c74 7320 6279 2076 616c 7565  results by value
-0001aad0: 7320 6f66 2074 6865 2073 7065 6369 6669  s of the specifi
-0001aae0: 6564 2061 7474 7269 6275 7465 2e0d 0a0d  ed attribute....
-0001aaf0: 0a20 2020 2020 2020 2060 736f 7274 5f6f  .        `sort_o
-0001ab00: 7264 6572 600d 0a20 2020 2020 2020 2053  rder`..        S
-0001ab10: 6f72 7420 7265 7375 6c74 7320 6973 2061  ort results is a
-0001ab20: 7363 656e 6469 6e67 206f 7220 6465 7363  scending or desc
-0001ab30: 656e 6469 6e67 206f 7264 6572 2066 6f72  ending order for
-0001ab40: 2061 7474 7269 6275 7465 2076 616c 7565   attribute value
-0001ab50: 7320 7370 6563 6966 6965 6420 6279 206f  s specified by o
-0001ab60: 7264 6572 5f62 792e 0d0a 0d0a 2020 2020  rder_by.....    
-0001ab70: 2020 2020 2323 2044 6573 6372 6970 7469      ## Descripti
-0001ab80: 6f6e 0d0a 2020 2020 2020 2020 6874 7470  on..        http
-0001ab90: 733a 2f2f 6672 6564 2e73 746c 6f75 6973  s://fred.stlouis
-0001aba0: 6665 642e 6f72 672f 646f 6373 2f61 7069  fed.org/docs/api
-0001abb0: 2f66 7265 642f 7365 7269 6573 5f73 6561  /fred/series_sea
-0001abc0: 7263 685f 7265 6c61 7465 645f 7461 6773  rch_related_tags
-0001abd0: 2e68 746d 6c0d 0a0d 0a20 2020 2020 2020  .html....       
-0001abe0: 2047 6574 2074 6865 2072 656c 6174 6564   Get the related
-0001abf0: 2046 5245 4420 7461 6773 2066 6f72 206f   FRED tags for o
-0001ac00: 6e65 206f 7220 6d6f 7265 2046 5245 4420  ne or more FRED 
-0001ac10: 7461 6773 206d 6174 6368 696e 6720 6120  tags matching a 
-0001ac20: 7365 7269 6573 2073 6561 7263 682e 204f  series search. O
-0001ac30: 7074 696f 6e61 6c6c 792c 2066 696c 7465  ptionally, filte
-0001ac40: 7220 7265 7375 6c74 7320 6279 2074 6167  r results by tag
-0001ac50: 2067 726f 7570 206f 7220 7461 6720 7365   group or tag se
-0001ac60: 6172 6368 2e0d 0a20 2020 2020 2020 2046  arch...        F
-0001ac70: 5245 4420 7461 6773 2061 7265 2061 7474  RED tags are att
-0001ac80: 7269 6275 7465 7320 6173 7369 676e 6564  ributes assigned
-0001ac90: 2074 6f20 7365 7269 6573 2e0d 0a20 2020   to series...   
-0001aca0: 2020 2020 2046 6f72 2074 6869 7320 7265       For this re
-0001acb0: 7175 6573 742c 2072 656c 6174 6564 2046  quest, related F
-0001acc0: 5245 4420 7461 6773 2061 7265 2074 6865  RED tags are the
-0001acd0: 2074 6167 7320 6173 7369 676e 6564 2074   tags assigned t
-0001ace0: 6f20 7365 7269 6573 2074 6861 7420 6d61  o series that ma
-0001acf0: 7463 6820 616c 6c20 7461 6773 2069 6e20  tch all tags in 
-0001ad00: 7468 6520 7461 675f 6e61 6d65 7320 7061  the tag_names pa
-0001ad10: 7261 6d65 7465 722c 206e 6f20 7461 6773  rameter, no tags
-0001ad20: 2069 6e20 7468 6520 6578 636c 7564 655f   in the exclude_
-0001ad30: 7461 675f 6e61 6d65 7320 7061 7261 6d65  tag_names parame
-0001ad40: 7465 722c 0d0a 2020 2020 2020 2020 616e  ter,..        an
-0001ad50: 6420 7468 6520 7365 6172 6368 2077 6f72  d the search wor
-0001ad60: 6473 2073 6574 2062 7920 7468 6520 7365  ds set by the se
-0001ad70: 7269 6573 5f73 6561 7263 685f 7465 7874  ries_search_text
-0001ad80: 2070 6172 616d 6574 6572 2e0d 0a20 2020   parameter...   
-0001ad90: 2020 2020 2053 6565 2074 6865 2072 656c       See the rel
-0001ada0: 6174 6564 2072 6571 7565 7374 2066 7265  ated request fre
-0001adb0: 642f 7365 7269 6573 2f73 6561 7263 682f  d/series/search/
-0001adc0: 7461 6773 2e0d 0a0d 0a20 2020 2020 2020  tags.....       
-0001add0: 2023 2320 4150 4920 5265 7175 6573 7420   ## API Request 
-0001ade0: 2848 5454 5053 2047 4554 290d 0a20 2020  (HTTPS GET)..   
-0001adf0: 2020 2020 2068 7474 7073 3a2f 2f61 7069       https://api
-0001ae00: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
-0001ae10: 6672 6564 2f73 6572 6965 732f 7365 6172  fred/series/sear
-0001ae20: 6368 2f72 656c 6174 6564 5f74 6167 733f  ch/related_tags?
-0001ae30: 7365 7269 6573 5f73 6561 7263 685f 7465  series_search_te
-0001ae40: 7874 3d6d 6f72 7467 6167 652b 7261 7465  xt=mortgage+rate
-0001ae50: 2674 6167 5f6e 616d 6573 3d33 302d 7965  &tag_names=30-ye
-0001ae60: 6172 3b66 7262 2661 7069 5f6b 6579 3d61  ar;frb&api_key=a
-0001ae70: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
-0001ae80: 7273 7475 7677 7879 7a31 3233 3435 3626  rstuvwxyz123456&
-0001ae90: 6669 6c65 5f74 7970 653d 6a73 6f6e 0d0a  file_type=json..
-0001aea0: 0d0a 2020 2020 2020 2020 2323 2041 5049  ..        ## API
-0001aeb0: 2052 6573 706f 6e73 650d 0a20 2020 2020   Response..     
-0001aec0: 2020 2060 6060 6a73 6f6e 0d0a 2020 2020     ```json..    
-0001aed0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-0001aee0: 2020 2022 7265 616c 7469 6d65 5f73 7461     "realtime_sta
-0001aef0: 7274 223a 2022 3230 3133 2d30 382d 3134  rt": "2013-08-14
-0001af00: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0001af10: 2272 6561 6c74 696d 655f 656e 6422 3a20  "realtime_end": 
-0001af20: 2232 3031 332d 3038 2d31 3422 2c0d 0a20  "2013-08-14",.. 
-0001af30: 2020 2020 2020 2020 2020 2022 6f72 6465             "orde
-0001af40: 725f 6279 223a 2022 7365 7269 6573 5f63  r_by": "series_c
-0001af50: 6f75 6e74 222c 0d0a 2020 2020 2020 2020  ount",..        
-0001af60: 2020 2020 2273 6f72 745f 6f72 6465 7222      "sort_order"
-0001af70: 3a20 2264 6573 6322 2c0d 0a20 2020 2020  : "desc",..     
-0001af80: 2020 2020 2020 2022 636f 756e 7422 3a20         "count": 
-0001af90: 3130 2c0d 0a20 2020 2020 2020 2020 2020  10,..           
-0001afa0: 2022 6f66 6673 6574 223a 2030 2c0d 0a20   "offset": 0,.. 
-0001afb0: 2020 2020 2020 2020 2020 2022 6c69 6d69             "limi
-0001afc0: 7422 3a20 3130 3030 2c0d 0a20 2020 2020  t": 1000,..     
-0001afd0: 2020 2020 2020 2022 7461 6773 223a 205b         "tags": [
-0001afe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001aff0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-0001b000: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-0001b010: 2022 636f 6e76 656e 7469 6f6e 616c 222c   "conventional",
-0001b020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b030: 2020 2020 2020 2267 726f 7570 5f69 6422        "group_id"
-0001b040: 3a20 2267 656e 222c 0d0a 2020 2020 2020  : "gen",..      
-0001b050: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-0001b060: 6f74 6573 223a 2022 222c 0d0a 2020 2020  otes": "",..    
-0001b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b080: 2263 7265 6174 6564 223a 2022 3230 3132  "created": "2012
-0001b090: 2d30 322d 3237 2031 303a 3138 3a31 392d  -02-27 10:18:19-
-0001b0a0: 3036 222c 0d0a 2020 2020 2020 2020 2020  06",..          
-0001b0b0: 2020 2020 2020 2020 2020 2270 6f70 756c            "popul
-0001b0c0: 6172 6974 7922 3a20 3633 2c0d 0a20 2020  arity": 63,..   
-0001b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b0e0: 2022 7365 7269 6573 5f63 6f75 6e74 223a   "series_count":
-0001b0f0: 2033 0d0a 2020 2020 2020 2020 2020 2020   3..            
-0001b100: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-0001b110: 2020 2020 2020 2020 2e2e 2e0d 0a20 2020          .....   
-0001b120: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
-0001b130: 2020 2020 7d0d 0a20 2020 2020 2020 2060      }..        `
-0001b140: 6060 0d0a 0d0a 2020 2020 2020 2020 2323  ``....        ##
-0001b150: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-0001b160: 2020 6070 616e 6461 732e 4461 7461 4672    `pandas.DataFr
-0001b170: 616d 6560 0d0a 0d0a 2020 2020 2020 2020  ame`....        
-0001b180: 2323 2045 7861 6d70 6c65 0d0a 2020 2020  ## Example..    
-0001b190: 2020 2020 6060 6070 7974 686f 6e0d 0a20      ```python.. 
-0001b1a0: 2020 2020 2020 203e 3e3e 2066 7265 6420         >>> fred 
-0001b1b0: 3d20 4652 4544 2861 7069 5f6b 6579 3d27  = FRED(api_key='
-0001b1c0: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
-0001b1d0: 7172 7374 7576 7778 797a 3132 3334 3536  qrstuvwxyz123456
-0001b1e0: 2729 0d0a 2020 2020 2020 2020 3e3e 3e20  ')..        >>> 
-0001b1f0: 6672 6564 2e73 6572 6965 735f 7365 6172  fred.series_sear
-0001b200: 6368 5f72 656c 6174 6564 5f74 6167 7328  ch_related_tags(
-0001b210: 7365 7269 6573 5f73 6561 7263 685f 7465  series_search_te
-0001b220: 7874 3d27 6d6f 7274 6761 6765 2072 6174  xt='mortgage rat
-0001b230: 6527 2c20 7461 675f 6e61 6d65 733d 5b27  e', tag_names=['
-0001b240: 3330 2d79 6561 7227 2c20 2766 7262 275d  30-year', 'frb']
-0001b250: 2c20 7265 616c 7469 6d65 5f73 7461 7274  , realtime_start
-0001b260: 3d64 6174 6528 3230 3232 2c20 312c 2035  =date(2022, 1, 5
-0001b270: 292c 2072 6561 6c74 696d 655f 656e 643d  ), realtime_end=
-0001b280: 6461 7465 2832 3032 322c 2031 2c20 3529  date(2022, 1, 5)
-0001b290: 292e 6865 6164 2829 0d0a 2020 2020 2020  ).head()..      
-0001b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2b0: 2020 2020 6772 6f75 705f 6964 2020 2020      group_id    
-0001b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2d0: 2020 2020 206e 6f74 6573 2020 2020 2020       notes      
-0001b2e0: 2020 2020 2020 2020 2020 2020 2063 7265               cre
-0001b2f0: 6174 6564 2020 706f 7075 6c61 7269 7479  ated  popularity
-0001b300: 2020 7365 7269 6573 5f63 6f75 6e74 0d0a    series_count..
-0001b310: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0001b320: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-0001b330: 6e76 656e 7469 6f6e 616c 2020 2020 2020  nventional      
-0001b340: 2067 656e 2020 2020 2020 2020 2020 2020   gen            
-0001b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b360: 2020 2032 3031 322d 3032 2d32 3720 3136     2012-02-27 16
-0001b370: 3a31 383a 3139 2b30 303a 3030 2020 2020  :18:19+00:00    
-0001b380: 2020 2020 2020 3231 2020 2020 2020 2020        21        
-0001b390: 2020 2020 2032 0d0a 2020 2020 2020 2020       2..        
-0001b3a0: 2020 2020 6469 7363 6f6e 7469 6e75 6564      discontinued
-0001b3b0: 2020 2020 2020 2067 656e 2020 2020 2020         gen      
-0001b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3d0: 2020 2020 2020 2020 2032 3031 322d 3032           2012-02
-0001b3e0: 2d32 3720 3136 3a31 383a 3139 2b30 303a  -27 16:18:19+00:
-0001b3f0: 3030 2020 2020 2020 2020 2020 3637 2020  00          67  
-0001b400: 2020 2020 2020 2020 2020 2032 0d0a 2020             2..  
-0001b410: 2020 2020 2020 2020 2020 6831 3520 2020            h15   
-0001b420: 2020 2020 2020 2020 2020 2020 2072 6c73               rls
-0001b430: 2020 482e 3135 2053 656c 6563 7465 6420    H.15 Selected 
-0001b440: 496e 7465 7265 7374 2052 6174 6573 2032  Interest Rates 2
-0001b450: 3031 322d 3038 2d31 3620 3230 3a32 313a  012-08-16 20:21:
-0001b460: 3137 2b30 303a 3030 2020 2020 2020 2020  17+00:00        
-0001b470: 2020 3537 2020 2020 2020 2020 2020 2020    57            
-0001b480: 2032 0d0a 2020 2020 2020 2020 2020 2020   2..            
-0001b490: 696e 7465 7265 7374 2020 2020 2020 2020  interest        
-0001b4a0: 2020 2067 656e 2020 2020 2020 2020 2020     gen          
+000187e0: 7365 6172 6368 5f74 7970 652c 2027 2c20  search_type, ', 
+000187f0: 272e 6a6f 696e 286d 6170 2873 7472 2c20  '.join(map(str, 
+00018800: 656e 756d 732e 5365 6172 6368 5479 7065  enums.SearchType
+00018810: 2929 2929 0d0a 0d0a 2020 2020 2020 2020  ))))....        
+00018820: 6966 2066 696c 7465 725f 7661 7269 6162  if filter_variab
+00018830: 6c65 2069 7320 6e6f 7420 4e6f 6e65 2061  le is not None a
+00018840: 6e64 2066 696c 7465 725f 7661 7269 6162  nd filter_variab
+00018850: 6c65 206e 6f74 2069 6e20 656e 756d 732e  le not in enums.
+00018860: 4669 6c74 6572 5661 7269 6162 6c65 3a0d  FilterVariable:.
+00018870: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00018880: 7365 2056 616c 7565 4572 726f 7228 2756  se ValueError('V
+00018890: 6172 6961 626c 6520 6669 6c74 6572 5f76  ariable filter_v
+000188a0: 6172 6961 626c 6520 287b 7d29 2069 7320  ariable ({}) is 
+000188b0: 6e6f 7420 6f6e 6520 6f66 2074 6865 2076  not one of the v
+000188c0: 616c 7565 733a 207b 7d27 2e66 6f72 6d61  alues: {}'.forma
+000188d0: 7428 6669 6c74 6572 5f76 6172 6961 626c  t(filter_variabl
+000188e0: 652c 2027 2c20 272e 6a6f 696e 286d 6170  e, ', '.join(map
+000188f0: 2873 7472 2c20 656e 756d 732e 4669 6c74  (str, enums.Filt
+00018900: 6572 5661 7269 6162 6c65 2929 2929 0d0a  erVariable))))..
+00018910: 0d0a 2020 2020 2020 2020 6966 2072 6561  ..        if rea
+00018920: 6c74 696d 655f 7374 6172 7420 6973 206e  ltime_start is n
+00018930: 6f74 204e 6f6e 6520 616e 6420 7265 616c  ot None and real
+00018940: 7469 6d65 5f73 7461 7274 203c 2064 6174  time_start < dat
+00018950: 6528 3137 3736 2c20 372c 2034 293a 0d0a  e(1776, 7, 4):..
+00018960: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00018970: 6520 5661 6c75 6545 7272 6f72 2827 5661  e ValueError('Va
+00018980: 7269 6162 6c65 2072 6561 6c74 696d 655f  riable realtime_
+00018990: 7374 6172 7420 2822 7b7d 2229 2069 7320  start ("{}") is 
+000189a0: 6265 666f 7265 206d 696e 2064 6174 6520  before min date 
+000189b0: 3137 3736 2d30 372d 3034 2e27 2e66 6f72  1776-07-04.'.for
+000189c0: 6d61 7428 7265 616c 7469 6d65 5f73 7461  mat(realtime_sta
+000189d0: 7274 2929 0d0a 0d0a 2020 2020 2020 2020  rt))....        
+000189e0: 6966 2072 6561 6c74 696d 655f 7374 6172  if realtime_star
+000189f0: 7420 6973 206e 6f74 204e 6f6e 6520 616e  t is not None an
+00018a00: 6420 7265 616c 7469 6d65 5f65 6e64 2069  d realtime_end i
+00018a10: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2072  s not None and r
+00018a20: 6561 6c74 696d 655f 7374 6172 7420 3e20  ealtime_start > 
+00018a30: 7265 616c 7469 6d65 5f65 6e64 3a0d 0a20  realtime_end:.. 
+00018a40: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00018a50: 2056 616c 7565 4572 726f 7228 2754 6865   ValueError('The
+00018a60: 2064 6174 6520 7365 7420 6279 2076 6172   date set by var
+00018a70: 6961 626c 6520 7265 616c 7469 6d65 5f73  iable realtime_s
+00018a80: 7461 7274 2028 227b 7d22 2920 6361 6e20  tart ("{}") can 
+00018a90: 6e6f 7420 6265 2061 6674 6572 2074 6865  not be after the
+00018aa0: 2064 6174 6520 7365 7420 6279 2076 6172   date set by var
+00018ab0: 6961 626c 6520 7265 616c 7469 6d65 5f65  iable realtime_e
+00018ac0: 6e64 2028 227b 7d22 292e 272e 666f 726d  nd ("{}").'.form
+00018ad0: 6174 2872 6561 6c74 696d 655f 7374 6172  at(realtime_star
+00018ae0: 742c 2072 6561 6c74 696d 655f 656e 6429  t, realtime_end)
+00018af0: 290d 0a0d 0a20 2020 2020 2020 2064 6620  )....        df 
+00018b00: 3d20 7064 2e44 6174 6146 7261 6d65 280d  = pd.DataFrame(.
+00018b10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00018b20: 662e 5f63 6c69 656e 742e 6765 7428 0d0a  f._client.get(..
+00018b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b40: 272f 6672 6564 2f73 6572 6965 732f 7365  '/fred/series/se
+00018b50: 6172 6368 272c 0d0a 2020 2020 2020 2020  arch',..        
+00018b60: 2020 2020 2020 2020 2773 6572 6965 7373          'seriess
+00018b70: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00018b80: 2020 2020 6c69 6d69 743d 3130 3030 2c0d      limit=1000,.
+00018b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018ba0: 2073 6561 7263 685f 7465 7874 3d73 6561   search_text=sea
+00018bb0: 7263 685f 7465 7874 2c0d 0a20 2020 2020  rch_text,..     
+00018bc0: 2020 2020 2020 2020 2020 2073 6561 7263             searc
+00018bd0: 685f 7479 7065 3d73 6561 7263 685f 7479  h_type=search_ty
+00018be0: 7065 2c0d 0a20 2020 2020 2020 2020 2020  pe,..           
+00018bf0: 2020 2020 2072 6561 6c74 696d 655f 7374       realtime_st
+00018c00: 6172 743d 7265 616c 7469 6d65 5f73 7461  art=realtime_sta
+00018c10: 7274 2c0d 0a20 2020 2020 2020 2020 2020  rt,..           
+00018c20: 2020 2020 2072 6561 6c74 696d 655f 656e       realtime_en
+00018c30: 643d 7265 616c 7469 6d65 5f65 6e64 2c0d  d=realtime_end,.
+00018c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018c50: 206f 7264 6572 5f62 793d 6f72 6465 725f   order_by=order_
+00018c60: 6279 2c0d 0a20 2020 2020 2020 2020 2020  by,..           
+00018c70: 2020 2020 2073 6f72 745f 6f72 6465 723d       sort_order=
+00018c80: 736f 7274 5f6f 7264 6572 2c0d 0a20 2020  sort_order,..   
+00018c90: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00018ca0: 7465 725f 7661 7269 6162 6c65 3d66 696c  ter_variable=fil
+00018cb0: 7465 725f 7661 7269 6162 6c65 2c0d 0a20  ter_variable,.. 
+00018cc0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00018cd0: 696c 7465 725f 7661 6c75 653d 6669 6c74  ilter_value=filt
+00018ce0: 6572 5f76 616c 7565 2c0d 0a20 2020 2020  er_value,..     
+00018cf0: 2020 2020 2020 2020 2020 2074 6167 5f6e             tag_n
+00018d00: 616d 6573 3d74 6167 5f6e 616d 6573 2c0d  ames=tag_names,.
+00018d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018d20: 2065 7863 6c75 6465 5f74 6167 5f6e 616d   exclude_tag_nam
+00018d30: 6573 3d65 7863 6c75 6465 5f74 6167 5f6e  es=exclude_tag_n
+00018d40: 616d 6573 0d0a 2020 2020 2020 2020 2020  ames..          
+00018d50: 2020 290d 0a20 2020 2020 2020 2029 0d0a    )..        )..
+00018d60: 0d0a 2020 2020 2020 2020 6461 7465 5f63  ..        date_c
+00018d70: 6f6c 756d 6e73 203d 205b 0d0a 2020 2020  olumns = [..    
+00018d80: 2020 2020 2020 2020 2772 6561 6c74 696d          'realtim
+00018d90: 655f 7374 6172 7427 2c20 2772 6561 6c74  e_start', 'realt
+00018da0: 696d 655f 656e 6427 2c0d 0a20 2020 2020  ime_end',..     
+00018db0: 2020 2020 2020 2027 6f62 7365 7276 6174         'observat
+00018dc0: 696f 6e5f 7374 6172 7427 2c20 276f 6273  ion_start', 'obs
+00018dd0: 6572 7661 7469 6f6e 5f65 6e64 272c 0d0a  ervation_end',..
+00018de0: 2020 2020 2020 2020 5d0d 0a0d 0a20 2020          ]....   
+00018df0: 2020 2020 2069 6620 6e6f 7420 6466 2e65       if not df.e
+00018e00: 6d70 7479 3a0d 0a20 2020 2020 2020 2020  mpty:..         
+00018e10: 2020 2064 665b 6461 7465 5f63 6f6c 756d     df[date_colum
+00018e20: 6e73 5d20 3d20 6466 5b64 6174 655f 636f  ns] = df[date_co
+00018e30: 6c75 6d6e 735d 2e61 7070 6c79 2870 642e  lumns].apply(pd.
+00018e40: 746f 5f64 6174 6574 696d 652c 2066 6f72  to_datetime, for
+00018e50: 6d61 743d 2725 592d 256d 2d25 6427 290d  mat='%Y-%m-%d').
+00018e60: 0a20 2020 2020 2020 2020 2020 2064 662e  .            df.
+00018e70: 6c61 7374 5f75 7064 6174 6564 203d 2070  last_updated = p
+00018e80: 642e 746f 5f64 6174 6574 696d 6528 6466  d.to_datetime(df
+00018e90: 2e6c 6173 745f 7570 6461 7465 6420 2b20  .last_updated + 
+00018ea0: 2730 3027 2c20 7574 633d 5472 7565 2c20  '00', utc=True, 
+00018eb0: 666f 726d 6174 3d27 2559 2d25 6d2d 2564  format='%Y-%m-%d
+00018ec0: 2025 483a 254d 3a25 5325 7a27 290d 0a0d   %H:%M:%S%z')...
+00018ed0: 0a20 2020 2020 2020 2020 2020 2064 6620  .            df 
+00018ee0: 3d20 6466 2e61 7374 7970 6528 6474 7970  = df.astype(dtyp
+00018ef0: 653d 7b0d 0a20 2020 2020 2020 2020 2020  e={..           
+00018f00: 2020 2020 2027 6964 273a 2027 7374 7269       'id': 'stri
+00018f10: 6e67 272c 0d0a 2020 2020 2020 2020 2020  ng',..          
+00018f20: 2020 2020 2020 2774 6974 6c65 273a 2027        'title': '
+00018f30: 7374 7269 6e67 272c 0d0a 2020 2020 2020  string',..      
+00018f40: 2020 2020 2020 2020 2020 276e 6f74 6573            'notes
+00018f50: 273a 2027 7374 7269 6e67 272c 0d0a 2020  ': 'string',..  
+00018f60: 2020 2020 2020 2020 2020 2020 2020 2766                'f
+00018f70: 7265 7175 656e 6379 273a 2027 6361 7465  requency': 'cate
+00018f80: 676f 7279 272c 0d0a 2020 2020 2020 2020  gory',..        
+00018f90: 2020 2020 2020 2020 2766 7265 7175 656e          'frequen
+00018fa0: 6379 5f73 686f 7274 273a 2027 6361 7465  cy_short': 'cate
+00018fb0: 676f 7279 272c 0d0a 2020 2020 2020 2020  gory',..        
+00018fc0: 2020 2020 2020 2020 2775 6e69 7473 5f73          'units_s
+00018fd0: 686f 7274 273a 2027 6361 7465 676f 7279  hort': 'category
+00018fe0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00018ff0: 2020 2020 2775 6e69 7473 273a 2027 6361      'units': 'ca
+00019000: 7465 676f 7279 272c 0d0a 2020 2020 2020  tegory',..      
+00019010: 2020 2020 2020 2020 2020 2773 6561 736f            'seaso
+00019020: 6e61 6c5f 6164 6a75 7374 6d65 6e74 273a  nal_adjustment':
+00019030: 2027 6361 7465 676f 7279 272c 0d0a 2020   'category',..  
+00019040: 2020 2020 2020 2020 2020 2020 2020 2773                's
+00019050: 6561 736f 6e61 6c5f 6164 6a75 7374 6d65  easonal_adjustme
+00019060: 6e74 5f73 686f 7274 273a 2027 6361 7465  nt_short': 'cate
+00019070: 676f 7279 270d 0a20 2020 2020 2020 2020  gory'..         
+00019080: 2020 207d 292e 7365 745f 696e 6465 7828     }).set_index(
+00019090: 2769 6427 290d 0a0d 0a20 2020 2020 2020  'id')....       
+000190a0: 2072 6574 7572 6e20 6466 0d0a 0d0a 2020   return df....  
+000190b0: 2020 6465 6620 7365 7269 6573 5f73 6561    def series_sea
+000190c0: 7263 685f 7461 6773 280d 0a20 2020 2020  rch_tags(..     
+000190d0: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+000190e0: 2020 2020 2020 2020 2020 7365 7269 6573            series
+000190f0: 5f73 6561 7263 685f 7465 7874 3a20 7374  _search_text: st
+00019100: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+00019110: 7265 616c 7469 6d65 5f73 7461 7274 3a20  realtime_start: 
+00019120: 6461 7465 203d 204e 6f6e 652c 0d0a 2020  date = None,..  
+00019130: 2020 2020 2020 2020 2020 7265 616c 7469            realti
+00019140: 6d65 5f65 6e64 3a20 6461 7465 203d 204e  me_end: date = N
+00019150: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+00019160: 2020 7461 675f 6e61 6d65 733a 204c 6973    tag_names: Lis
+00019170: 745b 7374 725d 203d 204e 6f6e 652c 0d0a  t[str] = None,..
+00019180: 2020 2020 2020 2020 2020 2020 7461 675f              tag_
+00019190: 6772 6f75 705f 6964 3a20 656e 756d 732e  group_id: enums.
+000191a0: 5461 6747 726f 7570 4944 203d 204e 6f6e  TagGroupID = Non
+000191b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000191c0: 7461 675f 7365 6172 6368 5f74 6578 743a  tag_search_text:
+000191d0: 2073 7472 203d 204e 6f6e 652c 0d0a 2020   str = None,..  
+000191e0: 2020 2020 2020 2020 2020 6f72 6465 725f            order_
+000191f0: 6279 3a20 656e 756d 732e 4f72 6465 7242  by: enums.OrderB
+00019200: 7920 3d20 656e 756d 732e 4f72 6465 7242  y = enums.OrderB
+00019210: 792e 7365 7269 6573 5f63 6f75 6e74 2c0d  y.series_count,.
+00019220: 0a20 2020 2020 2020 2020 2020 2073 6f72  .            sor
+00019230: 745f 6f72 6465 723a 2065 6e75 6d73 2e53  t_order: enums.S
+00019240: 6f72 744f 7264 6572 203d 2065 6e75 6d73  ortOrder = enums
+00019250: 2e53 6f72 744f 7264 6572 2e61 7363 0d0a  .SortOrder.asc..
+00019260: 2020 2020 2920 2d3e 2070 642e 4461 7461      ) -> pd.Data
+00019270: 4672 616d 653a 0d0a 2020 2020 2020 2020  Frame:..        
+00019280: 2222 220d 0a20 2020 2020 2020 2023 2320  """..        ## 
+00019290: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+000192a0: 2020 2020 6073 6572 6965 735f 7365 6172      `series_sear
+000192b0: 6368 5f74 6578 7460 0d0a 2020 2020 2020  ch_text`..      
+000192c0: 2020 5468 6520 776f 7264 7320 746f 206d    The words to m
+000192d0: 6174 6368 2061 6761 696e 7374 2065 636f  atch against eco
+000192e0: 6e6f 6d69 6320 6461 7461 2073 6572 6965  nomic data serie
+000192f0: 732e 0d0a 0d0a 2020 2020 2020 2020 6072  s.....        `r
+00019300: 6561 6c74 696d 655f 7374 6172 7460 0d0a  ealtime_start`..
+00019310: 2020 2020 2020 2020 5468 6520 7374 6172          The star
+00019320: 7420 6f66 2074 6865 2072 6561 6c2d 7469  t of the real-ti
+00019330: 6d65 2070 6572 696f 642e 2046 6f72 206d  me period. For m
+00019340: 6f72 6520 696e 666f 726d 6174 696f 6e2c  ore information,
+00019350: 2073 6565 205b 5265 616c 2d54 696d 6520   see [Real-Time 
+00019360: 5065 7269 6f64 735d 2868 7474 7073 3a2f  Periods](https:/
+00019370: 2f66 7265 642e 7374 6c6f 7569 7366 6564  /fred.stlouisfed
+00019380: 2e6f 7267 2f64 6f63 732f 6170 692f 6672  .org/docs/api/fr
+00019390: 6564 2f72 6561 6c74 696d 655f 7065 7269  ed/realtime_peri
+000193a0: 6f64 2e68 746d 6c29 2e0d 0a0d 0a20 2020  od.html).....   
+000193b0: 2020 2020 2060 7265 616c 7469 6d65 5f65       `realtime_e
+000193c0: 6e64 600d 0a20 2020 2020 2020 2054 6865  nd`..        The
+000193d0: 2065 6e64 206f 6620 7468 6520 7265 616c   end of the real
+000193e0: 2d74 696d 6520 7065 7269 6f64 2e20 466f  -time period. Fo
+000193f0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+00019400: 6f6e 2c20 7365 6520 5b52 6561 6c2d 5469  on, see [Real-Ti
+00019410: 6d65 2050 6572 696f 6473 5d28 6874 7470  me Periods](http
+00019420: 733a 2f2f 6672 6564 2e73 746c 6f75 6973  s://fred.stlouis
+00019430: 6665 642e 6f72 672f 646f 6373 2f61 7069  fed.org/docs/api
+00019440: 2f66 7265 642f 7265 616c 7469 6d65 5f70  /fred/realtime_p
+00019450: 6572 696f 642e 6874 6d6c 292e 0d0a 0d0a  eriod.html).....
+00019460: 2020 2020 2020 2020 6074 6167 5f6e 616d          `tag_nam
+00019470: 6573 600d 0a20 2020 2020 2020 2041 2073  es`..        A s
+00019480: 656d 6963 6f6c 6f6e 2064 656c 696d 6974  emicolon delimit
+00019490: 6564 206c 6973 7420 6f66 2074 6167 206e  ed list of tag n
+000194a0: 616d 6573 2074 6f20 6f6e 6c79 2069 6e63  ames to only inc
+000194b0: 6c75 6465 2069 6e20 7468 6520 7265 7370  lude in the resp
+000194c0: 6f6e 7365 2e20 5365 6520 7468 6520 7265  onse. See the re
+000194d0: 6c61 7465 6420 7265 7175 6573 7420 6672  lated request fr
+000194e0: 6564 2f73 6572 6965 732f 7365 6172 6368  ed/series/search
+000194f0: 2f72 656c 6174 6564 5f74 6167 732e 0d0a  /related_tags...
+00019500: 0d0a 2020 2020 2020 2020 6074 6167 5f67  ..        `tag_g
+00019510: 726f 7570 5f69 6460 0d0a 2020 2020 2020  roup_id`..      
+00019520: 2020 4120 7461 6720 6772 6f75 7020 6964    A tag group id
+00019530: 2074 6f20 6669 6c74 6572 2074 6167 7320   to filter tags 
+00019540: 6279 2074 7970 652e 0d0a 0d0a 2020 2020  by type.....    
+00019550: 2020 2020 6074 6167 5f73 6561 7263 685f      `tag_search_
+00019560: 7465 7874 600d 0a20 2020 2020 2020 2054  text`..        T
+00019570: 6865 2077 6f72 6473 2074 6f20 6669 6e64  he words to find
+00019580: 206d 6174 6368 696e 6720 7461 6773 2077   matching tags w
+00019590: 6974 682e 0d0a 0d0a 2020 2020 2020 2020  ith.....        
+000195a0: 606f 7264 6572 5f62 7960 0d0a 2020 2020  `order_by`..    
+000195b0: 2020 2020 4f72 6465 7220 7265 7375 6c74      Order result
+000195c0: 7320 6279 2076 616c 7565 7320 6f66 2074  s by values of t
+000195d0: 6865 2073 7065 6369 6669 6564 2061 7474  he specified att
+000195e0: 7269 6275 7465 2e0d 0a0d 0a20 2020 2020  ribute.....     
+000195f0: 2020 2060 736f 7274 5f6f 7264 6572 600d     `sort_order`.
+00019600: 0a20 2020 2020 2020 2053 6f72 7420 7265  .        Sort re
+00019610: 7375 6c74 7320 6973 2061 7363 656e 6469  sults is ascendi
+00019620: 6e67 206f 7220 6465 7363 656e 6469 6e67  ng or descending
+00019630: 206f 7264 6572 2066 6f72 2061 7474 7269   order for attri
+00019640: 6275 7465 2076 616c 7565 7320 7370 6563  bute values spec
+00019650: 6966 6965 6420 6279 206f 7264 6572 5f62  ified by order_b
+00019660: 792e 0d0a 0d0a 2020 2020 2020 2020 2323  y.....        ##
+00019670: 2044 6573 6372 6970 7469 6f6e 0d0a 2020   Description..  
+00019680: 2020 2020 2020 6874 7470 733a 2f2f 6672        https://fr
+00019690: 6564 2e73 746c 6f75 6973 6665 642e 6f72  ed.stlouisfed.or
+000196a0: 672f 646f 6373 2f61 7069 2f66 7265 642f  g/docs/api/fred/
+000196b0: 7365 7269 6573 5f73 6561 7263 685f 7461  series_search_ta
+000196c0: 6773 2e68 746d 6c0d 0a0d 0a20 2020 2020  gs.html....     
+000196d0: 2020 2047 6574 2074 6865 2046 5245 4420     Get the FRED 
+000196e0: 7461 6773 2066 6f72 2061 2073 6572 6965  tags for a serie
+000196f0: 7320 7365 6172 6368 2e20 4f70 7469 6f6e  s search. Option
+00019700: 616c 6c79 2c20 6669 6c74 6572 2072 6573  ally, filter res
+00019710: 756c 7473 2062 7920 7461 6720 6e61 6d65  ults by tag name
+00019720: 2c20 7461 6720 6772 6f75 702c 206f 7220  , tag group, or 
+00019730: 7461 6720 7365 6172 6368 2e20 5365 6520  tag search. See 
+00019740: 7468 6520 7265 6c61 7465 6420 7265 7175  the related requ
+00019750: 6573 7420 6672 6564 2f73 6572 6965 732f  est fred/series/
+00019760: 7365 6172 6368 2f72 656c 6174 6564 5f74  search/related_t
+00019770: 6167 732e 0d0a 0d0a 2020 2020 2020 2020  ags.....        
+00019780: 2323 2041 5049 2052 6571 7565 7374 2028  ## API Request (
+00019790: 4854 5450 5320 4745 5429 0d0a 2020 2020  HTTPS GET)..    
+000197a0: 2020 2020 6874 7470 733a 2f2f 6170 692e      https://api.
+000197b0: 7374 6c6f 7569 7366 6564 2e6f 7267 2f66  stlouisfed.org/f
+000197c0: 7265 642f 7365 7269 6573 2f73 6561 7263  red/series/searc
+000197d0: 682f 7461 6773 3f73 6572 6965 735f 7365  h/tags?series_se
+000197e0: 6172 6368 5f74 6578 743d 6d6f 6e65 7461  arch_text=moneta
+000197f0: 7279 2b73 6572 7669 6365 2b69 6e64 6578  ry+service+index
+00019800: 2661 7069 5f6b 6579 3d61 6263 6465 6667  &api_key=abcdefg
+00019810: 6869 6a6b 6c6d 6e6f 7071 7273 7475 7677  hijklmnopqrstuvw
+00019820: 7879 7a31 3233 3435 3626 6669 6c65 5f74  xyz123456&file_t
+00019830: 7970 653d 6a73 6f6e 0d0a 0d0a 2020 2020  ype=json....    
+00019840: 2020 2020 2323 2041 5049 2052 6573 706f      ## API Respo
+00019850: 6e73 650d 0a20 2020 2020 2020 2060 6060  nse..        ```
+00019860: 6a73 6f6e 0d0a 2020 2020 2020 2020 7b0d  json..        {.
+00019870: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00019880: 616c 7469 6d65 5f73 7461 7274 223a 2022  altime_start": "
+00019890: 3230 3133 2d30 382d 3134 222c 0d0a 2020  2013-08-14",..  
+000198a0: 2020 2020 2020 2020 2020 2272 6561 6c74            "realt
+000198b0: 696d 655f 656e 6422 3a20 2232 3031 332d  ime_end": "2013-
+000198c0: 3038 2d31 3422 2c0d 0a20 2020 2020 2020  08-14",..       
+000198d0: 2020 2020 2022 6f72 6465 725f 6279 223a       "order_by":
+000198e0: 2022 7365 7269 6573 5f63 6f75 6e74 222c   "series_count",
+000198f0: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
+00019900: 6f72 745f 6f72 6465 7222 3a20 2264 6573  ort_order": "des
+00019910: 6322 2c0d 0a20 2020 2020 2020 2020 2020  c",..           
+00019920: 2022 636f 756e 7422 3a20 3138 2c0d 0a20   "count": 18,.. 
+00019930: 2020 2020 2020 2020 2020 2022 6f66 6673             "offs
+00019940: 6574 223a 2030 2c0d 0a20 2020 2020 2020  et": 0,..       
+00019950: 2020 2020 2022 6c69 6d69 7422 3a20 3130       "limit": 10
+00019960: 3030 2c0d 0a20 2020 2020 2020 2020 2020  00,..           
+00019970: 2022 7461 6773 223a 205b 0d0a 2020 2020   "tags": [..    
+00019980: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
+00019990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199a0: 2020 2022 6e61 6d65 223a 2022 6163 6164     "name": "acad
+000199b0: 656d 6963 2064 6174 6122 2c0d 0a20 2020  emic data",..   
+000199c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199d0: 2022 6772 6f75 705f 6964 223a 2022 6765   "group_id": "ge
+000199e0: 6e22 2c0d 0a20 2020 2020 2020 2020 2020  n",..           
+000199f0: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
+00019a00: 3a20 2254 696d 6520 7365 7269 6573 2064  : "Time series d
+00019a10: 6174 6120 6372 6561 7465 6420 6d61 696e  ata created main
+00019a20: 6c79 2062 7920 6163 6164 656d 6961 2074  ly by academia t
+00019a30: 6f20 6164 6472 6573 7320 6772 6f77 696e  o address growin
+00019a40: 6720 6465 6d61 6e64 2069 6e20 756e 6465  g demand in unde
+00019a50: 7273 7461 6e64 696e 6720 7370 6563 6966  rstanding specif
+00019a60: 6963 2063 6f6e 6365 726e 7320 696e 2074  ic concerns in t
+00019a70: 6865 2065 636f 6e6f 6d79 2074 6861 7420  he economy that 
+00019a80: 6172 6520 6e6f 7420 7765 6c6c 206d 6f64  are not well mod
+00019a90: 656c 6564 2062 7920 6f72 6469 6e61 7279  eled by ordinary
+00019aa0: 2073 7461 7469 7374 6963 616c 2061 6765   statistical age
+00019ab0: 6e63 6965 732e 222c 0d0a 2020 2020 2020  ncies.",..      
+00019ac0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00019ad0: 7265 6174 6564 223a 2022 3230 3132 2d30  reated": "2012-0
+00019ae0: 382d 3239 2031 303a 3232 3a31 392d 3035  8-29 10:22:19-05
+00019af0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00019b00: 2020 2020 2020 2020 2270 6f70 756c 6172          "popular
+00019b10: 6974 7922 3a20 3632 2c0d 0a20 2020 2020  ity": 62,..     
+00019b20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00019b30: 7365 7269 6573 5f63 6f75 6e74 223a 2032  series_count": 2
+00019b40: 350d 0a20 2020 2020 2020 2020 2020 2020  5..             
+00019b50: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
+00019b60: 2020 2020 2020 202e 2e2e 0d0a 2020 2020         .....    
+00019b70: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
+00019b80: 2020 207d 0d0a 2020 2020 2020 2020 6060     }..        ``
+00019b90: 600d 0a0d 0a20 2020 2020 2020 2023 2320  `....        ## 
+00019ba0: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
+00019bb0: 2060 7061 6e64 6173 2e44 6174 6146 7261   `pandas.DataFra
+00019bc0: 6d65 600d 0a0d 0a20 2020 2020 2020 2023  me`....        #
+00019bd0: 2320 4578 616d 706c 650d 0a20 2020 2020  # Example..     
+00019be0: 2020 2060 6060 7079 7468 6f6e 0d0a 2020     ```python..  
+00019bf0: 2020 2020 2020 3e3e 3e20 6672 6564 203d        >>> fred =
+00019c00: 2046 5245 4428 6170 695f 6b65 793d 2761   FRED(api_key='a
+00019c10: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
+00019c20: 7273 7475 7677 7879 7a31 3233 3435 3627  rstuvwxyz123456'
+00019c30: 290d 0a20 2020 2020 2020 203e 3e3e 2066  )..        >>> f
+00019c40: 7265 642e 7365 7269 6573 5f73 6561 7263  red.series_searc
+00019c50: 685f 7461 6773 2873 6572 6965 735f 7365  h_tags(series_se
+00019c60: 6172 6368 5f74 6578 743d 276d 6f6e 6574  arch_text='monet
+00019c70: 6172 7920 7365 7276 6963 6520 696e 6465  ary service inde
+00019c80: 7827 292e 6865 6164 2829 0d0a 2020 2020  x').head()..    
+00019c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ca0: 2020 2020 2020 6772 6f75 705f 6964 2020        group_id  
+00019cb0: 2020 2020 2020 2020 2020 6e6f 7465 7320            notes 
+00019cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cd0: 2020 6372 6561 7465 6420 2070 6f70 756c    created  popul
+00019ce0: 6172 6974 7920 2073 6572 6965 735f 636f  arity  series_co
+00019cf0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+00019d00: 206e 616d 650d 0a20 2020 2020 2020 2020   name..         
+00019d10: 2020 2061 6363 6f75 6e74 696e 6720 2020     accounting   
+00019d20: 2020 2020 2020 6765 6e20 2020 2020 2020        gen       
+00019d30: 2020 2020 2020 2020 2020 2032 3031 322d             2012-
+00019d40: 3032 2d32 3720 3136 3a31 383a 3139 2b30  02-27 16:18:19+0
+00019d50: 303a 3030 2020 2020 2020 2020 2020 3433  0:00          43
+00019d60: 2020 2020 2020 2020 2020 2020 2032 0d0a               2..
+00019d70: 2020 2020 2020 2020 2020 2020 6164 7665              adve
+00019d80: 7274 6973 656d 656e 7420 2020 2020 2067  rtisement      g
+00019d90: 656e 2020 2020 2020 2020 2020 2020 2020  en              
+00019da0: 2020 2020 3230 3132 2d30 382d 3036 2031      2012-08-06 1
+00019db0: 393a 3530 3a30 372b 3030 3a30 3020 2020  9:50:07+00:00   
+00019dc0: 2020 2020 2020 2031 3720 2020 2020 2020         17       
+00019dd0: 2020 2020 2020 320d 0a20 2020 2020 2020        2..       
+00019de0: 2020 2020 2061 7373 6574 7320 2020 2020       assets     
+00019df0: 2020 2020 2020 2020 6765 6e20 2020 2020          gen     
+00019e00: 2020 2020 2020 2020 2020 2020 2032 3031               201
+00019e10: 322d 3032 2d32 3720 3136 3a31 383a 3139  2-02-27 16:18:19
+00019e20: 2b30 303a 3030 2020 2020 2020 2020 2020  +00:00          
+00019e30: 3634 2020 2020 2020 2020 2020 2020 2032  64             2
+00019e40: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
+00019e50: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00019e60: 2073 7263 2020 4261 6e6b 206f 6620 456e   src  Bank of En
+00019e70: 676c 616e 6420 3230 3133 2d30 322d 3235  gland 2013-02-25
+00019e80: 2032 323a 3231 3a31 392b 3030 3a30 3020   22:21:19+00:00 
+00019e90: 2020 2020 2020 2020 2034 3220 2020 2020           42     
+00019ea0: 2020 2020 2020 2020 320d 0a20 2020 2020          2..     
+00019eb0: 2020 2020 2020 2063 6f6d 6d75 6e69 6361         communica
+00019ec0: 7469 6f6e 2020 2020 2020 6765 6e20 2020  tion      gen   
+00019ed0: 2020 2020 2020 2020 2020 2020 2020 2032                 2
+00019ee0: 3031 322d 3032 2d32 3720 3136 3a31 383a  012-02-27 16:18:
+00019ef0: 3139 2b30 303a 3030 2020 2020 2020 2020  19+00:00        
+00019f00: 2020 3232 2020 2020 2020 2020 2020 2020    22            
+00019f10: 2032 0d0a 2020 2020 2020 2020 6060 600d   2..        ```.
+00019f20: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00019f30: 2020 2020 2020 616c 6c6f 7765 645f 6f72        allowed_or
+00019f40: 6465 7273 203d 205b 0d0a 2020 2020 2020  ders = [..      
+00019f50: 2020 2020 2020 656e 756d 732e 4f72 6465        enums.Orde
+00019f60: 7242 792e 7365 7269 6573 5f63 6f75 6e74  rBy.series_count
+00019f70: 2c0d 0a20 2020 2020 2020 2020 2020 2065  ,..            e
+00019f80: 6e75 6d73 2e4f 7264 6572 4279 2e70 6f70  nums.OrderBy.pop
+00019f90: 756c 6172 6974 792c 0d0a 2020 2020 2020  ularity,..      
+00019fa0: 2020 2020 2020 656e 756d 732e 4f72 6465        enums.Orde
+00019fb0: 7242 792e 6372 6561 7465 642c 0d0a 2020  rBy.created,..  
+00019fc0: 2020 2020 2020 2020 2020 656e 756d 732e            enums.
+00019fd0: 4f72 6465 7242 792e 6e61 6d65 2c0d 0a20  OrderBy.name,.. 
+00019fe0: 2020 2020 2020 2020 2020 2065 6e75 6d73             enums
+00019ff0: 2e4f 7264 6572 4279 2e67 726f 7570 5f69  .OrderBy.group_i
+0001a000: 642c 0d0a 2020 2020 2020 2020 5d0d 0a0d  d,..        ]...
+0001a010: 0a20 2020 2020 2020 2069 6620 6f72 6465  .        if orde
+0001a020: 725f 6279 206e 6f74 2069 6e20 616c 6c6f  r_by not in allo
+0001a030: 7765 645f 6f72 6465 7273 3a0d 0a20 2020  wed_orders:..   
+0001a040: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0001a050: 616c 7565 4572 726f 7228 2756 6172 6961  alueError('Varia
+0001a060: 626c 6520 6f72 6465 725f 6279 2028 7b7d  ble order_by ({}
+0001a070: 2920 6973 206e 6f74 206f 6e65 206f 6620  ) is not one of 
+0001a080: 7468 6520 7661 6c75 6573 3a20 7b7d 272e  the values: {}'.
+0001a090: 666f 726d 6174 286f 7264 6572 5f62 792c  format(order_by,
+0001a0a0: 2027 2c20 272e 6a6f 696e 286d 6170 2873   ', '.join(map(s
+0001a0b0: 7472 2c20 616c 6c6f 7765 645f 6f72 6465  tr, allowed_orde
+0001a0c0: 7273 2929 2929 0d0a 0d0a 2020 2020 2020  rs))))....      
+0001a0d0: 2020 6966 2072 6561 6c74 696d 655f 7374    if realtime_st
+0001a0e0: 6172 7420 6973 206e 6f74 204e 6f6e 6520  art is not None 
+0001a0f0: 616e 6420 7265 616c 7469 6d65 5f73 7461  and realtime_sta
+0001a100: 7274 203c 2064 6174 6528 3137 3736 2c20  rt < date(1776, 
+0001a110: 372c 2034 293a 0d0a 2020 2020 2020 2020  7, 4):..        
+0001a120: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0001a130: 7272 6f72 2827 5661 7269 6162 6c65 2072  rror('Variable r
+0001a140: 6561 6c74 696d 655f 7374 6172 7420 2822  ealtime_start ("
+0001a150: 7b7d 2229 2069 7320 6265 666f 7265 206d  {}") is before m
+0001a160: 696e 2064 6174 6520 3137 3736 2d30 372d  in date 1776-07-
+0001a170: 3034 2e27 2e66 6f72 6d61 7428 7265 616c  04.'.format(real
+0001a180: 7469 6d65 5f73 7461 7274 2929 0d0a 0d0a  time_start))....
+0001a190: 2020 2020 2020 2020 6966 2072 6561 6c74          if realt
+0001a1a0: 696d 655f 7374 6172 7420 6973 206e 6f74  ime_start is not
+0001a1b0: 204e 6f6e 6520 616e 6420 7265 616c 7469   None and realti
+0001a1c0: 6d65 5f65 6e64 2069 7320 6e6f 7420 4e6f  me_end is not No
+0001a1d0: 6e65 2061 6e64 2072 6561 6c74 696d 655f  ne and realtime_
+0001a1e0: 7374 6172 7420 3e20 7265 616c 7469 6d65  start > realtime
+0001a1f0: 5f65 6e64 3a0d 0a20 2020 2020 2020 2020  _end:..         
+0001a200: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0001a210: 726f 7228 2754 6865 2064 6174 6520 7365  ror('The date se
+0001a220: 7420 6279 2076 6172 6961 626c 6520 7265  t by variable re
+0001a230: 616c 7469 6d65 5f73 7461 7274 2028 227b  altime_start ("{
+0001a240: 7d22 2920 6361 6e20 6e6f 7420 6265 2061  }") can not be a
+0001a250: 6674 6572 2074 6865 2064 6174 6520 7365  fter the date se
+0001a260: 7420 6279 2076 6172 6961 626c 6520 7265  t by variable re
+0001a270: 616c 7469 6d65 5f65 6e64 2028 227b 7d22  altime_end ("{}"
+0001a280: 292e 272e 666f 726d 6174 2872 6561 6c74  ).'.format(realt
+0001a290: 696d 655f 7374 6172 742c 2072 6561 6c74  ime_start, realt
+0001a2a0: 696d 655f 656e 6429 290d 0a0d 0a20 2020  ime_end))....   
+0001a2b0: 2020 2020 2064 6620 3d20 7064 2e44 6174       df = pd.Dat
+0001a2c0: 6146 7261 6d65 280d 0a20 2020 2020 2020  aFrame(..       
+0001a2d0: 2020 2020 2073 656c 662e 5f63 6c69 656e       self._clien
+0001a2e0: 742e 6765 7428 0d0a 2020 2020 2020 2020  t.get(..        
+0001a2f0: 2020 2020 2020 2020 272f 6672 6564 2f73          '/fred/s
+0001a300: 6572 6965 732f 7365 6172 6368 2f74 6167  eries/search/tag
+0001a310: 7327 2c0d 0a20 2020 2020 2020 2020 2020  s',..           
+0001a320: 2020 2020 2027 7461 6773 272c 0d0a 2020       'tags',..  
+0001a330: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0001a340: 6d69 743d 3130 3030 2c0d 0a20 2020 2020  mit=1000,..     
+0001a350: 2020 2020 2020 2020 2020 2073 6572 6965             serie
+0001a360: 735f 7365 6172 6368 5f74 6578 743d 7365  s_search_text=se
+0001a370: 7269 6573 5f73 6561 7263 685f 7465 7874  ries_search_text
+0001a380: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001a390: 2020 2072 6561 6c74 696d 655f 7374 6172     realtime_star
+0001a3a0: 743d 7265 616c 7469 6d65 5f73 7461 7274  t=realtime_start
+0001a3b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001a3c0: 2020 2072 6561 6c74 696d 655f 656e 643d     realtime_end=
+0001a3d0: 7265 616c 7469 6d65 5f65 6e64 2c0d 0a20  realtime_end,.. 
+0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001a3f0: 6167 5f6e 616d 6573 3d74 6167 5f6e 616d  ag_names=tag_nam
+0001a400: 6573 2c0d 0a20 2020 2020 2020 2020 2020  es,..           
+0001a410: 2020 2020 2074 6167 5f67 726f 7570 5f69       tag_group_i
+0001a420: 643d 7461 675f 6772 6f75 705f 6964 2c0d  d=tag_group_id,.
+0001a430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a440: 2074 6167 5f73 6561 7263 685f 7465 7874   tag_search_text
+0001a450: 3d74 6167 5f73 6561 7263 685f 7465 7874  =tag_search_text
+0001a460: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001a470: 2020 206f 7264 6572 5f62 793d 6f72 6465     order_by=orde
+0001a480: 725f 6279 2c0d 0a20 2020 2020 2020 2020  r_by,..         
+0001a490: 2020 2020 2020 2073 6f72 745f 6f72 6465         sort_orde
+0001a4a0: 723d 736f 7274 5f6f 7264 6572 0d0a 2020  r=sort_order..  
+0001a4b0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0001a4c0: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+0001a4d0: 2020 6966 206e 6f74 2064 662e 656d 7074    if not df.empt
+0001a4e0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0001a4f0: 6466 2e63 7265 6174 6564 203d 2070 642e  df.created = pd.
+0001a500: 746f 5f64 6174 6574 696d 6528 6466 2e63  to_datetime(df.c
+0001a510: 7265 6174 6564 202b 2027 3030 272c 2075  reated + '00', u
+0001a520: 7463 3d54 7275 652c 2066 6f72 6d61 743d  tc=True, format=
+0001a530: 2725 592d 256d 2d25 6420 2548 3a25 4d3a  '%Y-%m-%d %H:%M:
+0001a540: 2553 257a 2729 0d0a 0d0a 2020 2020 2020  %S%z')....      
+0001a550: 2020 2020 2020 6466 203d 2064 662e 6173        df = df.as
+0001a560: 7479 7065 2864 7479 7065 3d7b 0d0a 2020  type(dtype={..  
+0001a570: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+0001a580: 616d 6527 3a20 2773 7472 696e 6727 2c0d  ame': 'string',.
+0001a590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a5a0: 2027 6e6f 7465 7327 3a20 2773 7472 696e   'notes': 'strin
+0001a5b0: 6727 2c0d 0a20 2020 2020 2020 2020 2020  g',..           
+0001a5c0: 2020 2020 2027 6772 6f75 705f 6964 273a       'group_id':
+0001a5d0: 2027 6361 7465 676f 7279 270d 0a20 2020   'category'..   
+0001a5e0: 2020 2020 2020 2020 207d 292e 7365 745f           }).set_
+0001a5f0: 696e 6465 7828 276e 616d 6527 290d 0a0d  index('name')...
+0001a600: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a610: 6466 0d0a 0d0a 2020 2020 6465 6620 7365  df....    def se
+0001a620: 7269 6573 5f73 6561 7263 685f 7265 6c61  ries_search_rela
+0001a630: 7465 645f 7461 6773 280d 0a20 2020 2020  ted_tags(..     
+0001a640: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+0001a650: 2020 2020 2020 2020 2020 7365 7269 6573            series
+0001a660: 5f73 6561 7263 685f 7465 7874 3a20 7374  _search_text: st
+0001a670: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+0001a680: 7265 616c 7469 6d65 5f73 7461 7274 3a20  realtime_start: 
+0001a690: 6461 7465 203d 204e 6f6e 652c 0d0a 2020  date = None,..  
+0001a6a0: 2020 2020 2020 2020 2020 7265 616c 7469            realti
+0001a6b0: 6d65 5f65 6e64 3a20 6461 7465 203d 204e  me_end: date = N
+0001a6c0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+0001a6d0: 2020 7461 675f 6e61 6d65 733a 204c 6973    tag_names: Lis
+0001a6e0: 745b 7374 725d 203d 204e 6f6e 652c 0d0a  t[str] = None,..
+0001a6f0: 2020 2020 2020 2020 2020 2020 6578 636c              excl
+0001a700: 7564 655f 7461 675f 6e61 6d65 733a 204c  ude_tag_names: L
+0001a710: 6973 745b 7374 725d 203d 204e 6f6e 652c  ist[str] = None,
+0001a720: 0d0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
+0001a730: 675f 6772 6f75 705f 6964 3a20 656e 756d  g_group_id: enum
+0001a740: 732e 5461 6747 726f 7570 4944 203d 204e  s.TagGroupID = N
+0001a750: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+0001a760: 2020 7461 675f 7365 6172 6368 5f74 6578    tag_search_tex
+0001a770: 743a 2073 7472 203d 204e 6f6e 652c 0d0a  t: str = None,..
+0001a780: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
+0001a790: 725f 6279 3a20 656e 756d 732e 4f72 6465  r_by: enums.Orde
+0001a7a0: 7242 7920 3d20 656e 756d 732e 4f72 6465  rBy = enums.Orde
+0001a7b0: 7242 792e 7365 7269 6573 5f63 6f75 6e74  rBy.series_count
+0001a7c0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+0001a7d0: 6f72 745f 6f72 6465 723a 2065 6e75 6d73  ort_order: enums
+0001a7e0: 2e53 6f72 744f 7264 6572 203d 2065 6e75  .SortOrder = enu
+0001a7f0: 6d73 2e53 6f72 744f 7264 6572 2e61 7363  ms.SortOrder.asc
+0001a800: 0d0a 2020 2020 2920 2d3e 2070 642e 4461  ..    ) -> pd.Da
+0001a810: 7461 4672 616d 653a 0d0a 2020 2020 2020  taFrame:..      
+0001a820: 2020 2222 220d 0a20 2020 2020 2020 2023    """..        #
+0001a830: 2320 5061 7261 6d65 7465 7273 0d0a 2020  # Parameters..  
+0001a840: 2020 2020 2020 6073 6572 6965 735f 7365        `series_se
+0001a850: 6172 6368 5f74 6578 7460 0d0a 2020 2020  arch_text`..    
+0001a860: 2020 2020 5468 6520 776f 7264 7320 746f      The words to
+0001a870: 206d 6174 6368 2061 6761 696e 7374 2065   match against e
+0001a880: 636f 6e6f 6d69 6320 6461 7461 2073 6572  conomic data ser
+0001a890: 6965 732e 0d0a 0d0a 2020 2020 2020 2020  ies.....        
+0001a8a0: 6072 6561 6c74 696d 655f 7374 6172 7460  `realtime_start`
+0001a8b0: 0d0a 2020 2020 2020 2020 5468 6520 7374  ..        The st
+0001a8c0: 6172 7420 6f66 2074 6865 2072 6561 6c2d  art of the real-
+0001a8d0: 7469 6d65 2070 6572 696f 642e 2046 6f72  time period. For
+0001a8e0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+0001a8f0: 6e2c 2073 6565 205b 5265 616c 2d54 696d  n, see [Real-Tim
+0001a900: 6520 5065 7269 6f64 735d 2868 7474 7073  e Periods](https
+0001a910: 3a2f 2f66 7265 642e 7374 6c6f 7569 7366  ://fred.stlouisf
+0001a920: 6564 2e6f 7267 2f64 6f63 732f 6170 692f  ed.org/docs/api/
+0001a930: 6672 6564 2f72 6561 6c74 696d 655f 7065  fred/realtime_pe
+0001a940: 7269 6f64 2e68 746d 6c29 2e0d 0a0d 0a20  riod.html)..... 
+0001a950: 2020 2020 2020 2060 7265 616c 7469 6d65         `realtime
+0001a960: 5f65 6e64 600d 0a20 2020 2020 2020 2054  _end`..        T
+0001a970: 6865 2065 6e64 206f 6620 7468 6520 7265  he end of the re
+0001a980: 616c 2d74 696d 6520 7065 7269 6f64 2e20  al-time period. 
+0001a990: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
+0001a9a0: 7469 6f6e 2c20 7365 6520 5b52 6561 6c2d  tion, see [Real-
+0001a9b0: 5469 6d65 2050 6572 696f 6473 5d28 6874  Time Periods](ht
+0001a9c0: 7470 733a 2f2f 6672 6564 2e73 746c 6f75  tps://fred.stlou
+0001a9d0: 6973 6665 642e 6f72 672f 646f 6373 2f61  isfed.org/docs/a
+0001a9e0: 7069 2f66 7265 642f 7265 616c 7469 6d65  pi/fred/realtime
+0001a9f0: 5f70 6572 696f 642e 6874 6d6c 292e 0d0a  _period.html)...
+0001aa00: 0d0a 2020 2020 2020 2020 6074 6167 5f6e  ..        `tag_n
+0001aa10: 616d 6573 600d 0a20 2020 2020 2020 2041  ames`..        A
+0001aa20: 2073 656d 6963 6f6c 6f6e 2064 656c 696d   semicolon delim
+0001aa30: 6974 6564 206c 6973 7420 6f66 2074 6167  ited list of tag
+0001aa40: 206e 616d 6573 2074 6f20 6f6e 6c79 2069   names to only i
+0001aa50: 6e63 6c75 6465 2069 6e20 7468 6520 7265  nclude in the re
+0001aa60: 7370 6f6e 7365 2e20 5365 6520 7468 6520  sponse. See the 
+0001aa70: 7265 6c61 7465 6420 7265 7175 6573 7420  related request 
+0001aa80: 6672 6564 2f73 6572 6965 732f 7365 6172  fred/series/sear
+0001aa90: 6368 2f72 656c 6174 6564 5f74 6167 732e  ch/related_tags.
+0001aaa0: 0d0a 0d0a 2020 2020 2020 2020 6065 7863  ....        `exc
+0001aab0: 6c75 6465 5f74 6167 5f6e 616d 6573 600d  lude_tag_names`.
+0001aac0: 0a20 2020 2020 2020 2054 7570 6c65 206f  .        Tuple o
+0001aad0: 6620 7461 6720 6e61 6d65 7320 7468 6174  f tag names that
+0001aae0: 2073 6572 6965 7320 6d61 7463 6820 6e6f   series match no
+0001aaf0: 6e65 206f 662e 0d0a 0d0a 2020 2020 2020  ne of.....      
+0001ab00: 2020 6074 6167 5f67 726f 7570 5f69 6460    `tag_group_id`
+0001ab10: 0d0a 2020 2020 2020 2020 4120 7461 6720  ..        A tag 
+0001ab20: 6772 6f75 7020 6964 2074 6f20 6669 6c74  group id to filt
+0001ab30: 6572 2074 6167 7320 6279 2074 7970 652e  er tags by type.
+0001ab40: 0d0a 0d0a 2020 2020 2020 2020 6074 6167  ....        `tag
+0001ab50: 5f73 6561 7263 685f 7465 7874 600d 0a20  _search_text`.. 
+0001ab60: 2020 2020 2020 2054 6865 2077 6f72 6473         The words
+0001ab70: 2074 6f20 6669 6e64 206d 6174 6368 696e   to find matchin
+0001ab80: 6720 7461 6773 2077 6974 682e 0d0a 0d0a  g tags with.....
+0001ab90: 2020 2020 2020 2020 606f 7264 6572 5f62          `order_b
+0001aba0: 7960 0d0a 2020 2020 2020 2020 4f72 6465  y`..        Orde
+0001abb0: 7220 7265 7375 6c74 7320 6279 2076 616c  r results by val
+0001abc0: 7565 7320 6f66 2074 6865 2073 7065 6369  ues of the speci
+0001abd0: 6669 6564 2061 7474 7269 6275 7465 2e0d  fied attribute..
+0001abe0: 0a0d 0a20 2020 2020 2020 2060 736f 7274  ...        `sort
+0001abf0: 5f6f 7264 6572 600d 0a20 2020 2020 2020  _order`..       
+0001ac00: 2053 6f72 7420 7265 7375 6c74 7320 6973   Sort results is
+0001ac10: 2061 7363 656e 6469 6e67 206f 7220 6465   ascending or de
+0001ac20: 7363 656e 6469 6e67 206f 7264 6572 2066  scending order f
+0001ac30: 6f72 2061 7474 7269 6275 7465 2076 616c  or attribute val
+0001ac40: 7565 7320 7370 6563 6966 6965 6420 6279  ues specified by
+0001ac50: 206f 7264 6572 5f62 792e 0d0a 0d0a 2020   order_by.....  
+0001ac60: 2020 2020 2020 2323 2044 6573 6372 6970        ## Descrip
+0001ac70: 7469 6f6e 0d0a 2020 2020 2020 2020 6874  tion..        ht
+0001ac80: 7470 733a 2f2f 6672 6564 2e73 746c 6f75  tps://fred.stlou
+0001ac90: 6973 6665 642e 6f72 672f 646f 6373 2f61  isfed.org/docs/a
+0001aca0: 7069 2f66 7265 642f 7365 7269 6573 5f73  pi/fred/series_s
+0001acb0: 6561 7263 685f 7265 6c61 7465 645f 7461  earch_related_ta
+0001acc0: 6773 2e68 746d 6c0d 0a0d 0a20 2020 2020  gs.html....     
+0001acd0: 2020 2047 6574 2074 6865 2072 656c 6174     Get the relat
+0001ace0: 6564 2046 5245 4420 7461 6773 2066 6f72  ed FRED tags for
+0001acf0: 206f 6e65 206f 7220 6d6f 7265 2046 5245   one or more FRE
+0001ad00: 4420 7461 6773 206d 6174 6368 696e 6720  D tags matching 
+0001ad10: 6120 7365 7269 6573 2073 6561 7263 682e  a series search.
+0001ad20: 204f 7074 696f 6e61 6c6c 792c 2066 696c   Optionally, fil
+0001ad30: 7465 7220 7265 7375 6c74 7320 6279 2074  ter results by t
+0001ad40: 6167 2067 726f 7570 206f 7220 7461 6720  ag group or tag 
+0001ad50: 7365 6172 6368 2e0d 0a20 2020 2020 2020  search...       
+0001ad60: 2046 5245 4420 7461 6773 2061 7265 2061   FRED tags are a
+0001ad70: 7474 7269 6275 7465 7320 6173 7369 676e  ttributes assign
+0001ad80: 6564 2074 6f20 7365 7269 6573 2e0d 0a20  ed to series... 
+0001ad90: 2020 2020 2020 2046 6f72 2074 6869 7320         For this 
+0001ada0: 7265 7175 6573 742c 2072 656c 6174 6564  request, related
+0001adb0: 2046 5245 4420 7461 6773 2061 7265 2074   FRED tags are t
+0001adc0: 6865 2074 6167 7320 6173 7369 676e 6564  he tags assigned
+0001add0: 2074 6f20 7365 7269 6573 2074 6861 7420   to series that 
+0001ade0: 6d61 7463 6820 616c 6c20 7461 6773 2069  match all tags i
+0001adf0: 6e20 7468 6520 7461 675f 6e61 6d65 7320  n the tag_names 
+0001ae00: 7061 7261 6d65 7465 722c 206e 6f20 7461  parameter, no ta
+0001ae10: 6773 2069 6e20 7468 6520 6578 636c 7564  gs in the exclud
+0001ae20: 655f 7461 675f 6e61 6d65 7320 7061 7261  e_tag_names para
+0001ae30: 6d65 7465 722c 0d0a 2020 2020 2020 2020  meter,..        
+0001ae40: 616e 6420 7468 6520 7365 6172 6368 2077  and the search w
+0001ae50: 6f72 6473 2073 6574 2062 7920 7468 6520  ords set by the 
+0001ae60: 7365 7269 6573 5f73 6561 7263 685f 7465  series_search_te
+0001ae70: 7874 2070 6172 616d 6574 6572 2e0d 0a20  xt parameter... 
+0001ae80: 2020 2020 2020 2053 6565 2074 6865 2072         See the r
+0001ae90: 656c 6174 6564 2072 6571 7565 7374 2066  elated request f
+0001aea0: 7265 642f 7365 7269 6573 2f73 6561 7263  red/series/searc
+0001aeb0: 682f 7461 6773 2e0d 0a0d 0a20 2020 2020  h/tags.....     
+0001aec0: 2020 2023 2320 4150 4920 5265 7175 6573     ## API Reques
+0001aed0: 7420 2848 5454 5053 2047 4554 290d 0a20  t (HTTPS GET).. 
+0001aee0: 2020 2020 2020 2068 7474 7073 3a2f 2f61         https://a
+0001aef0: 7069 2e73 746c 6f75 6973 6665 642e 6f72  pi.stlouisfed.or
+0001af00: 672f 6672 6564 2f73 6572 6965 732f 7365  g/fred/series/se
+0001af10: 6172 6368 2f72 656c 6174 6564 5f74 6167  arch/related_tag
+0001af20: 733f 7365 7269 6573 5f73 6561 7263 685f  s?series_search_
+0001af30: 7465 7874 3d6d 6f72 7467 6167 652b 7261  text=mortgage+ra
+0001af40: 7465 2674 6167 5f6e 616d 6573 3d33 302d  te&tag_names=30-
+0001af50: 7965 6172 3b66 7262 2661 7069 5f6b 6579  year;frb&api_key
+0001af60: 3d61 6263 6465 6667 6869 6a6b 6c6d 6e6f  =abcdefghijklmno
+0001af70: 7071 7273 7475 7677 7879 7a31 3233 3435  pqrstuvwxyz12345
+0001af80: 3626 6669 6c65 5f74 7970 653d 6a73 6f6e  6&file_type=json
+0001af90: 0d0a 0d0a 2020 2020 2020 2020 2323 2041  ....        ## A
+0001afa0: 5049 2052 6573 706f 6e73 650d 0a20 2020  PI Response..   
+0001afb0: 2020 2020 2060 6060 6a73 6f6e 0d0a 2020       ```json..  
+0001afc0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+0001afd0: 2020 2020 2022 7265 616c 7469 6d65 5f73       "realtime_s
+0001afe0: 7461 7274 223a 2022 3230 3133 2d30 382d  tart": "2013-08-
+0001aff0: 3134 222c 0d0a 2020 2020 2020 2020 2020  14",..          
+0001b000: 2020 2272 6561 6c74 696d 655f 656e 6422    "realtime_end"
+0001b010: 3a20 2232 3031 332d 3038 2d31 3422 2c0d  : "2013-08-14",.
+0001b020: 0a20 2020 2020 2020 2020 2020 2022 6f72  .            "or
+0001b030: 6465 725f 6279 223a 2022 7365 7269 6573  der_by": "series
+0001b040: 5f63 6f75 6e74 222c 0d0a 2020 2020 2020  _count",..      
+0001b050: 2020 2020 2020 2273 6f72 745f 6f72 6465        "sort_orde
+0001b060: 7222 3a20 2264 6573 6322 2c0d 0a20 2020  r": "desc",..   
+0001b070: 2020 2020 2020 2020 2022 636f 756e 7422           "count"
+0001b080: 3a20 3130 2c0d 0a20 2020 2020 2020 2020  : 10,..         
+0001b090: 2020 2022 6f66 6673 6574 223a 2030 2c0d     "offset": 0,.
+0001b0a0: 0a20 2020 2020 2020 2020 2020 2022 6c69  .            "li
+0001b0b0: 6d69 7422 3a20 3130 3030 2c0d 0a20 2020  mit": 1000,..   
+0001b0c0: 2020 2020 2020 2020 2022 7461 6773 223a           "tags":
+0001b0d0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+0001b0e0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
+0001b0f0: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+0001b100: 223a 2022 636f 6e76 656e 7469 6f6e 616c  ": "conventional
+0001b110: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0001b120: 2020 2020 2020 2020 2267 726f 7570 5f69          "group_i
+0001b130: 6422 3a20 2267 656e 222c 0d0a 2020 2020  d": "gen",..    
+0001b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b150: 226e 6f74 6573 223a 2022 222c 0d0a 2020  "notes": "",..  
+0001b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b170: 2020 2263 7265 6174 6564 223a 2022 3230    "created": "20
+0001b180: 3132 2d30 322d 3237 2031 303a 3138 3a31  12-02-27 10:18:1
+0001b190: 392d 3036 222c 0d0a 2020 2020 2020 2020  9-06",..        
+0001b1a0: 2020 2020 2020 2020 2020 2020 2270 6f70              "pop
+0001b1b0: 756c 6172 6974 7922 3a20 3633 2c0d 0a20  ularity": 63,.. 
+0001b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1d0: 2020 2022 7365 7269 6573 5f63 6f75 6e74     "series_count
+0001b1e0: 223a 2033 0d0a 2020 2020 2020 2020 2020  ": 3..          
+0001b1f0: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+0001b200: 2020 2020 2020 2020 2020 2e2e 2e0d 0a20            ..... 
+0001b210: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
+0001b220: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+0001b230: 2060 6060 0d0a 0d0a 2020 2020 2020 2020   ```....        
+0001b240: 2323 2052 6574 7572 6e73 0d0a 2020 2020  ## Returns..    
+0001b250: 2020 2020 6070 616e 6461 732e 4461 7461      `pandas.Data
+0001b260: 4672 616d 6560 0d0a 0d0a 2020 2020 2020  Frame`....      
+0001b270: 2020 2323 2045 7861 6d70 6c65 0d0a 2020    ## Example..  
+0001b280: 2020 2020 2020 6060 6070 7974 686f 6e0d        ```python.
+0001b290: 0a20 2020 2020 2020 203e 3e3e 2066 7265  .        >>> fre
+0001b2a0: 6420 3d20 4652 4544 2861 7069 5f6b 6579  d = FRED(api_key
+0001b2b0: 3d27 6162 6364 6566 6768 696a 6b6c 6d6e  ='abcdefghijklmn
+0001b2c0: 6f70 7172 7374 7576 7778 797a 3132 3334  opqrstuvwxyz1234
+0001b2d0: 3536 2729 0d0a 2020 2020 2020 2020 3e3e  56')..        >>
+0001b2e0: 3e20 6672 6564 2e73 6572 6965 735f 7365  > fred.series_se
+0001b2f0: 6172 6368 5f72 656c 6174 6564 5f74 6167  arch_related_tag
+0001b300: 7328 7365 7269 6573 5f73 6561 7263 685f  s(series_search_
+0001b310: 7465 7874 3d27 6d6f 7274 6761 6765 2072  text='mortgage r
+0001b320: 6174 6527 2c20 7461 675f 6e61 6d65 733d  ate', tag_names=
+0001b330: 5b27 3330 2d79 6561 7227 2c20 2766 7262  ['30-year', 'frb
+0001b340: 275d 2c20 7265 616c 7469 6d65 5f73 7461  '], realtime_sta
+0001b350: 7274 3d64 6174 6528 3230 3232 2c20 312c  rt=date(2022, 1,
+0001b360: 2035 292c 2072 6561 6c74 696d 655f 656e   5), realtime_en
+0001b370: 643d 6461 7465 2832 3032 322c 2031 2c20  d=date(2022, 1, 
+0001b380: 3529 292e 6865 6164 2829 0d0a 2020 2020  5)).head()..    
+0001b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3a0: 2020 2020 2020 6772 6f75 705f 6964 2020        group_id  
+0001b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3c0: 2020 2020 2020 206e 6f74 6573 2020 2020         notes    
+0001b3d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001b3e0: 7265 6174 6564 2020 706f 7075 6c61 7269  reated  populari
+0001b3f0: 7479 2020 7365 7269 6573 5f63 6f75 6e74  ty  series_count
+0001b400: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+0001b410: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
+0001b420: 636f 6e76 656e 7469 6f6e 616c 2020 2020  conventional    
+0001b430: 2020 2067 656e 2020 2020 2020 2020 2020     gen          
+0001b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b450: 2020 2020 2032 3031 322d 3032 2d32 3720       2012-02-27 
+0001b460: 3136 3a31 383a 3139 2b30 303a 3030 2020  16:18:19+00:00  
+0001b470: 2020 2020 2020 2020 3231 2020 2020 2020          21      
+0001b480: 2020 2020 2020 2032 0d0a 2020 2020 2020         2..      
+0001b490: 2020 2020 2020 6469 7363 6f6e 7469 6e75        discontinu
+0001b4a0: 6564 2020 2020 2020 2067 656e 2020 2020  ed       gen    
 0001b4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4c0: 2020 2020 2032 3031 322d 3032 2d32 3720       2012-02-27 
-0001b4d0: 3136 3a31 383a 3139 2b30 303a 3030 2020  16:18:19+00:00  
-0001b4e0: 2020 2020 2020 2020 3734 2020 2020 2020          74      
-0001b4f0: 2020 2020 2020 2032 0d0a 2020 2020 2020         2..      
-0001b500: 2020 2020 2020 696e 7465 7265 7374 2072        interest r
-0001b510: 6174 6520 2020 2020 2067 656e 2020 2020  ate      gen    
-0001b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b530: 2020 2020 2020 2020 2020 2032 3031 322d             2012-
-0001b540: 3035 2d32 3920 3135 3a31 343a 3139 2b30  05-29 15:14:19+0
-0001b550: 303a 3030 2020 2020 2020 2020 2020 3734  0:00          74
-0001b560: 2020 2020 2020 2020 2020 2020 2032 0d0a               2..
-0001b570: 2020 2020 2020 2020 2222 220d 0a0d 0a20          """.... 
-0001b580: 2020 2020 2020 2061 6c6c 6f77 6564 5f6f         allowed_o
-0001b590: 7264 6572 7320 3d20 5b0d 0a20 2020 2020  rders = [..     
-0001b5a0: 2020 2020 2020 2065 6e75 6d73 2e4f 7264         enums.Ord
-0001b5b0: 6572 4279 2e73 6572 6965 735f 636f 756e  erBy.series_coun
-0001b5c0: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
-0001b5d0: 656e 756d 732e 4f72 6465 7242 792e 706f  enums.OrderBy.po
-0001b5e0: 7075 6c61 7269 7479 2c0d 0a20 2020 2020  pularity,..     
-0001b5f0: 2020 2020 2020 2065 6e75 6d73 2e4f 7264         enums.Ord
-0001b600: 6572 4279 2e63 7265 6174 6564 2c0d 0a20  erBy.created,.. 
-0001b610: 2020 2020 2020 2020 2020 2065 6e75 6d73             enums
-0001b620: 2e4f 7264 6572 4279 2e6e 616d 652c 0d0a  .OrderBy.name,..
-0001b630: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-0001b640: 732e 4f72 6465 7242 792e 6772 6f75 705f  s.OrderBy.group_
-0001b650: 6964 2c0d 0a20 2020 2020 2020 205d 0d0a  id,..        ]..
-0001b660: 0d0a 2020 2020 2020 2020 6966 206f 7264  ..        if ord
-0001b670: 6572 5f62 7920 6e6f 7420 696e 2061 6c6c  er_by not in all
-0001b680: 6f77 6564 5f6f 7264 6572 733a 0d0a 2020  owed_orders:..  
-0001b690: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0001b6a0: 5661 6c75 6545 7272 6f72 2827 5661 7269  ValueError('Vari
-0001b6b0: 6162 6c65 206f 7264 6572 5f62 7920 287b  able order_by ({
-0001b6c0: 7d29 2069 7320 6e6f 7420 6f6e 6520 6f66  }) is not one of
-0001b6d0: 2074 6865 2076 616c 7565 733a 207b 7d27   the values: {}'
-0001b6e0: 2e66 6f72 6d61 7428 6f72 6465 725f 6279  .format(order_by
-0001b6f0: 2c20 272c 2027 2e6a 6f69 6e28 6d61 7028  , ', '.join(map(
-0001b700: 7374 722c 2061 6c6c 6f77 6564 5f6f 7264  str, allowed_ord
-0001b710: 6572 7329 2929 290d 0a0d 0a20 2020 2020  ers))))....     
-0001b720: 2020 2069 6620 7265 616c 7469 6d65 5f73     if realtime_s
-0001b730: 7461 7274 2069 7320 6e6f 7420 4e6f 6e65  tart is not None
-0001b740: 2061 6e64 2072 6561 6c74 696d 655f 7374   and realtime_st
-0001b750: 6172 7420 3c20 6461 7465 2831 3737 362c  art < date(1776,
-0001b760: 2037 2c20 3429 3a0d 0a20 2020 2020 2020   7, 4):..       
-0001b770: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0001b780: 4572 726f 7228 2756 6172 6961 626c 6520  Error('Variable 
-0001b790: 7265 616c 7469 6d65 5f73 7461 7274 2028  realtime_start (
-0001b7a0: 227b 7d22 2920 6973 2062 6566 6f72 6520  "{}") is before 
-0001b7b0: 6d69 6e20 6461 7465 2031 3737 362d 3037  min date 1776-07
-0001b7c0: 2d30 342e 272e 666f 726d 6174 2872 6561  -04.'.format(rea
-0001b7d0: 6c74 696d 655f 7374 6172 7429 290d 0a0d  ltime_start))...
-0001b7e0: 0a20 2020 2020 2020 2069 6620 7265 616c  .        if real
-0001b7f0: 7469 6d65 5f73 7461 7274 2069 7320 6e6f  time_start is no
-0001b800: 7420 4e6f 6e65 2061 6e64 2072 6561 6c74  t None and realt
-0001b810: 696d 655f 656e 6420 6973 206e 6f74 204e  ime_end is not N
-0001b820: 6f6e 6520 616e 6420 7265 616c 7469 6d65  one and realtime
-0001b830: 5f73 7461 7274 203e 2072 6561 6c74 696d  _start > realtim
-0001b840: 655f 656e 643a 0d0a 2020 2020 2020 2020  e_end:..        
-0001b850: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0001b860: 7272 6f72 2827 5468 6520 6461 7465 2073  rror('The date s
-0001b870: 6574 2062 7920 7661 7269 6162 6c65 2072  et by variable r
-0001b880: 6561 6c74 696d 655f 7374 6172 7420 2822  ealtime_start ("
-0001b890: 7b7d 2229 2063 616e 206e 6f74 2062 6520  {}") can not be 
-0001b8a0: 6166 7465 7220 7468 6520 6461 7465 2073  after the date s
-0001b8b0: 6574 2062 7920 7661 7269 6162 6c65 2072  et by variable r
-0001b8c0: 6561 6c74 696d 655f 656e 6420 2822 7b7d  ealtime_end ("{}
-0001b8d0: 2229 2e27 2e66 6f72 6d61 7428 7265 616c  ").'.format(real
-0001b8e0: 7469 6d65 5f73 7461 7274 2c20 7265 616c  time_start, real
-0001b8f0: 7469 6d65 5f65 6e64 2929 0d0a 0d0a 2020  time_end))....  
-0001b900: 2020 2020 2020 6466 203d 2070 642e 4461        df = pd.Da
-0001b910: 7461 4672 616d 6528 0d0a 2020 2020 2020  taFrame(..      
-0001b920: 2020 2020 2020 7365 6c66 2e5f 636c 6965        self._clie
-0001b930: 6e74 2e67 6574 280d 0a20 2020 2020 2020  nt.get(..       
-0001b940: 2020 2020 2020 2020 2027 2f66 7265 642f           '/fred/
-0001b950: 7365 7269 6573 2f73 6561 7263 682f 7265  series/search/re
-0001b960: 6c61 7465 645f 7461 6773 272c 0d0a 2020  lated_tags',..  
-0001b970: 2020 2020 2020 2020 2020 2020 2020 2774                't
-0001b980: 6167 7327 2c0d 0a20 2020 2020 2020 2020  ags',..         
-0001b990: 2020 2020 2020 206c 696d 6974 3d31 3030         limit=100
-0001b9a0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-0001b9b0: 2020 2020 7365 7269 6573 5f73 6561 7263      series_searc
-0001b9c0: 685f 7465 7874 3d73 6572 6965 735f 7365  h_text=series_se
-0001b9d0: 6172 6368 5f74 6578 742c 0d0a 2020 2020  arch_text,..    
-0001b9e0: 2020 2020 2020 2020 2020 2020 7265 616c              real
-0001b9f0: 7469 6d65 5f73 7461 7274 3d72 6561 6c74  time_start=realt
-0001ba00: 696d 655f 7374 6172 742c 0d0a 2020 2020  ime_start,..    
-0001ba10: 2020 2020 2020 2020 2020 2020 7265 616c              real
-0001ba20: 7469 6d65 5f65 6e64 3d72 6561 6c74 696d  time_end=realtim
-0001ba30: 655f 656e 642c 0d0a 2020 2020 2020 2020  e_end,..        
-0001ba40: 2020 2020 2020 2020 7461 675f 6e61 6d65          tag_name
-0001ba50: 733d 7461 675f 6e61 6d65 732c 0d0a 2020  s=tag_names,..  
-0001ba60: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-0001ba70: 636c 7564 655f 7461 675f 6e61 6d65 733d  clude_tag_names=
-0001ba80: 6578 636c 7564 655f 7461 675f 6e61 6d65  exclude_tag_name
-0001ba90: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-0001baa0: 2020 2020 7461 675f 6772 6f75 705f 6964      tag_group_id
-0001bab0: 3d74 6167 5f67 726f 7570 5f69 642c 0d0a  =tag_group_id,..
-0001bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bad0: 7461 675f 7365 6172 6368 5f74 6578 743d  tag_search_text=
-0001bae0: 7461 675f 7365 6172 6368 5f74 6578 742c  tag_search_text,
-0001baf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001bb00: 2020 6f72 6465 725f 6279 3d6f 7264 6572    order_by=order
-0001bb10: 5f62 792c 0d0a 2020 2020 2020 2020 2020  _by,..          
-0001bb20: 2020 2020 2020 736f 7274 5f6f 7264 6572        sort_order
-0001bb30: 3d73 6f72 745f 6f72 6465 720d 0a20 2020  =sort_order..   
-0001bb40: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0001bb50: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
-0001bb60: 2069 6620 6e6f 7420 6466 2e65 6d70 7479   if not df.empty
-0001bb70: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-0001bb80: 662e 6372 6561 7465 6420 3d20 7064 2e74  f.created = pd.t
-0001bb90: 6f5f 6461 7465 7469 6d65 2864 662e 6372  o_datetime(df.cr
-0001bba0: 6561 7465 6420 2b20 2730 3027 2c20 7574  eated + '00', ut
-0001bbb0: 633d 5472 7565 2c20 666f 726d 6174 3d27  c=True, format='
-0001bbc0: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
-0001bbd0: 5325 7a27 290d 0a0d 0a20 2020 2020 2020  S%z')....       
-0001bbe0: 2020 2020 2064 6620 3d20 6466 2e61 7374       df = df.ast
-0001bbf0: 7970 6528 6474 7970 653d 7b0d 0a20 2020  ype(dtype={..   
-0001bc00: 2020 2020 2020 2020 2020 2020 2027 6e61               'na
-0001bc10: 6d65 273a 2027 7374 7269 6e67 272c 0d0a  me': 'string',..
-0001bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc30: 276e 6f74 6573 273a 2027 7374 7269 6e67  'notes': 'string
-0001bc40: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-0001bc50: 2020 2020 2767 726f 7570 5f69 6427 3a20      'group_id': 
-0001bc60: 2763 6174 6567 6f72 7927 0d0a 2020 2020  'category'..    
-0001bc70: 2020 2020 2020 2020 7d29 2e73 6574 5f69          }).set_i
-0001bc80: 6e64 6578 2827 6e61 6d65 2729 0d0a 0d0a  ndex('name')....
-0001bc90: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-0001bca0: 660d 0a0d 0a20 2020 2064 6566 2073 6572  f....    def ser
-0001bcb0: 6965 735f 7461 6773 280d 0a20 2020 2020  ies_tags(..     
-0001bcc0: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-0001bcd0: 2020 2020 2020 2020 2020 7365 7269 6573            series
-0001bce0: 5f69 643a 2073 7472 2c0d 0a20 2020 2020  _id: str,..     
-0001bcf0: 2020 2020 2020 2072 6561 6c74 696d 655f         realtime_
-0001bd00: 7374 6172 743a 2064 6174 6520 3d20 4e6f  start: date = No
-0001bd10: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-0001bd20: 2072 6561 6c74 696d 655f 656e 643a 2064   realtime_end: d
-0001bd30: 6174 6520 3d20 4e6f 6e65 2c0d 0a20 2020  ate = None,..   
-0001bd40: 2020 2020 2020 2020 206f 7264 6572 5f62           order_b
-0001bd50: 793a 2065 6e75 6d73 2e4f 7264 6572 4279  y: enums.OrderBy
-0001bd60: 203d 2065 6e75 6d73 2e4f 7264 6572 4279   = enums.OrderBy
-0001bd70: 2e73 6572 6965 735f 636f 756e 742c 0d0a  .series_count,..
-0001bd80: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-0001bd90: 5f6f 7264 6572 3a20 656e 756d 732e 536f  _order: enums.So
-0001bda0: 7274 4f72 6465 7220 3d20 656e 756d 732e  rtOrder = enums.
-0001bdb0: 536f 7274 4f72 6465 722e 6173 630d 0a20  SortOrder.asc.. 
-0001bdc0: 2020 2029 202d 3e20 7064 2e44 6174 6146     ) -> pd.DataF
-0001bdd0: 7261 6d65 3a0d 0a20 2020 2020 2020 2022  rame:..        "
-0001bde0: 2222 0d0a 2020 2020 2020 2020 2323 2050  ""..        ## P
-0001bdf0: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-0001be00: 2020 2060 7365 7269 6573 5f69 6460 0d0a     `series_id`..
-0001be10: 2020 2020 2020 2020 5468 6520 6964 2066          The id f
-0001be20: 6f72 2061 2073 6572 6965 732e 0d0a 0d0a  or a series.....
-0001be30: 2020 2020 2020 2020 6072 6561 6c74 696d          `realtim
-0001be40: 655f 7374 6172 7460 0d0a 2020 2020 2020  e_start`..      
-0001be50: 2020 5468 6520 7374 6172 7420 6f66 2074    The start of t
-0001be60: 6865 2072 6561 6c2d 7469 6d65 2070 6572  he real-time per
-0001be70: 696f 642e 2046 6f72 206d 6f72 6520 696e  iod. For more in
-0001be80: 666f 726d 6174 696f 6e2c 2073 6565 205b  formation, see [
-0001be90: 5265 616c 2d54 696d 6520 5065 7269 6f64  Real-Time Period
-0001bea0: 735d 2868 7474 7073 3a2f 2f66 7265 642e  s](https://fred.
-0001beb0: 7374 6c6f 7569 7366 6564 2e6f 7267 2f64  stlouisfed.org/d
-0001bec0: 6f63 732f 6170 692f 6672 6564 2f72 6561  ocs/api/fred/rea
-0001bed0: 6c74 696d 655f 7065 7269 6f64 2e68 746d  ltime_period.htm
-0001bee0: 6c29 2e0d 0a0d 0a20 2020 2020 2020 2060  l).....        `
-0001bef0: 7265 616c 7469 6d65 5f65 6e64 600d 0a20  realtime_end`.. 
-0001bf00: 2020 2020 2020 2054 6865 2065 6e64 206f         The end o
-0001bf10: 6620 7468 6520 7265 616c 2d74 696d 6520  f the real-time 
-0001bf20: 7065 7269 6f64 2e20 466f 7220 6d6f 7265  period. For more
-0001bf30: 2069 6e66 6f72 6d61 7469 6f6e 2c20 7365   information, se
-0001bf40: 6520 5b52 6561 6c2d 5469 6d65 2050 6572  e [Real-Time Per
-0001bf50: 696f 6473 5d28 6874 7470 733a 2f2f 6672  iods](https://fr
-0001bf60: 6564 2e73 746c 6f75 6973 6665 642e 6f72  ed.stlouisfed.or
-0001bf70: 672f 646f 6373 2f61 7069 2f66 7265 642f  g/docs/api/fred/
-0001bf80: 7265 616c 7469 6d65 5f70 6572 696f 642e  realtime_period.
-0001bf90: 6874 6d6c 292e 0d0a 0d0a 2020 2020 2020  html).....      
-0001bfa0: 2020 606f 7264 6572 5f62 7960 0d0a 2020    `order_by`..  
-0001bfb0: 2020 2020 2020 4f72 6465 7220 7265 7375        Order resu
-0001bfc0: 6c74 7320 6279 2076 616c 7565 7320 6f66  lts by values of
-0001bfd0: 2074 6865 2073 7065 6369 6669 6564 2061   the specified a
-0001bfe0: 7474 7269 6275 7465 2e0d 0a0d 0a20 2020  ttribute.....   
-0001bff0: 2020 2020 2060 736f 7274 5f6f 7264 6572       `sort_order
-0001c000: 600d 0a20 2020 2020 2020 2053 6f72 7420  `..        Sort 
-0001c010: 7265 7375 6c74 7320 6973 2061 7363 656e  results is ascen
-0001c020: 6469 6e67 206f 7220 6465 7363 656e 6469  ding or descendi
-0001c030: 6e67 206f 7264 6572 2066 6f72 2061 7474  ng order for att
-0001c040: 7269 6275 7465 2076 616c 7565 7320 7370  ribute values sp
-0001c050: 6563 6966 6965 6420 6279 206f 7264 6572  ecified by order
-0001c060: 5f62 792e 0d0a 0d0a 2020 2020 2020 2020  _by.....        
-0001c070: 2323 2044 6573 6372 6970 7469 6f6e 0d0a  ## Description..
-0001c080: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-0001c090: 6672 6564 2e73 746c 6f75 6973 6665 642e  fred.stlouisfed.
-0001c0a0: 6f72 672f 646f 6373 2f61 7069 2f66 7265  org/docs/api/fre
-0001c0b0: 642f 7365 7269 6573 5f74 6167 732e 6874  d/series_tags.ht
-0001c0c0: 6d6c 0d0a 0d0a 2020 2020 2020 2020 4765  ml....        Ge
-0001c0d0: 7420 7468 6520 4652 4544 2074 6167 7320  t the FRED tags 
-0001c0e0: 666f 7220 6120 7365 7269 6573 2e0d 0a0d  for a series....
-0001c0f0: 0a20 2020 2020 2020 2023 2320 4150 4920  .        ## API 
-0001c100: 5265 7175 6573 7420 2848 5454 5053 2047  Request (HTTPS G
-0001c110: 4554 290d 0a20 2020 2020 2020 2068 7474  ET)..        htt
-0001c120: 7073 3a2f 2f61 7069 2e73 746c 6f75 6973  ps://api.stlouis
-0001c130: 6665 642e 6f72 672f 6672 6564 2f73 6572  fed.org/fred/ser
-0001c140: 6965 732f 7461 6773 3f73 6572 6965 735f  ies/tags?series_
-0001c150: 6964 3d53 544c 4653 4926 6170 695f 6b65  id=STLFSI&api_ke
-0001c160: 793d 6162 6364 6566 6768 696a 6b6c 6d6e  y=abcdefghijklmn
-0001c170: 6f70 7172 7374 7576 7778 797a 3132 3334  opqrstuvwxyz1234
-0001c180: 3536 2666 696c 655f 7479 7065 3d6a 736f  56&file_type=jso
-0001c190: 6e0d 0a0d 0a20 2020 2020 2020 2023 2320  n....        ## 
-0001c1a0: 4150 4920 5265 7370 6f6e 7365 0d0a 2020  API Response..  
-0001c1b0: 2020 2020 2020 6060 606a 736f 6e0d 0a20        ```json.. 
-0001c1c0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-0001c1d0: 2020 2020 2020 2272 6561 6c74 696d 655f        "realtime_
-0001c1e0: 7374 6172 7422 3a20 2232 3031 332d 3038  start": "2013-08
-0001c1f0: 2d31 3422 2c0d 0a20 2020 2020 2020 2020  -14",..         
-0001c200: 2020 2022 7265 616c 7469 6d65 5f65 6e64     "realtime_end
-0001c210: 223a 2022 3230 3133 2d30 382d 3134 222c  ": "2013-08-14",
-0001c220: 0d0a 2020 2020 2020 2020 2020 2020 226f  ..            "o
-0001c230: 7264 6572 5f62 7922 3a20 2273 6572 6965  rder_by": "serie
-0001c240: 735f 636f 756e 7422 2c0d 0a20 2020 2020  s_count",..     
-0001c250: 2020 2020 2020 2022 736f 7274 5f6f 7264         "sort_ord
-0001c260: 6572 223a 2022 6465 7363 222c 0d0a 2020  er": "desc",..  
-0001c270: 2020 2020 2020 2020 2020 2263 6f75 6e74            "count
-0001c280: 223a 2038 2c0d 0a20 2020 2020 2020 2020  ": 8,..         
-0001c290: 2020 2022 6f66 6673 6574 223a 2030 2c0d     "offset": 0,.
-0001c2a0: 0a20 2020 2020 2020 2020 2020 2022 6c69  .            "li
-0001c2b0: 6d69 7422 3a20 3130 3030 2c0d 0a20 2020  mit": 1000,..   
-0001c2c0: 2020 2020 2020 2020 2022 7461 6773 223a           "tags":
-0001c2d0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-0001c2e0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-0001c2f0: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
-0001c300: 223a 2022 6e61 7469 6f6e 222c 0d0a 2020  ": "nation",..  
-0001c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c320: 2020 2267 726f 7570 5f69 6422 3a20 2267    "group_id": "g
-0001c330: 656f 7422 2c0d 0a20 2020 2020 2020 2020  eot",..         
-0001c340: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
-0001c350: 7322 3a20 2243 6f75 6e74 7279 204c 6576  s": "Country Lev
-0001c360: 656c 222c 0d0a 2020 2020 2020 2020 2020  el",..          
-0001c370: 2020 2020 2020 2020 2020 2263 7265 6174            "creat
-0001c380: 6564 223a 2022 3230 3132 2d30 322d 3237  ed": "2012-02-27
-0001c390: 2031 303a 3138 3a31 392d 3036 222c 0d0a   10:18:19-06",..
-0001c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3b0: 2020 2020 2270 6f70 756c 6172 6974 7922      "popularity"
-0001c3c0: 3a20 3130 302c 0d0a 2020 2020 2020 2020  : 100,..        
-0001c3d0: 2020 2020 2020 2020 2020 2020 2273 6572              "ser
-0001c3e0: 6965 735f 636f 756e 7422 3a20 3130 3532  ies_count": 1052
-0001c3f0: 3030 0d0a 2020 2020 2020 2020 2020 2020  00..            
-0001c400: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-0001c410: 2020 2020 2020 2020 2e2e 2e0d 0a20 2020          .....   
-0001c420: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
-0001c430: 2020 2020 7d0d 0a20 2020 2020 2020 2060      }..        `
-0001c440: 6060 0d0a 0d0a 2020 2020 2020 2020 2323  ``....        ##
-0001c450: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-0001c460: 2020 6070 616e 6461 732e 4461 7461 4672    `pandas.DataFr
-0001c470: 616d 6560 0d0a 0d0a 2020 2020 2020 2020  ame`....        
-0001c480: 2323 2045 7861 6d70 6c65 0d0a 2020 2020  ## Example..    
-0001c490: 2020 2020 6060 6070 7974 686f 6e0d 0a20      ```python.. 
-0001c4a0: 2020 2020 2020 203e 3e3e 2066 7265 6420         >>> fred 
-0001c4b0: 3d20 4652 4544 2861 7069 5f6b 6579 3d27  = FRED(api_key='
-0001c4c0: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
-0001c4d0: 7172 7374 7576 7778 797a 3132 3334 3536  qrstuvwxyz123456
-0001c4e0: 2729 0d0a 2020 2020 2020 2020 3e3e 3e20  ')..        >>> 
-0001c4f0: 6672 6564 2e73 6572 6965 735f 7461 6773  fred.series_tags
-0001c500: 2873 6572 6965 735f 6964 3d27 5354 4c46  (series_id='STLF
-0001c510: 5349 2729 2e68 6561 6428 290d 0a20 2020  SI').head()..   
-0001c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c530: 2020 2020 2020 6772 6f75 705f 6964 2020        group_id  
-0001c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c550: 2020 2020 2020 2020 2020 206e 6f74 6573             notes
-0001c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c570: 2020 2063 7265 6174 6564 2020 706f 7075     created  popu
-0001c580: 6c61 7269 7479 2020 7365 7269 6573 5f63  larity  series_c
-0001c590: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
-0001c5a0: 2020 6e61 6d65 0d0a 2020 2020 2020 2020    name..        
-0001c5b0: 2020 2020 7374 6c66 7369 2020 2020 2020      stlfsi      
-0001c5c0: 2020 2020 2020 726c 7320 2053 742e 204c        rls  St. L
-0001c5d0: 6f75 6973 2046 696e 616e 6369 616c 2053  ouis Financial S
-0001c5e0: 7472 6573 7320 496e 6465 7820 3230 3132  tress Index 2012
-0001c5f0: 2d30 382d 3136 2032 303a 3231 3a31 372b  -08-16 20:21:17+
-0001c600: 3030 3a30 3020 2020 2020 2020 2020 2031  00:00          1
-0001c610: 3920 2020 2020 2020 2020 2020 2020 340d  9             4.
-0001c620: 0a20 2020 2020 2020 2020 2020 2066 7369  .            fsi
-0001c630: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-0001c640: 656e 2020 2020 2020 2020 2020 2020 4669  en            Fi
-0001c650: 6e61 6e63 6961 6c20 5374 7265 7373 2049  nancial Stress I
-0001c660: 6e64 6578 2032 3031 342d 3038 2d30 3820  ndex 2014-08-08 
-0001c670: 3139 3a30 313a 3337 2b30 303a 3030 2020  19:01:37+00:00  
-0001c680: 2020 2020 2020 2020 3236 2020 2020 2020          26      
-0001c690: 2020 2020 2020 3236 0d0a 2020 2020 2020        26..      
-0001c6a0: 2020 2020 2020 7765 656b 6c79 2020 2020        weekly    
-0001c6b0: 2020 2020 2020 2066 7265 7120 2020 2020         freq     
-0001c6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6d0: 2020 2020 2020 2020 2020 2020 2020 3230                20
-0001c6e0: 3132 2d30 322d 3237 2031 363a 3138 3a31  12-02-27 16:18:1
-0001c6f0: 392b 3030 3a30 3020 2020 2020 2020 2020  9+00:00         
-0001c700: 2036 3820 2020 2020 2020 2020 2033 3534   68          354
-0001c710: 380d 0a20 2020 2020 2020 2020 2020 2066  8..            f
-0001c720: 696e 616e 6369 616c 2020 2020 2020 2020  inancial        
+0001b4c0: 2020 2020 2020 2020 2020 2032 3031 322d             2012-
+0001b4d0: 3032 2d32 3720 3136 3a31 383a 3139 2b30  02-27 16:18:19+0
+0001b4e0: 303a 3030 2020 2020 2020 2020 2020 3637  0:00          67
+0001b4f0: 2020 2020 2020 2020 2020 2020 2032 0d0a               2..
+0001b500: 2020 2020 2020 2020 2020 2020 6831 3520              h15 
+0001b510: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001b520: 6c73 2020 482e 3135 2053 656c 6563 7465  ls  H.15 Selecte
+0001b530: 6420 496e 7465 7265 7374 2052 6174 6573  d Interest Rates
+0001b540: 2032 3031 322d 3038 2d31 3620 3230 3a32   2012-08-16 20:2
+0001b550: 313a 3137 2b30 303a 3030 2020 2020 2020  1:17+00:00      
+0001b560: 2020 2020 3537 2020 2020 2020 2020 2020      57          
+0001b570: 2020 2032 0d0a 2020 2020 2020 2020 2020     2..          
+0001b580: 2020 696e 7465 7265 7374 2020 2020 2020    interest      
+0001b590: 2020 2020 2067 656e 2020 2020 2020 2020       gen        
+0001b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b5b0: 2020 2020 2020 2032 3031 322d 3032 2d32         2012-02-2
+0001b5c0: 3720 3136 3a31 383a 3139 2b30 303a 3030  7 16:18:19+00:00
+0001b5d0: 2020 2020 2020 2020 2020 3734 2020 2020            74    
+0001b5e0: 2020 2020 2020 2020 2032 0d0a 2020 2020           2..    
+0001b5f0: 2020 2020 2020 2020 696e 7465 7265 7374          interest
+0001b600: 2072 6174 6520 2020 2020 2067 656e 2020   rate      gen  
+0001b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b620: 2020 2020 2020 2020 2020 2020 2032 3031               201
+0001b630: 322d 3035 2d32 3920 3135 3a31 343a 3139  2-05-29 15:14:19
+0001b640: 2b30 303a 3030 2020 2020 2020 2020 2020  +00:00          
+0001b650: 3734 2020 2020 2020 2020 2020 2020 2032  74             2
+0001b660: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
+0001b670: 0a20 2020 2020 2020 2061 6c6c 6f77 6564  .        allowed
+0001b680: 5f6f 7264 6572 7320 3d20 5b0d 0a20 2020  _orders = [..   
+0001b690: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
+0001b6a0: 7264 6572 4279 2e73 6572 6965 735f 636f  rderBy.series_co
+0001b6b0: 756e 742c 0d0a 2020 2020 2020 2020 2020  unt,..          
+0001b6c0: 2020 656e 756d 732e 4f72 6465 7242 792e    enums.OrderBy.
+0001b6d0: 706f 7075 6c61 7269 7479 2c0d 0a20 2020  popularity,..   
+0001b6e0: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
+0001b6f0: 7264 6572 4279 2e63 7265 6174 6564 2c0d  rderBy.created,.
+0001b700: 0a20 2020 2020 2020 2020 2020 2065 6e75  .            enu
+0001b710: 6d73 2e4f 7264 6572 4279 2e6e 616d 652c  ms.OrderBy.name,
+0001b720: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+0001b730: 756d 732e 4f72 6465 7242 792e 6772 6f75  ums.OrderBy.grou
+0001b740: 705f 6964 2c0d 0a20 2020 2020 2020 205d  p_id,..        ]
+0001b750: 0d0a 0d0a 2020 2020 2020 2020 6966 206f  ....        if o
+0001b760: 7264 6572 5f62 7920 6e6f 7420 696e 2061  rder_by not in a
+0001b770: 6c6c 6f77 6564 5f6f 7264 6572 733a 0d0a  llowed_orders:..
+0001b780: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0001b790: 6520 5661 6c75 6545 7272 6f72 2827 5661  e ValueError('Va
+0001b7a0: 7269 6162 6c65 206f 7264 6572 5f62 7920  riable order_by 
+0001b7b0: 287b 7d29 2069 7320 6e6f 7420 6f6e 6520  ({}) is not one 
+0001b7c0: 6f66 2074 6865 2076 616c 7565 733a 207b  of the values: {
+0001b7d0: 7d27 2e66 6f72 6d61 7428 6f72 6465 725f  }'.format(order_
+0001b7e0: 6279 2c20 272c 2027 2e6a 6f69 6e28 6d61  by, ', '.join(ma
+0001b7f0: 7028 7374 722c 2061 6c6c 6f77 6564 5f6f  p(str, allowed_o
+0001b800: 7264 6572 7329 2929 290d 0a0d 0a20 2020  rders))))....   
+0001b810: 2020 2020 2069 6620 7265 616c 7469 6d65       if realtime
+0001b820: 5f73 7461 7274 2069 7320 6e6f 7420 4e6f  _start is not No
+0001b830: 6e65 2061 6e64 2072 6561 6c74 696d 655f  ne and realtime_
+0001b840: 7374 6172 7420 3c20 6461 7465 2831 3737  start < date(177
+0001b850: 362c 2037 2c20 3429 3a0d 0a20 2020 2020  6, 7, 4):..     
+0001b860: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0001b870: 7565 4572 726f 7228 2756 6172 6961 626c  ueError('Variabl
+0001b880: 6520 7265 616c 7469 6d65 5f73 7461 7274  e realtime_start
+0001b890: 2028 227b 7d22 2920 6973 2062 6566 6f72   ("{}") is befor
+0001b8a0: 6520 6d69 6e20 6461 7465 2031 3737 362d  e min date 1776-
+0001b8b0: 3037 2d30 342e 272e 666f 726d 6174 2872  07-04.'.format(r
+0001b8c0: 6561 6c74 696d 655f 7374 6172 7429 290d  ealtime_start)).
+0001b8d0: 0a0d 0a20 2020 2020 2020 2069 6620 7265  ...        if re
+0001b8e0: 616c 7469 6d65 5f73 7461 7274 2069 7320  altime_start is 
+0001b8f0: 6e6f 7420 4e6f 6e65 2061 6e64 2072 6561  not None and rea
+0001b900: 6c74 696d 655f 656e 6420 6973 206e 6f74  ltime_end is not
+0001b910: 204e 6f6e 6520 616e 6420 7265 616c 7469   None and realti
+0001b920: 6d65 5f73 7461 7274 203e 2072 6561 6c74  me_start > realt
+0001b930: 696d 655f 656e 643a 0d0a 2020 2020 2020  ime_end:..      
+0001b940: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0001b950: 6545 7272 6f72 2827 5468 6520 6461 7465  eError('The date
+0001b960: 2073 6574 2062 7920 7661 7269 6162 6c65   set by variable
+0001b970: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
+0001b980: 2822 7b7d 2229 2063 616e 206e 6f74 2062  ("{}") can not b
+0001b990: 6520 6166 7465 7220 7468 6520 6461 7465  e after the date
+0001b9a0: 2073 6574 2062 7920 7661 7269 6162 6c65   set by variable
+0001b9b0: 2072 6561 6c74 696d 655f 656e 6420 2822   realtime_end ("
+0001b9c0: 7b7d 2229 2e27 2e66 6f72 6d61 7428 7265  {}").'.format(re
+0001b9d0: 616c 7469 6d65 5f73 7461 7274 2c20 7265  altime_start, re
+0001b9e0: 616c 7469 6d65 5f65 6e64 2929 0d0a 0d0a  altime_end))....
+0001b9f0: 2020 2020 2020 2020 6466 203d 2070 642e          df = pd.
+0001ba00: 4461 7461 4672 616d 6528 0d0a 2020 2020  DataFrame(..    
+0001ba10: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+0001ba20: 6965 6e74 2e67 6574 280d 0a20 2020 2020  ient.get(..     
+0001ba30: 2020 2020 2020 2020 2020 2027 2f66 7265             '/fre
+0001ba40: 642f 7365 7269 6573 2f73 6561 7263 682f  d/series/search/
+0001ba50: 7265 6c61 7465 645f 7461 6773 272c 0d0a  related_tags',..
+0001ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba70: 2774 6167 7327 2c0d 0a20 2020 2020 2020  'tags',..       
+0001ba80: 2020 2020 2020 2020 206c 696d 6974 3d31           limit=1
+0001ba90: 3030 302c 0d0a 2020 2020 2020 2020 2020  000,..          
+0001baa0: 2020 2020 2020 7365 7269 6573 5f73 6561        series_sea
+0001bab0: 7263 685f 7465 7874 3d73 6572 6965 735f  rch_text=series_
+0001bac0: 7365 6172 6368 5f74 6578 742c 0d0a 2020  search_text,..  
+0001bad0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001bae0: 616c 7469 6d65 5f73 7461 7274 3d72 6561  altime_start=rea
+0001baf0: 6c74 696d 655f 7374 6172 742c 0d0a 2020  ltime_start,..  
+0001bb00: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001bb10: 616c 7469 6d65 5f65 6e64 3d72 6561 6c74  altime_end=realt
+0001bb20: 696d 655f 656e 642c 0d0a 2020 2020 2020  ime_end,..      
+0001bb30: 2020 2020 2020 2020 2020 7461 675f 6e61            tag_na
+0001bb40: 6d65 733d 7461 675f 6e61 6d65 732c 0d0a  mes=tag_names,..
+0001bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb60: 6578 636c 7564 655f 7461 675f 6e61 6d65  exclude_tag_name
+0001bb70: 733d 6578 636c 7564 655f 7461 675f 6e61  s=exclude_tag_na
+0001bb80: 6d65 732c 0d0a 2020 2020 2020 2020 2020  mes,..          
+0001bb90: 2020 2020 2020 7461 675f 6772 6f75 705f        tag_group_
+0001bba0: 6964 3d74 6167 5f67 726f 7570 5f69 642c  id=tag_group_id,
+0001bbb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bbc0: 2020 7461 675f 7365 6172 6368 5f74 6578    tag_search_tex
+0001bbd0: 743d 7461 675f 7365 6172 6368 5f74 6578  t=tag_search_tex
+0001bbe0: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
+0001bbf0: 2020 2020 6f72 6465 725f 6279 3d6f 7264      order_by=ord
+0001bc00: 6572 5f62 792c 0d0a 2020 2020 2020 2020  er_by,..        
+0001bc10: 2020 2020 2020 2020 736f 7274 5f6f 7264          sort_ord
+0001bc20: 6572 3d73 6f72 745f 6f72 6465 720d 0a20  er=sort_order.. 
+0001bc30: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+0001bc40: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+0001bc50: 2020 2069 6620 6e6f 7420 6466 2e65 6d70     if not df.emp
+0001bc60: 7479 3a0d 0a20 2020 2020 2020 2020 2020  ty:..           
+0001bc70: 2064 662e 6372 6561 7465 6420 3d20 7064   df.created = pd
+0001bc80: 2e74 6f5f 6461 7465 7469 6d65 2864 662e  .to_datetime(df.
+0001bc90: 6372 6561 7465 6420 2b20 2730 3027 2c20  created + '00', 
+0001bca0: 7574 633d 5472 7565 2c20 666f 726d 6174  utc=True, format
+0001bcb0: 3d27 2559 2d25 6d2d 2564 2025 483a 254d  ='%Y-%m-%d %H:%M
+0001bcc0: 3a25 5325 7a27 290d 0a0d 0a20 2020 2020  :%S%z')....     
+0001bcd0: 2020 2020 2020 2064 6620 3d20 6466 2e61         df = df.a
+0001bce0: 7374 7970 6528 6474 7970 653d 7b0d 0a20  stype(dtype={.. 
+0001bcf0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001bd00: 6e61 6d65 273a 2027 7374 7269 6e67 272c  name': 'string',
+0001bd10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bd20: 2020 276e 6f74 6573 273a 2027 7374 7269    'notes': 'stri
+0001bd30: 6e67 272c 0d0a 2020 2020 2020 2020 2020  ng',..          
+0001bd40: 2020 2020 2020 2767 726f 7570 5f69 6427        'group_id'
+0001bd50: 3a20 2763 6174 6567 6f72 7927 0d0a 2020  : 'category'..  
+0001bd60: 2020 2020 2020 2020 2020 7d29 2e73 6574            }).set
+0001bd70: 5f69 6e64 6578 2827 6e61 6d65 2729 0d0a  _index('name')..
+0001bd80: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001bd90: 2064 660d 0a0d 0a20 2020 2064 6566 2073   df....    def s
+0001bda0: 6572 6965 735f 7461 6773 280d 0a20 2020  eries_tags(..   
+0001bdb0: 2020 2020 2020 2020 2073 656c 662c 0d0a           self,..
+0001bdc0: 2020 2020 2020 2020 2020 2020 7365 7269              seri
+0001bdd0: 6573 5f69 643a 2073 7472 2c0d 0a20 2020  es_id: str,..   
+0001bde0: 2020 2020 2020 2020 2072 6561 6c74 696d           realtim
+0001bdf0: 655f 7374 6172 743a 2064 6174 6520 3d20  e_start: date = 
+0001be00: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+0001be10: 2020 2072 6561 6c74 696d 655f 656e 643a     realtime_end:
+0001be20: 2064 6174 6520 3d20 4e6f 6e65 2c0d 0a20   date = None,.. 
+0001be30: 2020 2020 2020 2020 2020 206f 7264 6572             order
+0001be40: 5f62 793a 2065 6e75 6d73 2e4f 7264 6572  _by: enums.Order
+0001be50: 4279 203d 2065 6e75 6d73 2e4f 7264 6572  By = enums.Order
+0001be60: 4279 2e73 6572 6965 735f 636f 756e 742c  By.series_count,
+0001be70: 0d0a 2020 2020 2020 2020 2020 2020 736f  ..            so
+0001be80: 7274 5f6f 7264 6572 3a20 656e 756d 732e  rt_order: enums.
+0001be90: 536f 7274 4f72 6465 7220 3d20 656e 756d  SortOrder = enum
+0001bea0: 732e 536f 7274 4f72 6465 722e 6173 630d  s.SortOrder.asc.
+0001beb0: 0a20 2020 2029 202d 3e20 7064 2e44 6174  .    ) -> pd.Dat
+0001bec0: 6146 7261 6d65 3a0d 0a20 2020 2020 2020  aFrame:..       
+0001bed0: 2022 2222 0d0a 2020 2020 2020 2020 2323   """..        ##
+0001bee0: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+0001bef0: 2020 2020 2060 7365 7269 6573 5f69 6460       `series_id`
+0001bf00: 0d0a 2020 2020 2020 2020 5468 6520 6964  ..        The id
+0001bf10: 2066 6f72 2061 2073 6572 6965 732e 0d0a   for a series...
+0001bf20: 0d0a 2020 2020 2020 2020 6072 6561 6c74  ..        `realt
+0001bf30: 696d 655f 7374 6172 7460 0d0a 2020 2020  ime_start`..    
+0001bf40: 2020 2020 5468 6520 7374 6172 7420 6f66      The start of
+0001bf50: 2074 6865 2072 6561 6c2d 7469 6d65 2070   the real-time p
+0001bf60: 6572 696f 642e 2046 6f72 206d 6f72 6520  eriod. For more 
+0001bf70: 696e 666f 726d 6174 696f 6e2c 2073 6565  information, see
+0001bf80: 205b 5265 616c 2d54 696d 6520 5065 7269   [Real-Time Peri
+0001bf90: 6f64 735d 2868 7474 7073 3a2f 2f66 7265  ods](https://fre
+0001bfa0: 642e 7374 6c6f 7569 7366 6564 2e6f 7267  d.stlouisfed.org
+0001bfb0: 2f64 6f63 732f 6170 692f 6672 6564 2f72  /docs/api/fred/r
+0001bfc0: 6561 6c74 696d 655f 7065 7269 6f64 2e68  ealtime_period.h
+0001bfd0: 746d 6c29 2e0d 0a0d 0a20 2020 2020 2020  tml).....       
+0001bfe0: 2060 7265 616c 7469 6d65 5f65 6e64 600d   `realtime_end`.
+0001bff0: 0a20 2020 2020 2020 2054 6865 2065 6e64  .        The end
+0001c000: 206f 6620 7468 6520 7265 616c 2d74 696d   of the real-tim
+0001c010: 6520 7065 7269 6f64 2e20 466f 7220 6d6f  e period. For mo
+0001c020: 7265 2069 6e66 6f72 6d61 7469 6f6e 2c20  re information, 
+0001c030: 7365 6520 5b52 6561 6c2d 5469 6d65 2050  see [Real-Time P
+0001c040: 6572 696f 6473 5d28 6874 7470 733a 2f2f  eriods](https://
+0001c050: 6672 6564 2e73 746c 6f75 6973 6665 642e  fred.stlouisfed.
+0001c060: 6f72 672f 646f 6373 2f61 7069 2f66 7265  org/docs/api/fre
+0001c070: 642f 7265 616c 7469 6d65 5f70 6572 696f  d/realtime_perio
+0001c080: 642e 6874 6d6c 292e 0d0a 0d0a 2020 2020  d.html).....    
+0001c090: 2020 2020 606f 7264 6572 5f62 7960 0d0a      `order_by`..
+0001c0a0: 2020 2020 2020 2020 4f72 6465 7220 7265          Order re
+0001c0b0: 7375 6c74 7320 6279 2076 616c 7565 7320  sults by values 
+0001c0c0: 6f66 2074 6865 2073 7065 6369 6669 6564  of the specified
+0001c0d0: 2061 7474 7269 6275 7465 2e0d 0a0d 0a20   attribute..... 
+0001c0e0: 2020 2020 2020 2060 736f 7274 5f6f 7264         `sort_ord
+0001c0f0: 6572 600d 0a20 2020 2020 2020 2053 6f72  er`..        Sor
+0001c100: 7420 7265 7375 6c74 7320 6973 2061 7363  t results is asc
+0001c110: 656e 6469 6e67 206f 7220 6465 7363 656e  ending or descen
+0001c120: 6469 6e67 206f 7264 6572 2066 6f72 2061  ding order for a
+0001c130: 7474 7269 6275 7465 2076 616c 7565 7320  ttribute values 
+0001c140: 7370 6563 6966 6965 6420 6279 206f 7264  specified by ord
+0001c150: 6572 5f62 792e 0d0a 0d0a 2020 2020 2020  er_by.....      
+0001c160: 2020 2323 2044 6573 6372 6970 7469 6f6e    ## Description
+0001c170: 0d0a 2020 2020 2020 2020 6874 7470 733a  ..        https:
+0001c180: 2f2f 6672 6564 2e73 746c 6f75 6973 6665  //fred.stlouisfe
+0001c190: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
+0001c1a0: 7265 642f 7365 7269 6573 5f74 6167 732e  red/series_tags.
+0001c1b0: 6874 6d6c 0d0a 0d0a 2020 2020 2020 2020  html....        
+0001c1c0: 4765 7420 7468 6520 4652 4544 2074 6167  Get the FRED tag
+0001c1d0: 7320 666f 7220 6120 7365 7269 6573 2e0d  s for a series..
+0001c1e0: 0a0d 0a20 2020 2020 2020 2023 2320 4150  ...        ## AP
+0001c1f0: 4920 5265 7175 6573 7420 2848 5454 5053  I Request (HTTPS
+0001c200: 2047 4554 290d 0a20 2020 2020 2020 2068   GET)..        h
+0001c210: 7474 7073 3a2f 2f61 7069 2e73 746c 6f75  ttps://api.stlou
+0001c220: 6973 6665 642e 6f72 672f 6672 6564 2f73  isfed.org/fred/s
+0001c230: 6572 6965 732f 7461 6773 3f73 6572 6965  eries/tags?serie
+0001c240: 735f 6964 3d53 544c 4653 4926 6170 695f  s_id=STLFSI&api_
+0001c250: 6b65 793d 6162 6364 6566 6768 696a 6b6c  key=abcdefghijkl
+0001c260: 6d6e 6f70 7172 7374 7576 7778 797a 3132  mnopqrstuvwxyz12
+0001c270: 3334 3536 2666 696c 655f 7479 7065 3d6a  3456&file_type=j
+0001c280: 736f 6e0d 0a0d 0a20 2020 2020 2020 2023  son....        #
+0001c290: 2320 4150 4920 5265 7370 6f6e 7365 0d0a  # API Response..
+0001c2a0: 2020 2020 2020 2020 6060 606a 736f 6e0d          ```json.
+0001c2b0: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
+0001c2c0: 2020 2020 2020 2020 2272 6561 6c74 696d          "realtim
+0001c2d0: 655f 7374 6172 7422 3a20 2232 3031 332d  e_start": "2013-
+0001c2e0: 3038 2d31 3422 2c0d 0a20 2020 2020 2020  08-14",..       
+0001c2f0: 2020 2020 2022 7265 616c 7469 6d65 5f65       "realtime_e
+0001c300: 6e64 223a 2022 3230 3133 2d30 382d 3134  nd": "2013-08-14
+0001c310: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0001c320: 226f 7264 6572 5f62 7922 3a20 2273 6572  "order_by": "ser
+0001c330: 6965 735f 636f 756e 7422 2c0d 0a20 2020  ies_count",..   
+0001c340: 2020 2020 2020 2020 2022 736f 7274 5f6f           "sort_o
+0001c350: 7264 6572 223a 2022 6465 7363 222c 0d0a  rder": "desc",..
+0001c360: 2020 2020 2020 2020 2020 2020 2263 6f75              "cou
+0001c370: 6e74 223a 2038 2c0d 0a20 2020 2020 2020  nt": 8,..       
+0001c380: 2020 2020 2022 6f66 6673 6574 223a 2030       "offset": 0
+0001c390: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+0001c3a0: 6c69 6d69 7422 3a20 3130 3030 2c0d 0a20  limit": 1000,.. 
+0001c3b0: 2020 2020 2020 2020 2020 2022 7461 6773             "tags
+0001c3c0: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
+0001c3d0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+0001c3e0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
+0001c3f0: 6d65 223a 2022 6e61 7469 6f6e 222c 0d0a  me": "nation",..
+0001c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c410: 2020 2020 2267 726f 7570 5f69 6422 3a20      "group_id": 
+0001c420: 2267 656f 7422 2c0d 0a20 2020 2020 2020  "geot",..       
+0001c430: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
+0001c440: 7465 7322 3a20 2243 6f75 6e74 7279 204c  tes": "Country L
+0001c450: 6576 656c 222c 0d0a 2020 2020 2020 2020  evel",..        
+0001c460: 2020 2020 2020 2020 2020 2020 2263 7265              "cre
+0001c470: 6174 6564 223a 2022 3230 3132 2d30 322d  ated": "2012-02-
+0001c480: 3237 2031 303a 3138 3a31 392d 3036 222c  27 10:18:19-06",
+0001c490: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c4a0: 2020 2020 2020 2270 6f70 756c 6172 6974        "popularit
+0001c4b0: 7922 3a20 3130 302c 0d0a 2020 2020 2020  y": 100,..      
+0001c4c0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+0001c4d0: 6572 6965 735f 636f 756e 7422 3a20 3130  eries_count": 10
+0001c4e0: 3532 3030 0d0a 2020 2020 2020 2020 2020  5200..          
+0001c4f0: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+0001c500: 2020 2020 2020 2020 2020 2e2e 2e0d 0a20            ..... 
+0001c510: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
+0001c520: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+0001c530: 2060 6060 0d0a 0d0a 2020 2020 2020 2020   ```....        
+0001c540: 2323 2052 6574 7572 6e73 0d0a 2020 2020  ## Returns..    
+0001c550: 2020 2020 6070 616e 6461 732e 4461 7461      `pandas.Data
+0001c560: 4672 616d 6560 0d0a 0d0a 2020 2020 2020  Frame`....      
+0001c570: 2020 2323 2045 7861 6d70 6c65 0d0a 2020    ## Example..  
+0001c580: 2020 2020 2020 6060 6070 7974 686f 6e0d        ```python.
+0001c590: 0a20 2020 2020 2020 203e 3e3e 2066 7265  .        >>> fre
+0001c5a0: 6420 3d20 4652 4544 2861 7069 5f6b 6579  d = FRED(api_key
+0001c5b0: 3d27 6162 6364 6566 6768 696a 6b6c 6d6e  ='abcdefghijklmn
+0001c5c0: 6f70 7172 7374 7576 7778 797a 3132 3334  opqrstuvwxyz1234
+0001c5d0: 3536 2729 0d0a 2020 2020 2020 2020 3e3e  56')..        >>
+0001c5e0: 3e20 6672 6564 2e73 6572 6965 735f 7461  > fred.series_ta
+0001c5f0: 6773 2873 6572 6965 735f 6964 3d27 5354  gs(series_id='ST
+0001c600: 4c46 5349 2729 2e68 6561 6428 290d 0a20  LFSI').head().. 
+0001c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c620: 2020 2020 2020 2020 6772 6f75 705f 6964          group_id
+0001c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c640: 2020 2020 2020 2020 2020 2020 206e 6f74               not
+0001c650: 6573 2020 2020 2020 2020 2020 2020 2020  es              
+0001c660: 2020 2020 2063 7265 6174 6564 2020 706f       created  po
+0001c670: 7075 6c61 7269 7479 2020 7365 7269 6573  pularity  series
+0001c680: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
+0001c690: 2020 2020 6e61 6d65 0d0a 2020 2020 2020      name..      
+0001c6a0: 2020 2020 2020 7374 6c66 7369 2020 2020        stlfsi    
+0001c6b0: 2020 2020 2020 2020 726c 7320 2053 742e          rls  St.
+0001c6c0: 204c 6f75 6973 2046 696e 616e 6369 616c   Louis Financial
+0001c6d0: 2053 7472 6573 7320 496e 6465 7820 3230   Stress Index 20
+0001c6e0: 3132 2d30 382d 3136 2032 303a 3231 3a31  12-08-16 20:21:1
+0001c6f0: 372b 3030 3a30 3020 2020 2020 2020 2020  7+00:00         
+0001c700: 2031 3920 2020 2020 2020 2020 2020 2020   19             
+0001c710: 340d 0a20 2020 2020 2020 2020 2020 2066  4..            f
+0001c720: 7369 2020 2020 2020 2020 2020 2020 2020  si              
 0001c730: 2067 656e 2020 2020 2020 2020 2020 2020   gen            
-0001c740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c750: 2020 2020 2020 2032 3031 322d 3032 2d32         2012-02-2
-0001c760: 3720 3136 3a31 383a 3139 2b30 303a 3030  7 16:18:19+00:00
-0001c770: 2020 2020 2020 2020 2020 3535 2020 2020            55    
-0001c780: 2020 2020 2032 3136 3532 0d0a 2020 2020       21652..    
-0001c790: 2020 2020 2020 2020 6469 7363 6f6e 7469          disconti
-0001c7a0: 6e75 6564 2020 2020 2020 6765 6e20 2020  nued      gen   
+0001c740: 4669 6e61 6e63 6961 6c20 5374 7265 7373  Financial Stress
+0001c750: 2049 6e64 6578 2032 3031 342d 3038 2d30   Index 2014-08-0
+0001c760: 3820 3139 3a30 313a 3337 2b30 303a 3030  8 19:01:37+00:00
+0001c770: 2020 2020 2020 2020 2020 3236 2020 2020            26    
+0001c780: 2020 2020 2020 2020 3236 0d0a 2020 2020          26..    
+0001c790: 2020 2020 2020 2020 7765 656b 6c79 2020          weekly  
+0001c7a0: 2020 2020 2020 2020 2066 7265 7120 2020           freq   
 0001c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c7d0: 3230 3132 2d30 322d 3237 2031 363a 3138  2012-02-27 16:18
 0001c7e0: 3a31 392b 3030 3a30 3020 2020 2020 2020  :19+00:00       
-0001c7f0: 2020 2036 3720 2020 2020 2020 2020 3430     67         40
-0001c800: 3338 360d 0a20 2020 2020 2020 2022 2222  386..        """
-0001c810: 0d0a 0d0a 2020 2020 2020 2020 616c 6c6f  ....        allo
-0001c820: 7765 645f 6f72 6465 7273 203d 205b 0d0a  wed_orders = [..
-0001c830: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-0001c840: 732e 4f72 6465 7242 792e 7365 7269 6573  s.OrderBy.series
-0001c850: 5f63 6f75 6e74 2c0d 0a20 2020 2020 2020  _count,..       
-0001c860: 2020 2020 2065 6e75 6d73 2e4f 7264 6572       enums.Order
-0001c870: 4279 2e70 6f70 756c 6172 6974 792c 0d0a  By.popularity,..
-0001c880: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-0001c890: 732e 4f72 6465 7242 792e 6372 6561 7465  s.OrderBy.create
-0001c8a0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-0001c8b0: 656e 756d 732e 4f72 6465 7242 792e 6e61  enums.OrderBy.na
-0001c8c0: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
-0001c8d0: 2065 6e75 6d73 2e4f 7264 6572 4279 2e67   enums.OrderBy.g
-0001c8e0: 726f 7570 5f69 642c 0d0a 2020 2020 2020  roup_id,..      
-0001c8f0: 2020 5d0d 0a0d 0a20 2020 2020 2020 2069    ]....        i
-0001c900: 6620 6f72 6465 725f 6279 206e 6f74 2069  f order_by not i
-0001c910: 6e20 616c 6c6f 7765 645f 6f72 6465 7273  n allowed_orders
-0001c920: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0001c930: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0001c940: 2756 6172 6961 626c 6520 6f72 6465 725f  'Variable order_
-0001c950: 6279 2028 7b7d 2920 6973 206e 6f74 206f  by ({}) is not o
-0001c960: 6e65 206f 6620 7468 6520 7661 6c75 6573  ne of the values
-0001c970: 3a20 7b7d 272e 666f 726d 6174 286f 7264  : {}'.format(ord
-0001c980: 6572 5f62 792c 2027 2c20 272e 6a6f 696e  er_by, ', '.join
-0001c990: 286d 6170 2873 7472 2c20 616c 6c6f 7765  (map(str, allowe
-0001c9a0: 645f 6f72 6465 7273 2929 2929 0d0a 0d0a  d_orders))))....
-0001c9b0: 2020 2020 2020 2020 6966 2072 6561 6c74          if realt
-0001c9c0: 696d 655f 7374 6172 7420 6973 206e 6f74  ime_start is not
-0001c9d0: 204e 6f6e 6520 616e 6420 7265 616c 7469   None and realti
-0001c9e0: 6d65 5f73 7461 7274 203c 2064 6174 6528  me_start < date(
-0001c9f0: 3137 3736 2c20 372c 2034 293a 0d0a 2020  1776, 7, 4):..  
-0001ca00: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0001ca10: 5661 6c75 6545 7272 6f72 2827 5661 7269  ValueError('Vari
-0001ca20: 6162 6c65 2072 6561 6c74 696d 655f 7374  able realtime_st
-0001ca30: 6172 7420 2822 7b7d 2229 2069 7320 6265  art ("{}") is be
-0001ca40: 666f 7265 206d 696e 2064 6174 6520 3137  fore min date 17
-0001ca50: 3736 2d30 372d 3034 2e27 2e66 6f72 6d61  76-07-04.'.forma
-0001ca60: 7428 7265 616c 7469 6d65 5f73 7461 7274  t(realtime_start
-0001ca70: 2929 0d0a 0d0a 2020 2020 2020 2020 6966  ))....        if
-0001ca80: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
-0001ca90: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0001caa0: 7265 616c 7469 6d65 5f65 6e64 2069 7320  realtime_end is 
-0001cab0: 6e6f 7420 4e6f 6e65 2061 6e64 2072 6561  not None and rea
-0001cac0: 6c74 696d 655f 7374 6172 7420 3e20 7265  ltime_start > re
-0001cad0: 616c 7469 6d65 5f65 6e64 3a0d 0a20 2020  altime_end:..   
-0001cae0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0001caf0: 616c 7565 4572 726f 7228 2754 6865 2064  alueError('The d
-0001cb00: 6174 6520 7365 7420 6279 2076 6172 6961  ate set by varia
-0001cb10: 626c 6520 7265 616c 7469 6d65 5f73 7461  ble realtime_sta
-0001cb20: 7274 2028 227b 7d22 2920 6361 6e20 6e6f  rt ("{}") can no
-0001cb30: 7420 6265 2061 6674 6572 2074 6865 2064  t be after the d
-0001cb40: 6174 6520 7365 7420 6279 2076 6172 6961  ate set by varia
-0001cb50: 626c 6520 7265 616c 7469 6d65 5f65 6e64  ble realtime_end
-0001cb60: 2028 227b 7d22 292e 272e 666f 726d 6174   ("{}").'.format
-0001cb70: 2872 6561 6c74 696d 655f 7374 6172 742c  (realtime_start,
-0001cb80: 2072 6561 6c74 696d 655f 656e 6429 290d   realtime_end)).
-0001cb90: 0a0d 0a20 2020 2020 2020 2064 6620 3d20  ...        df = 
-0001cba0: 7064 2e44 6174 6146 7261 6d65 280d 0a20  pd.DataFrame(.. 
-0001cbb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001cbc0: 5f63 6c69 656e 742e 6765 7428 0d0a 2020  _client.get(..  
-0001cbd0: 2020 2020 2020 2020 2020 2020 2020 272f                '/
-0001cbe0: 6672 6564 2f73 6572 6965 732f 7461 6773  fred/series/tags
-0001cbf0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-0001cc00: 2020 2020 2774 6167 7327 2c0d 0a20 2020      'tags',..   
-0001cc10: 2020 2020 2020 2020 2020 2020 2073 6572               ser
-0001cc20: 6965 735f 6964 3d73 6572 6965 735f 6964  ies_id=series_id
-0001cc30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001cc40: 2020 2072 6561 6c74 696d 655f 7374 6172     realtime_star
-0001cc50: 743d 7265 616c 7469 6d65 5f73 7461 7274  t=realtime_start
-0001cc60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001cc70: 2020 2072 6561 6c74 696d 655f 656e 643d     realtime_end=
-0001cc80: 7265 616c 7469 6d65 5f65 6e64 2c0d 0a20  realtime_end,.. 
-0001cc90: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0001cca0: 7264 6572 5f62 793d 6f72 6465 725f 6279  rder_by=order_by
-0001ccb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001ccc0: 2020 2073 6f72 745f 6f72 6465 723d 736f     sort_order=so
-0001ccd0: 7274 5f6f 7264 6572 0d0a 2020 2020 2020  rt_order..      
-0001cce0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001ccf0: 2029 0d0a 0d0a 2020 2020 2020 2020 6966   )....        if
-0001cd00: 206e 6f74 2064 662e 656d 7074 793a 0d0a   not df.empty:..
-0001cd10: 2020 2020 2020 2020 2020 2020 6466 2e63              df.c
-0001cd20: 7265 6174 6564 203d 2070 642e 746f 5f64  reated = pd.to_d
-0001cd30: 6174 6574 696d 6528 6466 2e63 7265 6174  atetime(df.creat
-0001cd40: 6564 202b 2027 3030 272c 2075 7463 3d54  ed + '00', utc=T
-0001cd50: 7275 652c 2066 6f72 6d61 743d 2725 592d  rue, format='%Y-
-0001cd60: 256d 2d25 6420 2548 3a25 4d3a 2553 257a  %m-%d %H:%M:%S%z
-0001cd70: 2729 0d0a 0d0a 2020 2020 2020 2020 2020  ')....          
-0001cd80: 2020 6466 203d 2064 662e 6173 7479 7065    df = df.astype
-0001cd90: 2864 7479 7065 3d7b 0d0a 2020 2020 2020  (dtype={..      
-0001cda0: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
-0001cdb0: 3a20 2773 7472 696e 6727 2c0d 0a20 2020  : 'string',..   
-0001cdc0: 2020 2020 2020 2020 2020 2020 2027 6e6f               'no
-0001cdd0: 7465 7327 3a20 2773 7472 696e 6727 2c0d  tes': 'string',.
-0001cde0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001cdf0: 2027 6772 6f75 705f 6964 273a 2027 6361   'group_id': 'ca
-0001ce00: 7465 676f 7279 270d 0a20 2020 2020 2020  tegory'..       
-0001ce10: 2020 2020 207d 292e 7365 745f 696e 6465       }).set_inde
-0001ce20: 7828 276e 616d 6527 290d 0a0d 0a20 2020  x('name')....   
-0001ce30: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
-0001ce40: 0d0a 2020 2020 6465 6620 7365 7269 6573  ..    def series
-0001ce50: 5f75 7064 6174 6573 280d 0a20 2020 2020  _updates(..     
-0001ce60: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-0001ce70: 2020 2020 2020 2020 2020 7265 616c 7469            realti
-0001ce80: 6d65 5f73 7461 7274 3a20 6461 7465 203d  me_start: date =
-0001ce90: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-0001cea0: 2020 2020 7265 616c 7469 6d65 5f65 6e64      realtime_end
-0001ceb0: 3a20 6461 7465 203d 204e 6f6e 652c 0d0a  : date = None,..
-0001cec0: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-0001ced0: 6572 5f76 616c 7565 3a20 656e 756d 732e  er_value: enums.
-0001cee0: 4669 6c74 6572 5661 6c75 6520 3d20 656e  FilterValue = en
-0001cef0: 756d 732e 4669 6c74 6572 5661 6c75 652e  ums.FilterValue.
-0001cf00: 616c 6c2c 0d0a 2020 2020 2020 2020 2020  all,..          
-0001cf10: 2020 7374 6172 745f 7469 6d65 3a20 6461    start_time: da
-0001cf20: 7465 7469 6d65 203d 204e 6f6e 652c 0d0a  tetime = None,..
-0001cf30: 2020 2020 2020 2020 2020 2020 656e 645f              end_
-0001cf40: 7469 6d65 3a20 6461 7465 7469 6d65 203d  time: datetime =
-0001cf50: 204e 6f6e 650d 0a20 2020 2029 202d 3e20   None..    ) -> 
-0001cf60: 7064 2e44 6174 6146 7261 6d65 3a0d 0a20  pd.DataFrame:.. 
-0001cf70: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0001cf80: 2020 2020 2323 2050 6172 616d 6574 6572      ## Parameter
-0001cf90: 730d 0a0d 0a20 2020 2020 2020 2060 7265  s....        `re
-0001cfa0: 616c 7469 6d65 5f73 7461 7274 600d 0a20  altime_start`.. 
-0001cfb0: 2020 2020 2020 2054 6865 2073 7461 7274         The start
-0001cfc0: 206f 6620 7468 6520 7265 616c 2d74 696d   of the real-tim
-0001cfd0: 6520 7065 7269 6f64 2e20 466f 7220 6d6f  e period. For mo
-0001cfe0: 7265 2069 6e66 6f72 6d61 7469 6f6e 2c20  re information, 
-0001cff0: 7365 6520 5b52 6561 6c2d 5469 6d65 2050  see [Real-Time P
-0001d000: 6572 696f 6473 5d28 6874 7470 733a 2f2f  eriods](https://
-0001d010: 6672 6564 2e73 746c 6f75 6973 6665 642e  fred.stlouisfed.
-0001d020: 6f72 672f 646f 6373 2f61 7069 2f66 7265  org/docs/api/fre
-0001d030: 642f 7265 616c 7469 6d65 5f70 6572 696f  d/realtime_perio
-0001d040: 642e 6874 6d6c 292e 0d0a 0d0a 2020 2020  d.html).....    
-0001d050: 2020 2020 6072 6561 6c74 696d 655f 656e      `realtime_en
-0001d060: 6460 0d0a 2020 2020 2020 2020 5468 6520  d`..        The 
-0001d070: 656e 6420 6f66 2074 6865 2072 6561 6c2d  end of the real-
-0001d080: 7469 6d65 2070 6572 696f 642e 2046 6f72  time period. For
-0001d090: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-0001d0a0: 6e2c 2073 6565 205b 5265 616c 2d54 696d  n, see [Real-Tim
-0001d0b0: 6520 5065 7269 6f64 735d 2868 7474 7073  e Periods](https
-0001d0c0: 3a2f 2f66 7265 642e 7374 6c6f 7569 7366  ://fred.stlouisf
-0001d0d0: 6564 2e6f 7267 2f64 6f63 732f 6170 692f  ed.org/docs/api/
-0001d0e0: 6672 6564 2f72 6561 6c74 696d 655f 7065  fred/realtime_pe
-0001d0f0: 7269 6f64 2e68 746d 6c29 2e0d 0a0d 0a20  riod.html)..... 
-0001d100: 2020 2020 2020 2060 6669 6c74 6572 5f76         `filter_v
-0001d110: 616c 7565 600d 0a20 2020 2020 2020 204c  alue`..        L
-0001d120: 696d 6974 2072 6573 756c 7473 2062 7920  imit results by 
-0001d130: 6765 6f67 7261 7068 6963 2074 7970 6520  geographic type 
-0001d140: 6f66 2065 636f 6e6f 6d69 6320 6461 7461  of economic data
-0001d150: 2073 6572 6965 733b 206e 616d 656c 7920   series; namely 
-0001d160: 276d 6163 726f 272c 2027 7265 6769 6f6e  'macro', 'region
-0001d170: 616c 272c 2061 6e64 2027 616c 6c27 2e0d  al', and 'all'..
-0001d180: 0a0d 0a20 2020 2020 2020 2060 7374 6172  ...        `star
-0001d190: 745f 7469 6d65 600d 0a20 2020 2020 2020  t_time`..       
-0001d1a0: 2053 7461 7274 2074 696d 6520 666f 7220   Start time for 
-0001d1b0: 6c69 6d69 7469 6e67 2072 6573 756c 7473  limiting results
-0001d1c0: 2066 6f72 2061 2074 696d 6520 7261 6e67   for a time rang
-0001d1d0: 652c 2063 616e 2066 696c 7465 7220 646f  e, can filter do
-0001d1e0: 776e 2074 6f20 6d69 6e75 7465 730d 0a0d  wn to minutes...
-0001d1f0: 0a20 2020 2020 2020 2060 656e 645f 7469  .        `end_ti
-0001d200: 6d65 600d 0a20 2020 2020 2020 2045 6e64  me`..        End
-0001d210: 2074 696d 6520 666f 7220 6c69 6d69 7469   time for limiti
-0001d220: 6e67 2072 6573 756c 7473 2066 6f72 2061  ng results for a
-0001d230: 2074 696d 6520 7261 6e67 652c 2063 616e   time range, can
-0001d240: 2066 696c 7465 7220 646f 776e 2074 6f20   filter down to 
-0001d250: 6d69 6e75 7465 730d 0a0d 0a20 2020 2020  minutes....     
-0001d260: 2020 2023 2320 4465 7363 7269 7074 696f     ## Descriptio
-0001d270: 6e0d 0a20 2020 2020 2020 2068 7474 7073  n..        https
-0001d280: 3a2f 2f66 7265 642e 7374 6c6f 7569 7366  ://fred.stlouisf
-0001d290: 6564 2e6f 7267 2f64 6f63 732f 6170 692f  ed.org/docs/api/
-0001d2a0: 6672 6564 2f73 6572 6965 735f 7570 6461  fred/series_upda
-0001d2b0: 7465 732e 6874 6d6c 0d0a 0d0a 2020 2020  tes.html....    
-0001d2c0: 2020 2020 4765 7420 6563 6f6e 6f6d 6963      Get economic
-0001d2d0: 2064 6174 6120 7365 7269 6573 2073 6f72   data series sor
-0001d2e0: 7465 6420 6279 2077 6865 6e20 6f62 7365  ted by when obse
-0001d2f0: 7276 6174 696f 6e73 2077 6572 6520 7570  rvations were up
-0001d300: 6461 7465 6420 6f6e 2074 6865 2046 5245  dated on the FRE
-0001d310: 4420 7365 7276 6572 2028 6174 7472 6962  D server (attrib
-0001d320: 7574 6520 6c61 7374 5f75 7064 6174 6564  ute last_updated
-0001d330: 292e 0d0a 2020 2020 2020 2020 5265 7375  )...        Resu
-0001d340: 6c74 7320 6172 6520 6c69 6d69 7465 6420  lts are limited 
-0001d350: 746f 2073 6572 6965 7320 7570 6461 7465  to series update
-0001d360: 6420 7769 7468 696e 2074 6865 206c 6173  d within the las
-0001d370: 7420 7477 6f20 7765 656b 732e 0d0a 0d0a  t two weeks.....
-0001d380: 2020 2020 2020 2020 2323 2041 5049 2052          ## API R
-0001d390: 6571 7565 7374 2028 4854 5450 5320 4745  equest (HTTPS GE
-0001d3a0: 5429 0d0a 2020 2020 2020 2020 6874 7470  T)..        http
-0001d3b0: 733a 2f2f 6170 692e 7374 6c6f 7569 7366  s://api.stlouisf
-0001d3c0: 6564 2e6f 7267 2f66 7265 642f 7365 7269  ed.org/fred/seri
-0001d3d0: 6573 2f75 7064 6174 6573 3f61 7069 5f6b  es/updates?api_k
-0001d3e0: 6579 3d61 6263 6465 6667 6869 6a6b 6c6d  ey=abcdefghijklm
-0001d3f0: 6e6f 7071 7273 7475 7677 7879 7a31 3233  nopqrstuvwxyz123
-0001d400: 3435 3626 6669 6c65 5f74 7970 653d 6a73  456&file_type=js
-0001d410: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2323  on....        ##
-0001d420: 2041 5049 2052 6573 706f 6e73 650d 0a20   API Response.. 
-0001d430: 2020 2020 2020 2060 6060 6a73 6f6e 0d0a         ```json..
-0001d440: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-0001d450: 2020 2020 2020 2022 7265 616c 7469 6d65         "realtime
-0001d460: 5f73 7461 7274 223a 2022 3230 3133 2d30  _start": "2013-0
-0001d470: 382d 3134 222c 0d0a 2020 2020 2020 2020  8-14",..        
-0001d480: 2020 2020 2272 6561 6c74 696d 655f 656e      "realtime_en
-0001d490: 6422 3a20 2232 3031 332d 3038 2d31 3422  d": "2013-08-14"
-0001d4a0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-0001d4b0: 6669 6c74 6572 5f76 6172 6961 626c 6522  filter_variable"
-0001d4c0: 3a20 2267 656f 6772 6170 6879 222c 0d0a  : "geography",..
-0001d4d0: 2020 2020 2020 2020 2020 2020 2266 696c              "fil
-0001d4e0: 7465 725f 7661 6c75 6522 3a20 2261 6c6c  ter_value": "all
-0001d4f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0001d500: 226f 7264 6572 5f62 7922 3a20 226c 6173  "order_by": "las
-0001d510: 745f 7570 6461 7465 6422 2c0d 0a20 2020  t_updated",..   
-0001d520: 2020 2020 2020 2020 2022 736f 7274 5f6f           "sort_o
-0001d530: 7264 6572 223a 2022 6465 7363 222c 0d0a  rder": "desc",..
-0001d540: 2020 2020 2020 2020 2020 2020 2263 6f75              "cou
-0001d550: 6e74 223a 2031 3433 3533 352c 0d0a 2020  nt": 143535,..  
-0001d560: 2020 2020 2020 2020 2020 226f 6666 7365            "offse
-0001d570: 7422 3a20 302c 0d0a 2020 2020 2020 2020  t": 0,..        
-0001d580: 2020 2020 226c 696d 6974 223a 2031 3030      "limit": 100
-0001d590: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-0001d5a0: 7365 7269 6573 7322 3a20 5b0d 0a20 2020  seriess": [..   
-0001d5b0: 2020 2020 2020 2020 2020 2020 207b 0d0a               {..
-0001d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5d0: 2020 2020 2269 6422 3a20 2250 5049 4954      "id": "PPIIT
-0001d5e0: 4d22 2c0d 0a20 2020 2020 2020 2020 2020  M",..           
-0001d5f0: 2020 2020 2020 2020 2022 7265 616c 7469           "realti
-0001d600: 6d65 5f73 7461 7274 223a 2022 3230 3133  me_start": "2013
-0001d610: 2d30 382d 3134 222c 0d0a 2020 2020 2020  -08-14",..      
-0001d620: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-0001d630: 6561 6c74 696d 655f 656e 6422 3a20 2232  ealtime_end": "2
-0001d640: 3031 332d 3038 2d31 3422 2c0d 0a20 2020  013-08-14",..   
-0001d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d660: 2022 7469 746c 6522 3a20 2250 726f 6475   "title": "Produ
-0001d670: 6365 7220 5072 6963 6520 496e 6465 783a  cer Price Index:
-0001d680: 2049 6e74 6572 6d65 6469 6174 6520 4d61   Intermediate Ma
-0001d690: 7465 7269 616c 733a 2053 7570 706c 6965  terials: Supplie
-0001d6a0: 7320 2620 436f 6d70 6f6e 656e 7473 222c  s & Components",
+0001c7f0: 2020 2036 3820 2020 2020 2020 2020 2033     68          3
+0001c800: 3534 380d 0a20 2020 2020 2020 2020 2020  548..           
+0001c810: 2066 696e 616e 6369 616c 2020 2020 2020   financial      
+0001c820: 2020 2067 656e 2020 2020 2020 2020 2020     gen          
+0001c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c840: 2020 2020 2020 2020 2032 3031 322d 3032           2012-02
+0001c850: 2d32 3720 3136 3a31 383a 3139 2b30 303a  -27 16:18:19+00:
+0001c860: 3030 2020 2020 2020 2020 2020 3535 2020  00          55  
+0001c870: 2020 2020 2020 2032 3136 3532 0d0a 2020         21652..  
+0001c880: 2020 2020 2020 2020 2020 6469 7363 6f6e            discon
+0001c890: 7469 6e75 6564 2020 2020 2020 6765 6e20  tinued      gen 
+0001c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8c0: 2020 3230 3132 2d30 322d 3237 2031 363a    2012-02-27 16:
+0001c8d0: 3138 3a31 392b 3030 3a30 3020 2020 2020  18:19+00:00     
+0001c8e0: 2020 2020 2036 3720 2020 2020 2020 2020       67         
+0001c8f0: 3430 3338 360d 0a20 2020 2020 2020 2022  40386..        "
+0001c900: 2222 0d0a 0d0a 2020 2020 2020 2020 616c  ""....        al
+0001c910: 6c6f 7765 645f 6f72 6465 7273 203d 205b  lowed_orders = [
+0001c920: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+0001c930: 756d 732e 4f72 6465 7242 792e 7365 7269  ums.OrderBy.seri
+0001c940: 6573 5f63 6f75 6e74 2c0d 0a20 2020 2020  es_count,..     
+0001c950: 2020 2020 2020 2065 6e75 6d73 2e4f 7264         enums.Ord
+0001c960: 6572 4279 2e70 6f70 756c 6172 6974 792c  erBy.popularity,
+0001c970: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+0001c980: 756d 732e 4f72 6465 7242 792e 6372 6561  ums.OrderBy.crea
+0001c990: 7465 642c 0d0a 2020 2020 2020 2020 2020  ted,..          
+0001c9a0: 2020 656e 756d 732e 4f72 6465 7242 792e    enums.OrderBy.
+0001c9b0: 6e61 6d65 2c0d 0a20 2020 2020 2020 2020  name,..         
+0001c9c0: 2020 2065 6e75 6d73 2e4f 7264 6572 4279     enums.OrderBy
+0001c9d0: 2e67 726f 7570 5f69 642c 0d0a 2020 2020  .group_id,..    
+0001c9e0: 2020 2020 5d0d 0a0d 0a20 2020 2020 2020      ]....       
+0001c9f0: 2069 6620 6f72 6465 725f 6279 206e 6f74   if order_by not
+0001ca00: 2069 6e20 616c 6c6f 7765 645f 6f72 6465   in allowed_orde
+0001ca10: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
+0001ca20: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0001ca30: 7228 2756 6172 6961 626c 6520 6f72 6465  r('Variable orde
+0001ca40: 725f 6279 2028 7b7d 2920 6973 206e 6f74  r_by ({}) is not
+0001ca50: 206f 6e65 206f 6620 7468 6520 7661 6c75   one of the valu
+0001ca60: 6573 3a20 7b7d 272e 666f 726d 6174 286f  es: {}'.format(o
+0001ca70: 7264 6572 5f62 792c 2027 2c20 272e 6a6f  rder_by, ', '.jo
+0001ca80: 696e 286d 6170 2873 7472 2c20 616c 6c6f  in(map(str, allo
+0001ca90: 7765 645f 6f72 6465 7273 2929 2929 0d0a  wed_orders))))..
+0001caa0: 0d0a 2020 2020 2020 2020 6966 2072 6561  ..        if rea
+0001cab0: 6c74 696d 655f 7374 6172 7420 6973 206e  ltime_start is n
+0001cac0: 6f74 204e 6f6e 6520 616e 6420 7265 616c  ot None and real
+0001cad0: 7469 6d65 5f73 7461 7274 203c 2064 6174  time_start < dat
+0001cae0: 6528 3137 3736 2c20 372c 2034 293a 0d0a  e(1776, 7, 4):..
+0001caf0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0001cb00: 6520 5661 6c75 6545 7272 6f72 2827 5661  e ValueError('Va
+0001cb10: 7269 6162 6c65 2072 6561 6c74 696d 655f  riable realtime_
+0001cb20: 7374 6172 7420 2822 7b7d 2229 2069 7320  start ("{}") is 
+0001cb30: 6265 666f 7265 206d 696e 2064 6174 6520  before min date 
+0001cb40: 3137 3736 2d30 372d 3034 2e27 2e66 6f72  1776-07-04.'.for
+0001cb50: 6d61 7428 7265 616c 7469 6d65 5f73 7461  mat(realtime_sta
+0001cb60: 7274 2929 0d0a 0d0a 2020 2020 2020 2020  rt))....        
+0001cb70: 6966 2072 6561 6c74 696d 655f 7374 6172  if realtime_star
+0001cb80: 7420 6973 206e 6f74 204e 6f6e 6520 616e  t is not None an
+0001cb90: 6420 7265 616c 7469 6d65 5f65 6e64 2069  d realtime_end i
+0001cba0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2072  s not None and r
+0001cbb0: 6561 6c74 696d 655f 7374 6172 7420 3e20  ealtime_start > 
+0001cbc0: 7265 616c 7469 6d65 5f65 6e64 3a0d 0a20  realtime_end:.. 
+0001cbd0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0001cbe0: 2056 616c 7565 4572 726f 7228 2754 6865   ValueError('The
+0001cbf0: 2064 6174 6520 7365 7420 6279 2076 6172   date set by var
+0001cc00: 6961 626c 6520 7265 616c 7469 6d65 5f73  iable realtime_s
+0001cc10: 7461 7274 2028 227b 7d22 2920 6361 6e20  tart ("{}") can 
+0001cc20: 6e6f 7420 6265 2061 6674 6572 2074 6865  not be after the
+0001cc30: 2064 6174 6520 7365 7420 6279 2076 6172   date set by var
+0001cc40: 6961 626c 6520 7265 616c 7469 6d65 5f65  iable realtime_e
+0001cc50: 6e64 2028 227b 7d22 292e 272e 666f 726d  nd ("{}").'.form
+0001cc60: 6174 2872 6561 6c74 696d 655f 7374 6172  at(realtime_star
+0001cc70: 742c 2072 6561 6c74 696d 655f 656e 6429  t, realtime_end)
+0001cc80: 290d 0a0d 0a20 2020 2020 2020 2064 6620  )....        df 
+0001cc90: 3d20 7064 2e44 6174 6146 7261 6d65 280d  = pd.DataFrame(.
+0001cca0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001ccb0: 662e 5f63 6c69 656e 742e 6765 7428 0d0a  f._client.get(..
+0001ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ccd0: 272f 6672 6564 2f73 6572 6965 732f 7461  '/fred/series/ta
+0001cce0: 6773 272c 0d0a 2020 2020 2020 2020 2020  gs',..          
+0001ccf0: 2020 2020 2020 2774 6167 7327 2c0d 0a20        'tags',.. 
+0001cd00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001cd10: 6572 6965 735f 6964 3d73 6572 6965 735f  eries_id=series_
+0001cd20: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
+0001cd30: 2020 2020 2072 6561 6c74 696d 655f 7374       realtime_st
+0001cd40: 6172 743d 7265 616c 7469 6d65 5f73 7461  art=realtime_sta
+0001cd50: 7274 2c0d 0a20 2020 2020 2020 2020 2020  rt,..           
+0001cd60: 2020 2020 2072 6561 6c74 696d 655f 656e       realtime_en
+0001cd70: 643d 7265 616c 7469 6d65 5f65 6e64 2c0d  d=realtime_end,.
+0001cd80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cd90: 206f 7264 6572 5f62 793d 6f72 6465 725f   order_by=order_
+0001cda0: 6279 2c0d 0a20 2020 2020 2020 2020 2020  by,..           
+0001cdb0: 2020 2020 2073 6f72 745f 6f72 6465 723d       sort_order=
+0001cdc0: 736f 7274 5f6f 7264 6572 0d0a 2020 2020  sort_order..    
+0001cdd0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001cde0: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+0001cdf0: 6966 206e 6f74 2064 662e 656d 7074 793a  if not df.empty:
+0001ce00: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+0001ce10: 2e63 7265 6174 6564 203d 2070 642e 746f  .created = pd.to
+0001ce20: 5f64 6174 6574 696d 6528 6466 2e63 7265  _datetime(df.cre
+0001ce30: 6174 6564 202b 2027 3030 272c 2075 7463  ated + '00', utc
+0001ce40: 3d54 7275 652c 2066 6f72 6d61 743d 2725  =True, format='%
+0001ce50: 592d 256d 2d25 6420 2548 3a25 4d3a 2553  Y-%m-%d %H:%M:%S
+0001ce60: 257a 2729 0d0a 0d0a 2020 2020 2020 2020  %z')....        
+0001ce70: 2020 2020 6466 203d 2064 662e 6173 7479      df = df.asty
+0001ce80: 7065 2864 7479 7065 3d7b 0d0a 2020 2020  pe(dtype={..    
+0001ce90: 2020 2020 2020 2020 2020 2020 276e 616d              'nam
+0001cea0: 6527 3a20 2773 7472 696e 6727 2c0d 0a20  e': 'string',.. 
+0001ceb0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001cec0: 6e6f 7465 7327 3a20 2773 7472 696e 6727  notes': 'string'
+0001ced0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001cee0: 2020 2027 6772 6f75 705f 6964 273a 2027     'group_id': '
+0001cef0: 6361 7465 676f 7279 270d 0a20 2020 2020  category'..     
+0001cf00: 2020 2020 2020 207d 292e 7365 745f 696e         }).set_in
+0001cf10: 6465 7828 276e 616d 6527 290d 0a0d 0a20  dex('name').... 
+0001cf20: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
+0001cf30: 0d0a 0d0a 2020 2020 6465 6620 7365 7269  ....    def seri
+0001cf40: 6573 5f75 7064 6174 6573 280d 0a20 2020  es_updates(..   
+0001cf50: 2020 2020 2020 2020 2073 656c 662c 0d0a           self,..
+0001cf60: 2020 2020 2020 2020 2020 2020 7265 616c              real
+0001cf70: 7469 6d65 5f73 7461 7274 3a20 6461 7465  time_start: date
+0001cf80: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+0001cf90: 2020 2020 2020 7265 616c 7469 6d65 5f65        realtime_e
+0001cfa0: 6e64 3a20 6461 7465 203d 204e 6f6e 652c  nd: date = None,
+0001cfb0: 0d0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
+0001cfc0: 6c74 6572 5f76 616c 7565 3a20 656e 756d  lter_value: enum
+0001cfd0: 732e 4669 6c74 6572 5661 6c75 6520 3d20  s.FilterValue = 
+0001cfe0: 656e 756d 732e 4669 6c74 6572 5661 6c75  enums.FilterValu
+0001cff0: 652e 616c 6c2c 0d0a 2020 2020 2020 2020  e.all,..        
+0001d000: 2020 2020 7374 6172 745f 7469 6d65 3a20      start_time: 
+0001d010: 6461 7465 7469 6d65 203d 204e 6f6e 652c  datetime = None,
+0001d020: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+0001d030: 645f 7469 6d65 3a20 6461 7465 7469 6d65  d_time: datetime
+0001d040: 203d 204e 6f6e 650d 0a20 2020 2029 202d   = None..    ) -
+0001d050: 3e20 7064 2e44 6174 6146 7261 6d65 3a0d  > pd.DataFrame:.
+0001d060: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0001d070: 2020 2020 2020 2323 2050 6172 616d 6574        ## Paramet
+0001d080: 6572 730d 0a0d 0a20 2020 2020 2020 2060  ers....        `
+0001d090: 7265 616c 7469 6d65 5f73 7461 7274 600d  realtime_start`.
+0001d0a0: 0a20 2020 2020 2020 2054 6865 2073 7461  .        The sta
+0001d0b0: 7274 206f 6620 7468 6520 7265 616c 2d74  rt of the real-t
+0001d0c0: 696d 6520 7065 7269 6f64 2e20 466f 7220  ime period. For 
+0001d0d0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+0001d0e0: 2c20 7365 6520 5b52 6561 6c2d 5469 6d65  , see [Real-Time
+0001d0f0: 2050 6572 696f 6473 5d28 6874 7470 733a   Periods](https:
+0001d100: 2f2f 6672 6564 2e73 746c 6f75 6973 6665  //fred.stlouisfe
+0001d110: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
+0001d120: 7265 642f 7265 616c 7469 6d65 5f70 6572  red/realtime_per
+0001d130: 696f 642e 6874 6d6c 292e 0d0a 0d0a 2020  iod.html).....  
+0001d140: 2020 2020 2020 6072 6561 6c74 696d 655f        `realtime_
+0001d150: 656e 6460 0d0a 2020 2020 2020 2020 5468  end`..        Th
+0001d160: 6520 656e 6420 6f66 2074 6865 2072 6561  e end of the rea
+0001d170: 6c2d 7469 6d65 2070 6572 696f 642e 2046  l-time period. F
+0001d180: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+0001d190: 696f 6e2c 2073 6565 205b 5265 616c 2d54  ion, see [Real-T
+0001d1a0: 696d 6520 5065 7269 6f64 735d 2868 7474  ime Periods](htt
+0001d1b0: 7073 3a2f 2f66 7265 642e 7374 6c6f 7569  ps://fred.stloui
+0001d1c0: 7366 6564 2e6f 7267 2f64 6f63 732f 6170  sfed.org/docs/ap
+0001d1d0: 692f 6672 6564 2f72 6561 6c74 696d 655f  i/fred/realtime_
+0001d1e0: 7065 7269 6f64 2e68 746d 6c29 2e0d 0a0d  period.html)....
+0001d1f0: 0a20 2020 2020 2020 2060 6669 6c74 6572  .        `filter
+0001d200: 5f76 616c 7565 600d 0a20 2020 2020 2020  _value`..       
+0001d210: 204c 696d 6974 2072 6573 756c 7473 2062   Limit results b
+0001d220: 7920 6765 6f67 7261 7068 6963 2074 7970  y geographic typ
+0001d230: 6520 6f66 2065 636f 6e6f 6d69 6320 6461  e of economic da
+0001d240: 7461 2073 6572 6965 733b 206e 616d 656c  ta series; namel
+0001d250: 7920 276d 6163 726f 272c 2027 7265 6769  y 'macro', 'regi
+0001d260: 6f6e 616c 272c 2061 6e64 2027 616c 6c27  onal', and 'all'
+0001d270: 2e0d 0a0d 0a20 2020 2020 2020 2060 7374  .....        `st
+0001d280: 6172 745f 7469 6d65 600d 0a20 2020 2020  art_time`..     
+0001d290: 2020 2053 7461 7274 2074 696d 6520 666f     Start time fo
+0001d2a0: 7220 6c69 6d69 7469 6e67 2072 6573 756c  r limiting resul
+0001d2b0: 7473 2066 6f72 2061 2074 696d 6520 7261  ts for a time ra
+0001d2c0: 6e67 652c 2063 616e 2066 696c 7465 7220  nge, can filter 
+0001d2d0: 646f 776e 2074 6f20 6d69 6e75 7465 730d  down to minutes.
+0001d2e0: 0a0d 0a20 2020 2020 2020 2060 656e 645f  ...        `end_
+0001d2f0: 7469 6d65 600d 0a20 2020 2020 2020 2045  time`..        E
+0001d300: 6e64 2074 696d 6520 666f 7220 6c69 6d69  nd time for limi
+0001d310: 7469 6e67 2072 6573 756c 7473 2066 6f72  ting results for
+0001d320: 2061 2074 696d 6520 7261 6e67 652c 2063   a time range, c
+0001d330: 616e 2066 696c 7465 7220 646f 776e 2074  an filter down t
+0001d340: 6f20 6d69 6e75 7465 730d 0a0d 0a20 2020  o minutes....   
+0001d350: 2020 2020 2023 2320 4465 7363 7269 7074       ## Descript
+0001d360: 696f 6e0d 0a20 2020 2020 2020 2068 7474  ion..        htt
+0001d370: 7073 3a2f 2f66 7265 642e 7374 6c6f 7569  ps://fred.stloui
+0001d380: 7366 6564 2e6f 7267 2f64 6f63 732f 6170  sfed.org/docs/ap
+0001d390: 692f 6672 6564 2f73 6572 6965 735f 7570  i/fred/series_up
+0001d3a0: 6461 7465 732e 6874 6d6c 0d0a 0d0a 2020  dates.html....  
+0001d3b0: 2020 2020 2020 4765 7420 6563 6f6e 6f6d        Get econom
+0001d3c0: 6963 2064 6174 6120 7365 7269 6573 2073  ic data series s
+0001d3d0: 6f72 7465 6420 6279 2077 6865 6e20 6f62  orted by when ob
+0001d3e0: 7365 7276 6174 696f 6e73 2077 6572 6520  servations were 
+0001d3f0: 7570 6461 7465 6420 6f6e 2074 6865 2046  updated on the F
+0001d400: 5245 4420 7365 7276 6572 2028 6174 7472  RED server (attr
+0001d410: 6962 7574 6520 6c61 7374 5f75 7064 6174  ibute last_updat
+0001d420: 6564 292e 0d0a 2020 2020 2020 2020 5265  ed)...        Re
+0001d430: 7375 6c74 7320 6172 6520 6c69 6d69 7465  sults are limite
+0001d440: 6420 746f 2073 6572 6965 7320 7570 6461  d to series upda
+0001d450: 7465 6420 7769 7468 696e 2074 6865 206c  ted within the l
+0001d460: 6173 7420 7477 6f20 7765 656b 732e 0d0a  ast two weeks...
+0001d470: 0d0a 2020 2020 2020 2020 2323 2041 5049  ..        ## API
+0001d480: 2052 6571 7565 7374 2028 4854 5450 5320   Request (HTTPS 
+0001d490: 4745 5429 0d0a 2020 2020 2020 2020 6874  GET)..        ht
+0001d4a0: 7470 733a 2f2f 6170 692e 7374 6c6f 7569  tps://api.stloui
+0001d4b0: 7366 6564 2e6f 7267 2f66 7265 642f 7365  sfed.org/fred/se
+0001d4c0: 7269 6573 2f75 7064 6174 6573 3f61 7069  ries/updates?api
+0001d4d0: 5f6b 6579 3d61 6263 6465 6667 6869 6a6b  _key=abcdefghijk
+0001d4e0: 6c6d 6e6f 7071 7273 7475 7677 7879 7a31  lmnopqrstuvwxyz1
+0001d4f0: 3233 3435 3626 6669 6c65 5f74 7970 653d  23456&file_type=
+0001d500: 6a73 6f6e 0d0a 0d0a 2020 2020 2020 2020  json....        
+0001d510: 2323 2041 5049 2052 6573 706f 6e73 650d  ## API Response.
+0001d520: 0a20 2020 2020 2020 2060 6060 6a73 6f6e  .        ```json
+0001d530: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
+0001d540: 2020 2020 2020 2020 2022 7265 616c 7469           "realti
+0001d550: 6d65 5f73 7461 7274 223a 2022 3230 3133  me_start": "2013
+0001d560: 2d30 382d 3134 222c 0d0a 2020 2020 2020  -08-14",..      
+0001d570: 2020 2020 2020 2272 6561 6c74 696d 655f        "realtime_
+0001d580: 656e 6422 3a20 2232 3031 332d 3038 2d31  end": "2013-08-1
+0001d590: 3422 2c0d 0a20 2020 2020 2020 2020 2020  4",..           
+0001d5a0: 2022 6669 6c74 6572 5f76 6172 6961 626c   "filter_variabl
+0001d5b0: 6522 3a20 2267 656f 6772 6170 6879 222c  e": "geography",
+0001d5c0: 0d0a 2020 2020 2020 2020 2020 2020 2266  ..            "f
+0001d5d0: 696c 7465 725f 7661 6c75 6522 3a20 2261  ilter_value": "a
+0001d5e0: 6c6c 222c 0d0a 2020 2020 2020 2020 2020  ll",..          
+0001d5f0: 2020 226f 7264 6572 5f62 7922 3a20 226c    "order_by": "l
+0001d600: 6173 745f 7570 6461 7465 6422 2c0d 0a20  ast_updated",.. 
+0001d610: 2020 2020 2020 2020 2020 2022 736f 7274             "sort
+0001d620: 5f6f 7264 6572 223a 2022 6465 7363 222c  _order": "desc",
+0001d630: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
+0001d640: 6f75 6e74 223a 2031 3433 3533 352c 0d0a  ount": 143535,..
+0001d650: 2020 2020 2020 2020 2020 2020 226f 6666              "off
+0001d660: 7365 7422 3a20 302c 0d0a 2020 2020 2020  set": 0,..      
+0001d670: 2020 2020 2020 226c 696d 6974 223a 2031        "limit": 1
+0001d680: 3030 2c0d 0a20 2020 2020 2020 2020 2020  00,..           
+0001d690: 2022 7365 7269 6573 7322 3a20 5b0d 0a20   "seriess": [.. 
+0001d6a0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
 0001d6b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d6c0: 2020 2020 2020 226f 6273 6572 7661 7469        "observati
-0001d6d0: 6f6e 5f73 7461 7274 223a 2022 3139 3437  on_start": "1947
-0001d6e0: 2d30 342d 3031 222c 0d0a 2020 2020 2020  -04-01",..      
-0001d6f0: 2020 2020 2020 2020 2020 2020 2020 226f                "o
-0001d700: 6273 6572 7661 7469 6f6e 5f65 6e64 223a  bservation_end":
-0001d710: 2022 3230 3133 2d30 372d 3031 222c 0d0a   "2013-07-01",..
-0001d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d730: 2020 2020 2266 7265 7175 656e 6379 223a      "frequency":
-0001d740: 2022 4d6f 6e74 686c 7922 2c0d 0a20 2020   "Monthly",..   
-0001d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d760: 2022 6672 6571 7565 6e63 795f 7368 6f72   "frequency_shor
-0001d770: 7422 3a20 224d 222c 0d0a 2020 2020 2020  t": "M",..      
-0001d780: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-0001d790: 6e69 7473 223a 2022 496e 6465 7820 3139  nits": "Index 19
-0001d7a0: 3832 3d31 3030 222c 0d0a 2020 2020 2020  82=100",..      
-0001d7b0: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-0001d7c0: 6e69 7473 5f73 686f 7274 223a 2022 496e  nits_short": "In
-0001d7d0: 6465 7820 3139 3832 3d31 3030 222c 0d0a  dex 1982=100",..
+0001d6c0: 2020 2020 2020 2269 6422 3a20 2250 5049        "id": "PPI
+0001d6d0: 4954 4d22 2c0d 0a20 2020 2020 2020 2020  ITM",..         
+0001d6e0: 2020 2020 2020 2020 2020 2022 7265 616c             "real
+0001d6f0: 7469 6d65 5f73 7461 7274 223a 2022 3230  time_start": "20
+0001d700: 3133 2d30 382d 3134 222c 0d0a 2020 2020  13-08-14",..    
+0001d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d720: 2272 6561 6c74 696d 655f 656e 6422 3a20  "realtime_end": 
+0001d730: 2232 3031 332d 3038 2d31 3422 2c0d 0a20  "2013-08-14",.. 
+0001d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d750: 2020 2022 7469 746c 6522 3a20 2250 726f     "title": "Pro
+0001d760: 6475 6365 7220 5072 6963 6520 496e 6465  ducer Price Inde
+0001d770: 783a 2049 6e74 6572 6d65 6469 6174 6520  x: Intermediate 
+0001d780: 4d61 7465 7269 616c 733a 2053 7570 706c  Materials: Suppl
+0001d790: 6965 7320 2620 436f 6d70 6f6e 656e 7473  ies & Components
+0001d7a0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0001d7b0: 2020 2020 2020 2020 226f 6273 6572 7661          "observa
+0001d7c0: 7469 6f6e 5f73 7461 7274 223a 2022 3139  tion_start": "19
+0001d7d0: 3437 2d30 342d 3031 222c 0d0a 2020 2020  47-04-01",..    
 0001d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7f0: 2020 2020 2273 6561 736f 6e61 6c5f 6164      "seasonal_ad
-0001d800: 6a75 7374 6d65 6e74 223a 2022 5365 6173  justment": "Seas
-0001d810: 6f6e 616c 6c79 2041 646a 7573 7465 6422  onally Adjusted"
-0001d820: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001d830: 2020 2020 2020 2022 7365 6173 6f6e 616c         "seasonal
-0001d840: 5f61 646a 7573 746d 656e 745f 7368 6f72  _adjustment_shor
-0001d850: 7422 3a20 2253 4122 2c0d 0a20 2020 2020  t": "SA",..     
-0001d860: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001d870: 6c61 7374 5f75 7064 6174 6564 223a 2022  last_updated": "
-0001d880: 3230 3133 2d30 382d 3134 2030 383a 3336  2013-08-14 08:36
-0001d890: 3a30 352d 3035 222c 0d0a 2020 2020 2020  :05-05",..      
-0001d8a0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-0001d8b0: 6f70 756c 6172 6974 7922 3a20 3532 0d0a  opularity": 52..
-0001d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8d0: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-0001d8e0: 2020 2020 2e2e 2e0d 0a20 2020 2020 2020      .....       
-0001d8f0: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-0001d900: 7d0d 0a20 2020 2020 2020 2060 6060 0d0a  }..        ```..
-0001d910: 0d0a 2020 2020 2020 2020 2323 2052 6574  ..        ## Ret
-0001d920: 7572 6e73 0d0a 2020 2020 2020 2020 6070  urns..        `p
-0001d930: 616e 6461 732e 4461 7461 4672 616d 6560  andas.DataFrame`
-0001d940: 0d0a 0d0a 2020 2020 2020 2020 2323 2045  ....        ## E
-0001d950: 7861 6d70 6c65 0d0a 2020 2020 2020 2020  xample..        
-0001d960: 6060 6070 7974 686f 6e0d 0a20 2020 2020  ```python..     
-0001d970: 2020 203e 3e3e 2066 7265 6420 3d20 4652     >>> fred = FR
-0001d980: 4544 2861 7069 5f6b 6579 3d27 6162 6364  ED(api_key='abcd
-0001d990: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
-0001d9a0: 7576 7778 797a 3132 3334 3536 2729 0d0a  uvwxyz123456')..
-0001d9b0: 2020 2020 2020 2020 3e3e 3e20 6672 6564          >>> fred
-0001d9c0: 2e73 6572 6965 735f 7570 6461 7465 7328  .series_updates(
-0001d9d0: 7374 6172 745f 7469 6d65 3d64 6174 6574  start_time=datet
-0001d9e0: 696d 6528 3230 3232 2c20 312c 2031 3529  ime(2022, 1, 15)
-0001d9f0: 2c20 656e 645f 7469 6d65 3d64 6174 6574  , end_time=datet
-0001da00: 696d 6528 3230 3232 2c20 312c 2031 3629  ime(2022, 1, 16)
-0001da10: 292e 6865 6164 2829 0d0a 2020 2020 2020  ).head()..      
-0001da20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001da30: 6561 6c74 696d 655f 7374 6172 7420 7265  ealtime_start re
-0001da40: 616c 7469 6d65 5f65 6e64 2020 2020 2020  altime_end      
-0001da50: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-0001da60: 6520 6f62 7365 7276 6174 696f 6e5f 7374  e observation_st
-0001da70: 6172 7420 6f62 7365 7276 6174 696f 6e5f  art observation_
-0001da80: 656e 6420 2020 2020 6672 6571 7565 6e63  end     frequenc
-0001da90: 7920 6672 6571 7565 6e63 795f 7368 6f72  y frequency_shor
-0001daa0: 7420 2020 2020 2020 2020 756e 6974 7320  t         units 
-0001dab0: 756e 6974 735f 7368 6f72 7420 2020 2020  units_short     
-0001dac0: 2073 6561 736f 6e61 6c5f 6164 6a75 7374   seasonal_adjust
-0001dad0: 6d65 6e74 2073 6561 736f 6e61 6c5f 6164  ment seasonal_ad
-0001dae0: 6a75 7374 6d65 6e74 5f73 686f 7274 2020  justment_short  
-0001daf0: 2020 2020 2020 2020 2020 2020 6c61 7374              last
-0001db00: 5f75 7064 6174 6564 2020 706f 7075 6c61  _updated  popula
-0001db10: 7269 7479 2020 2020 2020 2020 2020 2020  rity            
-0001db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db40: 2020 6e6f 7465 730d 0a20 2020 2020 2020    notes..       
-0001db50: 2020 2020 2069 640d 0a20 2020 2020 2020       id..       
-0001db60: 2020 2020 2053 5035 3030 2020 2020 2020       SP500      
-0001db70: 2020 3230 3232 2d30 322d 3035 2020 2032    2022-02-05   2
-0001db80: 3032 322d 3032 2d30 3520 2020 2020 2020  022-02-05       
-0001db90: 2020 2020 2020 2020 2053 2650 2035 3030           S&P 500
-0001dba0: 2020 2020 2020 2020 3230 3132 2d30 322d          2012-02-
-0001dbb0: 3036 2020 2020 2020 3230 3232 2d30 322d  06      2022-02-
-0001dbc0: 3034 2020 4461 696c 792c 2043 6c6f 7365  04  Daily, Close
-0001dbd0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-0001dbe0: 2020 2020 2020 2020 2049 6e64 6578 2020           Index  
-0001dbf0: 2020 2020 2049 6e64 6578 2020 4e6f 7420       Index  Not 
-0001dc00: 5365 6173 6f6e 616c 6c79 2041 646a 7573  Seasonally Adjus
-0001dc10: 7465 6420 2020 2020 2020 2020 2020 2020  ted             
-0001dc20: 2020 2020 2020 2020 2020 4e53 4120 3230            NSA 20
-0001dc30: 3232 2d30 322d 3035 2030 313a 3131 3a30  22-02-05 01:11:0
-0001dc40: 342b 3030 3a30 3020 2020 2020 2020 2020  4+00:00         
-0001dc50: 2038 3520 2054 6865 206f 6273 6572 7661   85  The observa
-0001dc60: 7469 6f6e 7320 666f 7220 7468 6520 5326  tions for the S&
-0001dc70: 5020 3530 3020 7265 7072 6573 656e 7420  P 500 represent 
-0001dc80: 7468 652e 2e2e 0d0a 2020 2020 2020 2020  the.....        
-0001dc90: 2020 2020 4342 4243 4855 5344 2020 2020      CBBCHUSD    
-0001dca0: 2032 3032 322d 3032 2d30 3520 2020 3230   2022-02-05   20
-0001dcb0: 3232 2d30 322d 3035 2020 436f 696e 6261  22-02-05  Coinba
-0001dcc0: 7365 2042 6974 636f 696e 2043 6173 6820  se Bitcoin Cash 
-0001dcd0: 2020 2020 2020 2032 3031 372d 3132 2d32         2017-12-2
-0001dce0: 3020 2020 2020 2032 3032 322d 3032 2d30  0      2022-02-0
-0001dcf0: 3420 2044 6169 6c79 2c20 372d 4461 7920  4  Daily, 7-Day 
-0001dd00: 2020 2020 2020 2020 2020 2020 2020 4420                D 
-0001dd10: 2055 2e53 2e20 446f 6c6c 6172 7320 2020   U.S. Dollars   
-0001dd20: 2020 2055 2e53 2e20 2420 204e 6f74 2053     U.S. $  Not S
-0001dd30: 6561 736f 6e61 6c6c 7920 4164 6a75 7374  easonally Adjust
-0001dd40: 6564 2020 2020 2020 2020 2020 2020 2020  ed              
-0001dd50: 2020 2020 2020 2020 204e 5341 2032 3032           NSA 202
-0001dd60: 322d 3032 2d30 3520 3031 3a30 343a 3037  2-02-05 01:04:07
-0001dd70: 2b30 303a 3030 2020 2020 2020 2020 2020  +00:00          
-0001dd80: 3232 2020 416c 6c20 6461 7461 2069 7320  22  All data is 
-0001dd90: 6173 206f 6620 3520 504d 2050 5354 2e0d  as of 5 PM PST..
-0001dda0: 0a20 2020 2020 2020 2020 2020 2043 4242  .            CBB
-0001ddb0: 5443 5553 4420 2020 2020 3230 3232 2d30  TCUSD     2022-0
-0001ddc0: 322d 3035 2020 2032 3032 322d 3032 2d30  2-05   2022-02-0
-0001ddd0: 3520 2020 2020 2020 436f 696e 6261 7365  5       Coinbase
-0001dde0: 2042 6974 636f 696e 2020 2020 2020 2020   Bitcoin        
-0001ddf0: 3230 3134 2d31 322d 3031 2020 2020 2020  2014-12-01      
-0001de00: 3230 3232 2d30 322d 3034 2020 4461 696c  2022-02-04  Dail
-0001de10: 792c 2037 2d44 6179 2020 2020 2020 2020  y, 7-Day        
-0001de20: 2020 2020 2020 2044 2020 552e 532e 2044         D  U.S. D
-0001de30: 6f6c 6c61 7273 2020 2020 2020 552e 532e  ollars      U.S.
-0001de40: 2024 2020 4e6f 7420 5365 6173 6f6e 616c   $  Not Seasonal
-0001de50: 6c79 2041 646a 7573 7465 6420 2020 2020  ly Adjusted     
-0001de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de70: 2020 4e53 4120 3230 3232 2d30 322d 3035    NSA 2022-02-05
-0001de80: 2030 313a 3034 3a30 362b 3030 3a30 3020   01:04:06+00:00 
-0001de90: 2020 2020 2020 2020 2036 3520 2041 6c6c           65  All
-0001dea0: 2064 6174 6120 6973 2061 7320 6f66 2035   data is as of 5
-0001deb0: 2050 4d20 5053 542e 0d0a 2020 2020 2020   PM PST...      
-0001dec0: 2020 2020 2020 4342 4554 4855 5344 2020        CBETHUSD  
-0001ded0: 2020 2032 3032 322d 3032 2d30 3520 2020     2022-02-05   
-0001dee0: 3230 3232 2d30 322d 3035 2020 2020 2020  2022-02-05      
-0001def0: 436f 696e 6261 7365 2045 7468 6572 6575  Coinbase Ethereu
-0001df00: 6d20 2020 2020 2020 2032 3031 362d 3035  m        2016-05
-0001df10: 2d31 3820 2020 2020 2032 3032 322d 3032  -18      2022-02
-0001df20: 2d30 3420 2044 6169 6c79 2c20 372d 4461  -04  Daily, 7-Da
-0001df30: 7920 2020 2020 2020 2020 2020 2020 2020  y               
-0001df40: 4420 2055 2e53 2e20 446f 6c6c 6172 7320  D  U.S. Dollars 
-0001df50: 2020 2020 2055 2e53 2e20 2420 204e 6f74       U.S. $  Not
-0001df60: 2053 6561 736f 6e61 6c6c 7920 4164 6a75   Seasonally Adju
-0001df70: 7374 6564 2020 2020 2020 2020 2020 2020  sted            
-0001df80: 2020 2020 2020 2020 2020 204e 5341 2032             NSA 2
-0001df90: 3032 322d 3032 2d30 3520 3031 3a30 343a  022-02-05 01:04:
-0001dfa0: 3035 2b30 303a 3030 2020 2020 2020 2020  05+00:00        
-0001dfb0: 2020 3434 2020 416c 6c20 6461 7461 2069    44  All data i
-0001dfc0: 7320 6173 206f 6620 3520 504d 2050 5354  s as of 5 PM PST
-0001dfd0: 2e0d 0a20 2020 2020 2020 2020 2020 2043  ...            C
-0001dfe0: 424c 5443 5553 4420 2020 2020 3230 3232  BLTCUSD     2022
-0001dff0: 2d30 322d 3035 2020 2032 3032 322d 3032  -02-05   2022-02
-0001e000: 2d30 3520 2020 2020 2043 6f69 6e62 6173  -05      Coinbas
-0001e010: 6520 4c69 7465 636f 696e 2020 2020 2020  e Litecoin      
-0001e020: 2020 3230 3136 2d30 382d 3137 2020 2020    2016-08-17    
-0001e030: 2020 3230 3232 2d30 322d 3034 2020 4461    2022-02-04  Da
-0001e040: 696c 792c 2037 2d44 6179 2020 2020 2020  ily, 7-Day      
-0001e050: 2020 2020 2020 2020 2044 2020 552e 532e           D  U.S.
-0001e060: 2044 6f6c 6c61 7273 2020 2020 2020 552e   Dollars      U.
-0001e070: 532e 2024 2020 4e6f 7420 5365 6173 6f6e  S. $  Not Season
-0001e080: 616c 6c79 2041 646a 7573 7465 6420 2020  ally Adjusted   
-0001e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0a0: 2020 2020 4e53 4120 3230 3232 2d30 322d      NSA 2022-02-
-0001e0b0: 3035 2030 313a 3034 3a30 332b 3030 3a30  05 01:04:03+00:0
-0001e0c0: 3020 2020 2020 2020 2020 2032 3020 2041  0          20  A
-0001e0d0: 6c6c 2064 6174 6120 6973 2061 7320 6f66  ll data is as of
-0001e0e0: 2035 2050 4d20 5053 542e 0d0a 2020 2020   5 PM PST...    
-0001e0f0: 2020 2020 6060 600d 0a20 2020 2020 2020      ```..       
-0001e100: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-0001e110: 6966 2066 696c 7465 725f 7661 6c75 6520  if filter_value 
-0001e120: 6e6f 7420 696e 2065 6e75 6d73 2e46 696c  not in enums.Fil
-0001e130: 7465 7256 616c 7565 3a0d 0a20 2020 2020  terValue:..     
-0001e140: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0001e150: 7565 4572 726f 7228 2756 6172 6961 626c  ueError('Variabl
-0001e160: 6520 6669 6c74 6572 5f76 616c 7565 2028  e filter_value (
-0001e170: 7b7d 2920 6973 206e 6f74 206f 6e65 206f  {}) is not one o
-0001e180: 6620 7468 6520 7661 6c75 6573 3a20 7b7d  f the values: {}
-0001e190: 272e 666f 726d 6174 2866 696c 7465 725f  '.format(filter_
-0001e1a0: 7661 6c75 652c 2027 2c20 272e 6a6f 696e  value, ', '.join
-0001e1b0: 286d 6170 2873 7472 2c20 656e 756d 732e  (map(str, enums.
-0001e1c0: 4669 6c74 6572 5661 6c75 6529 2929 290d  FilterValue)))).
-0001e1d0: 0a0d 0a20 2020 2020 2020 2069 6620 7374  ...        if st
-0001e1e0: 6172 745f 7469 6d65 2069 7320 6e6f 7420  art_time is not 
-0001e1f0: 4e6f 6e65 2061 6e64 2065 6e64 5f74 696d  None and end_tim
-0001e200: 6520 6973 204e 6f6e 653a 0d0a 2020 2020  e is None:..    
-0001e210: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0001e220: 6c75 6545 7272 6f72 2827 656e 645f 7469  lueError('end_ti
-0001e230: 6d65 2069 7320 7265 7175 6972 6564 2069  me is required i
-0001e240: 6620 7374 6172 745f 7469 6d65 2069 7320  f start_time is 
-0001e250: 7365 7427 290d 0a0d 0a20 2020 2020 2020  set')....       
-0001e260: 2069 6620 656e 645f 7469 6d65 2069 7320   if end_time is 
-0001e270: 6e6f 7420 4e6f 6e65 2061 6e64 2073 7461  not None and sta
-0001e280: 7274 5f74 696d 6520 6973 204e 6f6e 653a  rt_time is None:
-0001e290: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-0001e2a0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-0001e2b0: 7374 6172 745f 7469 6d65 2069 7320 7265  start_time is re
-0001e2c0: 7175 6972 6564 2069 6620 656e 645f 7469  quired if end_ti
-0001e2d0: 6d65 2069 7320 7365 7427 290d 0a0d 0a20  me is set').... 
-0001e2e0: 2020 2020 2020 2069 6620 7374 6172 745f         if start_
-0001e2f0: 7469 6d65 2069 7320 6e6f 7420 4e6f 6e65  time is not None
-0001e300: 2061 6e64 2065 6e64 5f74 696d 6520 6973   and end_time is
-0001e310: 206e 6f74 204e 6f6e 6520 616e 6420 7374   not None and st
-0001e320: 6172 745f 7469 6d65 203e 3d20 656e 645f  art_time >= end_
-0001e330: 7469 6d65 3a0d 0a20 2020 2020 2020 2020  time:..         
-0001e340: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0001e350: 726f 7228 2765 6e64 5f74 696d 6520 6d75  ror('end_time mu
-0001e360: 7374 2062 6520 6772 6561 7465 7220 7468  st be greater th
-0001e370: 616e 2073 7461 7274 5f74 696d 6527 290d  an start_time').
-0001e380: 0a0d 0a20 2020 2020 2020 2069 6620 7265  ...        if re
-0001e390: 616c 7469 6d65 5f73 7461 7274 2069 7320  altime_start is 
-0001e3a0: 6e6f 7420 4e6f 6e65 2061 6e64 2072 6561  not None and rea
-0001e3b0: 6c74 696d 655f 7374 6172 7420 3c20 6461  ltime_start < da
-0001e3c0: 7465 2831 3737 362c 2037 2c20 3429 3a0d  te(1776, 7, 4):.
-0001e3d0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001e3e0: 7365 2056 616c 7565 4572 726f 7228 2756  se ValueError('V
-0001e3f0: 6172 6961 626c 6520 7265 616c 7469 6d65  ariable realtime
-0001e400: 5f73 7461 7274 2028 227b 7d22 2920 6973  _start ("{}") is
-0001e410: 2062 6566 6f72 6520 6d69 6e20 6461 7465   before min date
-0001e420: 2031 3737 362d 3037 2d30 342e 272e 666f   1776-07-04.'.fo
-0001e430: 726d 6174 2872 6561 6c74 696d 655f 7374  rmat(realtime_st
-0001e440: 6172 7429 290d 0a0d 0a20 2020 2020 2020  art))....       
-0001e450: 2069 6620 7265 616c 7469 6d65 5f73 7461   if realtime_sta
-0001e460: 7274 2069 7320 6e6f 7420 4e6f 6e65 2061  rt is not None a
-0001e470: 6e64 2072 6561 6c74 696d 655f 656e 6420  nd realtime_end 
-0001e480: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0001e490: 7265 616c 7469 6d65 5f73 7461 7274 203e  realtime_start >
-0001e4a0: 2072 6561 6c74 696d 655f 656e 643a 0d0a   realtime_end:..
-0001e4b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0001e4c0: 6520 5661 6c75 6545 7272 6f72 2827 5468  e ValueError('Th
-0001e4d0: 6520 6461 7465 2073 6574 2062 7920 7661  e date set by va
-0001e4e0: 7269 6162 6c65 2072 6561 6c74 696d 655f  riable realtime_
-0001e4f0: 7374 6172 7420 2822 7b7d 2229 2063 616e  start ("{}") can
-0001e500: 206e 6f74 2062 6520 6166 7465 7220 7468   not be after th
-0001e510: 6520 6461 7465 2073 6574 2062 7920 7661  e date set by va
-0001e520: 7269 6162 6c65 2072 6561 6c74 696d 655f  riable realtime_
-0001e530: 656e 6420 2822 7b7d 2229 2e27 2e66 6f72  end ("{}").'.for
-0001e540: 6d61 7428 7265 616c 7469 6d65 5f73 7461  mat(realtime_sta
-0001e550: 7274 2c20 7265 616c 7469 6d65 5f65 6e64  rt, realtime_end
-0001e560: 2929 0d0a 0d0a 2020 2020 2020 2020 6466  ))....        df
-0001e570: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-0001e580: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0001e590: 6c66 2e5f 636c 6965 6e74 2e67 6574 280d  lf._client.get(.
-0001e5a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e5b0: 2027 2f66 7265 642f 7365 7269 6573 2f75   '/fred/series/u
-0001e5c0: 7064 6174 6573 272c 0d0a 2020 2020 2020  pdates',..      
-0001e5d0: 2020 2020 2020 2020 2020 2773 6572 6965            'serie
-0001e5e0: 7373 272c 0d0a 2020 2020 2020 2020 2020  ss',..          
-0001e5f0: 2020 2020 2020 6c69 6d69 743d 3130 3030        limit=1000
-0001e600: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001e610: 2020 2072 6561 6c74 696d 655f 7374 6172     realtime_star
-0001e620: 743d 7265 616c 7469 6d65 5f73 7461 7274  t=realtime_start
-0001e630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001e640: 2020 2072 6561 6c74 696d 655f 656e 643d     realtime_end=
-0001e650: 7265 616c 7469 6d65 5f65 6e64 2c0d 0a20  realtime_end,.. 
-0001e660: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001e670: 696c 7465 725f 7661 6c75 653d 6669 6c74  ilter_value=filt
-0001e680: 6572 5f76 616c 7565 2c0d 0a20 2020 2020  er_value,..     
-0001e690: 2020 2020 2020 2020 2020 2073 7461 7274             start
-0001e6a0: 5f74 696d 653d 7374 6172 745f 7469 6d65  _time=start_time
-0001e6b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001e6c0: 2020 2065 6e64 5f74 696d 653d 656e 645f     end_time=end_
-0001e6d0: 7469 6d65 0d0a 2020 2020 2020 2020 2020  time..          
-0001e6e0: 2020 290d 0a20 2020 2020 2020 2029 0d0a    )..        )..
-0001e6f0: 0d0a 2020 2020 2020 2020 6461 7465 5f63  ..        date_c
-0001e700: 6f6c 756d 6e73 203d 205b 0d0a 2020 2020  olumns = [..    
-0001e710: 2020 2020 2020 2020 2772 6561 6c74 696d          'realtim
-0001e720: 655f 7374 6172 7427 2c20 2772 6561 6c74  e_start', 'realt
-0001e730: 696d 655f 656e 6427 2c0d 0a20 2020 2020  ime_end',..     
-0001e740: 2020 2020 2020 2027 6f62 7365 7276 6174         'observat
-0001e750: 696f 6e5f 7374 6172 7427 2c20 276f 6273  ion_start', 'obs
-0001e760: 6572 7661 7469 6f6e 5f65 6e64 270d 0a20  ervation_end'.. 
-0001e770: 2020 2020 2020 205d 0d0a 0d0a 2020 2020         ]....    
-0001e780: 2020 2020 6966 206e 6f74 2064 662e 656d      if not df.em
-0001e790: 7074 793a 0d0a 2020 2020 2020 2020 2020  pty:..          
-0001e7a0: 2020 6466 5b64 6174 655f 636f 6c75 6d6e    df[date_column
-0001e7b0: 735d 203d 2064 665b 6461 7465 5f63 6f6c  s] = df[date_col
-0001e7c0: 756d 6e73 5d2e 6170 706c 7928 7064 2e74  umns].apply(pd.t
-0001e7d0: 6f5f 6461 7465 7469 6d65 2c20 666f 726d  o_datetime, form
-0001e7e0: 6174 3d27 2559 2d25 6d2d 2564 2729 0d0a  at='%Y-%m-%d')..
-0001e7f0: 2020 2020 2020 2020 2020 2020 6466 2e6c              df.l
-0001e800: 6173 745f 7570 6461 7465 6420 3d20 7064  ast_updated = pd
-0001e810: 2e74 6f5f 6461 7465 7469 6d65 2864 662e  .to_datetime(df.
-0001e820: 6c61 7374 5f75 7064 6174 6564 202b 2027  last_updated + '
-0001e830: 3030 272c 2075 7463 3d54 7275 652c 2066  00', utc=True, f
-0001e840: 6f72 6d61 743d 2725 592d 256d 2d25 6420  ormat='%Y-%m-%d 
-0001e850: 2548 3a25 4d3a 2553 257a 2729 0d0a 0d0a  %H:%M:%S%z')....
-0001e860: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-0001e870: 2064 662e 6173 7479 7065 2864 7479 7065   df.astype(dtype
-0001e880: 3d7b 0d0a 2020 2020 2020 2020 2020 2020  ={..            
-0001e890: 2020 2020 2769 6427 3a20 2773 7472 696e      'id': 'strin
-0001e8a0: 6727 2c0d 0a20 2020 2020 2020 2020 2020  g',..           
-0001e8b0: 2020 2020 2027 6e6f 7465 7327 3a20 2773       'notes': 's
-0001e8c0: 7472 696e 6727 2c0d 0a20 2020 2020 2020  tring',..       
-0001e8d0: 2020 2020 2020 2020 2027 7469 746c 6527           'title'
-0001e8e0: 3a20 2773 7472 696e 6727 2c0d 0a20 2020  : 'string',..   
-0001e8f0: 2020 2020 2020 2020 2020 2020 2027 7365               'se
-0001e900: 6173 6f6e 616c 5f61 646a 7573 746d 656e  asonal_adjustmen
-0001e910: 7427 3a20 2763 6174 6567 6f72 7927 2c0d  t': 'category',.
-0001e920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e930: 2027 7365 6173 6f6e 616c 5f61 646a 7573   'seasonal_adjus
-0001e940: 746d 656e 745f 7368 6f72 7427 3a20 2763  tment_short': 'c
-0001e950: 6174 6567 6f72 7927 2c0d 0a20 2020 2020  ategory',..     
-0001e960: 2020 2020 2020 2020 2020 2027 756e 6974             'unit
-0001e970: 7327 3a20 2763 6174 6567 6f72 7927 2c0d  s': 'category',.
-0001e980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e990: 2027 756e 6974 735f 7368 6f72 7427 3a20   'units_short': 
-0001e9a0: 2763 6174 6567 6f72 7927 2c0d 0a20 2020  'category',..   
-0001e9b0: 2020 2020 2020 2020 2020 2020 2027 6672               'fr
-0001e9c0: 6571 7565 6e63 7927 3a20 2763 6174 6567  equency': 'categ
-0001e9d0: 6f72 7927 2c0d 0a20 2020 2020 2020 2020  ory',..         
-0001e9e0: 2020 2020 2020 2027 6672 6571 7565 6e63         'frequenc
-0001e9f0: 795f 7368 6f72 7427 3a20 2763 6174 6567  y_short': 'categ
-0001ea00: 6f72 7927 2c0d 0a20 2020 2020 2020 2020  ory',..         
-0001ea10: 2020 207d 292e 7365 745f 696e 6465 7828     }).set_index(
-0001ea20: 2769 6427 290d 0a0d 0a20 2020 2020 2020  'id')....       
-0001ea30: 2072 6574 7572 6e20 6466 0d0a 0d0a 2020   return df....  
-0001ea40: 2020 6465 6620 7365 7269 6573 5f76 696e    def series_vin
-0001ea50: 7461 6765 6461 7465 7328 0d0a 2020 2020  tagedates(..    
-0001ea60: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-0001ea70: 2020 2020 2020 2020 2020 2073 6572 6965             serie
-0001ea80: 735f 6964 3a20 7374 722c 0d0a 2020 2020  s_id: str,..    
-0001ea90: 2020 2020 2020 2020 7265 616c 7469 6d65          realtime
-0001eaa0: 5f73 7461 7274 3a20 6461 7465 203d 2064  _start: date = d
-0001eab0: 6174 6528 3137 3736 2c20 372c 2034 292c  ate(1776, 7, 4),
-0001eac0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001ead0: 616c 7469 6d65 5f65 6e64 3a20 6461 7465  altime_end: date
-0001eae0: 203d 2064 6174 6528 3939 3939 2c20 3132   = date(9999, 12
-0001eaf0: 2c20 3331 292c 0d0a 2020 2020 2020 2020  , 31),..        
-0001eb00: 2020 2020 736f 7274 5f6f 7264 6572 3a20      sort_order: 
-0001eb10: 656e 756d 732e 536f 7274 4f72 6465 7220  enums.SortOrder 
-0001eb20: 3d20 656e 756d 732e 536f 7274 4f72 6465  = enums.SortOrde
-0001eb30: 722e 6173 630d 0a20 2020 2029 202d 3e20  r.asc..    ) -> 
-0001eb40: 7064 2e53 6572 6965 733a 0d0a 2020 2020  pd.Series:..    
-0001eb50: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0001eb60: 2023 2320 5061 7261 6d65 7465 7273 0d0a   ## Parameters..
-0001eb70: 2020 2020 2020 2020 6073 6572 6965 735f          `series_
-0001eb80: 6964 600d 0a20 2020 2020 2020 2054 6865  id`..        The
-0001eb90: 2069 6420 666f 7220 6120 7365 7269 6573   id for a series
-0001eba0: 2e0d 0a0d 0a20 2020 2020 2020 2060 7265  .....        `re
-0001ebb0: 616c 7469 6d65 5f73 7461 7274 600d 0a20  altime_start`.. 
-0001ebc0: 2020 2020 2020 2054 6865 2073 7461 7274         The start
-0001ebd0: 206f 6620 7468 6520 7265 616c 2d74 696d   of the real-tim
-0001ebe0: 6520 7065 7269 6f64 2e20 466f 7220 6d6f  e period. For mo
-0001ebf0: 7265 2069 6e66 6f72 6d61 7469 6f6e 2c20  re information, 
-0001ec00: 7365 6520 5b52 6561 6c2d 5469 6d65 2050  see [Real-Time P
-0001ec10: 6572 696f 6473 5d28 6874 7470 733a 2f2f  eriods](https://
-0001ec20: 6672 6564 2e73 746c 6f75 6973 6665 642e  fred.stlouisfed.
-0001ec30: 6f72 672f 646f 6373 2f61 7069 2f66 7265  org/docs/api/fre
-0001ec40: 642f 7265 616c 7469 6d65 5f70 6572 696f  d/realtime_perio
-0001ec50: 642e 6874 6d6c 292e 0d0a 0d0a 2020 2020  d.html).....    
-0001ec60: 2020 2020 6072 6561 6c74 696d 655f 656e      `realtime_en
-0001ec70: 6460 0d0a 2020 2020 2020 2020 5468 6520  d`..        The 
-0001ec80: 656e 6420 6f66 2074 6865 2072 6561 6c2d  end of the real-
-0001ec90: 7469 6d65 2070 6572 696f 642e 2046 6f72  time period. For
-0001eca0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-0001ecb0: 6e2c 2073 6565 205b 5265 616c 2d54 696d  n, see [Real-Tim
-0001ecc0: 6520 5065 7269 6f64 735d 2868 7474 7073  e Periods](https
-0001ecd0: 3a2f 2f66 7265 642e 7374 6c6f 7569 7366  ://fred.stlouisf
-0001ece0: 6564 2e6f 7267 2f64 6f63 732f 6170 692f  ed.org/docs/api/
-0001ecf0: 6672 6564 2f72 6561 6c74 696d 655f 7065  fred/realtime_pe
-0001ed00: 7269 6f64 2e68 746d 6c29 2e0d 0a0d 0a20  riod.html)..... 
-0001ed10: 2020 2020 2020 2060 736f 7274 5f6f 7264         `sort_ord
-0001ed20: 6572 600d 0a20 2020 2020 2020 2053 6f72  er`..        Sor
-0001ed30: 7420 7265 7375 6c74 7320 6973 2061 7363  t results is asc
-0001ed40: 656e 6469 6e67 206f 7220 6465 7363 656e  ending or descen
-0001ed50: 6469 6e67 206f 7264 6572 2066 6f72 2061  ding order for a
-0001ed60: 7474 7269 6275 7465 2076 616c 7565 7320  ttribute values 
-0001ed70: 7370 6563 6966 6965 6420 6279 206f 7264  specified by ord
-0001ed80: 6572 5f62 792e 0d0a 0d0a 2020 2020 2020  er_by.....      
-0001ed90: 2020 2323 2044 6573 6372 6970 7469 6f6e    ## Description
-0001eda0: 0d0a 2020 2020 2020 2020 6874 7470 733a  ..        https:
-0001edb0: 2f2f 6672 6564 2e73 746c 6f75 6973 6665  //fred.stlouisfe
-0001edc0: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
-0001edd0: 7265 642f 7365 7269 6573 5f76 696e 7461  red/series_vinta
-0001ede0: 6765 6461 7465 732e 6874 6d6c 0d0a 0d0a  gedates.html....
-0001edf0: 2020 2020 2020 2020 4765 7420 7468 6520          Get the 
-0001ee00: 6461 7465 7320 696e 2068 6973 746f 7279  dates in history
-0001ee10: 2077 6865 6e20 6120 7365 7269 6573 2720   when a series' 
-0001ee20: 6461 7461 2076 616c 7565 7320 7765 7265  data values were
-0001ee30: 2072 6576 6973 6564 206f 7220 6e65 7720   revised or new 
-0001ee40: 6461 7461 2076 616c 7565 7320 7765 7265  data values were
-0001ee50: 2072 656c 6561 7365 642e 0d0a 2020 2020   released...    
-0001ee60: 2020 2020 5669 6e74 6167 6520 6461 7465      Vintage date
-0001ee70: 7320 6172 6520 7468 6520 7265 6c65 6173  s are the releas
-0001ee80: 6520 6461 7465 7320 666f 7220 6120 7365  e dates for a se
-0001ee90: 7269 6573 2065 7863 6c75 6469 6e67 2072  ries excluding r
-0001eea0: 656c 6561 7365 2064 6174 6573 2077 6865  elease dates whe
-0001eeb0: 6e20 7468 6520 6461 7461 2066 6f72 2074  n the data for t
-0001eec0: 6865 2073 6572 6965 7320 6469 6420 6e6f  he series did no
-0001eed0: 7420 6368 616e 6765 2e0d 0a0d 0a20 2020  t change.....   
-0001eee0: 2020 2020 2023 2320 4150 4920 5265 7175       ## API Requ
-0001eef0: 6573 7420 2848 5454 5053 2047 4554 290d  est (HTTPS GET).
-0001ef00: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
-0001ef10: 2f61 7069 2e73 746c 6f75 6973 6665 642e  /api.stlouisfed.
-0001ef20: 6f72 672f 6672 6564 2f73 6572 6965 732f  org/fred/series/
-0001ef30: 7669 6e74 6167 6564 6174 6573 3f73 6572  vintagedates?ser
-0001ef40: 6965 735f 6964 3d47 4e50 4341 2661 7069  ies_id=GNPCA&api
-0001ef50: 5f6b 6579 3d61 6263 6465 6667 6869 6a6b  _key=abcdefghijk
-0001ef60: 6c6d 6e6f 7071 7273 7475 7677 7879 7a31  lmnopqrstuvwxyz1
-0001ef70: 3233 3435 3626 6669 6c65 5f74 7970 653d  23456&file_type=
-0001ef80: 6a73 6f6e 0d0a 0d0a 2020 2020 2020 2020  json....        
-0001ef90: 2323 2041 5049 2052 6573 706f 6e73 650d  ## API Response.
-0001efa0: 0a20 2020 2020 2020 2060 6060 6a73 6f6e  .        ```json
-0001efb0: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-0001efc0: 2020 2020 2020 2020 2022 7265 616c 7469           "realti
-0001efd0: 6d65 5f73 7461 7274 223a 2022 3137 3736  me_start": "1776
-0001efe0: 2d30 372d 3034 222c 0d0a 2020 2020 2020  -07-04",..      
-0001eff0: 2020 2020 2020 2272 6561 6c74 696d 655f        "realtime_
-0001f000: 656e 6422 3a20 2239 3939 392d 3132 2d33  end": "9999-12-3
-0001f010: 3122 2c0d 0a20 2020 2020 2020 2020 2020  1",..           
-0001f020: 2022 6f72 6465 725f 6279 223a 2022 7669   "order_by": "vi
-0001f030: 6e74 6167 655f 6461 7465 222c 0d0a 2020  ntage_date",..  
-0001f040: 2020 2020 2020 2020 2020 2273 6f72 745f            "sort_
-0001f050: 6f72 6465 7222 3a20 2261 7363 222c 0d0a  order": "asc",..
-0001f060: 2020 2020 2020 2020 2020 2020 2263 6f75              "cou
-0001f070: 6e74 223a 2031 3632 2c0d 0a20 2020 2020  nt": 162,..     
-0001f080: 2020 2020 2020 2022 6f66 6673 6574 223a         "offset":
-0001f090: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
-0001f0a0: 2022 6c69 6d69 7422 3a20 3130 3030 302c   "limit": 10000,
-0001f0b0: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-0001f0c0: 696e 7461 6765 5f64 6174 6573 223a 205b  intage_dates": [
-0001f0d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001f0e0: 2020 2231 3935 382d 3132 2d32 3122 2c0d    "1958-12-21",.
-0001f0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f100: 2022 3139 3539 2d30 322d 3139 222c 0d0a   "1959-02-19",..
-0001f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f120: 2e2e 2e0d 0a20 2020 2020 2020 2020 2020  .....           
-0001f130: 205d 0d0a 2020 2020 2020 2020 7d0d 0a20   ]..        }.. 
-0001f140: 2020 2020 2020 2060 6060 0d0a 0d0a 2020         ```....  
-0001f150: 2020 2020 2020 2323 2052 6574 7572 6e73        ## Returns
-0001f160: 0d0a 2020 2020 2020 2020 6070 616e 6461  ..        `panda
-0001f170: 732e 5365 7269 6573 600d 0a0d 0a20 2020  s.Series`....   
-0001f180: 2020 2020 2023 2320 4578 616d 706c 650d       ## Example.
-0001f190: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
-0001f1a0: 6f6e 0d0a 2020 2020 2020 2020 3e3e 3e20  on..        >>> 
-0001f1b0: 6672 6564 203d 2046 5245 4428 6170 695f  fred = FRED(api_
-0001f1c0: 6b65 793d 2761 6263 6465 6667 6869 6a6b  key='abcdefghijk
-0001f1d0: 6c6d 6e6f 7071 7273 7475 7677 7879 7a31  lmnopqrstuvwxyz1
-0001f1e0: 3233 3435 3627 290d 0a20 2020 2020 2020  23456')..       
-0001f1f0: 203e 3e3e 2066 7265 642e 7365 7269 6573   >>> fred.series
-0001f200: 5f76 696e 7461 6765 6461 7465 7328 7365  _vintagedates(se
-0001f210: 7269 6573 5f69 643d 2747 4e50 4341 2729  ries_id='GNPCA')
-0001f220: 2e68 6561 6428 290d 0a20 2020 2020 2020  .head()..       
-0001f230: 2020 2020 2030 2020 2020 3139 3538 2d31       0    1958-1
-0001f240: 322d 3231 0d0a 2020 2020 2020 2020 2020  2-21..          
-0001f250: 2020 3120 2020 2031 3935 392d 3032 2d31    1    1959-02-1
-0001f260: 390d 0a20 2020 2020 2020 2020 2020 2032  9..            2
-0001f270: 2020 2020 3139 3539 2d30 372d 3139 0d0a      1959-07-19..
-0001f280: 2020 2020 2020 2020 2020 2020 3320 2020              3   
-0001f290: 2031 3936 302d 3032 2d31 360d 0a20 2020   1960-02-16..   
-0001f2a0: 2020 2020 2020 2020 2034 2020 2020 3139           4    19
-0001f2b0: 3630 2d30 372d 3232 0d0a 2020 2020 2020  60-07-22..      
-0001f2c0: 2020 6060 600d 0a20 2020 2020 2020 2022    ```..        "
-0001f2d0: 2222 0d0a 0d0a 2020 2020 2020 2020 6966  ""....        if
-0001f2e0: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
-0001f2f0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0001f300: 7265 616c 7469 6d65 5f73 7461 7274 203c  realtime_start <
-0001f310: 2064 6174 6528 3137 3736 2c20 372c 2034   date(1776, 7, 4
-0001f320: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0001f330: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0001f340: 2827 5661 7269 6162 6c65 2072 6561 6c74  ('Variable realt
-0001f350: 696d 655f 7374 6172 7420 2822 7b7d 2229  ime_start ("{}")
-0001f360: 2069 7320 6265 666f 7265 206d 696e 2064   is before min d
-0001f370: 6174 6520 3137 3736 2d30 372d 3034 2e27  ate 1776-07-04.'
-0001f380: 2e66 6f72 6d61 7428 7265 616c 7469 6d65  .format(realtime
-0001f390: 5f73 7461 7274 2929 0d0a 0d0a 2020 2020  _start))....    
-0001f3a0: 2020 2020 6966 2072 6561 6c74 696d 655f      if realtime_
-0001f3b0: 7374 6172 7420 3e20 7265 616c 7469 6d65  start > realtime
-0001f3c0: 5f65 6e64 3a0d 0a20 2020 2020 2020 2020  _end:..         
-0001f3d0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0001f3e0: 726f 7228 2754 6865 2064 6174 6520 7365  ror('The date se
-0001f3f0: 7420 6279 2076 6172 6961 626c 6520 7265  t by variable re
-0001f400: 616c 7469 6d65 5f73 7461 7274 2028 227b  altime_start ("{
-0001f410: 7d22 2920 6361 6e20 6e6f 7420 6265 2061  }") can not be a
-0001f420: 6674 6572 2074 6865 2064 6174 6520 7365  fter the date se
-0001f430: 7420 6279 2076 6172 6961 626c 6520 7265  t by variable re
-0001f440: 616c 7469 6d65 5f65 6e64 2028 227b 7d22  altime_end ("{}"
-0001f450: 292e 272e 666f 726d 6174 2872 6561 6c74  ).'.format(realt
-0001f460: 696d 655f 7374 6172 742c 2072 6561 6c74  ime_start, realt
-0001f470: 696d 655f 656e 6429 290d 0a0d 0a20 2020  ime_end))....   
-0001f480: 2020 2020 2072 6574 7572 6e20 7064 2e74       return pd.t
-0001f490: 6f5f 6461 7465 7469 6d65 280d 0a20 2020  o_datetime(..   
-0001f4a0: 2020 2020 2020 2020 2070 642e 5365 7269           pd.Seri
-0001f4b0: 6573 280d 0a20 2020 2020 2020 2020 2020  es(..           
-0001f4c0: 2020 2020 2073 656c 662e 5f63 6c69 656e       self._clien
-0001f4d0: 742e 6765 7428 0d0a 2020 2020 2020 2020  t.get(..        
-0001f4e0: 2020 2020 2020 2020 2020 2020 272f 6672              '/fr
-0001f4f0: 6564 2f73 6572 6965 732f 7669 6e74 6167  ed/series/vintag
-0001f500: 6564 6174 6573 272c 0d0a 2020 2020 2020  edates',..      
-0001f510: 2020 2020 2020 2020 2020 2020 2020 2776                'v
-0001f520: 696e 7461 6765 5f64 6174 6573 272c 0d0a  intage_dates',..
-0001f530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f540: 2020 2020 6c69 6d69 743d 3130 3030 302c      limit=10000,
-0001f550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001f560: 2020 2020 2020 7365 7269 6573 5f69 643d        series_id=
-0001f570: 7365 7269 6573 5f69 642c 0d0a 2020 2020  series_id,..    
-0001f580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f590: 7265 616c 7469 6d65 5f73 7461 7274 3d72  realtime_start=r
-0001f5a0: 6561 6c74 696d 655f 7374 6172 742c 0d0a  ealtime_start,..
-0001f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f5c0: 2020 2020 7265 616c 7469 6d65 5f65 6e64      realtime_end
-0001f5d0: 3d72 6561 6c74 696d 655f 656e 642c 0d0a  =realtime_end,..
-0001f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f5f0: 2020 2020 736f 7274 5f6f 7264 6572 3d73      sort_order=s
-0001f600: 6f72 745f 6f72 6465 720d 0a20 2020 2020  ort_order..     
-0001f610: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-0001f620: 2020 2020 2020 2020 2020 292c 2066 6f72            ), for
-0001f630: 6d61 743d 2725 592d 256d 2d25 6427 0d0a  mat='%Y-%m-%d'..
-0001f640: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-0001f650: 2022 2222 0d0a 2020 2020 536f 7572 6365   """..    Source
-0001f660: 730d 0a0d 0a20 2020 2068 7474 7073 3a2f  s....    https:/
-0001f670: 2f66 7265 642e 7374 6c6f 7569 7366 6564  /fred.stlouisfed
-0001f680: 2e6f 7267 2f73 6f75 7263 6573 0d0a 2020  .org/sources..  
-0001f690: 2020 2222 220d 0a0d 0a20 2020 2064 6566    """....    def
-0001f6a0: 2073 6f75 7263 6573 280d 0a20 2020 2020   sources(..     
-0001f6b0: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-0001f6c0: 2020 2020 2020 2020 2020 7265 616c 7469            realti
-0001f6d0: 6d65 5f73 7461 7274 3a20 6461 7465 203d  me_start: date =
-0001f6e0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-0001f6f0: 2020 2020 7265 616c 7469 6d65 5f65 6e64      realtime_end
-0001f700: 3a20 6461 7465 203d 204e 6f6e 652c 0d0a  : date = None,..
-0001f710: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-0001f720: 725f 6279 3a20 656e 756d 732e 4f72 6465  r_by: enums.Orde
-0001f730: 7242 7920 3d20 656e 756d 732e 4f72 6465  rBy = enums.Orde
-0001f740: 7242 792e 736f 7572 6365 5f69 642c 0d0a  rBy.source_id,..
-0001f750: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-0001f760: 5f6f 7264 6572 3a20 656e 756d 732e 536f  _order: enums.So
-0001f770: 7274 4f72 6465 7220 3d20 656e 756d 732e  rtOrder = enums.
-0001f780: 536f 7274 4f72 6465 722e 6173 630d 0a20  SortOrder.asc.. 
-0001f790: 2020 2029 202d 3e20 7064 2e44 6174 6146     ) -> pd.DataF
-0001f7a0: 7261 6d65 3a0d 0a20 2020 2020 2020 2022  rame:..        "
-0001f7b0: 2222 0d0a 2020 2020 2020 2020 2323 2050  ""..        ## P
-0001f7c0: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-0001f7d0: 2020 2060 7265 616c 7469 6d65 5f73 7461     `realtime_sta
-0001f7e0: 7274 600d 0a20 2020 2020 2020 2054 6865  rt`..        The
-0001f7f0: 2073 7461 7274 206f 6620 7468 6520 7265   start of the re
-0001f800: 616c 2d74 696d 6520 7065 7269 6f64 2e20  al-time period. 
-0001f810: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
-0001f820: 7469 6f6e 2c20 7365 6520 5b52 6561 6c2d  tion, see [Real-
-0001f830: 5469 6d65 2050 6572 696f 6473 5d28 6874  Time Periods](ht
-0001f840: 7470 733a 2f2f 6672 6564 2e73 746c 6f75  tps://fred.stlou
-0001f850: 6973 6665 642e 6f72 672f 646f 6373 2f61  isfed.org/docs/a
-0001f860: 7069 2f66 7265 642f 7265 616c 7469 6d65  pi/fred/realtime
-0001f870: 5f70 6572 696f 642e 6874 6d6c 292e 0d0a  _period.html)...
-0001f880: 0d0a 2020 2020 2020 2020 6072 6561 6c74  ..        `realt
-0001f890: 696d 655f 656e 6460 0d0a 2020 2020 2020  ime_end`..      
-0001f8a0: 2020 5468 6520 656e 6420 6f66 2074 6865    The end of the
-0001f8b0: 2072 6561 6c2d 7469 6d65 2070 6572 696f   real-time perio
-0001f8c0: 642e 2046 6f72 206d 6f72 6520 696e 666f  d. For more info
-0001f8d0: 726d 6174 696f 6e2c 2073 6565 205b 5265  rmation, see [Re
-0001f8e0: 616c 2d54 696d 6520 5065 7269 6f64 735d  al-Time Periods]
-0001f8f0: 2868 7474 7073 3a2f 2f66 7265 642e 7374  (https://fred.st
-0001f900: 6c6f 7569 7366 6564 2e6f 7267 2f64 6f63  louisfed.org/doc
-0001f910: 732f 6170 692f 6672 6564 2f72 6561 6c74  s/api/fred/realt
-0001f920: 696d 655f 7065 7269 6f64 2e68 746d 6c29  ime_period.html)
-0001f930: 2e0d 0a0d 0a20 2020 2020 2020 2060 6f72  .....        `or
-0001f940: 6465 725f 6279 600d 0a20 2020 2020 2020  der_by`..       
-0001f950: 204f 7264 6572 2072 6573 756c 7473 2062   Order results b
-0001f960: 7920 7661 6c75 6573 206f 6620 7468 6520  y values of the 
-0001f970: 7370 6563 6966 6965 6420 6174 7472 6962  specified attrib
-0001f980: 7574 652e 0d0a 0d0a 2020 2020 2020 2020  ute.....        
-0001f990: 6073 6f72 745f 6f72 6465 7260 0d0a 2020  `sort_order`..  
-0001f9a0: 2020 2020 2020 536f 7274 2072 6573 756c        Sort resul
-0001f9b0: 7473 2069 7320 6173 6365 6e64 696e 6720  ts is ascending 
-0001f9c0: 6f72 2064 6573 6365 6e64 696e 6720 6f72  or descending or
-0001f9d0: 6465 7220 666f 7220 6174 7472 6962 7574  der for attribut
-0001f9e0: 6520 7661 6c75 6573 2073 7065 6369 6669  e values specifi
-0001f9f0: 6564 2062 7920 6f72 6465 725f 6279 2e0d  ed by order_by..
-0001fa00: 0a0d 0a20 2020 2020 2020 2023 2320 4465  ...        ## De
-0001fa10: 7363 7269 7074 696f 6e0d 0a20 2020 2020  scription..     
-0001fa20: 2020 2068 7474 7073 3a2f 2f66 7265 642e     https://fred.
-0001fa30: 7374 6c6f 7569 7366 6564 2e6f 7267 2f64  stlouisfed.org/d
-0001fa40: 6f63 732f 6170 692f 6672 6564 2f73 6f75  ocs/api/fred/sou
-0001fa50: 7263 6573 2e68 746d 6c0d 0a0d 0a20 2020  rces.html....   
-0001fa60: 2020 2020 2047 6574 2061 6c6c 2073 6f75       Get all sou
-0001fa70: 7263 6573 206f 6620 6563 6f6e 6f6d 6963  rces of economic
-0001fa80: 2064 6174 612e 0d0a 0d0a 2020 2020 2020   data.....      
-0001fa90: 2020 2323 2041 5049 2052 6571 7565 7374    ## API Request
-0001faa0: 2028 4854 5450 5320 4745 5429 0d0a 2020   (HTTPS GET)..  
-0001fab0: 2020 2020 2020 6874 7470 733a 2f2f 6170        https://ap
-0001fac0: 692e 7374 6c6f 7569 7366 6564 2e6f 7267  i.stlouisfed.org
-0001fad0: 2f66 7265 642f 736f 7572 6365 733f 6170  /fred/sources?ap
-0001fae0: 695f 6b65 793d 6162 6364 6566 6768 696a  i_key=abcdefghij
-0001faf0: 6b6c 6d6e 6f70 7172 7374 7576 7778 797a  klmnopqrstuvwxyz
-0001fb00: 3132 3334 3536 2666 696c 655f 7479 7065  123456&file_type
-0001fb10: 3d6a 736f 6e0d 0a0d 0a20 2020 2020 2020  =json....       
-0001fb20: 2023 2320 4150 4920 5265 7370 6f6e 7365   ## API Response
-0001fb30: 0d0a 2020 2020 2020 2020 6060 606a 736f  ..        ```jso
-0001fb40: 6e0d 0a20 2020 2020 2020 207b 0d0a 2020  n..        {..  
-0001fb50: 2020 2020 2020 2020 2020 2272 6561 6c74            "realt
-0001fb60: 696d 655f 7374 6172 7422 3a20 2232 3031  ime_start": "201
-0001fb70: 332d 3038 2d31 3422 2c0d 0a20 2020 2020  3-08-14",..     
-0001fb80: 2020 2020 2020 2022 7265 616c 7469 6d65         "realtime
-0001fb90: 5f65 6e64 223a 2022 3230 3133 2d30 382d  _end": "2013-08-
-0001fba0: 3134 222c 0d0a 2020 2020 2020 2020 2020  14",..          
-0001fbb0: 2020 226f 7264 6572 5f62 7922 3a20 2273    "order_by": "s
-0001fbc0: 6f75 7263 655f 6964 222c 0d0a 2020 2020  ource_id",..    
-0001fbd0: 2020 2020 2020 2020 2273 6f72 745f 6f72          "sort_or
-0001fbe0: 6465 7222 3a20 2261 7363 222c 0d0a 2020  der": "asc",..  
-0001fbf0: 2020 2020 2020 2020 2020 2263 6f75 6e74            "count
-0001fc00: 223a 2035 382c 0d0a 2020 2020 2020 2020  ": 58,..        
-0001fc10: 2020 2020 226f 6666 7365 7422 3a20 302c      "offset": 0,
-0001fc20: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
-0001fc30: 696d 6974 223a 2031 3030 302c 0d0a 2020  imit": 1000,..  
-0001fc40: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
-0001fc50: 6573 223a 205b 0d0a 2020 2020 2020 2020  es": [..        
-0001fc60: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-0001fc70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001fc80: 6964 223a 2031 2c0d 0a20 2020 2020 2020  id": 1,..       
-0001fc90: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-0001fca0: 616c 7469 6d65 5f73 7461 7274 223a 2022  altime_start": "
-0001fcb0: 3230 3133 2d30 382d 3134 222c 0d0a 2020  2013-08-14",..  
-0001fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fcd0: 2020 2272 6561 6c74 696d 655f 656e 6422    "realtime_end"
-0001fce0: 3a20 2232 3031 332d 3038 2d31 3422 2c0d  : "2013-08-14",.
-0001fcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fd00: 2020 2020 2022 6e61 6d65 223a 2022 426f       "name": "Bo
-0001fd10: 6172 6420 6f66 2047 6f76 6572 6e6f 7273  ard of Governors
-0001fd20: 206f 6620 7468 6520 4665 6465 7261 6c20   of the Federal 
-0001fd30: 5265 7365 7276 6520 5379 7374 656d 222c  Reserve System",
-0001fd40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001fd50: 2020 2020 2020 226c 696e 6b22 3a20 2268        "link": "h
-0001fd60: 7474 703a 2f2f 7777 772e 6665 6465 7261  ttp://www.federa
-0001fd70: 6c72 6573 6572 7665 2e67 6f76 2f22 0d0a  lreserve.gov/"..
-0001fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd90: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-0001fda0: 2020 2020 2e2e 2e0d 0a20 2020 2020 2020      .....       
-0001fdb0: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-0001fdc0: 7d0d 0a20 2020 2020 2020 2060 6060 0d0a  }..        ```..
-0001fdd0: 0d0a 2020 2020 2020 2020 2323 2052 6574  ..        ## Ret
-0001fde0: 7572 6e73 0d0a 2020 2020 2020 2020 6070  urns..        `p
-0001fdf0: 616e 6461 732e 4461 7461 4672 616d 6560  andas.DataFrame`
-0001fe00: 0d0a 0d0a 2020 2020 2020 2020 2323 2045  ....        ## E
-0001fe10: 7861 6d70 6c65 0d0a 2020 2020 2020 2020  xample..        
-0001fe20: 6060 6070 7974 686f 6e0d 0a20 2020 2020  ```python..     
-0001fe30: 2020 203e 3e3e 2066 7265 6420 3d20 4652     >>> fred = FR
-0001fe40: 4544 2861 7069 5f6b 6579 3d27 6162 6364  ED(api_key='abcd
-0001fe50: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
-0001fe60: 7576 7778 797a 3132 3334 3536 2729 0d0a  uvwxyz123456')..
-0001fe70: 2020 2020 2020 2020 3e3e 3e20 6672 6564          >>> fred
-0001fe80: 2e73 6f75 7263 6573 2829 0d0a 2020 2020  .sources()..    
-0001fe90: 2020 2020 2020 2020 2020 2072 6561 6c74             realt
-0001fea0: 696d 655f 7374 6172 7420 7265 616c 7469  ime_start realti
-0001feb0: 6d65 5f65 6e64 2020 2020 2020 2020 2020  me_end          
-0001fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fee0: 2020 2020 206e 616d 6520 2020 2020 2020       name       
-0001fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff00: 2020 2020 2020 206c 696e 6b20 6e6f 7465         link note
-0001ff10: 730d 0a20 2020 2020 2020 2020 2020 2069  s..            i
-0001ff20: 640d 0a20 2020 2020 2020 2020 2020 2031  d..            1
-0001ff30: 2020 2020 2020 3230 3232 2d30 322d 3035        2022-02-05
-0001ff40: 2020 2032 3032 322d 3032 2d30 3520 2042     2022-02-05  B
-0001ff50: 6f61 7264 206f 6620 476f 7665 726e 6f72  oard of Governor
-0001ff60: 7320 6f66 2074 6865 2046 6564 6572 616c  s of the Federal
-0001ff70: 2052 6573 6572 7665 2053 7973 742e 2e2e   Reserve Syst...
-0001ff80: 2020 2020 6874 7470 3a2f 2f77 7777 2e66      http://www.f
-0001ff90: 6564 6572 616c 7265 7365 7276 652e 676f  ederalreserve.go
-0001ffa0: 762f 2020 3c4e 413e 0d0a 2020 2020 2020  v/  <NA>..      
-0001ffb0: 2020 2020 2020 3320 2020 2020 2032 3032        3      202
-0001ffc0: 322d 3032 2d30 3520 2020 3230 3232 2d30  2-02-05   2022-0
-0001ffd0: 322d 3035 2020 2020 2020 2020 2020 2020  2-05            
-0001ffe0: 2020 2046 6564 6572 616c 2052 6573 6572     Federal Reser
-0001fff0: 7665 2042 616e 6b20 6f66 2050 6869 6c61  ve Bank of Phila
-00020000: 6465 6c70 6869 6120 2068 7474 7073 3a2f  delphia  https:/
-00020010: 2f77 7777 2e70 6869 6c61 6465 6c70 6869  /www.philadelphi
-00020020: 6166 6564 2e6f 7267 2f20 203c 4e41 3e0d  afed.org/  <NA>.
-00020030: 0a20 2020 2020 2020 2020 2020 2034 2020  .            4  
-00020040: 2020 2020 3230 3232 2d30 322d 3035 2020      2022-02-05  
-00020050: 2032 3032 322d 3032 2d30 3520 2020 2020   2022-02-05     
-00020060: 2020 2020 2020 2020 2020 2020 2046 6564               Fed
-00020070: 6572 616c 2052 6573 6572 7665 2042 616e  eral Reserve Ban
-00020080: 6b20 6f66 2053 742e 204c 6f75 6973 2020  k of St. Louis  
-00020090: 2020 2020 2020 6874 7470 3a2f 2f77 7777        http://www
-000200a0: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
-000200b0: 2020 3c4e 413e 0d0a 2020 2020 2020 2020    <NA>..        
-000200c0: 2020 2020 3620 2020 2020 2032 3032 322d      6      2022-
-000200d0: 3032 2d30 3520 2020 3230 3232 2d30 322d  02-05   2022-02-
-000200e0: 3035 2020 4665 6465 7261 6c20 4669 6e61  05  Federal Fina
-000200f0: 6e63 6961 6c20 496e 7374 6974 7574 696f  ncial Institutio
-00020100: 6e73 2045 7861 6d69 6e61 7469 6f6e 2043  ns Examination C
-00020110: 6f75 2e2e 2e20 2020 2020 2020 2020 2020  ou...           
-00020120: 2020 6874 7470 3a2f 2f77 7777 2e66 6669    http://www.ffi
-00020130: 6563 2e67 6f76 2f20 203c 4e41 3e0d 0a20  ec.gov/  <NA>.. 
-00020140: 2020 2020 2020 2020 2020 2031 3120 2020             11   
-00020150: 2020 3230 3232 2d30 322d 3035 2020 2032    2022-02-05   2
-00020160: 3032 322d 3032 2d30 3520 2020 2020 2020  022-02-05       
-00020170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020180: 2020 2020 2020 2020 2044 6f77 204a 6f6e           Dow Jon
-00020190: 6573 2026 2043 6f6d 7061 6e79 2020 2020  es & Company    
-000201a0: 2020 2020 2020 2068 7474 703a 2f2f 7777         http://ww
-000201b0: 772e 646f 776a 6f6e 6573 2e63 6f6d 2020  w.dowjones.com  
-000201c0: 3c4e 413e 0d0a 2020 2020 2020 2020 6060  <NA>..        ``
-000201d0: 600d 0a20 2020 2020 2020 2022 2222 0d0a  `..        """..
-000201e0: 0d0a 2020 2020 2020 2020 616c 6c6f 7765  ..        allowe
-000201f0: 645f 6f72 6465 7273 203d 205b 0d0a 2020  d_orders = [..  
-00020200: 2020 2020 2020 2020 2020 656e 756d 732e            enums.
-00020210: 4f72 6465 7242 792e 736f 7572 6365 5f69  OrderBy.source_i
-00020220: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-00020230: 656e 756d 732e 4f72 6465 7242 792e 6e61  enums.OrderBy.na
-00020240: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
-00020250: 2065 6e75 6d73 2e4f 7264 6572 4279 2e72   enums.OrderBy.r
-00020260: 6561 6c74 696d 655f 7374 6172 742c 0d0a  ealtime_start,..
-00020270: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-00020280: 732e 4f72 6465 7242 792e 7265 616c 7469  s.OrderBy.realti
-00020290: 6d65 5f65 6e64 0d0a 2020 2020 2020 2020  me_end..        
-000202a0: 5d0d 0a0d 0a20 2020 2020 2020 2069 6620  ]....        if 
-000202b0: 6f72 6465 725f 6279 206e 6f74 2069 6e20  order_by not in 
-000202c0: 616c 6c6f 7765 645f 6f72 6465 7273 3a0d  allowed_orders:.
-000202d0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000202e0: 7365 2056 616c 7565 4572 726f 7228 2756  se ValueError('V
-000202f0: 6172 6961 626c 6520 6f72 6465 725f 6279  ariable order_by
-00020300: 2028 7b7d 2920 6973 206e 6f74 206f 6e65   ({}) is not one
-00020310: 206f 6620 7468 6520 7661 6c75 6573 3a20   of the values: 
-00020320: 7b7d 272e 666f 726d 6174 286f 7264 6572  {}'.format(order
-00020330: 5f62 792c 2027 2c20 272e 6a6f 696e 286d  _by, ', '.join(m
-00020340: 6170 2873 7472 2c20 616c 6c6f 7765 645f  ap(str, allowed_
-00020350: 6f72 6465 7273 2929 2929 0d0a 0d0a 2020  orders))))....  
-00020360: 2020 2020 2020 6966 2072 6561 6c74 696d        if realtim
-00020370: 655f 7374 6172 7420 6973 206e 6f74 204e  e_start is not N
-00020380: 6f6e 6520 616e 6420 7265 616c 7469 6d65  one and realtime
-00020390: 5f73 7461 7274 203c 2064 6174 6528 3137  _start < date(17
-000203a0: 3736 2c20 372c 2034 293a 0d0a 2020 2020  76, 7, 4):..    
-000203b0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-000203c0: 6c75 6545 7272 6f72 2827 5661 7269 6162  lueError('Variab
-000203d0: 6c65 2072 6561 6c74 696d 655f 7374 6172  le realtime_star
-000203e0: 7420 2822 7b7d 2229 2069 7320 6265 666f  t ("{}") is befo
-000203f0: 7265 206d 696e 2064 6174 6520 3137 3736  re min date 1776
-00020400: 2d30 372d 3034 2e27 2e66 6f72 6d61 7428  -07-04.'.format(
-00020410: 7265 616c 7469 6d65 5f73 7461 7274 2929  realtime_start))
-00020420: 0d0a 0d0a 2020 2020 2020 2020 6966 2072  ....        if r
-00020430: 6561 6c74 696d 655f 7374 6172 7420 6973  ealtime_start is
-00020440: 206e 6f74 204e 6f6e 6520 616e 6420 7265   not None and re
-00020450: 616c 7469 6d65 5f65 6e64 2069 7320 6e6f  altime_end is no
-00020460: 7420 4e6f 6e65 2061 6e64 2072 6561 6c74  t None and realt
-00020470: 696d 655f 7374 6172 7420 3e20 7265 616c  ime_start > real
-00020480: 7469 6d65 5f65 6e64 3a0d 0a20 2020 2020  time_end:..     
-00020490: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000204a0: 7565 4572 726f 7228 2754 6865 2064 6174  ueError('The dat
-000204b0: 6520 7365 7420 6279 2076 6172 6961 626c  e set by variabl
-000204c0: 6520 7265 616c 7469 6d65 5f73 7461 7274  e realtime_start
-000204d0: 2028 227b 7d22 2920 6361 6e20 6e6f 7420   ("{}") can not 
-000204e0: 6265 2061 6674 6572 2074 6865 2064 6174  be after the dat
-000204f0: 6520 7365 7420 6279 2076 6172 6961 626c  e set by variabl
-00020500: 6520 7265 616c 7469 6d65 5f65 6e64 2028  e realtime_end (
-00020510: 227b 7d22 292e 272e 666f 726d 6174 2872  "{}").'.format(r
-00020520: 6561 6c74 696d 655f 7374 6172 742c 2072  ealtime_start, r
-00020530: 6561 6c74 696d 655f 656e 6429 290d 0a0d  ealtime_end))...
-00020540: 0a20 2020 2020 2020 2064 6620 3d20 7064  .        df = pd
-00020550: 2e44 6174 6146 7261 6d65 280d 0a20 2020  .DataFrame(..   
-00020560: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-00020570: 6c69 656e 742e 6765 7428 0d0a 2020 2020  lient.get(..    
-00020580: 2020 2020 2020 2020 2020 2020 272f 6672              '/fr
-00020590: 6564 2f73 6f75 7263 6573 272c 0d0a 2020  ed/sources',..  
-000205a0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-000205b0: 6f75 7263 6573 272c 0d0a 2020 2020 2020  ources',..      
-000205c0: 2020 2020 2020 2020 2020 6c69 6d69 743d            limit=
-000205d0: 3130 3030 2c0d 0a20 2020 2020 2020 2020  1000,..         
-000205e0: 2020 2020 2020 2072 6561 6c74 696d 655f         realtime_
-000205f0: 7374 6172 743d 7265 616c 7469 6d65 5f73  start=realtime_s
-00020600: 7461 7274 2c0d 0a20 2020 2020 2020 2020  tart,..         
-00020610: 2020 2020 2020 2072 6561 6c74 696d 655f         realtime_
-00020620: 656e 643d 7265 616c 7469 6d65 5f65 6e64  end=realtime_end
-00020630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00020640: 2020 206f 7264 6572 5f62 793d 6f72 6465     order_by=orde
-00020650: 725f 6279 2c0d 0a20 2020 2020 2020 2020  r_by,..         
-00020660: 2020 2020 2020 2073 6f72 745f 6f72 6465         sort_orde
-00020670: 723d 736f 7274 5f6f 7264 6572 0d0a 2020  r=sort_order..  
-00020680: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00020690: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
-000206a0: 2020 6461 7465 5f63 6f6c 756d 6e73 203d    date_columns =
-000206b0: 205b 2772 6561 6c74 696d 655f 7374 6172   ['realtime_star
-000206c0: 7427 2c20 2772 6561 6c74 696d 655f 656e  t', 'realtime_en
-000206d0: 6427 5d0d 0a0d 0a20 2020 2020 2020 2069  d']....        i
-000206e0: 6620 6e6f 7420 6466 2e65 6d70 7479 3a0d  f not df.empty:.
-000206f0: 0a20 2020 2020 2020 2020 2020 2064 665b  .            df[
-00020700: 6461 7465 5f63 6f6c 756d 6e73 5d20 3d20  date_columns] = 
-00020710: 6466 5b64 6174 655f 636f 6c75 6d6e 735d  df[date_columns]
-00020720: 2e61 7070 6c79 2870 642e 746f 5f64 6174  .apply(pd.to_dat
-00020730: 6574 696d 652c 2066 6f72 6d61 743d 2725  etime, format='%
-00020740: 592d 256d 2d25 6427 290d 0a20 2020 2020  Y-%m-%d')..     
-00020750: 2020 2020 2020 2064 6620 3d20 6466 2e61         df = df.a
-00020760: 7374 7970 6528 6474 7970 653d 7b0d 0a20  stype(dtype={.. 
-00020770: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00020780: 6e61 6d65 273a 2027 7374 7269 6e67 272c  name': 'string',
-00020790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000207a0: 2020 276e 6f74 6573 273a 2027 7374 7269    'notes': 'stri
-000207b0: 6e67 272c 0d0a 2020 2020 2020 2020 2020  ng',..          
-000207c0: 2020 2020 2020 276c 696e 6b27 3a20 2773        'link': 's
-000207d0: 7472 696e 6727 0d0a 2020 2020 2020 2020  tring'..        
-000207e0: 2020 2020 7d29 2e73 6574 5f69 6e64 6578      }).set_index
-000207f0: 2827 6964 2729 0d0a 0d0a 2020 2020 2020  ('id')....      
-00020800: 2020 7265 7475 726e 2064 660d 0a0d 0a20    return df.... 
-00020810: 2020 2064 6566 2073 6f75 7263 6528 7365     def source(se
-00020820: 6c66 2c20 736f 7572 6365 5f69 643a 2069  lf, source_id: i
-00020830: 6e74 2c20 7265 616c 7469 6d65 5f73 7461  nt, realtime_sta
-00020840: 7274 3a20 6461 7465 203d 204e 6f6e 652c  rt: date = None,
-00020850: 2072 6561 6c74 696d 655f 656e 643a 2064   realtime_end: d
-00020860: 6174 6520 3d20 4e6f 6e65 2920 2d3e 206d  ate = None) -> m
-00020870: 6f64 656c 732e 536f 7572 6365 3a0d 0a20  odels.Source:.. 
-00020880: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00020890: 2020 2020 2323 2050 6172 616d 6574 6572      ## Parameter
-000208a0: 730d 0a20 2020 2020 2020 2060 736f 7572  s..        `sour
-000208b0: 6365 5f69 6460 0d0a 2020 2020 2020 2020  ce_id`..        
-000208c0: 5468 6520 6964 2066 6f72 2061 2073 6f75  The id for a sou
-000208d0: 7263 652e 0d0a 0d0a 2020 2020 2020 2020  rce.....        
-000208e0: 6072 6561 6c74 696d 655f 7374 6172 7460  `realtime_start`
-000208f0: 0d0a 2020 2020 2020 2020 5468 6520 7374  ..        The st
-00020900: 6172 7420 6f66 2074 6865 2072 6561 6c2d  art of the real-
-00020910: 7469 6d65 2070 6572 696f 642e 2046 6f72  time period. For
-00020920: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00020930: 6e2c 2073 6565 205b 5265 616c 2d54 696d  n, see [Real-Tim
-00020940: 6520 5065 7269 6f64 735d 2868 7474 7073  e Periods](https
-00020950: 3a2f 2f66 7265 642e 7374 6c6f 7569 7366  ://fred.stlouisf
-00020960: 6564 2e6f 7267 2f64 6f63 732f 6170 692f  ed.org/docs/api/
-00020970: 6672 6564 2f72 6561 6c74 696d 655f 7065  fred/realtime_pe
-00020980: 7269 6f64 2e68 746d 6c29 2e0d 0a0d 0a20  riod.html)..... 
-00020990: 2020 2020 2020 2060 7265 616c 7469 6d65         `realtime
-000209a0: 5f65 6e64 600d 0a20 2020 2020 2020 2054  _end`..        T
-000209b0: 6865 2065 6e64 206f 6620 7468 6520 7265  he end of the re
-000209c0: 616c 2d74 696d 6520 7065 7269 6f64 2e20  al-time period. 
-000209d0: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
-000209e0: 7469 6f6e 2c20 7365 6520 5b52 6561 6c2d  tion, see [Real-
-000209f0: 5469 6d65 2050 6572 696f 6473 5d28 6874  Time Periods](ht
-00020a00: 7470 733a 2f2f 6672 6564 2e73 746c 6f75  tps://fred.stlou
-00020a10: 6973 6665 642e 6f72 672f 646f 6373 2f61  isfed.org/docs/a
-00020a20: 7069 2f66 7265 642f 7265 616c 7469 6d65  pi/fred/realtime
-00020a30: 5f70 6572 696f 642e 6874 6d6c 292e 0d0a  _period.html)...
-00020a40: 0d0a 2020 2020 2020 2020 2323 2044 6573  ..        ## Des
-00020a50: 6372 6970 7469 6f6e 0d0a 2020 2020 2020  cription..      
-00020a60: 2020 6874 7470 733a 2f2f 6672 6564 2e73    https://fred.s
-00020a70: 746c 6f75 6973 6665 642e 6f72 672f 646f  tlouisfed.org/do
-00020a80: 6373 2f61 7069 2f66 7265 642f 736f 7572  cs/api/fred/sour
-00020a90: 6365 2e68 746d 6c0d 0a0d 0a20 2020 2020  ce.html....     
-00020aa0: 2020 2047 6574 2061 2073 6f75 7263 6520     Get a source 
-00020ab0: 6f66 2065 636f 6e6f 6d69 6320 6461 7461  of economic data
-00020ac0: 2e0d 0a0d 0a20 2020 2020 2020 2023 2320  .....        ## 
-00020ad0: 4150 4920 5265 7175 6573 7420 2848 5454  API Request (HTT
-00020ae0: 5053 2047 4554 290d 0a20 2020 2020 2020  PS GET)..       
-00020af0: 2068 7474 7073 3a2f 2f61 7069 2e73 746c   https://api.stl
-00020b00: 6f75 6973 6665 642e 6f72 672f 6672 6564  ouisfed.org/fred
-00020b10: 2f73 6f75 7263 653f 736f 7572 6365 5f69  /source?source_i
-00020b20: 643d 3126 6170 695f 6b65 793d 6162 6364  d=1&api_key=abcd
-00020b30: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
-00020b40: 7576 7778 797a 3132 3334 3536 2666 696c  uvwxyz123456&fil
-00020b50: 655f 7479 7065 3d6a 736f 6e0d 0a0d 0a20  e_type=json.... 
-00020b60: 2020 2020 2020 2023 2320 4150 4920 5265         ## API Re
-00020b70: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
-00020b80: 6060 606a 736f 6e0d 0a20 2020 2020 2020  ```json..       
-00020b90: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00020ba0: 2272 6561 6c74 696d 655f 7374 6172 7422  "realtime_start"
-00020bb0: 3a20 2232 3031 332d 3038 2d31 3422 2c0d  : "2013-08-14",.
-00020bc0: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-00020bd0: 616c 7469 6d65 5f65 6e64 223a 2022 3230  altime_end": "20
-00020be0: 3133 2d30 382d 3134 222c 0d0a 2020 2020  13-08-14",..    
-00020bf0: 2020 2020 2020 2020 2273 6f75 7263 6573          "sources
-00020c00: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
-00020c10: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00020c20: 2020 2020 2020 2020 2020 2020 2022 6964               "id
-00020c30: 223a 2031 2c0d 0a20 2020 2020 2020 2020  ": 1,..         
-00020c40: 2020 2020 2020 2020 2020 2022 7265 616c             "real
-00020c50: 7469 6d65 5f73 7461 7274 223a 2022 3230  time_start": "20
-00020c60: 3133 2d30 382d 3134 222c 0d0a 2020 2020  13-08-14",..    
-00020c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c80: 2272 6561 6c74 696d 655f 656e 6422 3a20  "realtime_end": 
-00020c90: 2232 3031 332d 3038 2d31 3422 2c0d 0a20  "2013-08-14",.. 
-00020ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020cb0: 2020 2022 6e61 6d65 223a 2022 426f 6172     "name": "Boar
-00020cc0: 6420 6f66 2047 6f76 6572 6e6f 7273 206f  d of Governors o
-00020cd0: 6620 7468 6520 4665 6465 7261 6c20 5265  f the Federal Re
-00020ce0: 7365 7276 6520 5379 7374 656d 222c 0d0a  serve System",..
-00020cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d00: 2020 2020 226c 696e 6b22 3a20 2268 7474      "link": "htt
-00020d10: 703a 2f2f 7777 772e 6665 6465 7261 6c72  p://www.federalr
-00020d20: 6573 6572 7665 2e67 6f76 2f22 0d0a 2020  eserve.gov/"..  
-00020d30: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-00020d40: 0a20 2020 2020 2020 2020 2020 205d 0d0a  .            ]..
-00020d50: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00020d60: 2020 2060 6060 0d0a 0d0a 2020 2020 2020     ```....      
-00020d70: 2020 2323 2052 6574 7572 6e73 0d0a 2020    ## Returns..  
-00020d80: 2020 2020 2020 6070 7973 746c 6f75 6973        `pystlouis
-00020d90: 6665 642e 6d6f 6465 6c73 2e53 6f75 7263  fed.models.Sourc
-00020da0: 6560 0d0a 0d0a 2020 2020 2020 2020 2323  e`....        ##
-00020db0: 2045 7861 6d70 6c65 0d0a 2020 2020 2020   Example..      
-00020dc0: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
-00020dd0: 2020 2020 203e 3e3e 2066 7265 6420 3d20       >>> fred = 
-00020de0: 4652 4544 2861 7069 5f6b 6579 3d27 6162  FRED(api_key='ab
-00020df0: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
-00020e00: 7374 7576 7778 797a 3132 3334 3536 2729  stuvwxyz123456')
-00020e10: 0d0a 2020 2020 2020 2020 3e3e 3e20 6672  ..        >>> fr
-00020e20: 6564 2e73 6f75 7263 6528 736f 7572 6365  ed.source(source
-00020e30: 5f69 643d 3129 0d0a 2020 2020 2020 2020  _id=1)..        
-00020e40: 2020 2020 536f 7572 6365 2869 643d 312c      Source(id=1,
-00020e50: 2072 6561 6c74 696d 655f 7374 6172 743d   realtime_start=
-00020e60: 2732 3032 322d 3031 2d31 3427 2c20 7265  '2022-01-14', re
-00020e70: 616c 7469 6d65 5f65 6e64 3d27 3230 3232  altime_end='2022
-00020e80: 2d30 312d 3134 272c 206e 616d 653d 2742  -01-14', name='B
-00020e90: 6f61 7264 206f 6620 476f 7665 726e 6f72  oard of Governor
-00020ea0: 7320 6f66 2074 6865 2046 6564 6572 616c  s of the Federal
-00020eb0: 2052 6573 6572 7665 2053 7973 7465 6d20   Reserve System 
-00020ec0: 2855 5329 272c 206c 696e 6b3d 2768 7474  (US)', link='htt
-00020ed0: 703a 2f2f 7777 772e 6665 6465 7261 6c72  p://www.federalr
-00020ee0: 6573 6572 7665 2e67 6f76 2f27 290d 0a20  eserve.gov/').. 
-00020ef0: 2020 2020 2020 2060 6060 0d0a 2020 2020         ```..    
-00020f00: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
-00020f10: 2020 2069 6620 7265 616c 7469 6d65 5f73     if realtime_s
-00020f20: 7461 7274 2069 7320 6e6f 7420 4e6f 6e65  tart is not None
-00020f30: 2061 6e64 2072 6561 6c74 696d 655f 7374   and realtime_st
-00020f40: 6172 7420 3c20 6461 7465 2831 3737 362c  art < date(1776,
-00020f50: 2037 2c20 3429 3a0d 0a20 2020 2020 2020   7, 4):..       
-00020f60: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00020f70: 4572 726f 7228 2756 6172 6961 626c 6520  Error('Variable 
-00020f80: 7265 616c 7469 6d65 5f73 7461 7274 2028  realtime_start (
-00020f90: 227b 7d22 2920 6973 2062 6566 6f72 6520  "{}") is before 
-00020fa0: 6d69 6e20 6461 7465 2031 3737 362d 3037  min date 1776-07
-00020fb0: 2d30 342e 272e 666f 726d 6174 2872 6561  -04.'.format(rea
-00020fc0: 6c74 696d 655f 7374 6172 7429 290d 0a0d  ltime_start))...
-00020fd0: 0a20 2020 2020 2020 2069 6620 7265 616c  .        if real
-00020fe0: 7469 6d65 5f73 7461 7274 2069 7320 6e6f  time_start is no
-00020ff0: 7420 4e6f 6e65 2061 6e64 2072 6561 6c74  t None and realt
-00021000: 696d 655f 656e 6420 6973 206e 6f74 204e  ime_end is not N
-00021010: 6f6e 6520 616e 6420 7265 616c 7469 6d65  one and realtime
-00021020: 5f73 7461 7274 203e 2072 6561 6c74 696d  _start > realtim
-00021030: 655f 656e 643a 0d0a 2020 2020 2020 2020  e_end:..        
-00021040: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00021050: 7272 6f72 2827 5468 6520 6461 7465 2073  rror('The date s
-00021060: 6574 2062 7920 7661 7269 6162 6c65 2072  et by variable r
-00021070: 6561 6c74 696d 655f 7374 6172 7420 2822  ealtime_start ("
-00021080: 7b7d 2229 2063 616e 206e 6f74 2062 6520  {}") can not be 
-00021090: 6166 7465 7220 7468 6520 6461 7465 2073  after the date s
-000210a0: 6574 2062 7920 7661 7269 6162 6c65 2072  et by variable r
-000210b0: 6561 6c74 696d 655f 656e 6420 2822 7b7d  ealtime_end ("{}
-000210c0: 2229 2e27 2e66 6f72 6d61 7428 7265 616c  ").'.format(real
-000210d0: 7469 6d65 5f73 7461 7274 2c20 7265 616c  time_start, real
-000210e0: 7469 6d65 5f65 6e64 2929 0d0a 0d0a 2020  time_end))....  
-000210f0: 2020 2020 2020 6461 7461 203d 2073 656c        data = sel
-00021100: 662e 5f63 6c69 656e 742e 6765 7428 0d0a  f._client.get(..
-00021110: 2020 2020 2020 2020 2020 2020 272f 6672              '/fr
-00021120: 6564 2f73 6f75 7263 6527 2c0d 0a20 2020  ed/source',..   
-00021130: 2020 2020 2020 2020 2027 736f 7572 6365           'source
-00021140: 7327 2c0d 0a20 2020 2020 2020 2020 2020  s',..           
-00021150: 2073 6f75 7263 655f 6964 3d73 6f75 7263   source_id=sourc
-00021160: 655f 6964 2c0d 0a20 2020 2020 2020 2020  e_id,..         
-00021170: 2020 2072 6561 6c74 696d 655f 7374 6172     realtime_star
-00021180: 743d 7265 616c 7469 6d65 5f73 7461 7274  t=realtime_start
-00021190: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-000211a0: 6561 6c74 696d 655f 656e 643d 7265 616c  ealtime_end=real
-000211b0: 7469 6d65 5f65 6e64 0d0a 2020 2020 2020  time_end..      
-000211c0: 2020 290d 0a0d 0a20 2020 2020 2020 2072    )....        r
-000211d0: 6574 7572 6e20 6d6f 6465 6c73 2e53 6f75  eturn models.Sou
-000211e0: 7263 6528 2a2a 6461 7461 5b30 5d29 0d0a  rce(**data[0])..
-000211f0: 0d0a 2020 2020 6465 6620 736f 7572 6365  ..    def source
-00021200: 5f72 656c 6561 7365 7328 0d0a 2020 2020  _releases(..    
-00021210: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00021220: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-00021230: 655f 6964 3a20 696e 742c 0d0a 2020 2020  e_id: int,..    
-00021240: 2020 2020 2020 2020 7265 616c 7469 6d65          realtime
-00021250: 5f73 7461 7274 3a20 6461 7465 203d 204e  _start: date = N
-00021260: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00021270: 2020 7265 616c 7469 6d65 5f65 6e64 3a20    realtime_end: 
-00021280: 6461 7465 203d 204e 6f6e 652c 0d0a 2020  date = None,..  
-00021290: 2020 2020 2020 2020 2020 6f72 6465 725f            order_
-000212a0: 6279 3a20 656e 756d 732e 4f72 6465 7242  by: enums.OrderB
-000212b0: 7920 3d20 656e 756d 732e 4f72 6465 7242  y = enums.OrderB
-000212c0: 792e 7265 6c65 6173 655f 6964 2c0d 0a20  y.release_id,.. 
-000212d0: 2020 2020 2020 2020 2020 2073 6f72 745f             sort_
-000212e0: 6f72 6465 723a 2065 6e75 6d73 2e53 6f72  order: enums.Sor
-000212f0: 744f 7264 6572 203d 2065 6e75 6d73 2e53  tOrder = enums.S
-00021300: 6f72 744f 7264 6572 2e61 7363 0d0a 2020  ortOrder.asc..  
-00021310: 2020 2920 2d3e 2070 642e 4461 7461 4672    ) -> pd.DataFr
-00021320: 616d 653a 0d0a 2020 2020 2020 2020 2222  ame:..        ""
-00021330: 220d 0a20 2020 2020 2020 2023 2320 5061  "..        ## Pa
-00021340: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-00021350: 2020 6073 6f75 7263 655f 6964 600d 0a20    `source_id`.. 
-00021360: 2020 2020 2020 2054 6865 2069 6420 666f         The id fo
-00021370: 7220 6120 736f 7572 6365 2e0d 0a0d 0a20  r a source..... 
-00021380: 2020 2020 2020 2060 7265 616c 7469 6d65         `realtime
-00021390: 5f73 7461 7274 600d 0a20 2020 2020 2020  _start`..       
-000213a0: 2054 6865 2073 7461 7274 206f 6620 7468   The start of th
-000213b0: 6520 7265 616c 2d74 696d 6520 7065 7269  e real-time peri
-000213c0: 6f64 2e20 466f 7220 6d6f 7265 2069 6e66  od. For more inf
-000213d0: 6f72 6d61 7469 6f6e 2c20 7365 6520 5b52  ormation, see [R
-000213e0: 6561 6c2d 5469 6d65 2050 6572 696f 6473  eal-Time Periods
-000213f0: 5d28 6874 7470 733a 2f2f 6672 6564 2e73  ](https://fred.s
-00021400: 746c 6f75 6973 6665 642e 6f72 672f 646f  tlouisfed.org/do
-00021410: 6373 2f61 7069 2f66 7265 642f 7265 616c  cs/api/fred/real
-00021420: 7469 6d65 5f70 6572 696f 642e 6874 6d6c  time_period.html
-00021430: 292e 0d0a 0d0a 2020 2020 2020 2020 6072  ).....        `r
-00021440: 6561 6c74 696d 655f 656e 6460 0d0a 2020  ealtime_end`..  
-00021450: 2020 2020 2020 5468 6520 656e 6420 6f66        The end of
-00021460: 2074 6865 2072 6561 6c2d 7469 6d65 2070   the real-time p
-00021470: 6572 696f 642e 2046 6f72 206d 6f72 6520  eriod. For more 
-00021480: 696e 666f 726d 6174 696f 6e2c 2073 6565  information, see
-00021490: 205b 5265 616c 2d54 696d 6520 5065 7269   [Real-Time Peri
-000214a0: 6f64 735d 2868 7474 7073 3a2f 2f66 7265  ods](https://fre
-000214b0: 642e 7374 6c6f 7569 7366 6564 2e6f 7267  d.stlouisfed.org
-000214c0: 2f64 6f63 732f 6170 692f 6672 6564 2f72  /docs/api/fred/r
-000214d0: 6561 6c74 696d 655f 7065 7269 6f64 2e68  ealtime_period.h
-000214e0: 746d 6c29 2e0d 0a0d 0a20 2020 2020 2020  tml).....       
-000214f0: 2060 6f72 6465 725f 6279 600d 0a20 2020   `order_by`..   
-00021500: 2020 2020 204f 7264 6572 2072 6573 756c       Order resul
-00021510: 7473 2062 7920 7661 6c75 6573 206f 6620  ts by values of 
-00021520: 7468 6520 7370 6563 6966 6965 6420 6174  the specified at
-00021530: 7472 6962 7574 652e 0d0a 0d0a 2020 2020  tribute.....    
-00021540: 2020 2020 6073 6f72 745f 6f72 6465 7260      `sort_order`
-00021550: 0d0a 2020 2020 2020 2020 536f 7274 2072  ..        Sort r
-00021560: 6573 756c 7473 2069 7320 6173 6365 6e64  esults is ascend
-00021570: 696e 6720 6f72 2064 6573 6365 6e64 696e  ing or descendin
-00021580: 6720 6f72 6465 7220 666f 7220 6174 7472  g order for attr
-00021590: 6962 7574 6520 7661 6c75 6573 2073 7065  ibute values spe
-000215a0: 6369 6669 6564 2062 7920 6f72 6465 725f  cified by order_
-000215b0: 6279 2e0d 0a0d 0a20 2020 2020 2020 2023  by.....        #
-000215c0: 2320 4465 7363 7269 7074 696f 6e0d 0a20  # Description.. 
-000215d0: 2020 2020 2020 2068 7474 7073 3a2f 2f66         https://f
-000215e0: 7265 642e 7374 6c6f 7569 7366 6564 2e6f  red.stlouisfed.o
-000215f0: 7267 2f64 6f63 732f 6170 692f 6672 6564  rg/docs/api/fred
-00021600: 2f73 6f75 7263 655f 7265 6c65 6173 6573  /source_releases
-00021610: 2e68 746d 6c0d 0a0d 0a20 2020 2020 2020  .html....       
-00021620: 2047 6574 2074 6865 2072 656c 6561 7365   Get the release
-00021630: 7320 666f 7220 6120 736f 7572 6365 2e0d  s for a source..
-00021640: 0a0d 0a20 2020 2020 2020 2023 2320 4150  ...        ## AP
-00021650: 4920 5265 7175 6573 7420 2848 5454 5053  I Request (HTTPS
-00021660: 2047 4554 290d 0a20 2020 2020 2020 2068   GET)..        h
-00021670: 7474 7073 3a2f 2f61 7069 2e73 746c 6f75  ttps://api.stlou
-00021680: 6973 6665 642e 6f72 672f 6672 6564 2f73  isfed.org/fred/s
-00021690: 6f75 7263 652f 7265 6c65 6173 6573 3f73  ource/releases?s
-000216a0: 6f75 7263 655f 6964 3d31 2661 7069 5f6b  ource_id=1&api_k
-000216b0: 6579 3d61 6263 6465 6667 6869 6a6b 6c6d  ey=abcdefghijklm
-000216c0: 6e6f 7071 7273 7475 7677 7879 7a31 3233  nopqrstuvwxyz123
-000216d0: 3435 3626 6669 6c65 5f74 7970 653d 6a73  456&file_type=js
-000216e0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2323  on....        ##
-000216f0: 2041 5049 2052 6573 706f 6e73 650d 0a20   API Response.. 
-00021700: 2020 2020 2020 2060 6060 6a73 6f6e 0d0a         ```json..
-00021710: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00021720: 2020 2020 2020 2022 7265 616c 7469 6d65         "realtime
-00021730: 5f73 7461 7274 223a 2022 3230 3133 2d30  _start": "2013-0
-00021740: 382d 3134 222c 0d0a 2020 2020 2020 2020  8-14",..        
-00021750: 2020 2020 2272 6561 6c74 696d 655f 656e      "realtime_en
-00021760: 6422 3a20 2232 3031 332d 3038 2d31 3422  d": "2013-08-14"
-00021770: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00021780: 6f72 6465 725f 6279 223a 2022 7265 6c65  order_by": "rele
-00021790: 6173 655f 6964 222c 0d0a 2020 2020 2020  ase_id",..      
-000217a0: 2020 2020 2020 2273 6f72 745f 6f72 6465        "sort_orde
-000217b0: 7222 3a20 2261 7363 222c 0d0a 2020 2020  r": "asc",..    
-000217c0: 2020 2020 2020 2020 2263 6f75 6e74 223a          "count":
-000217d0: 2032 362c 0d0a 2020 2020 2020 2020 2020   26,..          
-000217e0: 2020 226f 6666 7365 7422 3a20 302c 0d0a    "offset": 0,..
-000217f0: 2020 2020 2020 2020 2020 2020 226c 696d              "lim
-00021800: 6974 223a 2031 3030 302c 0d0a 2020 2020  it": 1000,..    
-00021810: 2020 2020 2020 2020 2272 656c 6561 7365          "release
-00021820: 7322 3a20 5b0d 0a20 2020 2020 2020 2020  s": [..         
-00021830: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00021840: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00021850: 6422 3a20 3133 2c0d 0a20 2020 2020 2020  d": 13,..       
-00021860: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00021870: 616c 7469 6d65 5f73 7461 7274 223a 2022  altime_start": "
-00021880: 3230 3133 2d30 382d 3134 222c 0d0a 2020  2013-08-14",..  
-00021890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000218a0: 2020 2272 6561 6c74 696d 655f 656e 6422    "realtime_end"
-000218b0: 3a20 2232 3031 332d 3038 2d31 3422 2c0d  : "2013-08-14",.
-000218c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000218d0: 2020 2020 2022 6e61 6d65 223a 2022 472e       "name": "G.
-000218e0: 3137 2049 6e64 7573 7472 6961 6c20 5072  17 Industrial Pr
-000218f0: 6f64 7563 7469 6f6e 2061 6e64 2043 6170  oduction and Cap
-00021900: 6163 6974 7920 5574 696c 697a 6174 696f  acity Utilizatio
-00021910: 6e22 2c0d 0a20 2020 2020 2020 2020 2020  n",..           
-00021920: 2020 2020 2020 2020 2022 7072 6573 735f           "press_
-00021930: 7265 6c65 6173 6522 3a20 7472 7565 2c0d  release": true,.
-00021940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021950: 2020 2020 2022 6c69 6e6b 223a 2022 6874       "link": "ht
-00021960: 7470 3a2f 2f77 7777 2e66 6564 6572 616c  tp://www.federal
-00021970: 7265 7365 7276 652e 676f 762f 7265 6c65  reserve.gov/rele
-00021980: 6173 6573 2f67 3137 2f22 0d0a 2020 2020  ases/g17/"..    
-00021990: 2020 2020 2020 2020 2020 2020 7d2c 0d0a              },..
-000219a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000219b0: 2e2e 2e0d 0a20 2020 2020 2020 2020 2020  .....           
-000219c0: 205d 0d0a 2020 2020 2020 2020 7d0d 0a20   ]..        }.. 
-000219d0: 2020 2020 2020 2060 6060 0d0a 0d0a 2020         ```....  
-000219e0: 2020 2020 2020 2323 2052 6574 7572 6e73        ## Returns
-000219f0: 0d0a 2020 2020 2020 2020 6070 616e 6461  ..        `panda
-00021a00: 732e 4461 7461 4672 616d 6560 0d0a 0d0a  s.DataFrame`....
-00021a10: 2020 2020 2020 2020 2323 2045 7861 6d70          ## Examp
-00021a20: 6c65 0d0a 2020 2020 2020 2020 6060 6070  le..        ```p
-00021a30: 7974 686f 6e0d 0a20 2020 2020 2020 203e  ython..        >
-00021a40: 3e3e 2066 7265 6420 3d20 4652 4544 2861  >> fred = FRED(a
-00021a50: 7069 5f6b 6579 3d27 6162 6364 6566 6768  pi_key='abcdefgh
-00021a60: 696a 6b6c 6d6e 6f70 7172 7374 7576 7778  ijklmnopqrstuvwx
-00021a70: 797a 3132 3334 3536 2729 0d0a 2020 2020  yz123456')..    
-00021a80: 2020 2020 3e3e 3e20 6672 6564 2e73 6f75      >>> fred.sou
-00021a90: 7263 655f 7265 6c65 6173 6573 2873 6f75  rce_releases(sou
-00021aa0: 7263 655f 6964 3d31 292e 6865 6164 2829  rce_id=1).head()
-00021ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021ac0: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
-00021ad0: 7265 616c 7469 6d65 5f65 6e64 2020 2020  realtime_end    
-00021ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b00: 2020 2020 2020 2020 2020 206e 616d 6520             name 
-00021b10: 2070 7265 7373 5f72 656c 6561 7365 2020   press_release  
-00021b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b40: 2020 2020 2020 206c 696e 6b20 6e6f 7465         link note
-00021b50: 730d 0a20 2020 2020 2020 2020 2020 2069  s..            i
-00021b60: 640d 0a20 2020 2020 2020 2020 2020 2031  d..            1
-00021b70: 3320 2020 2020 3230 3232 2d30 322d 3035  3     2022-02-05
-00021b80: 2020 2032 3032 322d 3032 2d30 3520 2047     2022-02-05  G
-00021b90: 2e31 3720 496e 6475 7374 7269 616c 2050  .17 Industrial P
-00021ba0: 726f 6475 6374 696f 6e20 616e 6420 4361  roduction and Ca
-00021bb0: 7061 6369 7479 2055 7469 6c69 7a2e 2e2e  pacity Utiliz...
-00021bc0: 2020 2020 2020 2020 2020 2054 7275 6520             True 
-00021bd0: 2068 7474 703a 2f2f 7777 772e 6665 6465   http://www.fede
-00021be0: 7261 6c72 6573 6572 7665 2e67 6f76 2f72  ralreserve.gov/r
-00021bf0: 656c 6561 7365 732f 6731 372f 2020 3c4e  eleases/g17/  <N
-00021c00: 413e 0d0a 2020 2020 2020 2020 2020 2020  A>..            
-00021c10: 3134 2020 2020 2032 3032 322d 3032 2d30  14     2022-02-0
-00021c20: 3520 2020 3230 3232 2d30 322d 3035 2020  5   2022-02-05  
-00021c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021c40: 2020 2020 2020 2020 2020 2020 2047 2e31               G.1
-00021c50: 3920 436f 6e73 756d 6572 2043 7265 6469  9 Consumer Credi
-00021c60: 7420 2020 2020 2020 2020 2020 5472 7565  t           True
-00021c70: 2020 6874 7470 3a2f 2f77 7777 2e66 6564    http://www.fed
-00021c80: 6572 616c 7265 7365 7276 652e 676f 762f  eralreserve.gov/
-00021c90: 7265 6c65 6173 6573 2f67 3139 2f20 203c  releases/g19/  <
-00021ca0: 4e41 3e0d 0a20 2020 2020 2020 2020 2020  NA>..           
-00021cb0: 2031 3520 2020 2020 3230 3232 2d30 322d   15     2022-02-
-00021cc0: 3035 2020 2032 3032 322d 3032 2d30 3520  05   2022-02-05 
-00021cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ce0: 2020 2020 2020 2020 472e 3520 466f 7265          G.5 Fore
-00021cf0: 6967 6e20 4578 6368 616e 6765 2052 6174  ign Exchange Rat
-00021d00: 6573 2020 2020 2020 2020 2020 2054 7275  es           Tru
-00021d10: 6520 2020 6874 7470 3a2f 2f77 7777 2e66  e   http://www.f
-00021d20: 6564 6572 616c 7265 7365 7276 652e 676f  ederalreserve.go
-00021d30: 762f 7265 6c65 6173 6573 2f67 352f 2020  v/releases/g5/  
-00021d40: 3c4e 413e 0d0a 2020 2020 2020 2020 2020  <NA>..          
-00021d50: 2020 3137 2020 2020 2032 3032 322d 3032    17     2022-02
-00021d60: 2d30 3520 2020 3230 3232 2d30 322d 3035  -05   2022-02-05
-00021d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021d80: 2020 2020 2020 2020 482e 3130 2046 6f72          H.10 For
-00021d90: 6569 676e 2045 7863 6861 6e67 6520 5261  eign Exchange Ra
-00021da0: 7465 7320 2020 2020 2020 2020 2020 5472  tes           Tr
-00021db0: 7565 2020 6874 7470 3a2f 2f77 7777 2e66  ue  http://www.f
-00021dc0: 6564 6572 616c 7265 7365 7276 652e 676f  ederalreserve.go
-00021dd0: 762f 7265 6c65 6173 6573 2f68 3130 2f20  v/releases/h10/ 
-00021de0: 203c 4e41 3e0d 0a20 2020 2020 2020 2020   <NA>..         
-00021df0: 2020 2031 3820 2020 2020 3230 3232 2d30     18     2022-0
-00021e00: 322d 3035 2020 2032 3032 322d 3032 2d30  2-05   2022-02-0
-00021e10: 3520 2020 2020 2020 2020 2020 2020 2020  5               
-00021e20: 2020 2020 2020 2020 482e 3135 2053 656c          H.15 Sel
-00021e30: 6563 7465 6420 496e 7465 7265 7374 2052  ected Interest R
-00021e40: 6174 6573 2020 2020 2020 2020 2020 2054  ates           T
-00021e50: 7275 6520 2068 7474 703a 2f2f 7777 772e  rue  http://www.
-00021e60: 6665 6465 7261 6c72 6573 6572 7665 2e67  federalreserve.g
-00021e70: 6f76 2f72 656c 6561 7365 732f 6831 352f  ov/releases/h15/
-00021e80: 2020 3c4e 413e 0d0a 2020 2020 2020 2020    <NA>..        
-00021e90: 6060 600d 0a20 2020 2020 2020 2022 2222  ```..        """
-00021ea0: 0d0a 0d0a 2020 2020 2020 2020 616c 6c6f  ....        allo
-00021eb0: 7765 645f 6f72 6465 7273 203d 205b 0d0a  wed_orders = [..
-00021ec0: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-00021ed0: 732e 4f72 6465 7242 792e 7265 6c65 6173  s.OrderBy.releas
-00021ee0: 655f 6964 2c0d 0a20 2020 2020 2020 2020  e_id,..         
-00021ef0: 2020 2065 6e75 6d73 2e4f 7264 6572 4279     enums.OrderBy
-00021f00: 2e6e 616d 652c 0d0a 2020 2020 2020 2020  .name,..        
-00021f10: 2020 2020 656e 756d 732e 4f72 6465 7242      enums.OrderB
-00021f20: 792e 7072 6573 735f 7265 6c65 6173 652c  y.press_release,
-00021f30: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
-00021f40: 756d 732e 4f72 6465 7242 792e 7265 616c  ums.OrderBy.real
-00021f50: 7469 6d65 5f73 7461 7274 2c0d 0a20 2020  time_start,..   
-00021f60: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
-00021f70: 7264 6572 4279 2e72 6561 6c74 696d 655f  rderBy.realtime_
-00021f80: 656e 640d 0a20 2020 2020 2020 205d 0d0a  end..        ]..
-00021f90: 0d0a 2020 2020 2020 2020 6966 206f 7264  ..        if ord
-00021fa0: 6572 5f62 7920 6e6f 7420 696e 2061 6c6c  er_by not in all
-00021fb0: 6f77 6564 5f6f 7264 6572 733a 0d0a 2020  owed_orders:..  
-00021fc0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00021fd0: 5661 6c75 6545 7272 6f72 2827 5661 7269  ValueError('Vari
-00021fe0: 6162 6c65 206f 7264 6572 5f62 7920 287b  able order_by ({
-00021ff0: 7d29 2069 7320 6e6f 7420 6f6e 6520 6f66  }) is not one of
-00022000: 2074 6865 2076 616c 7565 733a 207b 7d27   the values: {}'
-00022010: 2e66 6f72 6d61 7428 6f72 6465 725f 6279  .format(order_by
-00022020: 2c20 272c 2027 2e6a 6f69 6e28 6d61 7028  , ', '.join(map(
-00022030: 7374 722c 2061 6c6c 6f77 6564 5f6f 7264  str, allowed_ord
-00022040: 6572 7329 2929 290d 0a0d 0a20 2020 2020  ers))))....     
-00022050: 2020 2069 6620 7265 616c 7469 6d65 5f73     if realtime_s
-00022060: 7461 7274 2069 7320 6e6f 7420 4e6f 6e65  tart is not None
-00022070: 2061 6e64 2072 6561 6c74 696d 655f 7374   and realtime_st
-00022080: 6172 7420 3c20 6461 7465 2831 3737 362c  art < date(1776,
-00022090: 2037 2c20 3429 3a0d 0a20 2020 2020 2020   7, 4):..       
-000220a0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-000220b0: 4572 726f 7228 2756 6172 6961 626c 6520  Error('Variable 
-000220c0: 7265 616c 7469 6d65 5f73 7461 7274 2028  realtime_start (
-000220d0: 227b 7d22 2920 6973 2062 6566 6f72 6520  "{}") is before 
-000220e0: 6d69 6e20 6461 7465 2031 3737 362d 3037  min date 1776-07
-000220f0: 2d30 342e 272e 666f 726d 6174 2872 6561  -04.'.format(rea
-00022100: 6c74 696d 655f 7374 6172 7429 290d 0a0d  ltime_start))...
-00022110: 0a20 2020 2020 2020 2069 6620 7265 616c  .        if real
-00022120: 7469 6d65 5f73 7461 7274 2069 7320 6e6f  time_start is no
-00022130: 7420 4e6f 6e65 2061 6e64 2072 6561 6c74  t None and realt
-00022140: 696d 655f 656e 6420 6973 206e 6f74 204e  ime_end is not N
-00022150: 6f6e 6520 616e 6420 7265 616c 7469 6d65  one and realtime
-00022160: 5f73 7461 7274 203e 2072 6561 6c74 696d  _start > realtim
-00022170: 655f 656e 643a 0d0a 2020 2020 2020 2020  e_end:..        
-00022180: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00022190: 7272 6f72 2827 5468 6520 6461 7465 2073  rror('The date s
-000221a0: 6574 2062 7920 7661 7269 6162 6c65 2072  et by variable r
-000221b0: 6561 6c74 696d 655f 7374 6172 7420 2822  ealtime_start ("
-000221c0: 7b7d 2229 2063 616e 206e 6f74 2062 6520  {}") can not be 
-000221d0: 6166 7465 7220 7468 6520 6461 7465 2073  after the date s
-000221e0: 6574 2062 7920 7661 7269 6162 6c65 2072  et by variable r
-000221f0: 6561 6c74 696d 655f 656e 6420 2822 7b7d  ealtime_end ("{}
-00022200: 2229 2e27 2e66 6f72 6d61 7428 7265 616c  ").'.format(real
-00022210: 7469 6d65 5f73 7461 7274 2c20 7265 616c  time_start, real
-00022220: 7469 6d65 5f65 6e64 2929 0d0a 0d0a 2020  time_end))....  
-00022230: 2020 2020 2020 6466 203d 2070 642e 4461        df = pd.Da
-00022240: 7461 4672 616d 6528 0d0a 2020 2020 2020  taFrame(..      
-00022250: 2020 2020 2020 7365 6c66 2e5f 636c 6965        self._clie
-00022260: 6e74 2e67 6574 280d 0a20 2020 2020 2020  nt.get(..       
-00022270: 2020 2020 2020 2020 2027 2f66 7265 642f           '/fred/
-00022280: 736f 7572 6365 2f72 656c 6561 7365 7327  source/releases'
-00022290: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000222a0: 2020 2027 7265 6c65 6173 6573 272c 0d0a     'releases',..
-000222b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000222c0: 6c69 6d69 743d 3130 3030 2c0d 0a20 2020  limit=1000,..   
-000222d0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
-000222e0: 7263 655f 6964 3d73 6f75 7263 655f 6964  rce_id=source_id
-000222f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00022300: 2020 2072 6561 6c74 696d 655f 7374 6172     realtime_star
-00022310: 743d 7265 616c 7469 6d65 5f73 7461 7274  t=realtime_start
-00022320: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00022330: 2020 2072 6561 6c74 696d 655f 656e 643d     realtime_end=
-00022340: 7265 616c 7469 6d65 5f65 6e64 2c0d 0a20  realtime_end,.. 
-00022350: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00022360: 7264 6572 5f62 793d 6f72 6465 725f 6279  rder_by=order_by
-00022370: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00022380: 2020 2073 6f72 745f 6f72 6465 723d 736f     sort_order=so
-00022390: 7274 5f6f 7264 6572 0d0a 2020 2020 2020  rt_order..      
-000223a0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-000223b0: 2029 0d0a 0d0a 2020 2020 2020 2020 6461   )....        da
-000223c0: 7465 5f63 6f6c 756d 6e73 203d 205b 2772  te_columns = ['r
-000223d0: 6561 6c74 696d 655f 7374 6172 7427 2c20  ealtime_start', 
-000223e0: 2772 6561 6c74 696d 655f 656e 6427 5d0d  'realtime_end'].
-000223f0: 0a0d 0a20 2020 2020 2020 2069 6620 6e6f  ...        if no
-00022400: 7420 6466 2e65 6d70 7479 3a0d 0a20 2020  t df.empty:..   
-00022410: 2020 2020 2020 2020 2064 665b 6461 7465           df[date
-00022420: 5f63 6f6c 756d 6e73 5d20 3d20 6466 5b64  _columns] = df[d
-00022430: 6174 655f 636f 6c75 6d6e 735d 2e61 7070  ate_columns].app
-00022440: 6c79 2870 642e 746f 5f64 6174 6574 696d  ly(pd.to_datetim
-00022450: 652c 2066 6f72 6d61 743d 2725 592d 256d  e, format='%Y-%m
-00022460: 2d25 6427 290d 0a0d 0a20 2020 2020 2020  -%d')....       
-00022470: 2020 2020 2064 6620 3d20 6466 2e61 7374       df = df.ast
-00022480: 7970 6528 6474 7970 653d 7b0d 0a20 2020  ype(dtype={..   
-00022490: 2020 2020 2020 2020 2020 2020 2027 6e61               'na
-000224a0: 6d65 273a 2027 7374 7269 6e67 272c 0d0a  me': 'string',..
-000224b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000224c0: 276c 696e 6b27 3a20 2773 7472 696e 6727  'link': 'string'
-000224d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000224e0: 2020 2027 6e6f 7465 7327 3a20 2773 7472     'notes': 'str
-000224f0: 696e 6727 2c0d 0a20 2020 2020 2020 2020  ing',..         
-00022500: 2020 2020 2020 2027 7072 6573 735f 7265         'press_re
-00022510: 6c65 6173 6527 3a20 2762 6f6f 6c27 0d0a  lease': 'bool'..
-00022520: 2020 2020 2020 2020 2020 2020 7d29 2e73              }).s
-00022530: 6574 5f69 6e64 6578 2827 6964 2729 0d0a  et_index('id')..
-00022540: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00022550: 2064 660d 0a0d 0a20 2020 2022 2222 0d0a   df....    """..
-00022560: 2020 2020 5461 6773 0d0a 0d0a 2020 2020      Tags....    
-00022570: 6874 7470 733a 2f2f 6672 6564 2e73 746c  https://fred.stl
-00022580: 6f75 6973 6665 642e 6f72 672f 7461 6773  ouisfed.org/tags
-00022590: 0d0a 2020 2020 2222 220d 0a0d 0a20 2020  ..    """....   
-000225a0: 2064 6566 2074 6167 7328 0d0a 2020 2020   def tags(..    
-000225b0: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-000225c0: 2020 2020 2020 2020 2020 2072 6561 6c74             realt
-000225d0: 696d 655f 7374 6172 743a 2064 6174 6520  ime_start: date 
-000225e0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-000225f0: 2020 2020 2072 6561 6c74 696d 655f 656e       realtime_en
-00022600: 643a 2064 6174 6520 3d20 4e6f 6e65 2c0d  d: date = None,.
-00022610: 0a20 2020 2020 2020 2020 2020 2074 6167  .            tag
-00022620: 5f6e 616d 6573 3a20 4c69 7374 5b73 7472  _names: List[str
-00022630: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-00022640: 2020 2020 2020 2074 6167 5f67 726f 7570         tag_group
-00022650: 5f69 643a 2065 6e75 6d73 2e54 6167 4772  _id: enums.TagGr
-00022660: 6f75 7049 4420 3d20 4e6f 6e65 2c0d 0a20  oupID = None,.. 
-00022670: 2020 2020 2020 2020 2020 2073 6561 7263             searc
-00022680: 685f 7465 7874 3a20 7374 7220 3d20 4e6f  h_text: str = No
-00022690: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-000226a0: 206f 7264 6572 5f62 793a 2065 6e75 6d73   order_by: enums
-000226b0: 2e4f 7264 6572 4279 203d 2065 6e75 6d73  .OrderBy = enums
-000226c0: 2e4f 7264 6572 4279 2e73 6572 6965 735f  .OrderBy.series_
-000226d0: 636f 756e 742c 0d0a 2020 2020 2020 2020  count,..        
-000226e0: 2020 2020 736f 7274 5f6f 7264 6572 3a20      sort_order: 
-000226f0: 656e 756d 732e 536f 7274 4f72 6465 7220  enums.SortOrder 
-00022700: 3d20 656e 756d 732e 536f 7274 4f72 6465  = enums.SortOrde
-00022710: 722e 6173 630d 0a20 2020 2029 202d 3e20  r.asc..    ) -> 
-00022720: 7064 2e44 6174 6146 7261 6d65 3a0d 0a20  pd.DataFrame:.. 
-00022730: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00022740: 2020 2020 2323 2050 6172 616d 6574 6572      ## Parameter
-00022750: 730d 0a20 2020 2020 2020 2060 7265 616c  s..        `real
-00022760: 7469 6d65 5f73 7461 7274 600d 0a20 2020  time_start`..   
-00022770: 2020 2020 2054 6865 2073 7461 7274 206f       The start o
-00022780: 6620 7468 6520 7265 616c 2d74 696d 6520  f the real-time 
-00022790: 7065 7269 6f64 2e20 466f 7220 6d6f 7265  period. For more
-000227a0: 2069 6e66 6f72 6d61 7469 6f6e 2c20 7365   information, se
-000227b0: 6520 5b52 6561 6c2d 5469 6d65 2050 6572  e [Real-Time Per
-000227c0: 696f 6473 5d28 6874 7470 733a 2f2f 6672  iods](https://fr
-000227d0: 6564 2e73 746c 6f75 6973 6665 642e 6f72  ed.stlouisfed.or
-000227e0: 672f 646f 6373 2f61 7069 2f66 7265 642f  g/docs/api/fred/
-000227f0: 7265 616c 7469 6d65 5f70 6572 696f 642e  realtime_period.
-00022800: 6874 6d6c 292e 0d0a 0d0a 2020 2020 2020  html).....      
-00022810: 2020 6072 6561 6c74 696d 655f 656e 6460    `realtime_end`
-00022820: 0d0a 2020 2020 2020 2020 5468 6520 656e  ..        The en
-00022830: 6420 6f66 2074 6865 2072 6561 6c2d 7469  d of the real-ti
-00022840: 6d65 2070 6572 696f 642e 2046 6f72 206d  me period. For m
-00022850: 6f72 6520 696e 666f 726d 6174 696f 6e2c  ore information,
-00022860: 2073 6565 205b 5265 616c 2d54 696d 6520   see [Real-Time 
-00022870: 5065 7269 6f64 735d 2868 7474 7073 3a2f  Periods](https:/
-00022880: 2f66 7265 642e 7374 6c6f 7569 7366 6564  /fred.stlouisfed
-00022890: 2e6f 7267 2f64 6f63 732f 6170 692f 6672  .org/docs/api/fr
-000228a0: 6564 2f72 6561 6c74 696d 655f 7065 7269  ed/realtime_peri
-000228b0: 6f64 2e68 746d 6c29 2e0d 0a0d 0a20 2020  od.html).....   
-000228c0: 2020 2020 2060 7461 675f 6e61 6d65 7360       `tag_names`
-000228d0: 0d0a 2020 2020 2020 2020 5475 706c 6520  ..        Tuple 
-000228e0: 6f66 2074 6167 206e 616d 6573 2074 6861  of tag names tha
-000228f0: 7420 7365 7269 6573 206d 6174 6368 2061  t series match a
-00022900: 6c6c 206f 662e 0d0a 0d0a 2020 2020 2020  ll of.....      
-00022910: 2020 6074 6167 5f67 726f 7570 5f69 6460    `tag_group_id`
-00022920: 0d0a 2020 2020 2020 2020 4120 7461 6720  ..        A tag 
-00022930: 6772 6f75 7020 6964 2074 6f20 6669 6c74  group id to filt
-00022940: 6572 2074 6167 7320 6279 2074 7970 652e  er tags by type.
-00022950: 0d0a 0d0a 2020 2020 2020 2020 6073 6561  ....        `sea
-00022960: 7263 685f 7465 7874 600d 0a20 2020 2020  rch_text`..     
-00022970: 2020 2054 6865 2077 6f72 6473 2074 6f20     The words to 
-00022980: 6669 6e64 206d 6174 6368 696e 6720 7461  find matching ta
-00022990: 6773 2077 6974 682e 0d0a 0d0a 2020 2020  gs with.....    
-000229a0: 2020 2020 606f 7264 6572 5f62 7960 0d0a      `order_by`..
-000229b0: 2020 2020 2020 2020 4f72 6465 7220 7265          Order re
-000229c0: 7375 6c74 7320 6279 2076 616c 7565 7320  sults by values 
-000229d0: 6f66 2074 6865 2073 7065 6369 6669 6564  of the specified
-000229e0: 2061 7474 7269 6275 7465 2e0d 0a0d 0a20   attribute..... 
-000229f0: 2020 2020 2020 2060 736f 7274 5f6f 7264         `sort_ord
-00022a00: 6572 600d 0a20 2020 2020 2020 2053 6f72  er`..        Sor
-00022a10: 7420 7265 7375 6c74 7320 6973 2061 7363  t results is asc
-00022a20: 656e 6469 6e67 206f 7220 6465 7363 656e  ending or descen
-00022a30: 6469 6e67 206f 7264 6572 2066 6f72 2061  ding order for a
-00022a40: 7474 7269 6275 7465 2076 616c 7565 7320  ttribute values 
-00022a50: 7370 6563 6966 6965 6420 6279 206f 7264  specified by ord
-00022a60: 6572 5f62 792e 0d0a 0d0a 2020 2020 2020  er_by.....      
-00022a70: 2020 2323 2044 6573 6372 6970 7469 6f6e    ## Description
-00022a80: 0d0a 2020 2020 2020 2020 6874 7470 733a  ..        https:
-00022a90: 2f2f 6672 6564 2e73 746c 6f75 6973 6665  //fred.stlouisfe
-00022aa0: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
-00022ab0: 7265 642f 7461 6773 2e68 746d 6c0d 0a0d  red/tags.html...
-00022ac0: 0a20 2020 2020 2020 2047 6574 2046 5245  .        Get FRE
-00022ad0: 4420 7461 6773 2e20 4f70 7469 6f6e 616c  D tags. Optional
-00022ae0: 6c79 2c20 6669 6c74 6572 2072 6573 756c  ly, filter resul
-00022af0: 7473 2062 7920 7461 6720 6e61 6d65 2c20  ts by tag name, 
-00022b00: 7461 6720 6772 6f75 702c 206f 7220 7365  tag group, or se
-00022b10: 6172 6368 2e20 4652 4544 2074 6167 7320  arch. FRED tags 
-00022b20: 6172 6520 6174 7472 6962 7574 6573 2061  are attributes a
-00022b30: 7373 6967 6e65 6420 746f 2073 6572 6965  ssigned to serie
-00022b40: 732e 2053 6565 2074 6865 2072 656c 6174  s. See the relat
-00022b50: 6564 2072 6571 7565 7374 2066 7265 642f  ed request fred/
-00022b60: 7265 6c61 7465 645f 7461 6773 2e0d 0a0d  related_tags....
-00022b70: 0a20 2020 2020 2020 2023 2320 4150 4920  .        ## API 
-00022b80: 5265 7175 6573 7420 2848 5454 5053 2047  Request (HTTPS G
-00022b90: 4554 290d 0a20 2020 2020 2020 2068 7474  ET)..        htt
-00022ba0: 7073 3a2f 2f61 7069 2e73 746c 6f75 6973  ps://api.stlouis
-00022bb0: 6665 642e 6f72 672f 6672 6564 2f74 6167  fed.org/fred/tag
-00022bc0: 733f 6170 695f 6b65 793d 6162 6364 6566  s?api_key=abcdef
-00022bd0: 6768 696a 6b6c 6d6e 6f70 7172 7374 7576  ghijklmnopqrstuv
-00022be0: 7778 797a 3132 3334 3536 2666 696c 655f  wxyz123456&file_
-00022bf0: 7479 7065 3d6a 736f 6e0d 0a0d 0a20 2020  type=json....   
-00022c00: 2020 2020 2023 2320 4150 4920 5265 7370       ## API Resp
-00022c10: 6f6e 7365 0d0a 2020 2020 2020 2020 6060  onse..        ``
-00022c20: 606a 736f 6e0d 0a20 2020 2020 2020 207b  `json..        {
-00022c30: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-00022c40: 6561 6c74 696d 655f 7374 6172 7422 3a20  ealtime_start": 
-00022c50: 2232 3031 332d 3038 2d31 3422 2c0d 0a20  "2013-08-14",.. 
-00022c60: 2020 2020 2020 2020 2020 2022 7265 616c             "real
-00022c70: 7469 6d65 5f65 6e64 223a 2022 3230 3133  time_end": "2013
-00022c80: 2d30 382d 3134 222c 0d0a 2020 2020 2020  -08-14",..      
-00022c90: 2020 2020 2020 226f 7264 6572 5f62 7922        "order_by"
-00022ca0: 3a20 2273 6572 6965 735f 636f 756e 7422  : "series_count"
-00022cb0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00022cc0: 736f 7274 5f6f 7264 6572 223a 2022 6465  sort_order": "de
-00022cd0: 7363 222c 0d0a 2020 2020 2020 2020 2020  sc",..          
-00022ce0: 2020 2263 6f75 6e74 223a 2034 3739 342c    "count": 4794,
-00022cf0: 0d0a 2020 2020 2020 2020 2020 2020 226f  ..            "o
-00022d00: 6666 7365 7422 3a20 302c 0d0a 2020 2020  ffset": 0,..    
-00022d10: 2020 2020 2020 2020 226c 696d 6974 223a          "limit":
-00022d20: 2031 3030 302c 0d0a 2020 2020 2020 2020   1000,..        
-00022d30: 2020 2020 2274 6167 7322 3a20 5b0d 0a20      "tags": [.. 
-00022d40: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00022d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00022d60: 2020 2020 2020 226e 616d 6522 3a20 226e        "name": "n
-00022d70: 6174 696f 6e22 2c0d 0a20 2020 2020 2020  ation",..       
-00022d80: 2020 2020 2020 2020 2020 2020 2022 6772               "gr
-00022d90: 6f75 705f 6964 223a 2022 6765 6f74 222c  oup_id": "geot",
-00022da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00022db0: 2020 2020 2020 226e 6f74 6573 223a 2022        "notes": "
-00022dc0: 436f 756e 7472 7920 4c65 7665 6c22 2c0d  Country Level",.
-00022dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022de0: 2020 2020 2022 6372 6561 7465 6422 3a20       "created": 
-00022df0: 2232 3031 322d 3032 2d32 3720 3130 3a31  "2012-02-27 10:1
-00022e00: 383a 3139 2d30 3622 2c0d 0a20 2020 2020  8:19-06",..     
-00022e10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00022e20: 706f 7075 6c61 7269 7479 223a 2031 3030  popularity": 100
-00022e30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00022e40: 2020 2020 2020 2022 7365 7269 6573 5f63         "series_c
-00022e50: 6f75 6e74 223a 2031 3035 3230 300d 0a20  ount": 105200.. 
-00022e60: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00022e70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00022e80: 2020 202e 2e2e 0d0a 2020 2020 2020 2020     .....        
-00022e90: 2020 2020 5d0d 0a20 2020 2020 2020 207d      ]..        }
-00022ea0: 0d0a 2020 2020 2020 2020 6060 600d 0a0d  ..        ```...
-00022eb0: 0a20 2020 2020 2020 2023 2320 5265 7475  .        ## Retu
-00022ec0: 726e 730d 0a20 2020 2020 2020 2060 7061  rns..        `pa
-00022ed0: 6e64 6173 2e44 6174 6146 7261 6d65 600d  ndas.DataFrame`.
-00022ee0: 0a0d 0a20 2020 2020 2020 2023 2320 4578  ...        ## Ex
-00022ef0: 616d 706c 650d 0a20 2020 2020 2020 2060  ample..        `
-00022f00: 6060 7079 7468 6f6e 0d0a 2020 2020 2020  ``python..      
-00022f10: 2020 3e3e 3e20 6672 6564 203d 2046 5245    >>> fred = FRE
-00022f20: 4428 6170 695f 6b65 793d 2761 6263 6465  D(api_key='abcde
-00022f30: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
-00022f40: 7677 7879 7a31 3233 3435 3627 290d 0a20  vwxyz123456').. 
-00022f50: 2020 2020 2020 203e 3e3e 2066 7265 642e         >>> fred.
-00022f60: 7461 6773 2829 2e68 6561 6428 290d 0a20  tags().head().. 
-00022f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022f80: 2020 2020 2020 2020 2020 6772 6f75 705f            group_
-00022f90: 6964 206e 6f74 6573 2020 2020 2020 2020  id notes        
-00022fa0: 2020 2020 2020 2020 2020 2063 7265 6174             creat
-00022fb0: 6564 2020 706f 7075 6c61 7269 7479 2020  ed  popularity  
-00022fc0: 7365 7269 6573 5f63 6f75 6e74 0d0a 2020  series_count..  
-00022fd0: 2020 2020 2020 2020 2020 6e61 6d65 0d0a            name..
-00022fe0: 2020 2020 2020 2020 2020 2020 3134 2079              14 y
-00022ff0: 6561 7273 202b 2020 2020 2020 2020 2020  ears +          
-00023000: 6765 6e20 2020 2020 2020 3230 3132 2d30  gen       2012-0
-00023010: 382d 3036 2031 393a 3430 3a35 362b 3030  8-06 19:40:56+00
-00023020: 3a30 3020 2020 2020 2020 2020 202d 3620  :00          -6 
-00023030: 2020 2020 2020 2020 2020 2020 320d 0a20              2.. 
-00023040: 2020 2020 2020 2020 2020 2032 2d6d 6f6e             2-mon
-00023050: 7468 202b 2020 2020 2020 2020 2020 2067  th +           g
-00023060: 656e 2020 2020 2020 2032 3031 322d 3038  en       2012-08
-00023070: 2d30 3620 3139 3a33 343a 3035 2b30 303a  -06 19:34:05+00:
-00023080: 3030 2020 2020 2020 2020 202d 3632 2020  00         -62  
-00023090: 2020 2020 2020 2020 2020 2032 0d0a 2020             2..  
-000230a0: 2020 2020 2020 2020 2020 322d 7765 656b            2-week
-000230b0: 2020 2020 2020 2020 2020 2020 2020 6765                ge
-000230c0: 6e20 2020 2020 2020 3230 3132 2d30 352d  n       2012-05-
-000230d0: 3235 2031 363a 3239 3a33 342b 3030 3a30  25 16:29:34+00:0
-000230e0: 3020 2020 2020 2020 2020 202d 3620 2020  0          -6   
-000230f0: 2020 2020 2020 2020 2020 320d 0a20 2020            2..   
-00023100: 2020 2020 2020 2020 2033 3020 746f 2033           30 to 3
-00023110: 3420 7965 6172 7320 2020 2020 2067 656e  4 years      gen
-00023120: 2020 2020 2020 2032 3031 332d 3130 2d31         2013-10-1
-00023130: 3020 3231 3a31 333a 3034 2b30 303a 3030  0 21:13:04+00:00
-00023140: 2020 2020 2020 2020 202d 3133 2020 2020           -13    
-00023150: 2020 2020 2020 2020 2032 0d0a 2020 2020           2..    
-00023160: 2020 2020 2020 2020 332d 6661 6d69 6c79          3-family
-00023170: 202b 2020 2020 2020 2020 2020 6765 6e20   +          gen 
-00023180: 2020 2020 2020 3230 3132 2d30 382d 3036        2012-08-06
-00023190: 2031 393a 3438 3a31 312b 3030 3a30 3020   19:48:11+00:00 
-000231a0: 2020 2020 2020 2020 2d34 3920 2020 2020          -49     
-000231b0: 2020 2020 2020 2020 320d 0a20 2020 2020          2..     
-000231c0: 2020 2060 6060 0d0a 2020 2020 2020 2020     ```..        
-000231d0: 2222 220d 0a0d 0a20 2020 2020 2020 2061  """....        a
-000231e0: 6c6c 6f77 6564 5f6f 7264 6572 7320 3d20  llowed_orders = 
-000231f0: 5b0d 0a20 2020 2020 2020 2020 2020 2065  [..            e
-00023200: 6e75 6d73 2e4f 7264 6572 4279 2e73 6572  nums.OrderBy.ser
-00023210: 6965 735f 636f 756e 742c 0d0a 2020 2020  ies_count,..    
-00023220: 2020 2020 2020 2020 656e 756d 732e 4f72          enums.Or
-00023230: 6465 7242 792e 706f 7075 6c61 7269 7479  derBy.popularity
-00023240: 2c0d 0a20 2020 2020 2020 2020 2020 2065  ,..            e
-00023250: 6e75 6d73 2e4f 7264 6572 4279 2e63 7265  nums.OrderBy.cre
-00023260: 6174 6564 2c0d 0a20 2020 2020 2020 2020  ated,..         
-00023270: 2020 2065 6e75 6d73 2e4f 7264 6572 4279     enums.OrderBy
-00023280: 2e6e 616d 652c 0d0a 2020 2020 2020 2020  .name,..        
-00023290: 2020 2020 656e 756d 732e 4f72 6465 7242      enums.OrderB
-000232a0: 792e 6772 6f75 705f 6964 0d0a 2020 2020  y.group_id..    
-000232b0: 2020 2020 5d0d 0a0d 0a20 2020 2020 2020      ]....       
-000232c0: 2069 6620 6f72 6465 725f 6279 206e 6f74   if order_by not
-000232d0: 2069 6e20 616c 6c6f 7765 645f 6f72 6465   in allowed_orde
-000232e0: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
-000232f0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00023300: 7228 2756 6172 6961 626c 6520 6f72 6465  r('Variable orde
-00023310: 725f 6279 2028 7b7d 2920 6973 206e 6f74  r_by ({}) is not
-00023320: 206f 6e65 206f 6620 7468 6520 7661 6c75   one of the valu
-00023330: 6573 3a20 7b7d 272e 666f 726d 6174 286f  es: {}'.format(o
-00023340: 7264 6572 5f62 792c 2027 2c20 272e 6a6f  rder_by, ', '.jo
-00023350: 696e 286d 6170 2873 7472 2c20 616c 6c6f  in(map(str, allo
-00023360: 7765 645f 6f72 6465 7273 2929 2929 0d0a  wed_orders))))..
-00023370: 0d0a 2020 2020 2020 2020 6966 2074 6167  ..        if tag
-00023380: 5f67 726f 7570 5f69 6420 6973 206e 6f74  _group_id is not
-00023390: 204e 6f6e 6520 616e 6420 7461 675f 6772   None and tag_gr
-000233a0: 6f75 705f 6964 206e 6f74 2069 6e20 656e  oup_id not in en
-000233b0: 756d 732e 5461 6747 726f 7570 4944 3a0d  ums.TagGroupID:.
-000233c0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000233d0: 7365 2056 616c 7565 4572 726f 7228 2756  se ValueError('V
-000233e0: 6172 6961 626c 6520 7461 675f 6772 6f75  ariable tag_grou
-000233f0: 705f 6964 2028 7b7d 2920 6973 206e 6f74  p_id ({}) is not
-00023400: 206f 6e65 206f 6620 7468 6520 7661 6c75   one of the valu
-00023410: 6573 3a20 7b7d 272e 666f 726d 6174 2874  es: {}'.format(t
-00023420: 6167 5f67 726f 7570 5f69 642c 2027 2c20  ag_group_id, ', 
-00023430: 272e 6a6f 696e 286d 6170 2873 7472 2c20  '.join(map(str, 
-00023440: 656e 756d 732e 5461 6747 726f 7570 4944  enums.TagGroupID
-00023450: 2929 2929 0d0a 0d0a 2020 2020 2020 2020  ))))....        
-00023460: 6966 2072 6561 6c74 696d 655f 7374 6172  if realtime_star
-00023470: 7420 6973 206e 6f74 204e 6f6e 6520 616e  t is not None an
-00023480: 6420 7265 616c 7469 6d65 5f73 7461 7274  d realtime_start
-00023490: 203c 2064 6174 6528 3137 3736 2c20 372c   < date(1776, 7,
-000234a0: 2034 293a 0d0a 2020 2020 2020 2020 2020   4):..          
-000234b0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-000234c0: 6f72 2827 5661 7269 6162 6c65 2072 6561  or('Variable rea
-000234d0: 6c74 696d 655f 7374 6172 7420 2822 7b7d  ltime_start ("{}
-000234e0: 2229 2069 7320 6265 666f 7265 206d 696e  ") is before min
-000234f0: 2064 6174 6520 3137 3736 2d30 372d 3034   date 1776-07-04
-00023500: 2e27 2e66 6f72 6d61 7428 7265 616c 7469  .'.format(realti
-00023510: 6d65 5f73 7461 7274 2929 0d0a 0d0a 2020  me_start))....  
-00023520: 2020 2020 2020 6966 2072 6561 6c74 696d        if realtim
-00023530: 655f 7374 6172 7420 6973 206e 6f74 204e  e_start is not N
-00023540: 6f6e 6520 616e 6420 7265 616c 7469 6d65  one and realtime
-00023550: 5f65 6e64 2069 7320 6e6f 7420 4e6f 6e65  _end is not None
-00023560: 2061 6e64 2072 6561 6c74 696d 655f 7374   and realtime_st
-00023570: 6172 7420 3e20 7265 616c 7469 6d65 5f65  art > realtime_e
-00023580: 6e64 3a0d 0a20 2020 2020 2020 2020 2020  nd:..           
-00023590: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-000235a0: 7228 2754 6865 2064 6174 6520 7365 7420  r('The date set 
-000235b0: 6279 2076 6172 6961 626c 6520 7265 616c  by variable real
-000235c0: 7469 6d65 5f73 7461 7274 2028 227b 7d22  time_start ("{}"
-000235d0: 2920 6361 6e20 6e6f 7420 6265 2061 6674  ) can not be aft
-000235e0: 6572 2074 6865 2064 6174 6520 7365 7420  er the date set 
-000235f0: 6279 2076 6172 6961 626c 6520 7265 616c  by variable real
-00023600: 7469 6d65 5f65 6e64 2028 227b 7d22 292e  time_end ("{}").
-00023610: 272e 666f 726d 6174 2872 6561 6c74 696d  '.format(realtim
-00023620: 655f 7374 6172 742c 2072 6561 6c74 696d  e_start, realtim
-00023630: 655f 656e 6429 290d 0a0d 0a20 2020 2020  e_end))....     
-00023640: 2020 2064 6620 3d20 7064 2e44 6174 6146     df = pd.DataF
-00023650: 7261 6d65 280d 0a20 2020 2020 2020 2020  rame(..         
-00023660: 2020 2073 656c 662e 5f63 6c69 656e 742e     self._client.
-00023670: 6765 7428 0d0a 2020 2020 2020 2020 2020  get(..          
-00023680: 2020 2020 2020 272f 6672 6564 2f74 6167        '/fred/tag
-00023690: 7327 2c0d 0a20 2020 2020 2020 2020 2020  s',..           
-000236a0: 2020 2020 2027 7461 6773 272c 0d0a 2020       'tags',..  
-000236b0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-000236c0: 6d69 743d 3130 3030 2c0d 0a20 2020 2020  mit=1000,..     
-000236d0: 2020 2020 2020 2020 2020 2072 6561 6c74             realt
-000236e0: 696d 655f 7374 6172 743d 7265 616c 7469  ime_start=realti
-000236f0: 6d65 5f73 7461 7274 2c0d 0a20 2020 2020  me_start,..     
-00023700: 2020 2020 2020 2020 2020 2072 6561 6c74             realt
-00023710: 696d 655f 656e 643d 7265 616c 7469 6d65  ime_end=realtime
-00023720: 5f65 6e64 2c0d 0a20 2020 2020 2020 2020  _end,..         
-00023730: 2020 2020 2020 2074 6167 5f6e 616d 6573         tag_names
-00023740: 3d74 6167 5f6e 616d 6573 2c0d 0a20 2020  =tag_names,..   
-00023750: 2020 2020 2020 2020 2020 2020 2074 6167               tag
-00023760: 5f67 726f 7570 5f69 643d 7461 675f 6772  _group_id=tag_gr
-00023770: 6f75 705f 6964 2c0d 0a20 2020 2020 2020  oup_id,..       
-00023780: 2020 2020 2020 2020 2073 6561 7263 685f           search_
-00023790: 7465 7874 3d73 6561 7263 685f 7465 7874  text=search_text
-000237a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000237b0: 2020 206f 7264 6572 5f62 793d 6f72 6465     order_by=orde
-000237c0: 725f 6279 2c0d 0a20 2020 2020 2020 2020  r_by,..         
-000237d0: 2020 2020 2020 2073 6f72 745f 6f72 6465         sort_orde
-000237e0: 723d 736f 7274 5f6f 7264 6572 0d0a 2020  r=sort_order..  
-000237f0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00023800: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
-00023810: 2020 6966 206e 6f74 2064 662e 656d 7074    if not df.empt
-00023820: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00023830: 6466 2e63 7265 6174 6564 203d 2070 642e  df.created = pd.
-00023840: 746f 5f64 6174 6574 696d 6528 6466 2e63  to_datetime(df.c
-00023850: 7265 6174 6564 202b 2027 3030 272c 2075  reated + '00', u
-00023860: 7463 3d54 7275 652c 2066 6f72 6d61 743d  tc=True, format=
-00023870: 2725 592d 256d 2d25 6420 2548 3a25 4d3a  '%Y-%m-%d %H:%M:
-00023880: 2553 257a 2729 0d0a 0d0a 2020 2020 2020  %S%z')....      
-00023890: 2020 2020 2020 6466 203d 2064 662e 6173        df = df.as
-000238a0: 7479 7065 2864 7479 7065 3d7b 0d0a 2020  type(dtype={..  
-000238b0: 2020 2020 2020 2020 2020 2020 2020 276e                'n
-000238c0: 616d 6527 3a20 2773 7472 696e 6727 2c0d  ame': 'string',.
-000238d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000238e0: 2027 6e6f 7465 7327 3a20 2773 7472 696e   'notes': 'strin
-000238f0: 6727 2c0d 0a20 2020 2020 2020 2020 2020  g',..           
-00023900: 2020 2020 2027 6772 6f75 705f 6964 273a       'group_id':
-00023910: 2027 6361 7465 676f 7279 270d 0a20 2020   'category'..   
-00023920: 2020 2020 2020 2020 207d 292e 7365 745f           }).set_
-00023930: 696e 6465 7828 276e 616d 6527 290d 0a0d  index('name')...
-00023940: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00023950: 6466 0d0a 0d0a 2020 2020 6465 6620 7265  df....    def re
-00023960: 6c61 7465 645f 7461 6773 280d 0a20 2020  lated_tags(..   
-00023970: 2020 2020 2020 2020 2073 656c 662c 0d0a           self,..
-00023980: 2020 2020 2020 2020 2020 2020 7265 616c              real
-00023990: 7469 6d65 5f73 7461 7274 3a20 6461 7465  time_start: date
-000239a0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-000239b0: 2020 2020 2020 7265 616c 7469 6d65 5f65        realtime_e
-000239c0: 6e64 3a20 6461 7465 203d 204e 6f6e 652c  nd: date = None,
-000239d0: 0d0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
-000239e0: 675f 6e61 6d65 733a 204c 6973 745b 7374  g_names: List[st
-000239f0: 725d 203d 204e 6f6e 652c 0d0a 2020 2020  r] = None,..    
-00023a00: 2020 2020 2020 2020 6578 636c 7564 655f          exclude_
-00023a10: 7461 675f 6e61 6d65 733a 204c 6973 745b  tag_names: List[
-00023a20: 7374 725d 203d 204e 6f6e 652c 0d0a 2020  str] = None,..  
-00023a30: 2020 2020 2020 2020 2020 7461 675f 6772            tag_gr
-00023a40: 6f75 705f 6964 3a20 656e 756d 732e 5461  oup_id: enums.Ta
-00023a50: 6747 726f 7570 4944 203d 204e 6f6e 652c  gGroupID = None,
-00023a60: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00023a70: 6172 6368 5f74 6578 743a 2073 7472 203d  arch_text: str =
-00023a80: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00023a90: 2020 2020 6f72 6465 725f 6279 3a20 656e      order_by: en
-00023aa0: 756d 732e 4f72 6465 7242 7920 3d20 656e  ums.OrderBy = en
-00023ab0: 756d 732e 4f72 6465 7242 792e 7365 7269  ums.OrderBy.seri
-00023ac0: 6573 5f63 6f75 6e74 2c0d 0a20 2020 2020  es_count,..     
-00023ad0: 2020 2020 2020 2073 6f72 745f 6f72 6465         sort_orde
-00023ae0: 723a 2065 6e75 6d73 2e53 6f72 744f 7264  r: enums.SortOrd
-00023af0: 6572 203d 2065 6e75 6d73 2e53 6f72 744f  er = enums.SortO
-00023b00: 7264 6572 2e61 7363 0d0a 2020 2020 2920  rder.asc..    ) 
-00023b10: 2d3e 2070 642e 4461 7461 4672 616d 653a  -> pd.DataFrame:
-00023b20: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00023b30: 2020 2020 2020 2023 2320 5061 7261 6d65         ## Parame
-00023b40: 7465 7273 0d0a 2020 2020 2020 2020 6072  ters..        `r
-00023b50: 6561 6c74 696d 655f 7374 6172 7460 0d0a  ealtime_start`..
-00023b60: 2020 2020 2020 2020 5468 6520 7374 6172          The star
-00023b70: 7420 6f66 2074 6865 2072 6561 6c2d 7469  t of the real-ti
-00023b80: 6d65 2070 6572 696f 642e 2046 6f72 206d  me period. For m
-00023b90: 6f72 6520 696e 666f 726d 6174 696f 6e2c  ore information,
-00023ba0: 2073 6565 205b 5265 616c 2d54 696d 6520   see [Real-Time 
-00023bb0: 5065 7269 6f64 735d 2868 7474 7073 3a2f  Periods](https:/
-00023bc0: 2f66 7265 642e 7374 6c6f 7569 7366 6564  /fred.stlouisfed
-00023bd0: 2e6f 7267 2f64 6f63 732f 6170 692f 6672  .org/docs/api/fr
-00023be0: 6564 2f72 6561 6c74 696d 655f 7065 7269  ed/realtime_peri
-00023bf0: 6f64 2e68 746d 6c29 2e0d 0a0d 0a20 2020  od.html).....   
-00023c00: 2020 2020 2060 7265 616c 7469 6d65 5f65       `realtime_e
-00023c10: 6e64 600d 0a20 2020 2020 2020 2054 6865  nd`..        The
-00023c20: 2065 6e64 206f 6620 7468 6520 7265 616c   end of the real
-00023c30: 2d74 696d 6520 7065 7269 6f64 2e20 466f  -time period. Fo
-00023c40: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-00023c50: 6f6e 2c20 7365 6520 5b52 6561 6c2d 5469  on, see [Real-Ti
-00023c60: 6d65 2050 6572 696f 6473 5d28 6874 7470  me Periods](http
-00023c70: 733a 2f2f 6672 6564 2e73 746c 6f75 6973  s://fred.stlouis
-00023c80: 6665 642e 6f72 672f 646f 6373 2f61 7069  fed.org/docs/api
-00023c90: 2f66 7265 642f 7265 616c 7469 6d65 5f70  /fred/realtime_p
-00023ca0: 6572 696f 642e 6874 6d6c 292e 0d0a 0d0a  eriod.html).....
-00023cb0: 2020 2020 2020 2020 6074 6167 5f6e 616d          `tag_nam
-00023cc0: 6573 600d 0a20 2020 2020 2020 2054 7570  es`..        Tup
-00023cd0: 6c65 206f 6620 7461 6720 6e61 6d65 7320  le of tag names 
-00023ce0: 7468 6174 2073 6572 6965 7320 6d61 7463  that series matc
-00023cf0: 6820 616c 6c20 6f66 2e0d 0a0d 0a20 2020  h all of.....   
-00023d00: 2020 2020 2060 6578 636c 7564 655f 7461       `exclude_ta
-00023d10: 675f 6e61 6d65 7360 0d0a 2020 2020 2020  g_names`..      
-00023d20: 2020 5475 706c 6520 6f66 2074 6167 206e    Tuple of tag n
-00023d30: 616d 6573 2074 6861 7420 7365 7269 6573  ames that series
-00023d40: 206d 6174 6368 206e 6f6e 6520 6f66 2e0d   match none of..
-00023d50: 0a0d 0a20 2020 2020 2020 2060 7461 675f  ...        `tag_
-00023d60: 6772 6f75 705f 6964 600d 0a20 2020 2020  group_id`..     
-00023d70: 2020 2041 2074 6167 2067 726f 7570 2069     A tag group i
-00023d80: 6420 746f 2066 696c 7465 7220 7461 6773  d to filter tags
-00023d90: 2062 7920 7479 7065 2e0d 0a0d 0a20 2020   by type.....   
-00023da0: 2020 2020 2060 7365 6172 6368 5f74 6578       `search_tex
-00023db0: 7460 0d0a 2020 2020 2020 2020 5468 6520  t`..        The 
-00023dc0: 776f 7264 7320 746f 2066 696e 6420 6d61  words to find ma
-00023dd0: 7463 6869 6e67 2074 6167 7320 7769 7468  tching tags with
-00023de0: 2e0d 0a0d 0a20 2020 2020 2020 2060 6f72  .....        `or
-00023df0: 6465 725f 6279 600d 0a20 2020 2020 2020  der_by`..       
-00023e00: 204f 7264 6572 2072 6573 756c 7473 2062   Order results b
-00023e10: 7920 7661 6c75 6573 206f 6620 7468 6520  y values of the 
-00023e20: 7370 6563 6966 6965 6420 6174 7472 6962  specified attrib
-00023e30: 7574 652e 0d0a 0d0a 2020 2020 2020 2020  ute.....        
-00023e40: 6073 6f72 745f 6f72 6465 7260 0d0a 2020  `sort_order`..  
-00023e50: 2020 2020 2020 536f 7274 2072 6573 756c        Sort resul
-00023e60: 7473 2069 7320 6173 6365 6e64 696e 6720  ts is ascending 
-00023e70: 6f72 2064 6573 6365 6e64 696e 6720 6f72  or descending or
-00023e80: 6465 7220 666f 7220 6174 7472 6962 7574  der for attribut
-00023e90: 6520 7661 6c75 6573 2073 7065 6369 6669  e values specifi
-00023ea0: 6564 2062 7920 6f72 6465 725f 6279 2e0d  ed by order_by..
-00023eb0: 0a0d 0a20 2020 2020 2020 2023 2320 4465  ...        ## De
-00023ec0: 7363 7269 7074 696f 6e0d 0a20 2020 2020  scription..     
-00023ed0: 2020 2068 7474 7073 3a2f 2f66 7265 642e     https://fred.
-00023ee0: 7374 6c6f 7569 7366 6564 2e6f 7267 2f64  stlouisfed.org/d
-00023ef0: 6f63 732f 6170 692f 6672 6564 2f72 656c  ocs/api/fred/rel
-00023f00: 6174 6564 5f74 6167 732e 6874 6d6c 0d0a  ated_tags.html..
-00023f10: 0d0a 2020 2020 2020 2020 4765 7420 7468  ..        Get th
-00023f20: 6520 7265 6c61 7465 6420 4652 4544 2074  e related FRED t
-00023f30: 6167 7320 666f 7220 6f6e 6520 6f72 206d  ags for one or m
-00023f40: 6f72 6520 4652 4544 2074 6167 732e 0d0a  ore FRED tags...
-00023f50: 2020 2020 2020 2020 4f70 7469 6f6e 616c          Optional
-00023f60: 6c79 2c20 6669 6c74 6572 2072 6573 756c  ly, filter resul
-00023f70: 7473 2062 7920 7461 6720 6772 6f75 7020  ts by tag group 
-00023f80: 6f72 2073 6561 7263 682e 0d0a 2020 2020  or search...    
-00023f90: 2020 2020 4652 4544 2074 6167 7320 6172      FRED tags ar
-00023fa0: 6520 6174 7472 6962 7574 6573 2061 7373  e attributes ass
-00023fb0: 6967 6e65 6420 746f 2073 6572 6965 732e  igned to series.
-00023fc0: 0d0a 2020 2020 2020 2020 5265 6c61 7465  ..        Relate
-00023fd0: 6420 4652 4544 2074 6167 7320 6172 6520  d FRED tags are 
-00023fe0: 7468 6520 7461 6773 2061 7373 6967 6e65  the tags assigne
-00023ff0: 6420 746f 2073 6572 6965 7320 7468 6174  d to series that
-00024000: 206d 6174 6368 2061 6c6c 2074 6167 7320   match all tags 
-00024010: 696e 2074 6865 2074 6167 5f6e 616d 6573  in the tag_names
-00024020: 2070 6172 616d 6574 6572 2061 6e64 206e   parameter and n
-00024030: 6f20 7461 6773 2069 6e20 7468 6520 6578  o tags in the ex
-00024040: 636c 7564 655f 7461 675f 6e61 6d65 7320  clude_tag_names 
-00024050: 7061 7261 6d65 7465 722e 0d0a 2020 2020  parameter...    
-00024060: 2020 2020 5365 6520 7468 6520 7265 6c61      See the rela
-00024070: 7465 6420 7265 7175 6573 7420 6672 6564  ted request fred
-00024080: 2f74 6167 732e 0d0a 0d0a 2020 2020 2020  /tags.....      
-00024090: 2020 2323 2041 5049 2052 6571 7565 7374    ## API Request
-000240a0: 2028 4854 5450 5320 4745 5429 0d0a 2020   (HTTPS GET)..  
-000240b0: 2020 2020 2020 6874 7470 733a 2f2f 6170        https://ap
-000240c0: 692e 7374 6c6f 7569 7366 6564 2e6f 7267  i.stlouisfed.org
-000240d0: 2f66 7265 642f 7265 6c61 7465 645f 7461  /fred/related_ta
-000240e0: 6773 3f74 6167 5f6e 616d 6573 3d6d 6f6e  gs?tag_names=mon
-000240f0: 6574 6172 792b 6167 6772 6567 6174 6573  etary+aggregates
-00024100: 3b77 6565 6b6c 7926 6170 695f 6b65 793d  ;weekly&api_key=
-00024110: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
-00024120: 7172 7374 7576 7778 797a 3132 3334 3536  qrstuvwxyz123456
-00024130: 2666 696c 655f 7479 7065 3d6a 736f 6e0d  &file_type=json.
-00024140: 0a0d 0a20 2020 2020 2020 2023 2320 4150  ...        ## AP
-00024150: 4920 5265 7370 6f6e 7365 0d0a 2020 2020  I Response..    
-00024160: 2020 2020 6060 606a 736f 6e0d 0a20 2020      ```json..   
-00024170: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00024180: 2020 2020 2272 6561 6c74 696d 655f 7374      "realtime_st
-00024190: 6172 7422 3a20 2232 3031 332d 3038 2d31  art": "2013-08-1
-000241a0: 3422 2c0d 0a20 2020 2020 2020 2020 2020  4",..           
-000241b0: 2022 7265 616c 7469 6d65 5f65 6e64 223a   "realtime_end":
-000241c0: 2022 3230 3133 2d30 382d 3134 222c 0d0a   "2013-08-14",..
-000241d0: 2020 2020 2020 2020 2020 2020 226f 7264              "ord
-000241e0: 6572 5f62 7922 3a20 2273 6572 6965 735f  er_by": "series_
-000241f0: 636f 756e 7422 2c0d 0a20 2020 2020 2020  count",..       
-00024200: 2020 2020 2022 736f 7274 5f6f 7264 6572       "sort_order
-00024210: 223a 2022 6465 7363 222c 0d0a 2020 2020  ": "desc",..    
-00024220: 2020 2020 2020 2020 2263 6f75 6e74 223a          "count":
-00024230: 2031 332c 0d0a 2020 2020 2020 2020 2020   13,..          
-00024240: 2020 226f 6666 7365 7422 3a20 302c 0d0a    "offset": 0,..
-00024250: 2020 2020 2020 2020 2020 2020 226c 696d              "lim
-00024260: 6974 223a 2031 3030 302c 0d0a 2020 2020  it": 1000,..    
-00024270: 2020 2020 2020 2020 2274 6167 7322 3a20          "tags": 
-00024280: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
-00024290: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000242a0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-000242b0: 3a20 226e 6174 696f 6e22 2c0d 0a20 2020  : "nation",..   
-000242c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000242d0: 2022 6772 6f75 705f 6964 223a 2022 6765   "group_id": "ge
-000242e0: 6f74 222c 0d0a 2020 2020 2020 2020 2020  ot",..          
-000242f0: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
-00024300: 223a 2022 436f 756e 7472 7920 4c65 7665  ": "Country Leve
-00024310: 6c22 2c0d 0a20 2020 2020 2020 2020 2020  l",..           
-00024320: 2020 2020 2020 2020 2022 6372 6561 7465           "create
-00024330: 6422 3a20 2232 3031 322d 3032 2d32 3720  d": "2012-02-27 
-00024340: 3130 3a31 383a 3139 2d30 3622 2c0d 0a20  10:18:19-06",.. 
-00024350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024360: 2020 2022 706f 7075 6c61 7269 7479 223a     "popularity":
-00024370: 2031 3030 2c0d 0a20 2020 2020 2020 2020   100,..         
-00024380: 2020 2020 2020 2020 2020 2022 7365 7269             "seri
-00024390: 6573 5f63 6f75 6e74 223a 2031 320d 0a20  es_count": 12.. 
-000243a0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000243b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000243c0: 2020 202e 2e2e 0d0a 2020 2020 2020 2020     .....        
-000243d0: 2020 2020 5d0d 0a20 2020 2020 2020 207d      ]..        }
-000243e0: 0d0a 2020 2020 2020 2020 6060 600d 0a0d  ..        ```...
-000243f0: 0a20 2020 2020 2020 2023 2320 5265 7475  .        ## Retu
-00024400: 726e 730d 0a20 2020 2020 2020 2060 7061  rns..        `pa
-00024410: 6e64 6173 2e44 6174 6146 7261 6d65 600d  ndas.DataFrame`.
-00024420: 0a0d 0a20 2020 2020 2020 2023 2320 4578  ...        ## Ex
-00024430: 616d 706c 650d 0a20 2020 2020 2020 2060  ample..        `
-00024440: 6060 7079 7468 6f6e 0d0a 2020 2020 2020  ``python..      
-00024450: 2020 3e3e 3e20 6672 6564 203d 2046 5245    >>> fred = FRE
-00024460: 4428 6170 695f 6b65 793d 2761 6263 6465  D(api_key='abcde
-00024470: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
-00024480: 7677 7879 7a31 3233 3435 3627 290d 0a20  vwxyz123456').. 
-00024490: 2020 2020 2020 203e 3e3e 2066 7265 642e         >>> fred.
-000244a0: 7265 6c61 7465 645f 7461 6773 2874 6167  related_tags(tag
-000244b0: 5f6e 616d 6573 3d5b 276d 6f6e 6574 6172  _names=['monetar
-000244c0: 7920 6167 6772 6567 6174 6573 272c 2027  y aggregates', '
-000244d0: 7765 656b 6c79 275d 292e 6865 6164 2829  weekly']).head()
-000244e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000244f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024500: 2020 2020 2020 2020 2020 2020 2067 726f               gro
-00024510: 7570 5f69 6420 2020 2020 2020 2020 2020  up_id           
-00024520: 6e6f 7465 7320 2020 2020 2020 2020 2020  notes           
-00024530: 2020 2020 2020 2020 6372 6561 7465 6420          created 
-00024540: 2070 6f70 756c 6172 6974 7920 2073 6572   popularity  ser
-00024550: 6965 735f 636f 756e 740d 0a20 2020 2020  ies_count..     
-00024560: 2020 2020 2020 206e 616d 650d 0a20 2020         name..   
-00024570: 2020 2020 2020 2020 2063 6f70 7972 6967           copyrig
-00024580: 6874 6564 3a20 6369 7461 7469 6f6e 2072  hted: citation r
-00024590: 6571 7569 7265 6420 2020 2020 2020 6363  equired       cc
-000245a0: 2020 2020 2020 2020 2020 2020 3c4e 413e              <NA>
-000245b0: 2032 3031 382d 3132 2d31 3820 3035 3a33   2018-12-18 05:3
-000245c0: 333a 3133 2b30 303a 3030 2020 2020 2020  3:13+00:00      
-000245d0: 2020 2020 3838 2020 2020 2020 2020 2020      88          
-000245e0: 2020 2032 0d0a 2020 2020 2020 2020 2020     2..          
-000245f0: 2020 6375 7272 656e 6379 2020 2020 2020    currency      
-00024600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024610: 2020 2020 2020 6765 6e20 2020 2020 2020        gen       
-00024620: 2020 2020 2020 2020 2020 3230 3132 2d30            2012-0
-00024630: 322d 3237 2031 363a 3138 3a31 392b 3030  2-27 16:18:19+00
-00024640: 3a30 3020 2020 2020 2020 2020 2036 3220  :00          62 
-00024650: 2020 2020 2020 2020 2020 2020 320d 0a20              2.. 
-00024660: 2020 2020 2020 2020 2020 2066 7262 2073             frb s
-00024670: 746c 2020 2020 2020 2020 2020 2020 2020  tl              
-00024680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00024690: 7263 2020 2053 742e 204c 6f75 6973 2046  rc   St. Louis F
-000246a0: 6564 2032 3031 322d 3032 2d32 3720 3136  ed 2012-02-27 16
-000246b0: 3a31 383a 3139 2b30 303a 3030 2020 2020  :18:19+00:00    
-000246c0: 2020 2020 2020 3638 2020 2020 2020 2020        68        
+0001d7f0: 226f 6273 6572 7661 7469 6f6e 5f65 6e64  "observation_end
+0001d800: 223a 2022 3230 3133 2d30 372d 3031 222c  ": "2013-07-01",
+0001d810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d820: 2020 2020 2020 2266 7265 7175 656e 6379        "frequency
+0001d830: 223a 2022 4d6f 6e74 686c 7922 2c0d 0a20  ": "Monthly",.. 
+0001d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d850: 2020 2022 6672 6571 7565 6e63 795f 7368     "frequency_sh
+0001d860: 6f72 7422 3a20 224d 222c 0d0a 2020 2020  ort": "M",..    
+0001d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d880: 2275 6e69 7473 223a 2022 496e 6465 7820  "units": "Index 
+0001d890: 3139 3832 3d31 3030 222c 0d0a 2020 2020  1982=100",..    
+0001d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8b0: 2275 6e69 7473 5f73 686f 7274 223a 2022  "units_short": "
+0001d8c0: 496e 6465 7820 3139 3832 3d31 3030 222c  Index 1982=100",
+0001d8d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d8e0: 2020 2020 2020 2273 6561 736f 6e61 6c5f        "seasonal_
+0001d8f0: 6164 6a75 7374 6d65 6e74 223a 2022 5365  adjustment": "Se
+0001d900: 6173 6f6e 616c 6c79 2041 646a 7573 7465  asonally Adjuste
+0001d910: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
+0001d920: 2020 2020 2020 2020 2022 7365 6173 6f6e           "season
+0001d930: 616c 5f61 646a 7573 746d 656e 745f 7368  al_adjustment_sh
+0001d940: 6f72 7422 3a20 2253 4122 2c0d 0a20 2020  ort": "SA",..   
+0001d950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d960: 2022 6c61 7374 5f75 7064 6174 6564 223a   "last_updated":
+0001d970: 2022 3230 3133 2d30 382d 3134 2030 383a   "2013-08-14 08:
+0001d980: 3336 3a30 352d 3035 222c 0d0a 2020 2020  36:05-05",..    
+0001d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d9a0: 2270 6f70 756c 6172 6974 7922 3a20 3532  "popularity": 52
+0001d9b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d9c0: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
+0001d9d0: 2020 2020 2020 2e2e 2e0d 0a20 2020 2020        .....     
+0001d9e0: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+0001d9f0: 2020 7d0d 0a20 2020 2020 2020 2060 6060    }..        ```
+0001da00: 0d0a 0d0a 2020 2020 2020 2020 2323 2052  ....        ## R
+0001da10: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
+0001da20: 6070 616e 6461 732e 4461 7461 4672 616d  `pandas.DataFram
+0001da30: 6560 0d0a 0d0a 2020 2020 2020 2020 2323  e`....        ##
+0001da40: 2045 7861 6d70 6c65 0d0a 2020 2020 2020   Example..      
+0001da50: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
+0001da60: 2020 2020 203e 3e3e 2066 7265 6420 3d20       >>> fred = 
+0001da70: 4652 4544 2861 7069 5f6b 6579 3d27 6162  FRED(api_key='ab
+0001da80: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
+0001da90: 7374 7576 7778 797a 3132 3334 3536 2729  stuvwxyz123456')
+0001daa0: 0d0a 2020 2020 2020 2020 3e3e 3e20 6672  ..        >>> fr
+0001dab0: 6564 2e73 6572 6965 735f 7570 6461 7465  ed.series_update
+0001dac0: 7328 7374 6172 745f 7469 6d65 3d64 6174  s(start_time=dat
+0001dad0: 6574 696d 6528 3230 3232 2c20 312c 2031  etime(2022, 1, 1
+0001dae0: 3529 2c20 656e 645f 7469 6d65 3d64 6174  5), end_time=dat
+0001daf0: 6574 696d 6528 3230 3232 2c20 312c 2031  etime(2022, 1, 1
+0001db00: 3629 292e 6865 6164 2829 0d0a 2020 2020  6)).head()..    
+0001db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db20: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
+0001db30: 7265 616c 7469 6d65 5f65 6e64 2020 2020  realtime_end    
+0001db40: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+0001db50: 746c 6520 6f62 7365 7276 6174 696f 6e5f  tle observation_
+0001db60: 7374 6172 7420 6f62 7365 7276 6174 696f  start observatio
+0001db70: 6e5f 656e 6420 2020 2020 6672 6571 7565  n_end     freque
+0001db80: 6e63 7920 6672 6571 7565 6e63 795f 7368  ncy frequency_sh
+0001db90: 6f72 7420 2020 2020 2020 2020 756e 6974  ort         unit
+0001dba0: 7320 756e 6974 735f 7368 6f72 7420 2020  s units_short   
+0001dbb0: 2020 2073 6561 736f 6e61 6c5f 6164 6a75     seasonal_adju
+0001dbc0: 7374 6d65 6e74 2073 6561 736f 6e61 6c5f  stment seasonal_
+0001dbd0: 6164 6a75 7374 6d65 6e74 5f73 686f 7274  adjustment_short
+0001dbe0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0001dbf0: 7374 5f75 7064 6174 6564 2020 706f 7075  st_updated  popu
+0001dc00: 6c61 7269 7479 2020 2020 2020 2020 2020  larity          
+0001dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc30: 2020 2020 6e6f 7465 730d 0a20 2020 2020      notes..     
+0001dc40: 2020 2020 2020 2069 640d 0a20 2020 2020         id..     
+0001dc50: 2020 2020 2020 2053 5035 3030 2020 2020         SP500    
+0001dc60: 2020 2020 3230 3232 2d30 322d 3035 2020      2022-02-05  
+0001dc70: 2032 3032 322d 3032 2d30 3520 2020 2020   2022-02-05     
+0001dc80: 2020 2020 2020 2020 2020 2053 2650 2035             S&P 5
+0001dc90: 3030 2020 2020 2020 2020 3230 3132 2d30  00        2012-0
+0001dca0: 322d 3036 2020 2020 2020 3230 3232 2d30  2-06      2022-0
+0001dcb0: 322d 3034 2020 4461 696c 792c 2043 6c6f  2-04  Daily, Clo
+0001dcc0: 7365 2020 2020 2020 2020 2020 2020 2020  se              
+0001dcd0: 2044 2020 2020 2020 2020 2049 6e64 6578   D         Index
+0001dce0: 2020 2020 2020 2049 6e64 6578 2020 4e6f         Index  No
+0001dcf0: 7420 5365 6173 6f6e 616c 6c79 2041 646a  t Seasonally Adj
+0001dd00: 7573 7465 6420 2020 2020 2020 2020 2020  usted           
+0001dd10: 2020 2020 2020 2020 2020 2020 4e53 4120              NSA 
+0001dd20: 3230 3232 2d30 322d 3035 2030 313a 3131  2022-02-05 01:11
+0001dd30: 3a30 342b 3030 3a30 3020 2020 2020 2020  :04+00:00       
+0001dd40: 2020 2038 3520 2054 6865 206f 6273 6572     85  The obser
+0001dd50: 7661 7469 6f6e 7320 666f 7220 7468 6520  vations for the 
+0001dd60: 5326 5020 3530 3020 7265 7072 6573 656e  S&P 500 represen
+0001dd70: 7420 7468 652e 2e2e 0d0a 2020 2020 2020  t the.....      
+0001dd80: 2020 2020 2020 4342 4243 4855 5344 2020        CBBCHUSD  
+0001dd90: 2020 2032 3032 322d 3032 2d30 3520 2020     2022-02-05   
+0001dda0: 3230 3232 2d30 322d 3035 2020 436f 696e  2022-02-05  Coin
+0001ddb0: 6261 7365 2042 6974 636f 696e 2043 6173  base Bitcoin Cas
+0001ddc0: 6820 2020 2020 2020 2032 3031 372d 3132  h        2017-12
+0001ddd0: 2d32 3020 2020 2020 2032 3032 322d 3032  -20      2022-02
+0001dde0: 2d30 3420 2044 6169 6c79 2c20 372d 4461  -04  Daily, 7-Da
+0001ddf0: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+0001de00: 4420 2055 2e53 2e20 446f 6c6c 6172 7320  D  U.S. Dollars 
+0001de10: 2020 2020 2055 2e53 2e20 2420 204e 6f74       U.S. $  Not
+0001de20: 2053 6561 736f 6e61 6c6c 7920 4164 6a75   Seasonally Adju
+0001de30: 7374 6564 2020 2020 2020 2020 2020 2020  sted            
+0001de40: 2020 2020 2020 2020 2020 204e 5341 2032             NSA 2
+0001de50: 3032 322d 3032 2d30 3520 3031 3a30 343a  022-02-05 01:04:
+0001de60: 3037 2b30 303a 3030 2020 2020 2020 2020  07+00:00        
+0001de70: 2020 3232 2020 416c 6c20 6461 7461 2069    22  All data i
+0001de80: 7320 6173 206f 6620 3520 504d 2050 5354  s as of 5 PM PST
+0001de90: 2e0d 0a20 2020 2020 2020 2020 2020 2043  ...            C
+0001dea0: 4242 5443 5553 4420 2020 2020 3230 3232  BBTCUSD     2022
+0001deb0: 2d30 322d 3035 2020 2032 3032 322d 3032  -02-05   2022-02
+0001dec0: 2d30 3520 2020 2020 2020 436f 696e 6261  -05       Coinba
+0001ded0: 7365 2042 6974 636f 696e 2020 2020 2020  se Bitcoin      
+0001dee0: 2020 3230 3134 2d31 322d 3031 2020 2020    2014-12-01    
+0001def0: 2020 3230 3232 2d30 322d 3034 2020 4461    2022-02-04  Da
+0001df00: 696c 792c 2037 2d44 6179 2020 2020 2020  ily, 7-Day      
+0001df10: 2020 2020 2020 2020 2044 2020 552e 532e           D  U.S.
+0001df20: 2044 6f6c 6c61 7273 2020 2020 2020 552e   Dollars      U.
+0001df30: 532e 2024 2020 4e6f 7420 5365 6173 6f6e  S. $  Not Season
+0001df40: 616c 6c79 2041 646a 7573 7465 6420 2020  ally Adjusted   
+0001df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df60: 2020 2020 4e53 4120 3230 3232 2d30 322d      NSA 2022-02-
+0001df70: 3035 2030 313a 3034 3a30 362b 3030 3a30  05 01:04:06+00:0
+0001df80: 3020 2020 2020 2020 2020 2036 3520 2041  0          65  A
+0001df90: 6c6c 2064 6174 6120 6973 2061 7320 6f66  ll data is as of
+0001dfa0: 2035 2050 4d20 5053 542e 0d0a 2020 2020   5 PM PST...    
+0001dfb0: 2020 2020 2020 2020 4342 4554 4855 5344          CBETHUSD
+0001dfc0: 2020 2020 2032 3032 322d 3032 2d30 3520       2022-02-05 
+0001dfd0: 2020 3230 3232 2d30 322d 3035 2020 2020    2022-02-05    
+0001dfe0: 2020 436f 696e 6261 7365 2045 7468 6572    Coinbase Ether
+0001dff0: 6575 6d20 2020 2020 2020 2032 3031 362d  eum        2016-
+0001e000: 3035 2d31 3820 2020 2020 2032 3032 322d  05-18      2022-
+0001e010: 3032 2d30 3420 2044 6169 6c79 2c20 372d  02-04  Daily, 7-
+0001e020: 4461 7920 2020 2020 2020 2020 2020 2020  Day             
+0001e030: 2020 4420 2055 2e53 2e20 446f 6c6c 6172    D  U.S. Dollar
+0001e040: 7320 2020 2020 2055 2e53 2e20 2420 204e  s      U.S. $  N
+0001e050: 6f74 2053 6561 736f 6e61 6c6c 7920 4164  ot Seasonally Ad
+0001e060: 6a75 7374 6564 2020 2020 2020 2020 2020  justed          
+0001e070: 2020 2020 2020 2020 2020 2020 204e 5341               NSA
+0001e080: 2032 3032 322d 3032 2d30 3520 3031 3a30   2022-02-05 01:0
+0001e090: 343a 3035 2b30 303a 3030 2020 2020 2020  4:05+00:00      
+0001e0a0: 2020 2020 3434 2020 416c 6c20 6461 7461      44  All data
+0001e0b0: 2069 7320 6173 206f 6620 3520 504d 2050   is as of 5 PM P
+0001e0c0: 5354 2e0d 0a20 2020 2020 2020 2020 2020  ST...           
+0001e0d0: 2043 424c 5443 5553 4420 2020 2020 3230   CBLTCUSD     20
+0001e0e0: 3232 2d30 322d 3035 2020 2032 3032 322d  22-02-05   2022-
+0001e0f0: 3032 2d30 3520 2020 2020 2043 6f69 6e62  02-05      Coinb
+0001e100: 6173 6520 4c69 7465 636f 696e 2020 2020  ase Litecoin    
+0001e110: 2020 2020 3230 3136 2d30 382d 3137 2020      2016-08-17  
+0001e120: 2020 2020 3230 3232 2d30 322d 3034 2020      2022-02-04  
+0001e130: 4461 696c 792c 2037 2d44 6179 2020 2020  Daily, 7-Day    
+0001e140: 2020 2020 2020 2020 2020 2044 2020 552e             D  U.
+0001e150: 532e 2044 6f6c 6c61 7273 2020 2020 2020  S. Dollars      
+0001e160: 552e 532e 2024 2020 4e6f 7420 5365 6173  U.S. $  Not Seas
+0001e170: 6f6e 616c 6c79 2041 646a 7573 7465 6420  onally Adjusted 
+0001e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e190: 2020 2020 2020 4e53 4120 3230 3232 2d30        NSA 2022-0
+0001e1a0: 322d 3035 2030 313a 3034 3a30 332b 3030  2-05 01:04:03+00
+0001e1b0: 3a30 3020 2020 2020 2020 2020 2032 3020  :00          20 
+0001e1c0: 2041 6c6c 2064 6174 6120 6973 2061 7320   All data is as 
+0001e1d0: 6f66 2035 2050 4d20 5053 542e 0d0a 2020  of 5 PM PST...  
+0001e1e0: 2020 2020 2020 6060 600d 0a20 2020 2020        ```..     
+0001e1f0: 2020 2022 2222 0d0a 0d0a 2020 2020 2020     """....      
+0001e200: 2020 6966 2066 696c 7465 725f 7661 6c75    if filter_valu
+0001e210: 6520 6e6f 7420 696e 2065 6e75 6d73 2e46  e not in enums.F
+0001e220: 696c 7465 7256 616c 7565 3a0d 0a20 2020  ilterValue:..   
+0001e230: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0001e240: 616c 7565 4572 726f 7228 2756 6172 6961  alueError('Varia
+0001e250: 626c 6520 6669 6c74 6572 5f76 616c 7565  ble filter_value
+0001e260: 2028 7b7d 2920 6973 206e 6f74 206f 6e65   ({}) is not one
+0001e270: 206f 6620 7468 6520 7661 6c75 6573 3a20   of the values: 
+0001e280: 7b7d 272e 666f 726d 6174 2866 696c 7465  {}'.format(filte
+0001e290: 725f 7661 6c75 652c 2027 2c20 272e 6a6f  r_value, ', '.jo
+0001e2a0: 696e 286d 6170 2873 7472 2c20 656e 756d  in(map(str, enum
+0001e2b0: 732e 4669 6c74 6572 5661 6c75 6529 2929  s.FilterValue)))
+0001e2c0: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+0001e2d0: 7374 6172 745f 7469 6d65 2069 7320 6e6f  start_time is no
+0001e2e0: 7420 4e6f 6e65 2061 6e64 2065 6e64 5f74  t None and end_t
+0001e2f0: 696d 6520 6973 204e 6f6e 653a 0d0a 2020  ime is None:..  
+0001e300: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0001e310: 5661 6c75 6545 7272 6f72 2827 656e 645f  ValueError('end_
+0001e320: 7469 6d65 2069 7320 7265 7175 6972 6564  time is required
+0001e330: 2069 6620 7374 6172 745f 7469 6d65 2069   if start_time i
+0001e340: 7320 7365 7427 290d 0a0d 0a20 2020 2020  s set')....     
+0001e350: 2020 2069 6620 656e 645f 7469 6d65 2069     if end_time i
+0001e360: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
+0001e370: 7461 7274 5f74 696d 6520 6973 204e 6f6e  tart_time is Non
+0001e380: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0001e390: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0001e3a0: 2827 7374 6172 745f 7469 6d65 2069 7320  ('start_time is 
+0001e3b0: 7265 7175 6972 6564 2069 6620 656e 645f  required if end_
+0001e3c0: 7469 6d65 2069 7320 7365 7427 290d 0a0d  time is set')...
+0001e3d0: 0a20 2020 2020 2020 2069 6620 7374 6172  .        if star
+0001e3e0: 745f 7469 6d65 2069 7320 6e6f 7420 4e6f  t_time is not No
+0001e3f0: 6e65 2061 6e64 2065 6e64 5f74 696d 6520  ne and end_time 
+0001e400: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+0001e410: 7374 6172 745f 7469 6d65 203e 3d20 656e  start_time >= en
+0001e420: 645f 7469 6d65 3a0d 0a20 2020 2020 2020  d_time:..       
+0001e430: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0001e440: 4572 726f 7228 2765 6e64 5f74 696d 6520  Error('end_time 
+0001e450: 6d75 7374 2062 6520 6772 6561 7465 7220  must be greater 
+0001e460: 7468 616e 2073 7461 7274 5f74 696d 6527  than start_time'
+0001e470: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+0001e480: 7265 616c 7469 6d65 5f73 7461 7274 2069  realtime_start i
+0001e490: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2072  s not None and r
+0001e4a0: 6561 6c74 696d 655f 7374 6172 7420 3c20  ealtime_start < 
+0001e4b0: 6461 7465 2831 3737 362c 2037 2c20 3429  date(1776, 7, 4)
+0001e4c0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+0001e4d0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0001e4e0: 2756 6172 6961 626c 6520 7265 616c 7469  'Variable realti
+0001e4f0: 6d65 5f73 7461 7274 2028 227b 7d22 2920  me_start ("{}") 
+0001e500: 6973 2062 6566 6f72 6520 6d69 6e20 6461  is before min da
+0001e510: 7465 2031 3737 362d 3037 2d30 342e 272e  te 1776-07-04.'.
+0001e520: 666f 726d 6174 2872 6561 6c74 696d 655f  format(realtime_
+0001e530: 7374 6172 7429 290d 0a0d 0a20 2020 2020  start))....     
+0001e540: 2020 2069 6620 7265 616c 7469 6d65 5f73     if realtime_s
+0001e550: 7461 7274 2069 7320 6e6f 7420 4e6f 6e65  tart is not None
+0001e560: 2061 6e64 2072 6561 6c74 696d 655f 656e   and realtime_en
+0001e570: 6420 6973 206e 6f74 204e 6f6e 6520 616e  d is not None an
+0001e580: 6420 7265 616c 7469 6d65 5f73 7461 7274  d realtime_start
+0001e590: 203e 2072 6561 6c74 696d 655f 656e 643a   > realtime_end:
+0001e5a0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+0001e5b0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+0001e5c0: 5468 6520 6461 7465 2073 6574 2062 7920  The date set by 
+0001e5d0: 7661 7269 6162 6c65 2072 6561 6c74 696d  variable realtim
+0001e5e0: 655f 7374 6172 7420 2822 7b7d 2229 2063  e_start ("{}") c
+0001e5f0: 616e 206e 6f74 2062 6520 6166 7465 7220  an not be after 
+0001e600: 7468 6520 6461 7465 2073 6574 2062 7920  the date set by 
+0001e610: 7661 7269 6162 6c65 2072 6561 6c74 696d  variable realtim
+0001e620: 655f 656e 6420 2822 7b7d 2229 2e27 2e66  e_end ("{}").'.f
+0001e630: 6f72 6d61 7428 7265 616c 7469 6d65 5f73  ormat(realtime_s
+0001e640: 7461 7274 2c20 7265 616c 7469 6d65 5f65  tart, realtime_e
+0001e650: 6e64 2929 0d0a 0d0a 2020 2020 2020 2020  nd))....        
+0001e660: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
+0001e670: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+0001e680: 7365 6c66 2e5f 636c 6965 6e74 2e67 6574  self._client.get
+0001e690: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001e6a0: 2020 2027 2f66 7265 642f 7365 7269 6573     '/fred/series
+0001e6b0: 2f75 7064 6174 6573 272c 0d0a 2020 2020  /updates',..    
+0001e6c0: 2020 2020 2020 2020 2020 2020 2773 6572              'ser
+0001e6d0: 6965 7373 272c 0d0a 2020 2020 2020 2020  iess',..        
+0001e6e0: 2020 2020 2020 2020 6c69 6d69 743d 3130          limit=10
+0001e6f0: 3030 2c0d 0a20 2020 2020 2020 2020 2020  00,..           
+0001e700: 2020 2020 2072 6561 6c74 696d 655f 7374       realtime_st
+0001e710: 6172 743d 7265 616c 7469 6d65 5f73 7461  art=realtime_sta
+0001e720: 7274 2c0d 0a20 2020 2020 2020 2020 2020  rt,..           
+0001e730: 2020 2020 2072 6561 6c74 696d 655f 656e       realtime_en
+0001e740: 643d 7265 616c 7469 6d65 5f65 6e64 2c0d  d=realtime_end,.
+0001e750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e760: 2066 696c 7465 725f 7661 6c75 653d 6669   filter_value=fi
+0001e770: 6c74 6572 5f76 616c 7565 2c0d 0a20 2020  lter_value,..   
+0001e780: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0001e790: 7274 5f74 696d 653d 7374 6172 745f 7469  rt_time=start_ti
+0001e7a0: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
+0001e7b0: 2020 2020 2065 6e64 5f74 696d 653d 656e       end_time=en
+0001e7c0: 645f 7469 6d65 0d0a 2020 2020 2020 2020  d_time..        
+0001e7d0: 2020 2020 290d 0a20 2020 2020 2020 2029      )..        )
+0001e7e0: 0d0a 0d0a 2020 2020 2020 2020 6461 7465  ....        date
+0001e7f0: 5f63 6f6c 756d 6e73 203d 205b 0d0a 2020  _columns = [..  
+0001e800: 2020 2020 2020 2020 2020 2772 6561 6c74            'realt
+0001e810: 696d 655f 7374 6172 7427 2c20 2772 6561  ime_start', 'rea
+0001e820: 6c74 696d 655f 656e 6427 2c0d 0a20 2020  ltime_end',..   
+0001e830: 2020 2020 2020 2020 2027 6f62 7365 7276           'observ
+0001e840: 6174 696f 6e5f 7374 6172 7427 2c20 276f  ation_start', 'o
+0001e850: 6273 6572 7661 7469 6f6e 5f65 6e64 270d  bservation_end'.
+0001e860: 0a20 2020 2020 2020 205d 0d0a 0d0a 2020  .        ]....  
+0001e870: 2020 2020 2020 6966 206e 6f74 2064 662e        if not df.
+0001e880: 656d 7074 793a 0d0a 2020 2020 2020 2020  empty:..        
+0001e890: 2020 2020 6466 5b64 6174 655f 636f 6c75      df[date_colu
+0001e8a0: 6d6e 735d 203d 2064 665b 6461 7465 5f63  mns] = df[date_c
+0001e8b0: 6f6c 756d 6e73 5d2e 6170 706c 7928 7064  olumns].apply(pd
+0001e8c0: 2e74 6f5f 6461 7465 7469 6d65 2c20 666f  .to_datetime, fo
+0001e8d0: 726d 6174 3d27 2559 2d25 6d2d 2564 2729  rmat='%Y-%m-%d')
+0001e8e0: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+0001e8f0: 2e6c 6173 745f 7570 6461 7465 6420 3d20  .last_updated = 
+0001e900: 7064 2e74 6f5f 6461 7465 7469 6d65 2864  pd.to_datetime(d
+0001e910: 662e 6c61 7374 5f75 7064 6174 6564 202b  f.last_updated +
+0001e920: 2027 3030 272c 2075 7463 3d54 7275 652c   '00', utc=True,
+0001e930: 2066 6f72 6d61 743d 2725 592d 256d 2d25   format='%Y-%m-%
+0001e940: 6420 2548 3a25 4d3a 2553 257a 2729 0d0a  d %H:%M:%S%z')..
+0001e950: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+0001e960: 203d 2064 662e 6173 7479 7065 2864 7479   = df.astype(dty
+0001e970: 7065 3d7b 0d0a 2020 2020 2020 2020 2020  pe={..          
+0001e980: 2020 2020 2020 2769 6427 3a20 2773 7472        'id': 'str
+0001e990: 696e 6727 2c0d 0a20 2020 2020 2020 2020  ing',..         
+0001e9a0: 2020 2020 2020 2027 6e6f 7465 7327 3a20         'notes': 
+0001e9b0: 2773 7472 696e 6727 2c0d 0a20 2020 2020  'string',..     
+0001e9c0: 2020 2020 2020 2020 2020 2027 7469 746c             'titl
+0001e9d0: 6527 3a20 2773 7472 696e 6727 2c0d 0a20  e': 'string',.. 
+0001e9e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001e9f0: 7365 6173 6f6e 616c 5f61 646a 7573 746d  seasonal_adjustm
+0001ea00: 656e 7427 3a20 2763 6174 6567 6f72 7927  ent': 'category'
+0001ea10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001ea20: 2020 2027 7365 6173 6f6e 616c 5f61 646a     'seasonal_adj
+0001ea30: 7573 746d 656e 745f 7368 6f72 7427 3a20  ustment_short': 
+0001ea40: 2763 6174 6567 6f72 7927 2c0d 0a20 2020  'category',..   
+0001ea50: 2020 2020 2020 2020 2020 2020 2027 756e               'un
+0001ea60: 6974 7327 3a20 2763 6174 6567 6f72 7927  its': 'category'
+0001ea70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001ea80: 2020 2027 756e 6974 735f 7368 6f72 7427     'units_short'
+0001ea90: 3a20 2763 6174 6567 6f72 7927 2c0d 0a20  : 'category',.. 
+0001eaa0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001eab0: 6672 6571 7565 6e63 7927 3a20 2763 6174  frequency': 'cat
+0001eac0: 6567 6f72 7927 2c0d 0a20 2020 2020 2020  egory',..       
+0001ead0: 2020 2020 2020 2020 2027 6672 6571 7565           'freque
+0001eae0: 6e63 795f 7368 6f72 7427 3a20 2763 6174  ncy_short': 'cat
+0001eaf0: 6567 6f72 7927 2c0d 0a20 2020 2020 2020  egory',..       
+0001eb00: 2020 2020 207d 292e 7365 745f 696e 6465       }).set_inde
+0001eb10: 7828 2769 6427 290d 0a0d 0a20 2020 2020  x('id')....     
+0001eb20: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
+0001eb30: 2020 2020 6465 6620 7365 7269 6573 5f76      def series_v
+0001eb40: 696e 7461 6765 6461 7465 7328 0d0a 2020  intagedates(..  
+0001eb50: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+0001eb60: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+0001eb70: 6965 735f 6964 3a20 7374 722c 0d0a 2020  ies_id: str,..  
+0001eb80: 2020 2020 2020 2020 2020 7265 616c 7469            realti
+0001eb90: 6d65 5f73 7461 7274 3a20 6461 7465 203d  me_start: date =
+0001eba0: 2064 6174 6528 3137 3736 2c20 372c 2034   date(1776, 7, 4
+0001ebb0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0001ebc0: 7265 616c 7469 6d65 5f65 6e64 3a20 6461  realtime_end: da
+0001ebd0: 7465 203d 2064 6174 6528 3939 3939 2c20  te = date(9999, 
+0001ebe0: 3132 2c20 3331 292c 0d0a 2020 2020 2020  12, 31),..      
+0001ebf0: 2020 2020 2020 736f 7274 5f6f 7264 6572        sort_order
+0001ec00: 3a20 656e 756d 732e 536f 7274 4f72 6465  : enums.SortOrde
+0001ec10: 7220 3d20 656e 756d 732e 536f 7274 4f72  r = enums.SortOr
+0001ec20: 6465 722e 6173 630d 0a20 2020 2029 202d  der.asc..    ) -
+0001ec30: 3e20 7064 2e53 6572 6965 733a 0d0a 2020  > pd.Series:..  
+0001ec40: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0001ec50: 2020 2023 2320 5061 7261 6d65 7465 7273     ## Parameters
+0001ec60: 0d0a 2020 2020 2020 2020 6073 6572 6965  ..        `serie
+0001ec70: 735f 6964 600d 0a20 2020 2020 2020 2054  s_id`..        T
+0001ec80: 6865 2069 6420 666f 7220 6120 7365 7269  he id for a seri
+0001ec90: 6573 2e0d 0a0d 0a20 2020 2020 2020 2060  es.....        `
+0001eca0: 7265 616c 7469 6d65 5f73 7461 7274 600d  realtime_start`.
+0001ecb0: 0a20 2020 2020 2020 2054 6865 2073 7461  .        The sta
+0001ecc0: 7274 206f 6620 7468 6520 7265 616c 2d74  rt of the real-t
+0001ecd0: 696d 6520 7065 7269 6f64 2e20 466f 7220  ime period. For 
+0001ece0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+0001ecf0: 2c20 7365 6520 5b52 6561 6c2d 5469 6d65  , see [Real-Time
+0001ed00: 2050 6572 696f 6473 5d28 6874 7470 733a   Periods](https:
+0001ed10: 2f2f 6672 6564 2e73 746c 6f75 6973 6665  //fred.stlouisfe
+0001ed20: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
+0001ed30: 7265 642f 7265 616c 7469 6d65 5f70 6572  red/realtime_per
+0001ed40: 696f 642e 6874 6d6c 292e 0d0a 0d0a 2020  iod.html).....  
+0001ed50: 2020 2020 2020 6072 6561 6c74 696d 655f        `realtime_
+0001ed60: 656e 6460 0d0a 2020 2020 2020 2020 5468  end`..        Th
+0001ed70: 6520 656e 6420 6f66 2074 6865 2072 6561  e end of the rea
+0001ed80: 6c2d 7469 6d65 2070 6572 696f 642e 2046  l-time period. F
+0001ed90: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+0001eda0: 696f 6e2c 2073 6565 205b 5265 616c 2d54  ion, see [Real-T
+0001edb0: 696d 6520 5065 7269 6f64 735d 2868 7474  ime Periods](htt
+0001edc0: 7073 3a2f 2f66 7265 642e 7374 6c6f 7569  ps://fred.stloui
+0001edd0: 7366 6564 2e6f 7267 2f64 6f63 732f 6170  sfed.org/docs/ap
+0001ede0: 692f 6672 6564 2f72 6561 6c74 696d 655f  i/fred/realtime_
+0001edf0: 7065 7269 6f64 2e68 746d 6c29 2e0d 0a0d  period.html)....
+0001ee00: 0a20 2020 2020 2020 2060 736f 7274 5f6f  .        `sort_o
+0001ee10: 7264 6572 600d 0a20 2020 2020 2020 2053  rder`..        S
+0001ee20: 6f72 7420 7265 7375 6c74 7320 6973 2061  ort results is a
+0001ee30: 7363 656e 6469 6e67 206f 7220 6465 7363  scending or desc
+0001ee40: 656e 6469 6e67 206f 7264 6572 2066 6f72  ending order for
+0001ee50: 2061 7474 7269 6275 7465 2076 616c 7565   attribute value
+0001ee60: 7320 7370 6563 6966 6965 6420 6279 206f  s specified by o
+0001ee70: 7264 6572 5f62 792e 0d0a 0d0a 2020 2020  rder_by.....    
+0001ee80: 2020 2020 2323 2044 6573 6372 6970 7469      ## Descripti
+0001ee90: 6f6e 0d0a 2020 2020 2020 2020 6874 7470  on..        http
+0001eea0: 733a 2f2f 6672 6564 2e73 746c 6f75 6973  s://fred.stlouis
+0001eeb0: 6665 642e 6f72 672f 646f 6373 2f61 7069  fed.org/docs/api
+0001eec0: 2f66 7265 642f 7365 7269 6573 5f76 696e  /fred/series_vin
+0001eed0: 7461 6765 6461 7465 732e 6874 6d6c 0d0a  tagedates.html..
+0001eee0: 0d0a 2020 2020 2020 2020 4765 7420 7468  ..        Get th
+0001eef0: 6520 6461 7465 7320 696e 2068 6973 746f  e dates in histo
+0001ef00: 7279 2077 6865 6e20 6120 7365 7269 6573  ry when a series
+0001ef10: 2720 6461 7461 2076 616c 7565 7320 7765  ' data values we
+0001ef20: 7265 2072 6576 6973 6564 206f 7220 6e65  re revised or ne
+0001ef30: 7720 6461 7461 2076 616c 7565 7320 7765  w data values we
+0001ef40: 7265 2072 656c 6561 7365 642e 0d0a 2020  re released...  
+0001ef50: 2020 2020 2020 5669 6e74 6167 6520 6461        Vintage da
+0001ef60: 7465 7320 6172 6520 7468 6520 7265 6c65  tes are the rele
+0001ef70: 6173 6520 6461 7465 7320 666f 7220 6120  ase dates for a 
+0001ef80: 7365 7269 6573 2065 7863 6c75 6469 6e67  series excluding
+0001ef90: 2072 656c 6561 7365 2064 6174 6573 2077   release dates w
+0001efa0: 6865 6e20 7468 6520 6461 7461 2066 6f72  hen the data for
+0001efb0: 2074 6865 2073 6572 6965 7320 6469 6420   the series did 
+0001efc0: 6e6f 7420 6368 616e 6765 2e0d 0a0d 0a20  not change..... 
+0001efd0: 2020 2020 2020 2023 2320 4150 4920 5265         ## API Re
+0001efe0: 7175 6573 7420 2848 5454 5053 2047 4554  quest (HTTPS GET
+0001eff0: 290d 0a20 2020 2020 2020 2068 7474 7073  )..        https
+0001f000: 3a2f 2f61 7069 2e73 746c 6f75 6973 6665  ://api.stlouisfe
+0001f010: 642e 6f72 672f 6672 6564 2f73 6572 6965  d.org/fred/serie
+0001f020: 732f 7669 6e74 6167 6564 6174 6573 3f73  s/vintagedates?s
+0001f030: 6572 6965 735f 6964 3d47 4e50 4341 2661  eries_id=GNPCA&a
+0001f040: 7069 5f6b 6579 3d61 6263 6465 6667 6869  pi_key=abcdefghi
+0001f050: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
+0001f060: 7a31 3233 3435 3626 6669 6c65 5f74 7970  z123456&file_typ
+0001f070: 653d 6a73 6f6e 0d0a 0d0a 2020 2020 2020  e=json....      
+0001f080: 2020 2323 2041 5049 2052 6573 706f 6e73    ## API Respons
+0001f090: 650d 0a20 2020 2020 2020 2060 6060 6a73  e..        ```js
+0001f0a0: 6f6e 0d0a 2020 2020 2020 2020 7b0d 0a20  on..        {.. 
+0001f0b0: 2020 2020 2020 2020 2020 2022 7265 616c             "real
+0001f0c0: 7469 6d65 5f73 7461 7274 223a 2022 3137  time_start": "17
+0001f0d0: 3736 2d30 372d 3034 222c 0d0a 2020 2020  76-07-04",..    
+0001f0e0: 2020 2020 2020 2020 2272 6561 6c74 696d          "realtim
+0001f0f0: 655f 656e 6422 3a20 2239 3939 392d 3132  e_end": "9999-12
+0001f100: 2d33 3122 2c0d 0a20 2020 2020 2020 2020  -31",..         
+0001f110: 2020 2022 6f72 6465 725f 6279 223a 2022     "order_by": "
+0001f120: 7669 6e74 6167 655f 6461 7465 222c 0d0a  vintage_date",..
+0001f130: 2020 2020 2020 2020 2020 2020 2273 6f72              "sor
+0001f140: 745f 6f72 6465 7222 3a20 2261 7363 222c  t_order": "asc",
+0001f150: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
+0001f160: 6f75 6e74 223a 2031 3632 2c0d 0a20 2020  ount": 162,..   
+0001f170: 2020 2020 2020 2020 2022 6f66 6673 6574           "offset
+0001f180: 223a 2030 2c0d 0a20 2020 2020 2020 2020  ": 0,..         
+0001f190: 2020 2022 6c69 6d69 7422 3a20 3130 3030     "limit": 1000
+0001f1a0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+0001f1b0: 2276 696e 7461 6765 5f64 6174 6573 223a  "vintage_dates":
+0001f1c0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+0001f1d0: 2020 2020 2231 3935 382d 3132 2d32 3122      "1958-12-21"
+0001f1e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001f1f0: 2020 2022 3139 3539 2d30 322d 3139 222c     "1959-02-19",
+0001f200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001f210: 2020 2e2e 2e0d 0a20 2020 2020 2020 2020    .....         
+0001f220: 2020 205d 0d0a 2020 2020 2020 2020 7d0d     ]..        }.
+0001f230: 0a20 2020 2020 2020 2060 6060 0d0a 0d0a  .        ```....
+0001f240: 2020 2020 2020 2020 2323 2052 6574 7572          ## Retur
+0001f250: 6e73 0d0a 2020 2020 2020 2020 6070 616e  ns..        `pan
+0001f260: 6461 732e 5365 7269 6573 600d 0a0d 0a20  das.Series`.... 
+0001f270: 2020 2020 2020 2023 2320 4578 616d 706c         ## Exampl
+0001f280: 650d 0a20 2020 2020 2020 2060 6060 7079  e..        ```py
+0001f290: 7468 6f6e 0d0a 2020 2020 2020 2020 3e3e  thon..        >>
+0001f2a0: 3e20 6672 6564 203d 2046 5245 4428 6170  > fred = FRED(ap
+0001f2b0: 695f 6b65 793d 2761 6263 6465 6667 6869  i_key='abcdefghi
+0001f2c0: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
+0001f2d0: 7a31 3233 3435 3627 290d 0a20 2020 2020  z123456')..     
+0001f2e0: 2020 203e 3e3e 2066 7265 642e 7365 7269     >>> fred.seri
+0001f2f0: 6573 5f76 696e 7461 6765 6461 7465 7328  es_vintagedates(
+0001f300: 7365 7269 6573 5f69 643d 2747 4e50 4341  series_id='GNPCA
+0001f310: 2729 2e68 6561 6428 290d 0a20 2020 2020  ').head()..     
+0001f320: 2020 2020 2020 2030 2020 2020 3139 3538         0    1958
+0001f330: 2d31 322d 3231 0d0a 2020 2020 2020 2020  -12-21..        
+0001f340: 2020 2020 3120 2020 2031 3935 392d 3032      1    1959-02
+0001f350: 2d31 390d 0a20 2020 2020 2020 2020 2020  -19..           
+0001f360: 2032 2020 2020 3139 3539 2d30 372d 3139   2    1959-07-19
+0001f370: 0d0a 2020 2020 2020 2020 2020 2020 3320  ..            3 
+0001f380: 2020 2031 3936 302d 3032 2d31 360d 0a20     1960-02-16.. 
+0001f390: 2020 2020 2020 2020 2020 2034 2020 2020             4    
+0001f3a0: 3139 3630 2d30 372d 3232 0d0a 2020 2020  1960-07-22..    
+0001f3b0: 2020 2020 6060 600d 0a20 2020 2020 2020      ```..       
+0001f3c0: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
+0001f3d0: 6966 2072 6561 6c74 696d 655f 7374 6172  if realtime_star
+0001f3e0: 7420 6973 206e 6f74 204e 6f6e 6520 616e  t is not None an
+0001f3f0: 6420 7265 616c 7469 6d65 5f73 7461 7274  d realtime_start
+0001f400: 203c 2064 6174 6528 3137 3736 2c20 372c   < date(1776, 7,
+0001f410: 2034 293a 0d0a 2020 2020 2020 2020 2020   4):..          
+0001f420: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0001f430: 6f72 2827 5661 7269 6162 6c65 2072 6561  or('Variable rea
+0001f440: 6c74 696d 655f 7374 6172 7420 2822 7b7d  ltime_start ("{}
+0001f450: 2229 2069 7320 6265 666f 7265 206d 696e  ") is before min
+0001f460: 2064 6174 6520 3137 3736 2d30 372d 3034   date 1776-07-04
+0001f470: 2e27 2e66 6f72 6d61 7428 7265 616c 7469  .'.format(realti
+0001f480: 6d65 5f73 7461 7274 2929 0d0a 0d0a 2020  me_start))....  
+0001f490: 2020 2020 2020 6966 2072 6561 6c74 696d        if realtim
+0001f4a0: 655f 7374 6172 7420 3e20 7265 616c 7469  e_start > realti
+0001f4b0: 6d65 5f65 6e64 3a0d 0a20 2020 2020 2020  me_end:..       
+0001f4c0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0001f4d0: 4572 726f 7228 2754 6865 2064 6174 6520  Error('The date 
+0001f4e0: 7365 7420 6279 2076 6172 6961 626c 6520  set by variable 
+0001f4f0: 7265 616c 7469 6d65 5f73 7461 7274 2028  realtime_start (
+0001f500: 227b 7d22 2920 6361 6e20 6e6f 7420 6265  "{}") can not be
+0001f510: 2061 6674 6572 2074 6865 2064 6174 6520   after the date 
+0001f520: 7365 7420 6279 2076 6172 6961 626c 6520  set by variable 
+0001f530: 7265 616c 7469 6d65 5f65 6e64 2028 227b  realtime_end ("{
+0001f540: 7d22 292e 272e 666f 726d 6174 2872 6561  }").'.format(rea
+0001f550: 6c74 696d 655f 7374 6172 742c 2072 6561  ltime_start, rea
+0001f560: 6c74 696d 655f 656e 6429 290d 0a0d 0a20  ltime_end)).... 
+0001f570: 2020 2020 2020 2072 6574 7572 6e20 7064         return pd
+0001f580: 2e74 6f5f 6461 7465 7469 6d65 280d 0a20  .to_datetime(.. 
+0001f590: 2020 2020 2020 2020 2020 2070 642e 5365             pd.Se
+0001f5a0: 7269 6573 280d 0a20 2020 2020 2020 2020  ries(..         
+0001f5b0: 2020 2020 2020 2073 656c 662e 5f63 6c69         self._cli
+0001f5c0: 656e 742e 6765 7428 0d0a 2020 2020 2020  ent.get(..      
+0001f5d0: 2020 2020 2020 2020 2020 2020 2020 272f                '/
+0001f5e0: 6672 6564 2f73 6572 6965 732f 7669 6e74  fred/series/vint
+0001f5f0: 6167 6564 6174 6573 272c 0d0a 2020 2020  agedates',..    
+0001f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f610: 2776 696e 7461 6765 5f64 6174 6573 272c  'vintage_dates',
+0001f620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001f630: 2020 2020 2020 6c69 6d69 743d 3130 3030        limit=1000
+0001f640: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+0001f650: 2020 2020 2020 2020 7365 7269 6573 5f69          series_i
+0001f660: 643d 7365 7269 6573 5f69 642c 0d0a 2020  d=series_id,..  
+0001f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f680: 2020 7265 616c 7469 6d65 5f73 7461 7274    realtime_start
+0001f690: 3d72 6561 6c74 696d 655f 7374 6172 742c  =realtime_start,
+0001f6a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001f6b0: 2020 2020 2020 7265 616c 7469 6d65 5f65        realtime_e
+0001f6c0: 6e64 3d72 6561 6c74 696d 655f 656e 642c  nd=realtime_end,
+0001f6d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001f6e0: 2020 2020 2020 736f 7274 5f6f 7264 6572        sort_order
+0001f6f0: 3d73 6f72 745f 6f72 6465 720d 0a20 2020  =sort_order..   
+0001f700: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0001f710: 2020 2020 2020 2020 2020 2020 292c 2066              ), f
+0001f720: 6f72 6d61 743d 2725 592d 256d 2d25 6427  ormat='%Y-%m-%d'
+0001f730: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
+0001f740: 2020 2022 2222 0d0a 2020 2020 536f 7572     """..    Sour
+0001f750: 6365 730d 0a0d 0a20 2020 2068 7474 7073  ces....    https
+0001f760: 3a2f 2f66 7265 642e 7374 6c6f 7569 7366  ://fred.stlouisf
+0001f770: 6564 2e6f 7267 2f73 6f75 7263 6573 0d0a  ed.org/sources..
+0001f780: 2020 2020 2222 220d 0a0d 0a20 2020 2064      """....    d
+0001f790: 6566 2073 6f75 7263 6573 280d 0a20 2020  ef sources(..   
+0001f7a0: 2020 2020 2020 2020 2073 656c 662c 0d0a           self,..
+0001f7b0: 2020 2020 2020 2020 2020 2020 7265 616c              real
+0001f7c0: 7469 6d65 5f73 7461 7274 3a20 6461 7465  time_start: date
+0001f7d0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+0001f7e0: 2020 2020 2020 7265 616c 7469 6d65 5f65        realtime_e
+0001f7f0: 6e64 3a20 6461 7465 203d 204e 6f6e 652c  nd: date = None,
+0001f800: 0d0a 2020 2020 2020 2020 2020 2020 6f72  ..            or
+0001f810: 6465 725f 6279 3a20 656e 756d 732e 4f72  der_by: enums.Or
+0001f820: 6465 7242 7920 3d20 656e 756d 732e 4f72  derBy = enums.Or
+0001f830: 6465 7242 792e 736f 7572 6365 5f69 642c  derBy.source_id,
+0001f840: 0d0a 2020 2020 2020 2020 2020 2020 736f  ..            so
+0001f850: 7274 5f6f 7264 6572 3a20 656e 756d 732e  rt_order: enums.
+0001f860: 536f 7274 4f72 6465 7220 3d20 656e 756d  SortOrder = enum
+0001f870: 732e 536f 7274 4f72 6465 722e 6173 630d  s.SortOrder.asc.
+0001f880: 0a20 2020 2029 202d 3e20 7064 2e44 6174  .    ) -> pd.Dat
+0001f890: 6146 7261 6d65 3a0d 0a20 2020 2020 2020  aFrame:..       
+0001f8a0: 2022 2222 0d0a 2020 2020 2020 2020 2323   """..        ##
+0001f8b0: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+0001f8c0: 2020 2020 2060 7265 616c 7469 6d65 5f73       `realtime_s
+0001f8d0: 7461 7274 600d 0a20 2020 2020 2020 2054  tart`..        T
+0001f8e0: 6865 2073 7461 7274 206f 6620 7468 6520  he start of the 
+0001f8f0: 7265 616c 2d74 696d 6520 7065 7269 6f64  real-time period
+0001f900: 2e20 466f 7220 6d6f 7265 2069 6e66 6f72  . For more infor
+0001f910: 6d61 7469 6f6e 2c20 7365 6520 5b52 6561  mation, see [Rea
+0001f920: 6c2d 5469 6d65 2050 6572 696f 6473 5d28  l-Time Periods](
+0001f930: 6874 7470 733a 2f2f 6672 6564 2e73 746c  https://fred.stl
+0001f940: 6f75 6973 6665 642e 6f72 672f 646f 6373  ouisfed.org/docs
+0001f950: 2f61 7069 2f66 7265 642f 7265 616c 7469  /api/fred/realti
+0001f960: 6d65 5f70 6572 696f 642e 6874 6d6c 292e  me_period.html).
+0001f970: 0d0a 0d0a 2020 2020 2020 2020 6072 6561  ....        `rea
+0001f980: 6c74 696d 655f 656e 6460 0d0a 2020 2020  ltime_end`..    
+0001f990: 2020 2020 5468 6520 656e 6420 6f66 2074      The end of t
+0001f9a0: 6865 2072 6561 6c2d 7469 6d65 2070 6572  he real-time per
+0001f9b0: 696f 642e 2046 6f72 206d 6f72 6520 696e  iod. For more in
+0001f9c0: 666f 726d 6174 696f 6e2c 2073 6565 205b  formation, see [
+0001f9d0: 5265 616c 2d54 696d 6520 5065 7269 6f64  Real-Time Period
+0001f9e0: 735d 2868 7474 7073 3a2f 2f66 7265 642e  s](https://fred.
+0001f9f0: 7374 6c6f 7569 7366 6564 2e6f 7267 2f64  stlouisfed.org/d
+0001fa00: 6f63 732f 6170 692f 6672 6564 2f72 6561  ocs/api/fred/rea
+0001fa10: 6c74 696d 655f 7065 7269 6f64 2e68 746d  ltime_period.htm
+0001fa20: 6c29 2e0d 0a0d 0a20 2020 2020 2020 2060  l).....        `
+0001fa30: 6f72 6465 725f 6279 600d 0a20 2020 2020  order_by`..     
+0001fa40: 2020 204f 7264 6572 2072 6573 756c 7473     Order results
+0001fa50: 2062 7920 7661 6c75 6573 206f 6620 7468   by values of th
+0001fa60: 6520 7370 6563 6966 6965 6420 6174 7472  e specified attr
+0001fa70: 6962 7574 652e 0d0a 0d0a 2020 2020 2020  ibute.....      
+0001fa80: 2020 6073 6f72 745f 6f72 6465 7260 0d0a    `sort_order`..
+0001fa90: 2020 2020 2020 2020 536f 7274 2072 6573          Sort res
+0001faa0: 756c 7473 2069 7320 6173 6365 6e64 696e  ults is ascendin
+0001fab0: 6720 6f72 2064 6573 6365 6e64 696e 6720  g or descending 
+0001fac0: 6f72 6465 7220 666f 7220 6174 7472 6962  order for attrib
+0001fad0: 7574 6520 7661 6c75 6573 2073 7065 6369  ute values speci
+0001fae0: 6669 6564 2062 7920 6f72 6465 725f 6279  fied by order_by
+0001faf0: 2e0d 0a0d 0a20 2020 2020 2020 2023 2320  .....        ## 
+0001fb00: 4465 7363 7269 7074 696f 6e0d 0a20 2020  Description..   
+0001fb10: 2020 2020 2068 7474 7073 3a2f 2f66 7265       https://fre
+0001fb20: 642e 7374 6c6f 7569 7366 6564 2e6f 7267  d.stlouisfed.org
+0001fb30: 2f64 6f63 732f 6170 692f 6672 6564 2f73  /docs/api/fred/s
+0001fb40: 6f75 7263 6573 2e68 746d 6c0d 0a0d 0a20  ources.html.... 
+0001fb50: 2020 2020 2020 2047 6574 2061 6c6c 2073         Get all s
+0001fb60: 6f75 7263 6573 206f 6620 6563 6f6e 6f6d  ources of econom
+0001fb70: 6963 2064 6174 612e 0d0a 0d0a 2020 2020  ic data.....    
+0001fb80: 2020 2020 2323 2041 5049 2052 6571 7565      ## API Reque
+0001fb90: 7374 2028 4854 5450 5320 4745 5429 0d0a  st (HTTPS GET)..
+0001fba0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+0001fbb0: 6170 692e 7374 6c6f 7569 7366 6564 2e6f  api.stlouisfed.o
+0001fbc0: 7267 2f66 7265 642f 736f 7572 6365 733f  rg/fred/sources?
+0001fbd0: 6170 695f 6b65 793d 6162 6364 6566 6768  api_key=abcdefgh
+0001fbe0: 696a 6b6c 6d6e 6f70 7172 7374 7576 7778  ijklmnopqrstuvwx
+0001fbf0: 797a 3132 3334 3536 2666 696c 655f 7479  yz123456&file_ty
+0001fc00: 7065 3d6a 736f 6e0d 0a0d 0a20 2020 2020  pe=json....     
+0001fc10: 2020 2023 2320 4150 4920 5265 7370 6f6e     ## API Respon
+0001fc20: 7365 0d0a 2020 2020 2020 2020 6060 606a  se..        ```j
+0001fc30: 736f 6e0d 0a20 2020 2020 2020 207b 0d0a  son..        {..
+0001fc40: 2020 2020 2020 2020 2020 2020 2272 6561              "rea
+0001fc50: 6c74 696d 655f 7374 6172 7422 3a20 2232  ltime_start": "2
+0001fc60: 3031 332d 3038 2d31 3422 2c0d 0a20 2020  013-08-14",..   
+0001fc70: 2020 2020 2020 2020 2022 7265 616c 7469           "realti
+0001fc80: 6d65 5f65 6e64 223a 2022 3230 3133 2d30  me_end": "2013-0
+0001fc90: 382d 3134 222c 0d0a 2020 2020 2020 2020  8-14",..        
+0001fca0: 2020 2020 226f 7264 6572 5f62 7922 3a20      "order_by": 
+0001fcb0: 2273 6f75 7263 655f 6964 222c 0d0a 2020  "source_id",..  
+0001fcc0: 2020 2020 2020 2020 2020 2273 6f72 745f            "sort_
+0001fcd0: 6f72 6465 7222 3a20 2261 7363 222c 0d0a  order": "asc",..
+0001fce0: 2020 2020 2020 2020 2020 2020 2263 6f75              "cou
+0001fcf0: 6e74 223a 2035 382c 0d0a 2020 2020 2020  nt": 58,..      
+0001fd00: 2020 2020 2020 226f 6666 7365 7422 3a20        "offset": 
+0001fd10: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+0001fd20: 226c 696d 6974 223a 2031 3030 302c 0d0a  "limit": 1000,..
+0001fd30: 2020 2020 2020 2020 2020 2020 2273 6f75              "sou
+0001fd40: 7263 6573 223a 205b 0d0a 2020 2020 2020  rces": [..      
+0001fd50: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
+0001fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fd70: 2022 6964 223a 2031 2c0d 0a20 2020 2020   "id": 1,..     
+0001fd80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001fd90: 7265 616c 7469 6d65 5f73 7461 7274 223a  realtime_start":
+0001fda0: 2022 3230 3133 2d30 382d 3134 222c 0d0a   "2013-08-14",..
+0001fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fdc0: 2020 2020 2272 6561 6c74 696d 655f 656e      "realtime_en
+0001fdd0: 6422 3a20 2232 3031 332d 3038 2d31 3422  d": "2013-08-14"
+0001fde0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001fdf0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+0001fe00: 426f 6172 6420 6f66 2047 6f76 6572 6e6f  Board of Governo
+0001fe10: 7273 206f 6620 7468 6520 4665 6465 7261  rs of the Federa
+0001fe20: 6c20 5265 7365 7276 6520 5379 7374 656d  l Reserve System
+0001fe30: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0001fe40: 2020 2020 2020 2020 226c 696e 6b22 3a20          "link": 
+0001fe50: 2268 7474 703a 2f2f 7777 772e 6665 6465  "http://www.fede
+0001fe60: 7261 6c72 6573 6572 7665 2e67 6f76 2f22  ralreserve.gov/"
+0001fe70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001fe80: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
+0001fe90: 2020 2020 2020 2e2e 2e0d 0a20 2020 2020        .....     
+0001fea0: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+0001feb0: 2020 7d0d 0a20 2020 2020 2020 2060 6060    }..        ```
+0001fec0: 0d0a 0d0a 2020 2020 2020 2020 2323 2052  ....        ## R
+0001fed0: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
+0001fee0: 6070 616e 6461 732e 4461 7461 4672 616d  `pandas.DataFram
+0001fef0: 6560 0d0a 0d0a 2020 2020 2020 2020 2323  e`....        ##
+0001ff00: 2045 7861 6d70 6c65 0d0a 2020 2020 2020   Example..      
+0001ff10: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
+0001ff20: 2020 2020 203e 3e3e 2066 7265 6420 3d20       >>> fred = 
+0001ff30: 4652 4544 2861 7069 5f6b 6579 3d27 6162  FRED(api_key='ab
+0001ff40: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
+0001ff50: 7374 7576 7778 797a 3132 3334 3536 2729  stuvwxyz123456')
+0001ff60: 0d0a 2020 2020 2020 2020 3e3e 3e20 6672  ..        >>> fr
+0001ff70: 6564 2e73 6f75 7263 6573 2829 0d0a 2020  ed.sources()..  
+0001ff80: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+0001ff90: 6c74 696d 655f 7374 6172 7420 7265 616c  ltime_start real
+0001ffa0: 7469 6d65 5f65 6e64 2020 2020 2020 2020  time_end        
+0001ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ffd0: 2020 2020 2020 206e 616d 6520 2020 2020         name     
+0001ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fff0: 2020 2020 2020 2020 206c 696e 6b20 6e6f           link no
+00020000: 7465 730d 0a20 2020 2020 2020 2020 2020  tes..           
+00020010: 2069 640d 0a20 2020 2020 2020 2020 2020   id..           
+00020020: 2031 2020 2020 2020 3230 3232 2d30 322d   1      2022-02-
+00020030: 3035 2020 2032 3032 322d 3032 2d30 3520  05   2022-02-05 
+00020040: 2042 6f61 7264 206f 6620 476f 7665 726e   Board of Govern
+00020050: 6f72 7320 6f66 2074 6865 2046 6564 6572  ors of the Feder
+00020060: 616c 2052 6573 6572 7665 2053 7973 742e  al Reserve Syst.
+00020070: 2e2e 2020 2020 6874 7470 3a2f 2f77 7777  ..    http://www
+00020080: 2e66 6564 6572 616c 7265 7365 7276 652e  .federalreserve.
+00020090: 676f 762f 2020 3c4e 413e 0d0a 2020 2020  gov/  <NA>..    
+000200a0: 2020 2020 2020 2020 3320 2020 2020 2032          3      2
+000200b0: 3032 322d 3032 2d30 3520 2020 3230 3232  022-02-05   2022
+000200c0: 2d30 322d 3035 2020 2020 2020 2020 2020  -02-05          
+000200d0: 2020 2020 2046 6564 6572 616c 2052 6573       Federal Res
+000200e0: 6572 7665 2042 616e 6b20 6f66 2050 6869  erve Bank of Phi
+000200f0: 6c61 6465 6c70 6869 6120 2068 7474 7073  ladelphia  https
+00020100: 3a2f 2f77 7777 2e70 6869 6c61 6465 6c70  ://www.philadelp
+00020110: 6869 6166 6564 2e6f 7267 2f20 203c 4e41  hiafed.org/  <NA
+00020120: 3e0d 0a20 2020 2020 2020 2020 2020 2034  >..            4
+00020130: 2020 2020 2020 3230 3232 2d30 322d 3035        2022-02-05
+00020140: 2020 2032 3032 322d 3032 2d30 3520 2020     2022-02-05   
+00020150: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+00020160: 6564 6572 616c 2052 6573 6572 7665 2042  ederal Reserve B
+00020170: 616e 6b20 6f66 2053 742e 204c 6f75 6973  ank of St. Louis
+00020180: 2020 2020 2020 2020 6874 7470 3a2f 2f77          http://w
+00020190: 7777 2e73 746c 6f75 6973 6665 642e 6f72  ww.stlouisfed.or
+000201a0: 672f 2020 3c4e 413e 0d0a 2020 2020 2020  g/  <NA>..      
+000201b0: 2020 2020 2020 3620 2020 2020 2032 3032        6      202
+000201c0: 322d 3032 2d30 3520 2020 3230 3232 2d30  2-02-05   2022-0
+000201d0: 322d 3035 2020 4665 6465 7261 6c20 4669  2-05  Federal Fi
+000201e0: 6e61 6e63 6961 6c20 496e 7374 6974 7574  nancial Institut
+000201f0: 696f 6e73 2045 7861 6d69 6e61 7469 6f6e  ions Examination
+00020200: 2043 6f75 2e2e 2e20 2020 2020 2020 2020   Cou...         
+00020210: 2020 2020 6874 7470 3a2f 2f77 7777 2e66      http://www.f
+00020220: 6669 6563 2e67 6f76 2f20 203c 4e41 3e0d  fiec.gov/  <NA>.
+00020230: 0a20 2020 2020 2020 2020 2020 2031 3120  .            11 
+00020240: 2020 2020 3230 3232 2d30 322d 3035 2020      2022-02-05  
+00020250: 2032 3032 322d 3032 2d30 3520 2020 2020   2022-02-05     
+00020260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020270: 2020 2020 2020 2020 2020 2044 6f77 204a             Dow J
+00020280: 6f6e 6573 2026 2043 6f6d 7061 6e79 2020  ones & Company  
+00020290: 2020 2020 2020 2020 2068 7474 703a 2f2f           http://
+000202a0: 7777 772e 646f 776a 6f6e 6573 2e63 6f6d  www.dowjones.com
+000202b0: 2020 3c4e 413e 0d0a 2020 2020 2020 2020    <NA>..        
+000202c0: 6060 600d 0a20 2020 2020 2020 2022 2222  ```..        """
+000202d0: 0d0a 0d0a 2020 2020 2020 2020 616c 6c6f  ....        allo
+000202e0: 7765 645f 6f72 6465 7273 203d 205b 0d0a  wed_orders = [..
+000202f0: 2020 2020 2020 2020 2020 2020 656e 756d              enum
+00020300: 732e 4f72 6465 7242 792e 736f 7572 6365  s.OrderBy.source
+00020310: 5f69 642c 0d0a 2020 2020 2020 2020 2020  _id,..          
+00020320: 2020 656e 756d 732e 4f72 6465 7242 792e    enums.OrderBy.
+00020330: 6e61 6d65 2c0d 0a20 2020 2020 2020 2020  name,..         
+00020340: 2020 2065 6e75 6d73 2e4f 7264 6572 4279     enums.OrderBy
+00020350: 2e72 6561 6c74 696d 655f 7374 6172 742c  .realtime_start,
+00020360: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+00020370: 756d 732e 4f72 6465 7242 792e 7265 616c  ums.OrderBy.real
+00020380: 7469 6d65 5f65 6e64 0d0a 2020 2020 2020  time_end..      
+00020390: 2020 5d0d 0a0d 0a20 2020 2020 2020 2069    ]....        i
+000203a0: 6620 6f72 6465 725f 6279 206e 6f74 2069  f order_by not i
+000203b0: 6e20 616c 6c6f 7765 645f 6f72 6465 7273  n allowed_orders
+000203c0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000203d0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000203e0: 2756 6172 6961 626c 6520 6f72 6465 725f  'Variable order_
+000203f0: 6279 2028 7b7d 2920 6973 206e 6f74 206f  by ({}) is not o
+00020400: 6e65 206f 6620 7468 6520 7661 6c75 6573  ne of the values
+00020410: 3a20 7b7d 272e 666f 726d 6174 286f 7264  : {}'.format(ord
+00020420: 6572 5f62 792c 2027 2c20 272e 6a6f 696e  er_by, ', '.join
+00020430: 286d 6170 2873 7472 2c20 616c 6c6f 7765  (map(str, allowe
+00020440: 645f 6f72 6465 7273 2929 2929 0d0a 0d0a  d_orders))))....
+00020450: 2020 2020 2020 2020 6966 2072 6561 6c74          if realt
+00020460: 696d 655f 7374 6172 7420 6973 206e 6f74  ime_start is not
+00020470: 204e 6f6e 6520 616e 6420 7265 616c 7469   None and realti
+00020480: 6d65 5f73 7461 7274 203c 2064 6174 6528  me_start < date(
+00020490: 3137 3736 2c20 372c 2034 293a 0d0a 2020  1776, 7, 4):..  
+000204a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000204b0: 5661 6c75 6545 7272 6f72 2827 5661 7269  ValueError('Vari
+000204c0: 6162 6c65 2072 6561 6c74 696d 655f 7374  able realtime_st
+000204d0: 6172 7420 2822 7b7d 2229 2069 7320 6265  art ("{}") is be
+000204e0: 666f 7265 206d 696e 2064 6174 6520 3137  fore min date 17
+000204f0: 3736 2d30 372d 3034 2e27 2e66 6f72 6d61  76-07-04.'.forma
+00020500: 7428 7265 616c 7469 6d65 5f73 7461 7274  t(realtime_start
+00020510: 2929 0d0a 0d0a 2020 2020 2020 2020 6966  ))....        if
+00020520: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
+00020530: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00020540: 7265 616c 7469 6d65 5f65 6e64 2069 7320  realtime_end is 
+00020550: 6e6f 7420 4e6f 6e65 2061 6e64 2072 6561  not None and rea
+00020560: 6c74 696d 655f 7374 6172 7420 3e20 7265  ltime_start > re
+00020570: 616c 7469 6d65 5f65 6e64 3a0d 0a20 2020  altime_end:..   
+00020580: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00020590: 616c 7565 4572 726f 7228 2754 6865 2064  alueError('The d
+000205a0: 6174 6520 7365 7420 6279 2076 6172 6961  ate set by varia
+000205b0: 626c 6520 7265 616c 7469 6d65 5f73 7461  ble realtime_sta
+000205c0: 7274 2028 227b 7d22 2920 6361 6e20 6e6f  rt ("{}") can no
+000205d0: 7420 6265 2061 6674 6572 2074 6865 2064  t be after the d
+000205e0: 6174 6520 7365 7420 6279 2076 6172 6961  ate set by varia
+000205f0: 626c 6520 7265 616c 7469 6d65 5f65 6e64  ble realtime_end
+00020600: 2028 227b 7d22 292e 272e 666f 726d 6174   ("{}").'.format
+00020610: 2872 6561 6c74 696d 655f 7374 6172 742c  (realtime_start,
+00020620: 2072 6561 6c74 696d 655f 656e 6429 290d   realtime_end)).
+00020630: 0a0d 0a20 2020 2020 2020 2064 6620 3d20  ...        df = 
+00020640: 7064 2e44 6174 6146 7261 6d65 280d 0a20  pd.DataFrame(.. 
+00020650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00020660: 5f63 6c69 656e 742e 6765 7428 0d0a 2020  _client.get(..  
+00020670: 2020 2020 2020 2020 2020 2020 2020 272f                '/
+00020680: 6672 6564 2f73 6f75 7263 6573 272c 0d0a  fred/sources',..
+00020690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000206a0: 2773 6f75 7263 6573 272c 0d0a 2020 2020  'sources',..    
+000206b0: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
+000206c0: 743d 3130 3030 2c0d 0a20 2020 2020 2020  t=1000,..       
+000206d0: 2020 2020 2020 2020 2072 6561 6c74 696d           realtim
+000206e0: 655f 7374 6172 743d 7265 616c 7469 6d65  e_start=realtime
+000206f0: 5f73 7461 7274 2c0d 0a20 2020 2020 2020  _start,..       
+00020700: 2020 2020 2020 2020 2072 6561 6c74 696d           realtim
+00020710: 655f 656e 643d 7265 616c 7469 6d65 5f65  e_end=realtime_e
+00020720: 6e64 2c0d 0a20 2020 2020 2020 2020 2020  nd,..           
+00020730: 2020 2020 206f 7264 6572 5f62 793d 6f72       order_by=or
+00020740: 6465 725f 6279 2c0d 0a20 2020 2020 2020  der_by,..       
+00020750: 2020 2020 2020 2020 2073 6f72 745f 6f72           sort_or
+00020760: 6465 723d 736f 7274 5f6f 7264 6572 0d0a  der=sort_order..
+00020770: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00020780: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+00020790: 2020 2020 6461 7465 5f63 6f6c 756d 6e73      date_columns
+000207a0: 203d 205b 2772 6561 6c74 696d 655f 7374   = ['realtime_st
+000207b0: 6172 7427 2c20 2772 6561 6c74 696d 655f  art', 'realtime_
+000207c0: 656e 6427 5d0d 0a0d 0a20 2020 2020 2020  end']....       
+000207d0: 2069 6620 6e6f 7420 6466 2e65 6d70 7479   if not df.empty
+000207e0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+000207f0: 665b 6461 7465 5f63 6f6c 756d 6e73 5d20  f[date_columns] 
+00020800: 3d20 6466 5b64 6174 655f 636f 6c75 6d6e  = df[date_column
+00020810: 735d 2e61 7070 6c79 2870 642e 746f 5f64  s].apply(pd.to_d
+00020820: 6174 6574 696d 652c 2066 6f72 6d61 743d  atetime, format=
+00020830: 2725 592d 256d 2d25 6427 290d 0a20 2020  '%Y-%m-%d')..   
+00020840: 2020 2020 2020 2020 2064 6620 3d20 6466           df = df
+00020850: 2e61 7374 7970 6528 6474 7970 653d 7b0d  .astype(dtype={.
+00020860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020870: 2027 6e61 6d65 273a 2027 7374 7269 6e67   'name': 'string
+00020880: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00020890: 2020 2020 276e 6f74 6573 273a 2027 7374      'notes': 'st
+000208a0: 7269 6e67 272c 0d0a 2020 2020 2020 2020  ring',..        
+000208b0: 2020 2020 2020 2020 276c 696e 6b27 3a20          'link': 
+000208c0: 2773 7472 696e 6727 0d0a 2020 2020 2020  'string'..      
+000208d0: 2020 2020 2020 7d29 2e73 6574 5f69 6e64        }).set_ind
+000208e0: 6578 2827 6964 2729 0d0a 0d0a 2020 2020  ex('id')....    
+000208f0: 2020 2020 7265 7475 726e 2064 660d 0a0d      return df...
+00020900: 0a20 2020 2064 6566 2073 6f75 7263 6528  .    def source(
+00020910: 7365 6c66 2c20 736f 7572 6365 5f69 643a  self, source_id:
+00020920: 2069 6e74 2c20 7265 616c 7469 6d65 5f73   int, realtime_s
+00020930: 7461 7274 3a20 6461 7465 203d 204e 6f6e  tart: date = Non
+00020940: 652c 2072 6561 6c74 696d 655f 656e 643a  e, realtime_end:
+00020950: 2064 6174 6520 3d20 4e6f 6e65 2920 2d3e   date = None) ->
+00020960: 206d 6f64 656c 732e 536f 7572 6365 3a0d   models.Source:.
+00020970: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00020980: 2020 2020 2020 2323 2050 6172 616d 6574        ## Paramet
+00020990: 6572 730d 0a20 2020 2020 2020 2060 736f  ers..        `so
+000209a0: 7572 6365 5f69 6460 0d0a 2020 2020 2020  urce_id`..      
+000209b0: 2020 5468 6520 6964 2066 6f72 2061 2073    The id for a s
+000209c0: 6f75 7263 652e 0d0a 0d0a 2020 2020 2020  ource.....      
+000209d0: 2020 6072 6561 6c74 696d 655f 7374 6172    `realtime_star
+000209e0: 7460 0d0a 2020 2020 2020 2020 5468 6520  t`..        The 
+000209f0: 7374 6172 7420 6f66 2074 6865 2072 6561  start of the rea
+00020a00: 6c2d 7469 6d65 2070 6572 696f 642e 2046  l-time period. F
+00020a10: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00020a20: 696f 6e2c 2073 6565 205b 5265 616c 2d54  ion, see [Real-T
+00020a30: 696d 6520 5065 7269 6f64 735d 2868 7474  ime Periods](htt
+00020a40: 7073 3a2f 2f66 7265 642e 7374 6c6f 7569  ps://fred.stloui
+00020a50: 7366 6564 2e6f 7267 2f64 6f63 732f 6170  sfed.org/docs/ap
+00020a60: 692f 6672 6564 2f72 6561 6c74 696d 655f  i/fred/realtime_
+00020a70: 7065 7269 6f64 2e68 746d 6c29 2e0d 0a0d  period.html)....
+00020a80: 0a20 2020 2020 2020 2060 7265 616c 7469  .        `realti
+00020a90: 6d65 5f65 6e64 600d 0a20 2020 2020 2020  me_end`..       
+00020aa0: 2054 6865 2065 6e64 206f 6620 7468 6520   The end of the 
+00020ab0: 7265 616c 2d74 696d 6520 7065 7269 6f64  real-time period
+00020ac0: 2e20 466f 7220 6d6f 7265 2069 6e66 6f72  . For more infor
+00020ad0: 6d61 7469 6f6e 2c20 7365 6520 5b52 6561  mation, see [Rea
+00020ae0: 6c2d 5469 6d65 2050 6572 696f 6473 5d28  l-Time Periods](
+00020af0: 6874 7470 733a 2f2f 6672 6564 2e73 746c  https://fred.stl
+00020b00: 6f75 6973 6665 642e 6f72 672f 646f 6373  ouisfed.org/docs
+00020b10: 2f61 7069 2f66 7265 642f 7265 616c 7469  /api/fred/realti
+00020b20: 6d65 5f70 6572 696f 642e 6874 6d6c 292e  me_period.html).
+00020b30: 0d0a 0d0a 2020 2020 2020 2020 2323 2044  ....        ## D
+00020b40: 6573 6372 6970 7469 6f6e 0d0a 2020 2020  escription..    
+00020b50: 2020 2020 6874 7470 733a 2f2f 6672 6564      https://fred
+00020b60: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
+00020b70: 646f 6373 2f61 7069 2f66 7265 642f 736f  docs/api/fred/so
+00020b80: 7572 6365 2e68 746d 6c0d 0a0d 0a20 2020  urce.html....   
+00020b90: 2020 2020 2047 6574 2061 2073 6f75 7263       Get a sourc
+00020ba0: 6520 6f66 2065 636f 6e6f 6d69 6320 6461  e of economic da
+00020bb0: 7461 2e0d 0a0d 0a20 2020 2020 2020 2023  ta.....        #
+00020bc0: 2320 4150 4920 5265 7175 6573 7420 2848  # API Request (H
+00020bd0: 5454 5053 2047 4554 290d 0a20 2020 2020  TTPS GET)..     
+00020be0: 2020 2068 7474 7073 3a2f 2f61 7069 2e73     https://api.s
+00020bf0: 746c 6f75 6973 6665 642e 6f72 672f 6672  tlouisfed.org/fr
+00020c00: 6564 2f73 6f75 7263 653f 736f 7572 6365  ed/source?source
+00020c10: 5f69 643d 3126 6170 695f 6b65 793d 6162  _id=1&api_key=ab
+00020c20: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
+00020c30: 7374 7576 7778 797a 3132 3334 3536 2666  stuvwxyz123456&f
+00020c40: 696c 655f 7479 7065 3d6a 736f 6e0d 0a0d  ile_type=json...
+00020c50: 0a20 2020 2020 2020 2023 2320 4150 4920  .        ## API 
+00020c60: 5265 7370 6f6e 7365 0d0a 2020 2020 2020  Response..      
+00020c70: 2020 6060 606a 736f 6e0d 0a20 2020 2020    ```json..     
+00020c80: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00020c90: 2020 2272 6561 6c74 696d 655f 7374 6172    "realtime_star
+00020ca0: 7422 3a20 2232 3031 332d 3038 2d31 3422  t": "2013-08-14"
+00020cb0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00020cc0: 7265 616c 7469 6d65 5f65 6e64 223a 2022  realtime_end": "
+00020cd0: 3230 3133 2d30 382d 3134 222c 0d0a 2020  2013-08-14",..  
+00020ce0: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
+00020cf0: 6573 223a 205b 0d0a 2020 2020 2020 2020  es": [..        
+00020d00: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00020d10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00020d20: 6964 223a 2031 2c0d 0a20 2020 2020 2020  id": 1,..       
+00020d30: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00020d40: 616c 7469 6d65 5f73 7461 7274 223a 2022  altime_start": "
+00020d50: 3230 3133 2d30 382d 3134 222c 0d0a 2020  2013-08-14",..  
+00020d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d70: 2020 2272 6561 6c74 696d 655f 656e 6422    "realtime_end"
+00020d80: 3a20 2232 3031 332d 3038 2d31 3422 2c0d  : "2013-08-14",.
+00020d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020da0: 2020 2020 2022 6e61 6d65 223a 2022 426f       "name": "Bo
+00020db0: 6172 6420 6f66 2047 6f76 6572 6e6f 7273  ard of Governors
+00020dc0: 206f 6620 7468 6520 4665 6465 7261 6c20   of the Federal 
+00020dd0: 5265 7365 7276 6520 5379 7374 656d 222c  Reserve System",
+00020de0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020df0: 2020 2020 2020 226c 696e 6b22 3a20 2268        "link": "h
+00020e00: 7474 703a 2f2f 7777 772e 6665 6465 7261  ttp://www.federa
+00020e10: 6c72 6573 6572 7665 2e67 6f76 2f22 0d0a  lreserve.gov/"..
+00020e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e30: 7d0d 0a20 2020 2020 2020 2020 2020 205d  }..            ]
+00020e40: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
+00020e50: 2020 2020 2060 6060 0d0a 0d0a 2020 2020       ```....    
+00020e60: 2020 2020 2323 2052 6574 7572 6e73 0d0a      ## Returns..
+00020e70: 2020 2020 2020 2020 6070 7973 746c 6f75          `pystlou
+00020e80: 6973 6665 642e 6d6f 6465 6c73 2e53 6f75  isfed.models.Sou
+00020e90: 7263 6560 0d0a 0d0a 2020 2020 2020 2020  rce`....        
+00020ea0: 2323 2045 7861 6d70 6c65 0d0a 2020 2020  ## Example..    
+00020eb0: 2020 2020 6060 6070 7974 686f 6e0d 0a20      ```python.. 
+00020ec0: 2020 2020 2020 203e 3e3e 2066 7265 6420         >>> fred 
+00020ed0: 3d20 4652 4544 2861 7069 5f6b 6579 3d27  = FRED(api_key='
+00020ee0: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
+00020ef0: 7172 7374 7576 7778 797a 3132 3334 3536  qrstuvwxyz123456
+00020f00: 2729 0d0a 2020 2020 2020 2020 3e3e 3e20  ')..        >>> 
+00020f10: 6672 6564 2e73 6f75 7263 6528 736f 7572  fred.source(sour
+00020f20: 6365 5f69 643d 3129 0d0a 2020 2020 2020  ce_id=1)..      
+00020f30: 2020 2020 2020 536f 7572 6365 2869 643d        Source(id=
+00020f40: 312c 2072 6561 6c74 696d 655f 7374 6172  1, realtime_star
+00020f50: 743d 2732 3032 322d 3031 2d31 3427 2c20  t='2022-01-14', 
+00020f60: 7265 616c 7469 6d65 5f65 6e64 3d27 3230  realtime_end='20
+00020f70: 3232 2d30 312d 3134 272c 206e 616d 653d  22-01-14', name=
+00020f80: 2742 6f61 7264 206f 6620 476f 7665 726e  'Board of Govern
+00020f90: 6f72 7320 6f66 2074 6865 2046 6564 6572  ors of the Feder
+00020fa0: 616c 2052 6573 6572 7665 2053 7973 7465  al Reserve Syste
+00020fb0: 6d20 2855 5329 272c 206c 696e 6b3d 2768  m (US)', link='h
+00020fc0: 7474 703a 2f2f 7777 772e 6665 6465 7261  ttp://www.federa
+00020fd0: 6c72 6573 6572 7665 2e67 6f76 2f27 290d  lreserve.gov/').
+00020fe0: 0a20 2020 2020 2020 2060 6060 0d0a 2020  .        ```..  
+00020ff0: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
+00021000: 2020 2020 2069 6620 7265 616c 7469 6d65       if realtime
+00021010: 5f73 7461 7274 2069 7320 6e6f 7420 4e6f  _start is not No
+00021020: 6e65 2061 6e64 2072 6561 6c74 696d 655f  ne and realtime_
+00021030: 7374 6172 7420 3c20 6461 7465 2831 3737  start < date(177
+00021040: 362c 2037 2c20 3429 3a0d 0a20 2020 2020  6, 7, 4):..     
+00021050: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00021060: 7565 4572 726f 7228 2756 6172 6961 626c  ueError('Variabl
+00021070: 6520 7265 616c 7469 6d65 5f73 7461 7274  e realtime_start
+00021080: 2028 227b 7d22 2920 6973 2062 6566 6f72   ("{}") is befor
+00021090: 6520 6d69 6e20 6461 7465 2031 3737 362d  e min date 1776-
+000210a0: 3037 2d30 342e 272e 666f 726d 6174 2872  07-04.'.format(r
+000210b0: 6561 6c74 696d 655f 7374 6172 7429 290d  ealtime_start)).
+000210c0: 0a0d 0a20 2020 2020 2020 2069 6620 7265  ...        if re
+000210d0: 616c 7469 6d65 5f73 7461 7274 2069 7320  altime_start is 
+000210e0: 6e6f 7420 4e6f 6e65 2061 6e64 2072 6561  not None and rea
+000210f0: 6c74 696d 655f 656e 6420 6973 206e 6f74  ltime_end is not
+00021100: 204e 6f6e 6520 616e 6420 7265 616c 7469   None and realti
+00021110: 6d65 5f73 7461 7274 203e 2072 6561 6c74  me_start > realt
+00021120: 696d 655f 656e 643a 0d0a 2020 2020 2020  ime_end:..      
+00021130: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00021140: 6545 7272 6f72 2827 5468 6520 6461 7465  eError('The date
+00021150: 2073 6574 2062 7920 7661 7269 6162 6c65   set by variable
+00021160: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
+00021170: 2822 7b7d 2229 2063 616e 206e 6f74 2062  ("{}") can not b
+00021180: 6520 6166 7465 7220 7468 6520 6461 7465  e after the date
+00021190: 2073 6574 2062 7920 7661 7269 6162 6c65   set by variable
+000211a0: 2072 6561 6c74 696d 655f 656e 6420 2822   realtime_end ("
+000211b0: 7b7d 2229 2e27 2e66 6f72 6d61 7428 7265  {}").'.format(re
+000211c0: 616c 7469 6d65 5f73 7461 7274 2c20 7265  altime_start, re
+000211d0: 616c 7469 6d65 5f65 6e64 2929 0d0a 0d0a  altime_end))....
+000211e0: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
+000211f0: 656c 662e 5f63 6c69 656e 742e 6765 7428  elf._client.get(
+00021200: 0d0a 2020 2020 2020 2020 2020 2020 272f  ..            '/
+00021210: 6672 6564 2f73 6f75 7263 6527 2c0d 0a20  fred/source',.. 
+00021220: 2020 2020 2020 2020 2020 2027 736f 7572             'sour
+00021230: 6365 7327 2c0d 0a20 2020 2020 2020 2020  ces',..         
+00021240: 2020 2073 6f75 7263 655f 6964 3d73 6f75     source_id=sou
+00021250: 7263 655f 6964 2c0d 0a20 2020 2020 2020  rce_id,..       
+00021260: 2020 2020 2072 6561 6c74 696d 655f 7374       realtime_st
+00021270: 6172 743d 7265 616c 7469 6d65 5f73 7461  art=realtime_sta
+00021280: 7274 2c0d 0a20 2020 2020 2020 2020 2020  rt,..           
+00021290: 2072 6561 6c74 696d 655f 656e 643d 7265   realtime_end=re
+000212a0: 616c 7469 6d65 5f65 6e64 0d0a 2020 2020  altime_end..    
+000212b0: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
+000212c0: 2072 6574 7572 6e20 6d6f 6465 6c73 2e53   return models.S
+000212d0: 6f75 7263 6528 2a2a 6461 7461 5b30 5d29  ource(**data[0])
+000212e0: 0d0a 0d0a 2020 2020 6465 6620 736f 7572  ....    def sour
+000212f0: 6365 5f72 656c 6561 7365 7328 0d0a 2020  ce_releases(..  
+00021300: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+00021310: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
+00021320: 7263 655f 6964 3a20 696e 742c 0d0a 2020  rce_id: int,..  
+00021330: 2020 2020 2020 2020 2020 7265 616c 7469            realti
+00021340: 6d65 5f73 7461 7274 3a20 6461 7465 203d  me_start: date =
+00021350: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00021360: 2020 2020 7265 616c 7469 6d65 5f65 6e64      realtime_end
+00021370: 3a20 6461 7465 203d 204e 6f6e 652c 0d0a  : date = None,..
+00021380: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
+00021390: 725f 6279 3a20 656e 756d 732e 4f72 6465  r_by: enums.Orde
+000213a0: 7242 7920 3d20 656e 756d 732e 4f72 6465  rBy = enums.Orde
+000213b0: 7242 792e 7265 6c65 6173 655f 6964 2c0d  rBy.release_id,.
+000213c0: 0a20 2020 2020 2020 2020 2020 2073 6f72  .            sor
+000213d0: 745f 6f72 6465 723a 2065 6e75 6d73 2e53  t_order: enums.S
+000213e0: 6f72 744f 7264 6572 203d 2065 6e75 6d73  ortOrder = enums
+000213f0: 2e53 6f72 744f 7264 6572 2e61 7363 0d0a  .SortOrder.asc..
+00021400: 2020 2020 2920 2d3e 2070 642e 4461 7461      ) -> pd.Data
+00021410: 4672 616d 653a 0d0a 2020 2020 2020 2020  Frame:..        
+00021420: 2222 220d 0a20 2020 2020 2020 2023 2320  """..        ## 
+00021430: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00021440: 2020 2020 6073 6f75 7263 655f 6964 600d      `source_id`.
+00021450: 0a20 2020 2020 2020 2054 6865 2069 6420  .        The id 
+00021460: 666f 7220 6120 736f 7572 6365 2e0d 0a0d  for a source....
+00021470: 0a20 2020 2020 2020 2060 7265 616c 7469  .        `realti
+00021480: 6d65 5f73 7461 7274 600d 0a20 2020 2020  me_start`..     
+00021490: 2020 2054 6865 2073 7461 7274 206f 6620     The start of 
+000214a0: 7468 6520 7265 616c 2d74 696d 6520 7065  the real-time pe
+000214b0: 7269 6f64 2e20 466f 7220 6d6f 7265 2069  riod. For more i
+000214c0: 6e66 6f72 6d61 7469 6f6e 2c20 7365 6520  nformation, see 
+000214d0: 5b52 6561 6c2d 5469 6d65 2050 6572 696f  [Real-Time Perio
+000214e0: 6473 5d28 6874 7470 733a 2f2f 6672 6564  ds](https://fred
+000214f0: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
+00021500: 646f 6373 2f61 7069 2f66 7265 642f 7265  docs/api/fred/re
+00021510: 616c 7469 6d65 5f70 6572 696f 642e 6874  altime_period.ht
+00021520: 6d6c 292e 0d0a 0d0a 2020 2020 2020 2020  ml).....        
+00021530: 6072 6561 6c74 696d 655f 656e 6460 0d0a  `realtime_end`..
+00021540: 2020 2020 2020 2020 5468 6520 656e 6420          The end 
+00021550: 6f66 2074 6865 2072 6561 6c2d 7469 6d65  of the real-time
+00021560: 2070 6572 696f 642e 2046 6f72 206d 6f72   period. For mor
+00021570: 6520 696e 666f 726d 6174 696f 6e2c 2073  e information, s
+00021580: 6565 205b 5265 616c 2d54 696d 6520 5065  ee [Real-Time Pe
+00021590: 7269 6f64 735d 2868 7474 7073 3a2f 2f66  riods](https://f
+000215a0: 7265 642e 7374 6c6f 7569 7366 6564 2e6f  red.stlouisfed.o
+000215b0: 7267 2f64 6f63 732f 6170 692f 6672 6564  rg/docs/api/fred
+000215c0: 2f72 6561 6c74 696d 655f 7065 7269 6f64  /realtime_period
+000215d0: 2e68 746d 6c29 2e0d 0a0d 0a20 2020 2020  .html).....     
+000215e0: 2020 2060 6f72 6465 725f 6279 600d 0a20     `order_by`.. 
+000215f0: 2020 2020 2020 204f 7264 6572 2072 6573         Order res
+00021600: 756c 7473 2062 7920 7661 6c75 6573 206f  ults by values o
+00021610: 6620 7468 6520 7370 6563 6966 6965 6420  f the specified 
+00021620: 6174 7472 6962 7574 652e 0d0a 0d0a 2020  attribute.....  
+00021630: 2020 2020 2020 6073 6f72 745f 6f72 6465        `sort_orde
+00021640: 7260 0d0a 2020 2020 2020 2020 536f 7274  r`..        Sort
+00021650: 2072 6573 756c 7473 2069 7320 6173 6365   results is asce
+00021660: 6e64 696e 6720 6f72 2064 6573 6365 6e64  nding or descend
+00021670: 696e 6720 6f72 6465 7220 666f 7220 6174  ing order for at
+00021680: 7472 6962 7574 6520 7661 6c75 6573 2073  tribute values s
+00021690: 7065 6369 6669 6564 2062 7920 6f72 6465  pecified by orde
+000216a0: 725f 6279 2e0d 0a0d 0a20 2020 2020 2020  r_by.....       
+000216b0: 2023 2320 4465 7363 7269 7074 696f 6e0d   ## Description.
+000216c0: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
+000216d0: 2f66 7265 642e 7374 6c6f 7569 7366 6564  /fred.stlouisfed
+000216e0: 2e6f 7267 2f64 6f63 732f 6170 692f 6672  .org/docs/api/fr
+000216f0: 6564 2f73 6f75 7263 655f 7265 6c65 6173  ed/source_releas
+00021700: 6573 2e68 746d 6c0d 0a0d 0a20 2020 2020  es.html....     
+00021710: 2020 2047 6574 2074 6865 2072 656c 6561     Get the relea
+00021720: 7365 7320 666f 7220 6120 736f 7572 6365  ses for a source
+00021730: 2e0d 0a0d 0a20 2020 2020 2020 2023 2320  .....        ## 
+00021740: 4150 4920 5265 7175 6573 7420 2848 5454  API Request (HTT
+00021750: 5053 2047 4554 290d 0a20 2020 2020 2020  PS GET)..       
+00021760: 2068 7474 7073 3a2f 2f61 7069 2e73 746c   https://api.stl
+00021770: 6f75 6973 6665 642e 6f72 672f 6672 6564  ouisfed.org/fred
+00021780: 2f73 6f75 7263 652f 7265 6c65 6173 6573  /source/releases
+00021790: 3f73 6f75 7263 655f 6964 3d31 2661 7069  ?source_id=1&api
+000217a0: 5f6b 6579 3d61 6263 6465 6667 6869 6a6b  _key=abcdefghijk
+000217b0: 6c6d 6e6f 7071 7273 7475 7677 7879 7a31  lmnopqrstuvwxyz1
+000217c0: 3233 3435 3626 6669 6c65 5f74 7970 653d  23456&file_type=
+000217d0: 6a73 6f6e 0d0a 0d0a 2020 2020 2020 2020  json....        
+000217e0: 2323 2041 5049 2052 6573 706f 6e73 650d  ## API Response.
+000217f0: 0a20 2020 2020 2020 2060 6060 6a73 6f6e  .        ```json
+00021800: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
+00021810: 2020 2020 2020 2020 2022 7265 616c 7469           "realti
+00021820: 6d65 5f73 7461 7274 223a 2022 3230 3133  me_start": "2013
+00021830: 2d30 382d 3134 222c 0d0a 2020 2020 2020  -08-14",..      
+00021840: 2020 2020 2020 2272 6561 6c74 696d 655f        "realtime_
+00021850: 656e 6422 3a20 2232 3031 332d 3038 2d31  end": "2013-08-1
+00021860: 3422 2c0d 0a20 2020 2020 2020 2020 2020  4",..           
+00021870: 2022 6f72 6465 725f 6279 223a 2022 7265   "order_by": "re
+00021880: 6c65 6173 655f 6964 222c 0d0a 2020 2020  lease_id",..    
+00021890: 2020 2020 2020 2020 2273 6f72 745f 6f72          "sort_or
+000218a0: 6465 7222 3a20 2261 7363 222c 0d0a 2020  der": "asc",..  
+000218b0: 2020 2020 2020 2020 2020 2263 6f75 6e74            "count
+000218c0: 223a 2032 362c 0d0a 2020 2020 2020 2020  ": 26,..        
+000218d0: 2020 2020 226f 6666 7365 7422 3a20 302c      "offset": 0,
+000218e0: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
+000218f0: 696d 6974 223a 2031 3030 302c 0d0a 2020  imit": 1000,..  
+00021900: 2020 2020 2020 2020 2020 2272 656c 6561            "relea
+00021910: 7365 7322 3a20 5b0d 0a20 2020 2020 2020  ses": [..       
+00021920: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
+00021930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021940: 2269 6422 3a20 3133 2c0d 0a20 2020 2020  "id": 13,..     
+00021950: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00021960: 7265 616c 7469 6d65 5f73 7461 7274 223a  realtime_start":
+00021970: 2022 3230 3133 2d30 382d 3134 222c 0d0a   "2013-08-14",..
+00021980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021990: 2020 2020 2272 6561 6c74 696d 655f 656e      "realtime_en
+000219a0: 6422 3a20 2232 3031 332d 3038 2d31 3422  d": "2013-08-14"
+000219b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000219c0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+000219d0: 472e 3137 2049 6e64 7573 7472 6961 6c20  G.17 Industrial 
+000219e0: 5072 6f64 7563 7469 6f6e 2061 6e64 2043  Production and C
+000219f0: 6170 6163 6974 7920 5574 696c 697a 6174  apacity Utilizat
+00021a00: 696f 6e22 2c0d 0a20 2020 2020 2020 2020  ion",..         
+00021a10: 2020 2020 2020 2020 2020 2022 7072 6573             "pres
+00021a20: 735f 7265 6c65 6173 6522 3a20 7472 7565  s_release": true
+00021a30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00021a40: 2020 2020 2020 2022 6c69 6e6b 223a 2022         "link": "
+00021a50: 6874 7470 3a2f 2f77 7777 2e66 6564 6572  http://www.feder
+00021a60: 616c 7265 7365 7276 652e 676f 762f 7265  alreserve.gov/re
+00021a70: 6c65 6173 6573 2f67 3137 2f22 0d0a 2020  leases/g17/"..  
+00021a80: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00021a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00021aa0: 2020 2e2e 2e0d 0a20 2020 2020 2020 2020    .....         
+00021ab0: 2020 205d 0d0a 2020 2020 2020 2020 7d0d     ]..        }.
+00021ac0: 0a20 2020 2020 2020 2060 6060 0d0a 0d0a  .        ```....
+00021ad0: 2020 2020 2020 2020 2323 2052 6574 7572          ## Retur
+00021ae0: 6e73 0d0a 2020 2020 2020 2020 6070 616e  ns..        `pan
+00021af0: 6461 732e 4461 7461 4672 616d 6560 0d0a  das.DataFrame`..
+00021b00: 0d0a 2020 2020 2020 2020 2323 2045 7861  ..        ## Exa
+00021b10: 6d70 6c65 0d0a 2020 2020 2020 2020 6060  mple..        ``
+00021b20: 6070 7974 686f 6e0d 0a20 2020 2020 2020  `python..       
+00021b30: 203e 3e3e 2066 7265 6420 3d20 4652 4544   >>> fred = FRED
+00021b40: 2861 7069 5f6b 6579 3d27 6162 6364 6566  (api_key='abcdef
+00021b50: 6768 696a 6b6c 6d6e 6f70 7172 7374 7576  ghijklmnopqrstuv
+00021b60: 7778 797a 3132 3334 3536 2729 0d0a 2020  wxyz123456')..  
+00021b70: 2020 2020 2020 3e3e 3e20 6672 6564 2e73        >>> fred.s
+00021b80: 6f75 7263 655f 7265 6c65 6173 6573 2873  ource_releases(s
+00021b90: 6f75 7263 655f 6964 3d31 292e 6865 6164  ource_id=1).head
+00021ba0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00021bb0: 2020 2072 6561 6c74 696d 655f 7374 6172     realtime_star
+00021bc0: 7420 7265 616c 7469 6d65 5f65 6e64 2020  t realtime_end  
+00021bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021bf0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00021c00: 6520 2070 7265 7373 5f72 656c 6561 7365  e  press_release
+00021c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c30: 2020 2020 2020 2020 206c 696e 6b20 6e6f           link no
+00021c40: 7465 730d 0a20 2020 2020 2020 2020 2020  tes..           
+00021c50: 2069 640d 0a20 2020 2020 2020 2020 2020   id..           
+00021c60: 2031 3320 2020 2020 3230 3232 2d30 322d   13     2022-02-
+00021c70: 3035 2020 2032 3032 322d 3032 2d30 3520  05   2022-02-05 
+00021c80: 2047 2e31 3720 496e 6475 7374 7269 616c   G.17 Industrial
+00021c90: 2050 726f 6475 6374 696f 6e20 616e 6420   Production and 
+00021ca0: 4361 7061 6369 7479 2055 7469 6c69 7a2e  Capacity Utiliz.
+00021cb0: 2e2e 2020 2020 2020 2020 2020 2054 7275  ..           Tru
+00021cc0: 6520 2068 7474 703a 2f2f 7777 772e 6665  e  http://www.fe
+00021cd0: 6465 7261 6c72 6573 6572 7665 2e67 6f76  deralreserve.gov
+00021ce0: 2f72 656c 6561 7365 732f 6731 372f 2020  /releases/g17/  
+00021cf0: 3c4e 413e 0d0a 2020 2020 2020 2020 2020  <NA>..          
+00021d00: 2020 3134 2020 2020 2032 3032 322d 3032    14     2022-02
+00021d10: 2d30 3520 2020 3230 3232 2d30 322d 3035  -05   2022-02-05
+00021d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021d30: 2020 2020 2020 2020 2020 2020 2020 2047                 G
+00021d40: 2e31 3920 436f 6e73 756d 6572 2043 7265  .19 Consumer Cre
+00021d50: 6469 7420 2020 2020 2020 2020 2020 5472  dit           Tr
+00021d60: 7565 2020 6874 7470 3a2f 2f77 7777 2e66  ue  http://www.f
+00021d70: 6564 6572 616c 7265 7365 7276 652e 676f  ederalreserve.go
+00021d80: 762f 7265 6c65 6173 6573 2f67 3139 2f20  v/releases/g19/ 
+00021d90: 203c 4e41 3e0d 0a20 2020 2020 2020 2020   <NA>..         
+00021da0: 2020 2031 3520 2020 2020 3230 3232 2d30     15     2022-0
+00021db0: 322d 3035 2020 2032 3032 322d 3032 2d30  2-05   2022-02-0
+00021dc0: 3520 2020 2020 2020 2020 2020 2020 2020  5               
+00021dd0: 2020 2020 2020 2020 2020 472e 3520 466f            G.5 Fo
+00021de0: 7265 6967 6e20 4578 6368 616e 6765 2052  reign Exchange R
+00021df0: 6174 6573 2020 2020 2020 2020 2020 2054  ates           T
+00021e00: 7275 6520 2020 6874 7470 3a2f 2f77 7777  rue   http://www
+00021e10: 2e66 6564 6572 616c 7265 7365 7276 652e  .federalreserve.
+00021e20: 676f 762f 7265 6c65 6173 6573 2f67 352f  gov/releases/g5/
+00021e30: 2020 3c4e 413e 0d0a 2020 2020 2020 2020    <NA>..        
+00021e40: 2020 2020 3137 2020 2020 2032 3032 322d      17     2022-
+00021e50: 3032 2d30 3520 2020 3230 3232 2d30 322d  02-05   2022-02-
+00021e60: 3035 2020 2020 2020 2020 2020 2020 2020  05              
+00021e70: 2020 2020 2020 2020 2020 482e 3130 2046            H.10 F
+00021e80: 6f72 6569 676e 2045 7863 6861 6e67 6520  oreign Exchange 
+00021e90: 5261 7465 7320 2020 2020 2020 2020 2020  Rates           
+00021ea0: 5472 7565 2020 6874 7470 3a2f 2f77 7777  True  http://www
+00021eb0: 2e66 6564 6572 616c 7265 7365 7276 652e  .federalreserve.
+00021ec0: 676f 762f 7265 6c65 6173 6573 2f68 3130  gov/releases/h10
+00021ed0: 2f20 203c 4e41 3e0d 0a20 2020 2020 2020  /  <NA>..       
+00021ee0: 2020 2020 2031 3820 2020 2020 3230 3232       18     2022
+00021ef0: 2d30 322d 3035 2020 2032 3032 322d 3032  -02-05   2022-02
+00021f00: 2d30 3520 2020 2020 2020 2020 2020 2020  -05             
+00021f10: 2020 2020 2020 2020 2020 482e 3135 2053            H.15 S
+00021f20: 656c 6563 7465 6420 496e 7465 7265 7374  elected Interest
+00021f30: 2052 6174 6573 2020 2020 2020 2020 2020   Rates          
+00021f40: 2054 7275 6520 2068 7474 703a 2f2f 7777   True  http://ww
+00021f50: 772e 6665 6465 7261 6c72 6573 6572 7665  w.federalreserve
+00021f60: 2e67 6f76 2f72 656c 6561 7365 732f 6831  .gov/releases/h1
+00021f70: 352f 2020 3c4e 413e 0d0a 2020 2020 2020  5/  <NA>..      
+00021f80: 2020 6060 600d 0a20 2020 2020 2020 2022    ```..        "
+00021f90: 2222 0d0a 0d0a 2020 2020 2020 2020 616c  ""....        al
+00021fa0: 6c6f 7765 645f 6f72 6465 7273 203d 205b  lowed_orders = [
+00021fb0: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+00021fc0: 756d 732e 4f72 6465 7242 792e 7265 6c65  ums.OrderBy.rele
+00021fd0: 6173 655f 6964 2c0d 0a20 2020 2020 2020  ase_id,..       
+00021fe0: 2020 2020 2065 6e75 6d73 2e4f 7264 6572       enums.Order
+00021ff0: 4279 2e6e 616d 652c 0d0a 2020 2020 2020  By.name,..      
+00022000: 2020 2020 2020 656e 756d 732e 4f72 6465        enums.Orde
+00022010: 7242 792e 7072 6573 735f 7265 6c65 6173  rBy.press_releas
+00022020: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00022030: 656e 756d 732e 4f72 6465 7242 792e 7265  enums.OrderBy.re
+00022040: 616c 7469 6d65 5f73 7461 7274 2c0d 0a20  altime_start,.. 
+00022050: 2020 2020 2020 2020 2020 2065 6e75 6d73             enums
+00022060: 2e4f 7264 6572 4279 2e72 6561 6c74 696d  .OrderBy.realtim
+00022070: 655f 656e 640d 0a20 2020 2020 2020 205d  e_end..        ]
+00022080: 0d0a 0d0a 2020 2020 2020 2020 6966 206f  ....        if o
+00022090: 7264 6572 5f62 7920 6e6f 7420 696e 2061  rder_by not in a
+000220a0: 6c6c 6f77 6564 5f6f 7264 6572 733a 0d0a  llowed_orders:..
+000220b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000220c0: 6520 5661 6c75 6545 7272 6f72 2827 5661  e ValueError('Va
+000220d0: 7269 6162 6c65 206f 7264 6572 5f62 7920  riable order_by 
+000220e0: 287b 7d29 2069 7320 6e6f 7420 6f6e 6520  ({}) is not one 
+000220f0: 6f66 2074 6865 2076 616c 7565 733a 207b  of the values: {
+00022100: 7d27 2e66 6f72 6d61 7428 6f72 6465 725f  }'.format(order_
+00022110: 6279 2c20 272c 2027 2e6a 6f69 6e28 6d61  by, ', '.join(ma
+00022120: 7028 7374 722c 2061 6c6c 6f77 6564 5f6f  p(str, allowed_o
+00022130: 7264 6572 7329 2929 290d 0a0d 0a20 2020  rders))))....   
+00022140: 2020 2020 2069 6620 7265 616c 7469 6d65       if realtime
+00022150: 5f73 7461 7274 2069 7320 6e6f 7420 4e6f  _start is not No
+00022160: 6e65 2061 6e64 2072 6561 6c74 696d 655f  ne and realtime_
+00022170: 7374 6172 7420 3c20 6461 7465 2831 3737  start < date(177
+00022180: 362c 2037 2c20 3429 3a0d 0a20 2020 2020  6, 7, 4):..     
+00022190: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+000221a0: 7565 4572 726f 7228 2756 6172 6961 626c  ueError('Variabl
+000221b0: 6520 7265 616c 7469 6d65 5f73 7461 7274  e realtime_start
+000221c0: 2028 227b 7d22 2920 6973 2062 6566 6f72   ("{}") is befor
+000221d0: 6520 6d69 6e20 6461 7465 2031 3737 362d  e min date 1776-
+000221e0: 3037 2d30 342e 272e 666f 726d 6174 2872  07-04.'.format(r
+000221f0: 6561 6c74 696d 655f 7374 6172 7429 290d  ealtime_start)).
+00022200: 0a0d 0a20 2020 2020 2020 2069 6620 7265  ...        if re
+00022210: 616c 7469 6d65 5f73 7461 7274 2069 7320  altime_start is 
+00022220: 6e6f 7420 4e6f 6e65 2061 6e64 2072 6561  not None and rea
+00022230: 6c74 696d 655f 656e 6420 6973 206e 6f74  ltime_end is not
+00022240: 204e 6f6e 6520 616e 6420 7265 616c 7469   None and realti
+00022250: 6d65 5f73 7461 7274 203e 2072 6561 6c74  me_start > realt
+00022260: 696d 655f 656e 643a 0d0a 2020 2020 2020  ime_end:..      
+00022270: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00022280: 6545 7272 6f72 2827 5468 6520 6461 7465  eError('The date
+00022290: 2073 6574 2062 7920 7661 7269 6162 6c65   set by variable
+000222a0: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
+000222b0: 2822 7b7d 2229 2063 616e 206e 6f74 2062  ("{}") can not b
+000222c0: 6520 6166 7465 7220 7468 6520 6461 7465  e after the date
+000222d0: 2073 6574 2062 7920 7661 7269 6162 6c65   set by variable
+000222e0: 2072 6561 6c74 696d 655f 656e 6420 2822   realtime_end ("
+000222f0: 7b7d 2229 2e27 2e66 6f72 6d61 7428 7265  {}").'.format(re
+00022300: 616c 7469 6d65 5f73 7461 7274 2c20 7265  altime_start, re
+00022310: 616c 7469 6d65 5f65 6e64 2929 0d0a 0d0a  altime_end))....
+00022320: 2020 2020 2020 2020 6466 203d 2070 642e          df = pd.
+00022330: 4461 7461 4672 616d 6528 0d0a 2020 2020  DataFrame(..    
+00022340: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+00022350: 6965 6e74 2e67 6574 280d 0a20 2020 2020  ient.get(..     
+00022360: 2020 2020 2020 2020 2020 2027 2f66 7265             '/fre
+00022370: 642f 736f 7572 6365 2f72 656c 6561 7365  d/source/release
+00022380: 7327 2c0d 0a20 2020 2020 2020 2020 2020  s',..           
+00022390: 2020 2020 2027 7265 6c65 6173 6573 272c       'releases',
+000223a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000223b0: 2020 6c69 6d69 743d 3130 3030 2c0d 0a20    limit=1000,.. 
+000223c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000223d0: 6f75 7263 655f 6964 3d73 6f75 7263 655f  ource_id=source_
+000223e0: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
+000223f0: 2020 2020 2072 6561 6c74 696d 655f 7374       realtime_st
+00022400: 6172 743d 7265 616c 7469 6d65 5f73 7461  art=realtime_sta
+00022410: 7274 2c0d 0a20 2020 2020 2020 2020 2020  rt,..           
+00022420: 2020 2020 2072 6561 6c74 696d 655f 656e       realtime_en
+00022430: 643d 7265 616c 7469 6d65 5f65 6e64 2c0d  d=realtime_end,.
+00022440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022450: 206f 7264 6572 5f62 793d 6f72 6465 725f   order_by=order_
+00022460: 6279 2c0d 0a20 2020 2020 2020 2020 2020  by,..           
+00022470: 2020 2020 2073 6f72 745f 6f72 6465 723d       sort_order=
+00022480: 736f 7274 5f6f 7264 6572 0d0a 2020 2020  sort_order..    
+00022490: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+000224a0: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+000224b0: 6461 7465 5f63 6f6c 756d 6e73 203d 205b  date_columns = [
+000224c0: 2772 6561 6c74 696d 655f 7374 6172 7427  'realtime_start'
+000224d0: 2c20 2772 6561 6c74 696d 655f 656e 6427  , 'realtime_end'
+000224e0: 5d0d 0a0d 0a20 2020 2020 2020 2069 6620  ]....        if 
+000224f0: 6e6f 7420 6466 2e65 6d70 7479 3a0d 0a20  not df.empty:.. 
+00022500: 2020 2020 2020 2020 2020 2064 665b 6461             df[da
+00022510: 7465 5f63 6f6c 756d 6e73 5d20 3d20 6466  te_columns] = df
+00022520: 5b64 6174 655f 636f 6c75 6d6e 735d 2e61  [date_columns].a
+00022530: 7070 6c79 2870 642e 746f 5f64 6174 6574  pply(pd.to_datet
+00022540: 696d 652c 2066 6f72 6d61 743d 2725 592d  ime, format='%Y-
+00022550: 256d 2d25 6427 290d 0a0d 0a20 2020 2020  %m-%d')....     
+00022560: 2020 2020 2020 2064 6620 3d20 6466 2e61         df = df.a
+00022570: 7374 7970 6528 6474 7970 653d 7b0d 0a20  stype(dtype={.. 
+00022580: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00022590: 6e61 6d65 273a 2027 7374 7269 6e67 272c  name': 'string',
+000225a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000225b0: 2020 276c 696e 6b27 3a20 2773 7472 696e    'link': 'strin
+000225c0: 6727 2c0d 0a20 2020 2020 2020 2020 2020  g',..           
+000225d0: 2020 2020 2027 6e6f 7465 7327 3a20 2773       'notes': 's
+000225e0: 7472 696e 6727 2c0d 0a20 2020 2020 2020  tring',..       
+000225f0: 2020 2020 2020 2020 2027 7072 6573 735f           'press_
+00022600: 7265 6c65 6173 6527 3a20 2762 6f6f 6c27  release': 'bool'
+00022610: 0d0a 2020 2020 2020 2020 2020 2020 7d29  ..            })
+00022620: 2e73 6574 5f69 6e64 6578 2827 6964 2729  .set_index('id')
+00022630: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+00022640: 726e 2064 660d 0a0d 0a20 2020 2022 2222  rn df....    """
+00022650: 0d0a 2020 2020 5461 6773 0d0a 0d0a 2020  ..    Tags....  
+00022660: 2020 6874 7470 733a 2f2f 6672 6564 2e73    https://fred.s
+00022670: 746c 6f75 6973 6665 642e 6f72 672f 7461  tlouisfed.org/ta
+00022680: 6773 0d0a 2020 2020 2222 220d 0a0d 0a20  gs..    """.... 
+00022690: 2020 2064 6566 2074 6167 7328 0d0a 2020     def tags(..  
+000226a0: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+000226b0: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+000226c0: 6c74 696d 655f 7374 6172 743a 2064 6174  ltime_start: dat
+000226d0: 6520 3d20 4e6f 6e65 2c0d 0a20 2020 2020  e = None,..     
+000226e0: 2020 2020 2020 2072 6561 6c74 696d 655f         realtime_
+000226f0: 656e 643a 2064 6174 6520 3d20 4e6f 6e65  end: date = None
+00022700: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00022710: 6167 5f6e 616d 6573 3a20 4c69 7374 5b73  ag_names: List[s
+00022720: 7472 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  tr] = None,..   
+00022730: 2020 2020 2020 2020 2074 6167 5f67 726f           tag_gro
+00022740: 7570 5f69 643a 2065 6e75 6d73 2e54 6167  up_id: enums.Tag
+00022750: 4772 6f75 7049 4420 3d20 4e6f 6e65 2c0d  GroupID = None,.
+00022760: 0a20 2020 2020 2020 2020 2020 2073 6561  .            sea
+00022770: 7263 685f 7465 7874 3a20 7374 7220 3d20  rch_text: str = 
+00022780: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+00022790: 2020 206f 7264 6572 5f62 793a 2065 6e75     order_by: enu
+000227a0: 6d73 2e4f 7264 6572 4279 203d 2065 6e75  ms.OrderBy = enu
+000227b0: 6d73 2e4f 7264 6572 4279 2e73 6572 6965  ms.OrderBy.serie
+000227c0: 735f 636f 756e 742c 0d0a 2020 2020 2020  s_count,..      
+000227d0: 2020 2020 2020 736f 7274 5f6f 7264 6572        sort_order
+000227e0: 3a20 656e 756d 732e 536f 7274 4f72 6465  : enums.SortOrde
+000227f0: 7220 3d20 656e 756d 732e 536f 7274 4f72  r = enums.SortOr
+00022800: 6465 722e 6173 630d 0a20 2020 2029 202d  der.asc..    ) -
+00022810: 3e20 7064 2e44 6174 6146 7261 6d65 3a0d  > pd.DataFrame:.
+00022820: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00022830: 2020 2020 2020 2323 2050 6172 616d 6574        ## Paramet
+00022840: 6572 730d 0a20 2020 2020 2020 2060 7265  ers..        `re
+00022850: 616c 7469 6d65 5f73 7461 7274 600d 0a20  altime_start`.. 
+00022860: 2020 2020 2020 2054 6865 2073 7461 7274         The start
+00022870: 206f 6620 7468 6520 7265 616c 2d74 696d   of the real-tim
+00022880: 6520 7065 7269 6f64 2e20 466f 7220 6d6f  e period. For mo
+00022890: 7265 2069 6e66 6f72 6d61 7469 6f6e 2c20  re information, 
+000228a0: 7365 6520 5b52 6561 6c2d 5469 6d65 2050  see [Real-Time P
+000228b0: 6572 696f 6473 5d28 6874 7470 733a 2f2f  eriods](https://
+000228c0: 6672 6564 2e73 746c 6f75 6973 6665 642e  fred.stlouisfed.
+000228d0: 6f72 672f 646f 6373 2f61 7069 2f66 7265  org/docs/api/fre
+000228e0: 642f 7265 616c 7469 6d65 5f70 6572 696f  d/realtime_perio
+000228f0: 642e 6874 6d6c 292e 0d0a 0d0a 2020 2020  d.html).....    
+00022900: 2020 2020 6072 6561 6c74 696d 655f 656e      `realtime_en
+00022910: 6460 0d0a 2020 2020 2020 2020 5468 6520  d`..        The 
+00022920: 656e 6420 6f66 2074 6865 2072 6561 6c2d  end of the real-
+00022930: 7469 6d65 2070 6572 696f 642e 2046 6f72  time period. For
+00022940: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+00022950: 6e2c 2073 6565 205b 5265 616c 2d54 696d  n, see [Real-Tim
+00022960: 6520 5065 7269 6f64 735d 2868 7474 7073  e Periods](https
+00022970: 3a2f 2f66 7265 642e 7374 6c6f 7569 7366  ://fred.stlouisf
+00022980: 6564 2e6f 7267 2f64 6f63 732f 6170 692f  ed.org/docs/api/
+00022990: 6672 6564 2f72 6561 6c74 696d 655f 7065  fred/realtime_pe
+000229a0: 7269 6f64 2e68 746d 6c29 2e0d 0a0d 0a20  riod.html)..... 
+000229b0: 2020 2020 2020 2060 7461 675f 6e61 6d65         `tag_name
+000229c0: 7360 0d0a 2020 2020 2020 2020 5475 706c  s`..        Tupl
+000229d0: 6520 6f66 2074 6167 206e 616d 6573 2074  e of tag names t
+000229e0: 6861 7420 7365 7269 6573 206d 6174 6368  hat series match
+000229f0: 2061 6c6c 206f 662e 0d0a 0d0a 2020 2020   all of.....    
+00022a00: 2020 2020 6074 6167 5f67 726f 7570 5f69      `tag_group_i
+00022a10: 6460 0d0a 2020 2020 2020 2020 4120 7461  d`..        A ta
+00022a20: 6720 6772 6f75 7020 6964 2074 6f20 6669  g group id to fi
+00022a30: 6c74 6572 2074 6167 7320 6279 2074 7970  lter tags by typ
+00022a40: 652e 0d0a 0d0a 2020 2020 2020 2020 6073  e.....        `s
+00022a50: 6561 7263 685f 7465 7874 600d 0a20 2020  earch_text`..   
+00022a60: 2020 2020 2054 6865 2077 6f72 6473 2074       The words t
+00022a70: 6f20 6669 6e64 206d 6174 6368 696e 6720  o find matching 
+00022a80: 7461 6773 2077 6974 682e 0d0a 0d0a 2020  tags with.....  
+00022a90: 2020 2020 2020 606f 7264 6572 5f62 7960        `order_by`
+00022aa0: 0d0a 2020 2020 2020 2020 4f72 6465 7220  ..        Order 
+00022ab0: 7265 7375 6c74 7320 6279 2076 616c 7565  results by value
+00022ac0: 7320 6f66 2074 6865 2073 7065 6369 6669  s of the specifi
+00022ad0: 6564 2061 7474 7269 6275 7465 2e0d 0a0d  ed attribute....
+00022ae0: 0a20 2020 2020 2020 2060 736f 7274 5f6f  .        `sort_o
+00022af0: 7264 6572 600d 0a20 2020 2020 2020 2053  rder`..        S
+00022b00: 6f72 7420 7265 7375 6c74 7320 6973 2061  ort results is a
+00022b10: 7363 656e 6469 6e67 206f 7220 6465 7363  scending or desc
+00022b20: 656e 6469 6e67 206f 7264 6572 2066 6f72  ending order for
+00022b30: 2061 7474 7269 6275 7465 2076 616c 7565   attribute value
+00022b40: 7320 7370 6563 6966 6965 6420 6279 206f  s specified by o
+00022b50: 7264 6572 5f62 792e 0d0a 0d0a 2020 2020  rder_by.....    
+00022b60: 2020 2020 2323 2044 6573 6372 6970 7469      ## Descripti
+00022b70: 6f6e 0d0a 2020 2020 2020 2020 6874 7470  on..        http
+00022b80: 733a 2f2f 6672 6564 2e73 746c 6f75 6973  s://fred.stlouis
+00022b90: 6665 642e 6f72 672f 646f 6373 2f61 7069  fed.org/docs/api
+00022ba0: 2f66 7265 642f 7461 6773 2e68 746d 6c0d  /fred/tags.html.
+00022bb0: 0a0d 0a20 2020 2020 2020 2047 6574 2046  ...        Get F
+00022bc0: 5245 4420 7461 6773 2e20 4f70 7469 6f6e  RED tags. Option
+00022bd0: 616c 6c79 2c20 6669 6c74 6572 2072 6573  ally, filter res
+00022be0: 756c 7473 2062 7920 7461 6720 6e61 6d65  ults by tag name
+00022bf0: 2c20 7461 6720 6772 6f75 702c 206f 7220  , tag group, or 
+00022c00: 7365 6172 6368 2e20 4652 4544 2074 6167  search. FRED tag
+00022c10: 7320 6172 6520 6174 7472 6962 7574 6573  s are attributes
+00022c20: 2061 7373 6967 6e65 6420 746f 2073 6572   assigned to ser
+00022c30: 6965 732e 2053 6565 2074 6865 2072 656c  ies. See the rel
+00022c40: 6174 6564 2072 6571 7565 7374 2066 7265  ated request fre
+00022c50: 642f 7265 6c61 7465 645f 7461 6773 2e0d  d/related_tags..
+00022c60: 0a0d 0a20 2020 2020 2020 2023 2320 4150  ...        ## AP
+00022c70: 4920 5265 7175 6573 7420 2848 5454 5053  I Request (HTTPS
+00022c80: 2047 4554 290d 0a20 2020 2020 2020 2068   GET)..        h
+00022c90: 7474 7073 3a2f 2f61 7069 2e73 746c 6f75  ttps://api.stlou
+00022ca0: 6973 6665 642e 6f72 672f 6672 6564 2f74  isfed.org/fred/t
+00022cb0: 6167 733f 6170 695f 6b65 793d 6162 6364  ags?api_key=abcd
+00022cc0: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
+00022cd0: 7576 7778 797a 3132 3334 3536 2666 696c  uvwxyz123456&fil
+00022ce0: 655f 7479 7065 3d6a 736f 6e0d 0a0d 0a20  e_type=json.... 
+00022cf0: 2020 2020 2020 2023 2320 4150 4920 5265         ## API Re
+00022d00: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
+00022d10: 6060 606a 736f 6e0d 0a20 2020 2020 2020  ```json..       
+00022d20: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00022d30: 2272 6561 6c74 696d 655f 7374 6172 7422  "realtime_start"
+00022d40: 3a20 2232 3031 332d 3038 2d31 3422 2c0d  : "2013-08-14",.
+00022d50: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00022d60: 616c 7469 6d65 5f65 6e64 223a 2022 3230  altime_end": "20
+00022d70: 3133 2d30 382d 3134 222c 0d0a 2020 2020  13-08-14",..    
+00022d80: 2020 2020 2020 2020 226f 7264 6572 5f62          "order_b
+00022d90: 7922 3a20 2273 6572 6965 735f 636f 756e  y": "series_coun
+00022da0: 7422 2c0d 0a20 2020 2020 2020 2020 2020  t",..           
+00022db0: 2022 736f 7274 5f6f 7264 6572 223a 2022   "sort_order": "
+00022dc0: 6465 7363 222c 0d0a 2020 2020 2020 2020  desc",..        
+00022dd0: 2020 2020 2263 6f75 6e74 223a 2034 3739      "count": 479
+00022de0: 342c 0d0a 2020 2020 2020 2020 2020 2020  4,..            
+00022df0: 226f 6666 7365 7422 3a20 302c 0d0a 2020  "offset": 0,..  
+00022e00: 2020 2020 2020 2020 2020 226c 696d 6974            "limit
+00022e10: 223a 2031 3030 302c 0d0a 2020 2020 2020  ": 1000,..      
+00022e20: 2020 2020 2020 2274 6167 7322 3a20 5b0d        "tags": [.
+00022e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022e40: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00022e50: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00022e60: 226e 6174 696f 6e22 2c0d 0a20 2020 2020  "nation",..     
+00022e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00022e80: 6772 6f75 705f 6964 223a 2022 6765 6f74  group_id": "geot
+00022e90: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00022ea0: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
+00022eb0: 2022 436f 756e 7472 7920 4c65 7665 6c22   "Country Level"
+00022ec0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00022ed0: 2020 2020 2020 2022 6372 6561 7465 6422         "created"
+00022ee0: 3a20 2232 3031 322d 3032 2d32 3720 3130  : "2012-02-27 10
+00022ef0: 3a31 383a 3139 2d30 3622 2c0d 0a20 2020  :18:19-06",..   
+00022f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022f10: 2022 706f 7075 6c61 7269 7479 223a 2031   "popularity": 1
+00022f20: 3030 2c0d 0a20 2020 2020 2020 2020 2020  00,..           
+00022f30: 2020 2020 2020 2020 2022 7365 7269 6573           "series
+00022f40: 5f63 6f75 6e74 223a 2031 3035 3230 300d  _count": 105200.
+00022f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022f60: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
+00022f70: 2020 2020 202e 2e2e 0d0a 2020 2020 2020       .....      
+00022f80: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
+00022f90: 207d 0d0a 2020 2020 2020 2020 6060 600d   }..        ```.
+00022fa0: 0a0d 0a20 2020 2020 2020 2023 2320 5265  ...        ## Re
+00022fb0: 7475 726e 730d 0a20 2020 2020 2020 2060  turns..        `
+00022fc0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+00022fd0: 600d 0a0d 0a20 2020 2020 2020 2023 2320  `....        ## 
+00022fe0: 4578 616d 706c 650d 0a20 2020 2020 2020  Example..       
+00022ff0: 2060 6060 7079 7468 6f6e 0d0a 2020 2020   ```python..    
+00023000: 2020 2020 3e3e 3e20 6672 6564 203d 2046      >>> fred = F
+00023010: 5245 4428 6170 695f 6b65 793d 2761 6263  RED(api_key='abc
+00023020: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
+00023030: 7475 7677 7879 7a31 3233 3435 3627 290d  tuvwxyz123456').
+00023040: 0a20 2020 2020 2020 203e 3e3e 2066 7265  .        >>> fre
+00023050: 642e 7461 6773 2829 2e68 6561 6428 290d  d.tags().head().
+00023060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023070: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+00023080: 705f 6964 206e 6f74 6573 2020 2020 2020  p_id notes      
+00023090: 2020 2020 2020 2020 2020 2020 2063 7265               cre
+000230a0: 6174 6564 2020 706f 7075 6c61 7269 7479  ated  popularity
+000230b0: 2020 7365 7269 6573 5f63 6f75 6e74 0d0a    series_count..
+000230c0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000230d0: 0d0a 2020 2020 2020 2020 2020 2020 3134  ..            14
+000230e0: 2079 6561 7273 202b 2020 2020 2020 2020   years +        
+000230f0: 2020 6765 6e20 2020 2020 2020 3230 3132    gen       2012
+00023100: 2d30 382d 3036 2031 393a 3430 3a35 362b  -08-06 19:40:56+
+00023110: 3030 3a30 3020 2020 2020 2020 2020 202d  00:00          -
+00023120: 3620 2020 2020 2020 2020 2020 2020 320d  6             2.
+00023130: 0a20 2020 2020 2020 2020 2020 2032 2d6d  .            2-m
+00023140: 6f6e 7468 202b 2020 2020 2020 2020 2020  onth +          
+00023150: 2067 656e 2020 2020 2020 2032 3031 322d   gen       2012-
+00023160: 3038 2d30 3620 3139 3a33 343a 3035 2b30  08-06 19:34:05+0
+00023170: 303a 3030 2020 2020 2020 2020 202d 3632  0:00         -62
+00023180: 2020 2020 2020 2020 2020 2020 2032 0d0a               2..
+00023190: 2020 2020 2020 2020 2020 2020 322d 7765              2-we
+000231a0: 656b 2020 2020 2020 2020 2020 2020 2020  ek              
+000231b0: 6765 6e20 2020 2020 2020 3230 3132 2d30  gen       2012-0
+000231c0: 352d 3235 2031 363a 3239 3a33 342b 3030  5-25 16:29:34+00
+000231d0: 3a30 3020 2020 2020 2020 2020 202d 3620  :00          -6 
+000231e0: 2020 2020 2020 2020 2020 2020 320d 0a20              2.. 
+000231f0: 2020 2020 2020 2020 2020 2033 3020 746f             30 to
+00023200: 2033 3420 7965 6172 7320 2020 2020 2067   34 years      g
+00023210: 656e 2020 2020 2020 2032 3031 332d 3130  en       2013-10
+00023220: 2d31 3020 3231 3a31 333a 3034 2b30 303a  -10 21:13:04+00:
+00023230: 3030 2020 2020 2020 2020 202d 3133 2020  00         -13  
+00023240: 2020 2020 2020 2020 2020 2032 0d0a 2020             2..  
+00023250: 2020 2020 2020 2020 2020 332d 6661 6d69            3-fami
+00023260: 6c79 202b 2020 2020 2020 2020 2020 6765  ly +          ge
+00023270: 6e20 2020 2020 2020 3230 3132 2d30 382d  n       2012-08-
+00023280: 3036 2031 393a 3438 3a31 312b 3030 3a30  06 19:48:11+00:0
+00023290: 3020 2020 2020 2020 2020 2d34 3920 2020  0         -49   
+000232a0: 2020 2020 2020 2020 2020 320d 0a20 2020            2..   
+000232b0: 2020 2020 2060 6060 0d0a 2020 2020 2020       ```..      
+000232c0: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+000232d0: 2061 6c6c 6f77 6564 5f6f 7264 6572 7320   allowed_orders 
+000232e0: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
+000232f0: 2065 6e75 6d73 2e4f 7264 6572 4279 2e73   enums.OrderBy.s
+00023300: 6572 6965 735f 636f 756e 742c 0d0a 2020  eries_count,..  
+00023310: 2020 2020 2020 2020 2020 656e 756d 732e            enums.
+00023320: 4f72 6465 7242 792e 706f 7075 6c61 7269  OrderBy.populari
+00023330: 7479 2c0d 0a20 2020 2020 2020 2020 2020  ty,..           
+00023340: 2065 6e75 6d73 2e4f 7264 6572 4279 2e63   enums.OrderBy.c
+00023350: 7265 6174 6564 2c0d 0a20 2020 2020 2020  reated,..       
+00023360: 2020 2020 2065 6e75 6d73 2e4f 7264 6572       enums.Order
+00023370: 4279 2e6e 616d 652c 0d0a 2020 2020 2020  By.name,..      
+00023380: 2020 2020 2020 656e 756d 732e 4f72 6465        enums.Orde
+00023390: 7242 792e 6772 6f75 705f 6964 0d0a 2020  rBy.group_id..  
+000233a0: 2020 2020 2020 5d0d 0a0d 0a20 2020 2020        ]....     
+000233b0: 2020 2069 6620 6f72 6465 725f 6279 206e     if order_by n
+000233c0: 6f74 2069 6e20 616c 6c6f 7765 645f 6f72  ot in allowed_or
+000233d0: 6465 7273 3a0d 0a20 2020 2020 2020 2020  ders:..         
+000233e0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+000233f0: 726f 7228 2756 6172 6961 626c 6520 6f72  ror('Variable or
+00023400: 6465 725f 6279 2028 7b7d 2920 6973 206e  der_by ({}) is n
+00023410: 6f74 206f 6e65 206f 6620 7468 6520 7661  ot one of the va
+00023420: 6c75 6573 3a20 7b7d 272e 666f 726d 6174  lues: {}'.format
+00023430: 286f 7264 6572 5f62 792c 2027 2c20 272e  (order_by, ', '.
+00023440: 6a6f 696e 286d 6170 2873 7472 2c20 616c  join(map(str, al
+00023450: 6c6f 7765 645f 6f72 6465 7273 2929 2929  lowed_orders))))
+00023460: 0d0a 0d0a 2020 2020 2020 2020 6966 2074  ....        if t
+00023470: 6167 5f67 726f 7570 5f69 6420 6973 206e  ag_group_id is n
+00023480: 6f74 204e 6f6e 6520 616e 6420 7461 675f  ot None and tag_
+00023490: 6772 6f75 705f 6964 206e 6f74 2069 6e20  group_id not in 
+000234a0: 656e 756d 732e 5461 6747 726f 7570 4944  enums.TagGroupID
+000234b0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000234c0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000234d0: 2756 6172 6961 626c 6520 7461 675f 6772  'Variable tag_gr
+000234e0: 6f75 705f 6964 2028 7b7d 2920 6973 206e  oup_id ({}) is n
+000234f0: 6f74 206f 6e65 206f 6620 7468 6520 7661  ot one of the va
+00023500: 6c75 6573 3a20 7b7d 272e 666f 726d 6174  lues: {}'.format
+00023510: 2874 6167 5f67 726f 7570 5f69 642c 2027  (tag_group_id, '
+00023520: 2c20 272e 6a6f 696e 286d 6170 2873 7472  , '.join(map(str
+00023530: 2c20 656e 756d 732e 5461 6747 726f 7570  , enums.TagGroup
+00023540: 4944 2929 2929 0d0a 0d0a 2020 2020 2020  ID))))....      
+00023550: 2020 6966 2072 6561 6c74 696d 655f 7374    if realtime_st
+00023560: 6172 7420 6973 206e 6f74 204e 6f6e 6520  art is not None 
+00023570: 616e 6420 7265 616c 7469 6d65 5f73 7461  and realtime_sta
+00023580: 7274 203c 2064 6174 6528 3137 3736 2c20  rt < date(1776, 
+00023590: 372c 2034 293a 0d0a 2020 2020 2020 2020  7, 4):..        
+000235a0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000235b0: 7272 6f72 2827 5661 7269 6162 6c65 2072  rror('Variable r
+000235c0: 6561 6c74 696d 655f 7374 6172 7420 2822  ealtime_start ("
+000235d0: 7b7d 2229 2069 7320 6265 666f 7265 206d  {}") is before m
+000235e0: 696e 2064 6174 6520 3137 3736 2d30 372d  in date 1776-07-
+000235f0: 3034 2e27 2e66 6f72 6d61 7428 7265 616c  04.'.format(real
+00023600: 7469 6d65 5f73 7461 7274 2929 0d0a 0d0a  time_start))....
+00023610: 2020 2020 2020 2020 6966 2072 6561 6c74          if realt
+00023620: 696d 655f 7374 6172 7420 6973 206e 6f74  ime_start is not
+00023630: 204e 6f6e 6520 616e 6420 7265 616c 7469   None and realti
+00023640: 6d65 5f65 6e64 2069 7320 6e6f 7420 4e6f  me_end is not No
+00023650: 6e65 2061 6e64 2072 6561 6c74 696d 655f  ne and realtime_
+00023660: 7374 6172 7420 3e20 7265 616c 7469 6d65  start > realtime
+00023670: 5f65 6e64 3a0d 0a20 2020 2020 2020 2020  _end:..         
+00023680: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00023690: 726f 7228 2754 6865 2064 6174 6520 7365  ror('The date se
+000236a0: 7420 6279 2076 6172 6961 626c 6520 7265  t by variable re
+000236b0: 616c 7469 6d65 5f73 7461 7274 2028 227b  altime_start ("{
+000236c0: 7d22 2920 6361 6e20 6e6f 7420 6265 2061  }") can not be a
+000236d0: 6674 6572 2074 6865 2064 6174 6520 7365  fter the date se
+000236e0: 7420 6279 2076 6172 6961 626c 6520 7265  t by variable re
+000236f0: 616c 7469 6d65 5f65 6e64 2028 227b 7d22  altime_end ("{}"
+00023700: 292e 272e 666f 726d 6174 2872 6561 6c74  ).'.format(realt
+00023710: 696d 655f 7374 6172 742c 2072 6561 6c74  ime_start, realt
+00023720: 696d 655f 656e 6429 290d 0a0d 0a20 2020  ime_end))....   
+00023730: 2020 2020 2064 6620 3d20 7064 2e44 6174       df = pd.Dat
+00023740: 6146 7261 6d65 280d 0a20 2020 2020 2020  aFrame(..       
+00023750: 2020 2020 2073 656c 662e 5f63 6c69 656e       self._clien
+00023760: 742e 6765 7428 0d0a 2020 2020 2020 2020  t.get(..        
+00023770: 2020 2020 2020 2020 272f 6672 6564 2f74          '/fred/t
+00023780: 6167 7327 2c0d 0a20 2020 2020 2020 2020  ags',..         
+00023790: 2020 2020 2020 2027 7461 6773 272c 0d0a         'tags',..
+000237a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000237b0: 6c69 6d69 743d 3130 3030 2c0d 0a20 2020  limit=1000,..   
+000237c0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+000237d0: 6c74 696d 655f 7374 6172 743d 7265 616c  ltime_start=real
+000237e0: 7469 6d65 5f73 7461 7274 2c0d 0a20 2020  time_start,..   
+000237f0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00023800: 6c74 696d 655f 656e 643d 7265 616c 7469  ltime_end=realti
+00023810: 6d65 5f65 6e64 2c0d 0a20 2020 2020 2020  me_end,..       
+00023820: 2020 2020 2020 2020 2074 6167 5f6e 616d           tag_nam
+00023830: 6573 3d74 6167 5f6e 616d 6573 2c0d 0a20  es=tag_names,.. 
+00023840: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00023850: 6167 5f67 726f 7570 5f69 643d 7461 675f  ag_group_id=tag_
+00023860: 6772 6f75 705f 6964 2c0d 0a20 2020 2020  group_id,..     
+00023870: 2020 2020 2020 2020 2020 2073 6561 7263             searc
+00023880: 685f 7465 7874 3d73 6561 7263 685f 7465  h_text=search_te
+00023890: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
+000238a0: 2020 2020 206f 7264 6572 5f62 793d 6f72       order_by=or
+000238b0: 6465 725f 6279 2c0d 0a20 2020 2020 2020  der_by,..       
+000238c0: 2020 2020 2020 2020 2073 6f72 745f 6f72           sort_or
+000238d0: 6465 723d 736f 7274 5f6f 7264 6572 0d0a  der=sort_order..
+000238e0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+000238f0: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+00023900: 2020 2020 6966 206e 6f74 2064 662e 656d      if not df.em
+00023910: 7074 793a 0d0a 2020 2020 2020 2020 2020  pty:..          
+00023920: 2020 6466 2e63 7265 6174 6564 203d 2070    df.created = p
+00023930: 642e 746f 5f64 6174 6574 696d 6528 6466  d.to_datetime(df
+00023940: 2e63 7265 6174 6564 202b 2027 3030 272c  .created + '00',
+00023950: 2075 7463 3d54 7275 652c 2066 6f72 6d61   utc=True, forma
+00023960: 743d 2725 592d 256d 2d25 6420 2548 3a25  t='%Y-%m-%d %H:%
+00023970: 4d3a 2553 257a 2729 0d0a 0d0a 2020 2020  M:%S%z')....    
+00023980: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
+00023990: 6173 7479 7065 2864 7479 7065 3d7b 0d0a  astype(dtype={..
+000239a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000239b0: 276e 616d 6527 3a20 2773 7472 696e 6727  'name': 'string'
+000239c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000239d0: 2020 2027 6e6f 7465 7327 3a20 2773 7472     'notes': 'str
+000239e0: 696e 6727 2c0d 0a20 2020 2020 2020 2020  ing',..         
+000239f0: 2020 2020 2020 2027 6772 6f75 705f 6964         'group_id
+00023a00: 273a 2027 6361 7465 676f 7279 270d 0a20  ': 'category'.. 
+00023a10: 2020 2020 2020 2020 2020 207d 292e 7365             }).se
+00023a20: 745f 696e 6465 7828 276e 616d 6527 290d  t_index('name').
+00023a30: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00023a40: 6e20 6466 0d0a 0d0a 2020 2020 6465 6620  n df....    def 
+00023a50: 7265 6c61 7465 645f 7461 6773 280d 0a20  related_tags(.. 
+00023a60: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00023a70: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00023a80: 616c 7469 6d65 5f73 7461 7274 3a20 6461  altime_start: da
+00023a90: 7465 203d 204e 6f6e 652c 0d0a 2020 2020  te = None,..    
+00023aa0: 2020 2020 2020 2020 7265 616c 7469 6d65          realtime
+00023ab0: 5f65 6e64 3a20 6461 7465 203d 204e 6f6e  _end: date = Non
+00023ac0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00023ad0: 7461 675f 6e61 6d65 733a 204c 6973 745b  tag_names: List[
+00023ae0: 7374 725d 203d 204e 6f6e 652c 0d0a 2020  str] = None,..  
+00023af0: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
+00023b00: 655f 7461 675f 6e61 6d65 733a 204c 6973  e_tag_names: Lis
+00023b10: 745b 7374 725d 203d 204e 6f6e 652c 0d0a  t[str] = None,..
+00023b20: 2020 2020 2020 2020 2020 2020 7461 675f              tag_
+00023b30: 6772 6f75 705f 6964 3a20 656e 756d 732e  group_id: enums.
+00023b40: 5461 6747 726f 7570 4944 203d 204e 6f6e  TagGroupID = Non
+00023b50: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00023b60: 7365 6172 6368 5f74 6578 743a 2073 7472  search_text: str
+00023b70: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+00023b80: 2020 2020 2020 6f72 6465 725f 6279 3a20        order_by: 
+00023b90: 656e 756d 732e 4f72 6465 7242 7920 3d20  enums.OrderBy = 
+00023ba0: 656e 756d 732e 4f72 6465 7242 792e 7365  enums.OrderBy.se
+00023bb0: 7269 6573 5f63 6f75 6e74 2c0d 0a20 2020  ries_count,..   
+00023bc0: 2020 2020 2020 2020 2073 6f72 745f 6f72           sort_or
+00023bd0: 6465 723a 2065 6e75 6d73 2e53 6f72 744f  der: enums.SortO
+00023be0: 7264 6572 203d 2065 6e75 6d73 2e53 6f72  rder = enums.Sor
+00023bf0: 744f 7264 6572 2e61 7363 0d0a 2020 2020  tOrder.asc..    
+00023c00: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
+00023c10: 653a 0d0a 2020 2020 2020 2020 2222 220d  e:..        """.
+00023c20: 0a20 2020 2020 2020 2023 2320 5061 7261  .        ## Para
+00023c30: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
+00023c40: 6072 6561 6c74 696d 655f 7374 6172 7460  `realtime_start`
+00023c50: 0d0a 2020 2020 2020 2020 5468 6520 7374  ..        The st
+00023c60: 6172 7420 6f66 2074 6865 2072 6561 6c2d  art of the real-
+00023c70: 7469 6d65 2070 6572 696f 642e 2046 6f72  time period. For
+00023c80: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+00023c90: 6e2c 2073 6565 205b 5265 616c 2d54 696d  n, see [Real-Tim
+00023ca0: 6520 5065 7269 6f64 735d 2868 7474 7073  e Periods](https
+00023cb0: 3a2f 2f66 7265 642e 7374 6c6f 7569 7366  ://fred.stlouisf
+00023cc0: 6564 2e6f 7267 2f64 6f63 732f 6170 692f  ed.org/docs/api/
+00023cd0: 6672 6564 2f72 6561 6c74 696d 655f 7065  fred/realtime_pe
+00023ce0: 7269 6f64 2e68 746d 6c29 2e0d 0a0d 0a20  riod.html)..... 
+00023cf0: 2020 2020 2020 2060 7265 616c 7469 6d65         `realtime
+00023d00: 5f65 6e64 600d 0a20 2020 2020 2020 2054  _end`..        T
+00023d10: 6865 2065 6e64 206f 6620 7468 6520 7265  he end of the re
+00023d20: 616c 2d74 696d 6520 7065 7269 6f64 2e20  al-time period. 
+00023d30: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
+00023d40: 7469 6f6e 2c20 7365 6520 5b52 6561 6c2d  tion, see [Real-
+00023d50: 5469 6d65 2050 6572 696f 6473 5d28 6874  Time Periods](ht
+00023d60: 7470 733a 2f2f 6672 6564 2e73 746c 6f75  tps://fred.stlou
+00023d70: 6973 6665 642e 6f72 672f 646f 6373 2f61  isfed.org/docs/a
+00023d80: 7069 2f66 7265 642f 7265 616c 7469 6d65  pi/fred/realtime
+00023d90: 5f70 6572 696f 642e 6874 6d6c 292e 0d0a  _period.html)...
+00023da0: 0d0a 2020 2020 2020 2020 6074 6167 5f6e  ..        `tag_n
+00023db0: 616d 6573 600d 0a20 2020 2020 2020 2054  ames`..        T
+00023dc0: 7570 6c65 206f 6620 7461 6720 6e61 6d65  uple of tag name
+00023dd0: 7320 7468 6174 2073 6572 6965 7320 6d61  s that series ma
+00023de0: 7463 6820 616c 6c20 6f66 2e0d 0a0d 0a20  tch all of..... 
+00023df0: 2020 2020 2020 2060 6578 636c 7564 655f         `exclude_
+00023e00: 7461 675f 6e61 6d65 7360 0d0a 2020 2020  tag_names`..    
+00023e10: 2020 2020 5475 706c 6520 6f66 2074 6167      Tuple of tag
+00023e20: 206e 616d 6573 2074 6861 7420 7365 7269   names that seri
+00023e30: 6573 206d 6174 6368 206e 6f6e 6520 6f66  es match none of
+00023e40: 2e0d 0a0d 0a20 2020 2020 2020 2060 7461  .....        `ta
+00023e50: 675f 6772 6f75 705f 6964 600d 0a20 2020  g_group_id`..   
+00023e60: 2020 2020 2041 2074 6167 2067 726f 7570       A tag group
+00023e70: 2069 6420 746f 2066 696c 7465 7220 7461   id to filter ta
+00023e80: 6773 2062 7920 7479 7065 2e0d 0a0d 0a20  gs by type..... 
+00023e90: 2020 2020 2020 2060 7365 6172 6368 5f74         `search_t
+00023ea0: 6578 7460 0d0a 2020 2020 2020 2020 5468  ext`..        Th
+00023eb0: 6520 776f 7264 7320 746f 2066 696e 6420  e words to find 
+00023ec0: 6d61 7463 6869 6e67 2074 6167 7320 7769  matching tags wi
+00023ed0: 7468 2e0d 0a0d 0a20 2020 2020 2020 2060  th.....        `
+00023ee0: 6f72 6465 725f 6279 600d 0a20 2020 2020  order_by`..     
+00023ef0: 2020 204f 7264 6572 2072 6573 756c 7473     Order results
+00023f00: 2062 7920 7661 6c75 6573 206f 6620 7468   by values of th
+00023f10: 6520 7370 6563 6966 6965 6420 6174 7472  e specified attr
+00023f20: 6962 7574 652e 0d0a 0d0a 2020 2020 2020  ibute.....      
+00023f30: 2020 6073 6f72 745f 6f72 6465 7260 0d0a    `sort_order`..
+00023f40: 2020 2020 2020 2020 536f 7274 2072 6573          Sort res
+00023f50: 756c 7473 2069 7320 6173 6365 6e64 696e  ults is ascendin
+00023f60: 6720 6f72 2064 6573 6365 6e64 696e 6720  g or descending 
+00023f70: 6f72 6465 7220 666f 7220 6174 7472 6962  order for attrib
+00023f80: 7574 6520 7661 6c75 6573 2073 7065 6369  ute values speci
+00023f90: 6669 6564 2062 7920 6f72 6465 725f 6279  fied by order_by
+00023fa0: 2e0d 0a0d 0a20 2020 2020 2020 2023 2320  .....        ## 
+00023fb0: 4465 7363 7269 7074 696f 6e0d 0a20 2020  Description..   
+00023fc0: 2020 2020 2068 7474 7073 3a2f 2f66 7265       https://fre
+00023fd0: 642e 7374 6c6f 7569 7366 6564 2e6f 7267  d.stlouisfed.org
+00023fe0: 2f64 6f63 732f 6170 692f 6672 6564 2f72  /docs/api/fred/r
+00023ff0: 656c 6174 6564 5f74 6167 732e 6874 6d6c  elated_tags.html
+00024000: 0d0a 0d0a 2020 2020 2020 2020 4765 7420  ....        Get 
+00024010: 7468 6520 7265 6c61 7465 6420 4652 4544  the related FRED
+00024020: 2074 6167 7320 666f 7220 6f6e 6520 6f72   tags for one or
+00024030: 206d 6f72 6520 4652 4544 2074 6167 732e   more FRED tags.
+00024040: 0d0a 2020 2020 2020 2020 4f70 7469 6f6e  ..        Option
+00024050: 616c 6c79 2c20 6669 6c74 6572 2072 6573  ally, filter res
+00024060: 756c 7473 2062 7920 7461 6720 6772 6f75  ults by tag grou
+00024070: 7020 6f72 2073 6561 7263 682e 0d0a 2020  p or search...  
+00024080: 2020 2020 2020 4652 4544 2074 6167 7320        FRED tags 
+00024090: 6172 6520 6174 7472 6962 7574 6573 2061  are attributes a
+000240a0: 7373 6967 6e65 6420 746f 2073 6572 6965  ssigned to serie
+000240b0: 732e 0d0a 2020 2020 2020 2020 5265 6c61  s...        Rela
+000240c0: 7465 6420 4652 4544 2074 6167 7320 6172  ted FRED tags ar
+000240d0: 6520 7468 6520 7461 6773 2061 7373 6967  e the tags assig
+000240e0: 6e65 6420 746f 2073 6572 6965 7320 7468  ned to series th
+000240f0: 6174 206d 6174 6368 2061 6c6c 2074 6167  at match all tag
+00024100: 7320 696e 2074 6865 2074 6167 5f6e 616d  s in the tag_nam
+00024110: 6573 2070 6172 616d 6574 6572 2061 6e64  es parameter and
+00024120: 206e 6f20 7461 6773 2069 6e20 7468 6520   no tags in the 
+00024130: 6578 636c 7564 655f 7461 675f 6e61 6d65  exclude_tag_name
+00024140: 7320 7061 7261 6d65 7465 722e 0d0a 2020  s parameter...  
+00024150: 2020 2020 2020 5365 6520 7468 6520 7265        See the re
+00024160: 6c61 7465 6420 7265 7175 6573 7420 6672  lated request fr
+00024170: 6564 2f74 6167 732e 0d0a 0d0a 2020 2020  ed/tags.....    
+00024180: 2020 2020 2323 2041 5049 2052 6571 7565      ## API Reque
+00024190: 7374 2028 4854 5450 5320 4745 5429 0d0a  st (HTTPS GET)..
+000241a0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+000241b0: 6170 692e 7374 6c6f 7569 7366 6564 2e6f  api.stlouisfed.o
+000241c0: 7267 2f66 7265 642f 7265 6c61 7465 645f  rg/fred/related_
+000241d0: 7461 6773 3f74 6167 5f6e 616d 6573 3d6d  tags?tag_names=m
+000241e0: 6f6e 6574 6172 792b 6167 6772 6567 6174  onetary+aggregat
+000241f0: 6573 3b77 6565 6b6c 7926 6170 695f 6b65  es;weekly&api_ke
+00024200: 793d 6162 6364 6566 6768 696a 6b6c 6d6e  y=abcdefghijklmn
+00024210: 6f70 7172 7374 7576 7778 797a 3132 3334  opqrstuvwxyz1234
+00024220: 3536 2666 696c 655f 7479 7065 3d6a 736f  56&file_type=jso
+00024230: 6e0d 0a0d 0a20 2020 2020 2020 2023 2320  n....        ## 
+00024240: 4150 4920 5265 7370 6f6e 7365 0d0a 2020  API Response..  
+00024250: 2020 2020 2020 6060 606a 736f 6e0d 0a20        ```json.. 
+00024260: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+00024270: 2020 2020 2020 2272 6561 6c74 696d 655f        "realtime_
+00024280: 7374 6172 7422 3a20 2232 3031 332d 3038  start": "2013-08
+00024290: 2d31 3422 2c0d 0a20 2020 2020 2020 2020  -14",..         
+000242a0: 2020 2022 7265 616c 7469 6d65 5f65 6e64     "realtime_end
+000242b0: 223a 2022 3230 3133 2d30 382d 3134 222c  ": "2013-08-14",
+000242c0: 0d0a 2020 2020 2020 2020 2020 2020 226f  ..            "o
+000242d0: 7264 6572 5f62 7922 3a20 2273 6572 6965  rder_by": "serie
+000242e0: 735f 636f 756e 7422 2c0d 0a20 2020 2020  s_count",..     
+000242f0: 2020 2020 2020 2022 736f 7274 5f6f 7264         "sort_ord
+00024300: 6572 223a 2022 6465 7363 222c 0d0a 2020  er": "desc",..  
+00024310: 2020 2020 2020 2020 2020 2263 6f75 6e74            "count
+00024320: 223a 2031 332c 0d0a 2020 2020 2020 2020  ": 13,..        
+00024330: 2020 2020 226f 6666 7365 7422 3a20 302c      "offset": 0,
+00024340: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
+00024350: 696d 6974 223a 2031 3030 302c 0d0a 2020  imit": 1000,..  
+00024360: 2020 2020 2020 2020 2020 2274 6167 7322            "tags"
+00024370: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
+00024380: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00024390: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+000243a0: 6522 3a20 226e 6174 696f 6e22 2c0d 0a20  e": "nation",.. 
+000243b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000243c0: 2020 2022 6772 6f75 705f 6964 223a 2022     "group_id": "
+000243d0: 6765 6f74 222c 0d0a 2020 2020 2020 2020  geot",..        
+000243e0: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
+000243f0: 6573 223a 2022 436f 756e 7472 7920 4c65  es": "Country Le
+00024400: 7665 6c22 2c0d 0a20 2020 2020 2020 2020  vel",..         
+00024410: 2020 2020 2020 2020 2020 2022 6372 6561             "crea
+00024420: 7465 6422 3a20 2232 3031 322d 3032 2d32  ted": "2012-02-2
+00024430: 3720 3130 3a31 383a 3139 2d30 3622 2c0d  7 10:18:19-06",.
+00024440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024450: 2020 2020 2022 706f 7075 6c61 7269 7479       "popularity
+00024460: 223a 2031 3030 2c0d 0a20 2020 2020 2020  ": 100,..       
+00024470: 2020 2020 2020 2020 2020 2020 2022 7365               "se
+00024480: 7269 6573 5f63 6f75 6e74 223a 2031 320d  ries_count": 12.
+00024490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000244a0: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
+000244b0: 2020 2020 202e 2e2e 0d0a 2020 2020 2020       .....      
+000244c0: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
+000244d0: 207d 0d0a 2020 2020 2020 2020 6060 600d   }..        ```.
+000244e0: 0a0d 0a20 2020 2020 2020 2023 2320 5265  ...        ## Re
+000244f0: 7475 726e 730d 0a20 2020 2020 2020 2060  turns..        `
+00024500: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+00024510: 600d 0a0d 0a20 2020 2020 2020 2023 2320  `....        ## 
+00024520: 4578 616d 706c 650d 0a20 2020 2020 2020  Example..       
+00024530: 2060 6060 7079 7468 6f6e 0d0a 2020 2020   ```python..    
+00024540: 2020 2020 3e3e 3e20 6672 6564 203d 2046      >>> fred = F
+00024550: 5245 4428 6170 695f 6b65 793d 2761 6263  RED(api_key='abc
+00024560: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
+00024570: 7475 7677 7879 7a31 3233 3435 3627 290d  tuvwxyz123456').
+00024580: 0a20 2020 2020 2020 203e 3e3e 2066 7265  .        >>> fre
+00024590: 642e 7265 6c61 7465 645f 7461 6773 2874  d.related_tags(t
+000245a0: 6167 5f6e 616d 6573 3d5b 276d 6f6e 6574  ag_names=['monet
+000245b0: 6172 7920 6167 6772 6567 6174 6573 272c  ary aggregates',
+000245c0: 2027 7765 656b 6c79 275d 292e 6865 6164   'weekly']).head
+000245d0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+000245e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000245f0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00024600: 726f 7570 5f69 6420 2020 2020 2020 2020  roup_id         
+00024610: 2020 6e6f 7465 7320 2020 2020 2020 2020    notes         
+00024620: 2020 2020 2020 2020 2020 6372 6561 7465            create
+00024630: 6420 2070 6f70 756c 6172 6974 7920 2073  d  popularity  s
+00024640: 6572 6965 735f 636f 756e 740d 0a20 2020  eries_count..   
+00024650: 2020 2020 2020 2020 206e 616d 650d 0a20           name.. 
+00024660: 2020 2020 2020 2020 2020 2063 6f70 7972             copyr
+00024670: 6967 6874 6564 3a20 6369 7461 7469 6f6e  ighted: citation
+00024680: 2072 6571 7569 7265 6420 2020 2020 2020   required       
+00024690: 6363 2020 2020 2020 2020 2020 2020 3c4e  cc            <N
+000246a0: 413e 2032 3031 382d 3132 2d31 3820 3035  A> 2018-12-18 05
+000246b0: 3a33 333a 3133 2b30 303a 3030 2020 2020  :33:13+00:00    
+000246c0: 2020 2020 2020 3838 2020 2020 2020 2020        88        
 000246d0: 2020 2020 2032 0d0a 2020 2020 2020 2020       2..        
-000246e0: 2020 2020 6d31 2020 2020 2020 2020 2020      m1          
+000246e0: 2020 2020 6375 7272 656e 6379 2020 2020      currency    
 000246f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024700: 2020 2020 2020 2020 6765 6e20 204d 3120          gen  M1 
-00024710: 4d6f 6e65 7920 5374 6f63 6b20 3230 3132  Money Stock 2012
+00024700: 2020 2020 2020 2020 6765 6e20 2020 2020          gen     
+00024710: 2020 2020 2020 2020 2020 2020 3230 3132              2012
 00024720: 2d30 322d 3237 2031 363a 3138 3a31 392b  -02-27 16:18:19+
-00024730: 3030 3a30 3020 2020 2020 2020 2020 2034  00:00          4
-00024740: 3720 2020 2020 2020 2020 2020 2020 320d  7             2.
-00024750: 0a20 2020 2020 2020 2020 2020 206d 3320  .            m3 
-00024760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024730: 3030 3a30 3020 2020 2020 2020 2020 2036  00:00          6
+00024740: 3220 2020 2020 2020 2020 2020 2020 320d  2             2.
+00024750: 0a20 2020 2020 2020 2020 2020 2066 7262  .            frb
+00024760: 2073 746c 2020 2020 2020 2020 2020 2020   stl            
 00024770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024780: 2067 656e 2020 4d33 204d 6f6e 6579 2053   gen  M3 Money S
-00024790: 746f 636b 2032 3031 322d 3032 2d32 3720  tock 2012-02-27 
+00024780: 2073 7263 2020 2053 742e 204c 6f75 6973   src   St. Louis
+00024790: 2046 6564 2032 3031 322d 3032 2d32 3720   Fed 2012-02-27 
 000247a0: 3136 3a31 383a 3139 2b30 303a 3030 2020  16:18:19+00:00  
-000247b0: 2020 2020 2020 2020 3339 2020 2020 2020          39      
+000247b0: 2020 2020 2020 2020 3638 2020 2020 2020          68      
 000247c0: 2020 2020 2020 2032 0d0a 2020 2020 2020         2..      
-000247d0: 2020 6060 600d 0a20 2020 2020 2020 2022    ```..        "
-000247e0: 2222 0d0a 0d0a 2020 2020 2020 2020 616c  ""....        al
-000247f0: 6c6f 7765 645f 6f72 6465 7273 203d 205b  lowed_orders = [
-00024800: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
-00024810: 756d 732e 4f72 6465 7242 792e 7365 7269  ums.OrderBy.seri
-00024820: 6573 5f63 6f75 6e74 2c0d 0a20 2020 2020  es_count,..     
-00024830: 2020 2020 2020 2065 6e75 6d73 2e4f 7264         enums.Ord
-00024840: 6572 4279 2e70 6f70 756c 6172 6974 792c  erBy.popularity,
-00024850: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
-00024860: 756d 732e 4f72 6465 7242 792e 6372 6561  ums.OrderBy.crea
-00024870: 7465 642c 0d0a 2020 2020 2020 2020 2020  ted,..          
-00024880: 2020 656e 756d 732e 4f72 6465 7242 792e    enums.OrderBy.
-00024890: 6e61 6d65 2c0d 0a20 2020 2020 2020 2020  name,..         
-000248a0: 2020 2065 6e75 6d73 2e4f 7264 6572 4279     enums.OrderBy
-000248b0: 2e67 726f 7570 5f69 640d 0a20 2020 2020  .group_id..     
-000248c0: 2020 205d 0d0a 0d0a 2020 2020 2020 2020     ]....        
-000248d0: 616c 6c6f 7765 645f 7461 675f 6772 6f75  allowed_tag_grou
-000248e0: 705f 6964 7320 3d20 5b0d 0a20 2020 2020  p_ids = [..     
-000248f0: 2020 2020 2020 2065 6e75 6d73 2e54 6167         enums.Tag
-00024900: 4772 6f75 7049 442e 6672 6571 7565 6e63  GroupID.frequenc
-00024910: 792c 0d0a 2020 2020 2020 2020 2020 2020  y,..            
-00024920: 656e 756d 732e 5461 6747 726f 7570 4944  enums.TagGroupID
-00024930: 2e67 656e 6572 616c 5f6f 725f 636f 6e63  .general_or_conc
-00024940: 6570 742c 0d0a 2020 2020 2020 2020 2020  ept,..          
-00024950: 2020 656e 756d 732e 5461 6747 726f 7570    enums.TagGroup
-00024960: 4944 2e67 656f 6772 6170 6879 2c0d 0a20  ID.geography,.. 
-00024970: 2020 2020 2020 2020 2020 2065 6e75 6d73             enums
-00024980: 2e54 6167 4772 6f75 7049 442e 6765 6f67  .TagGroupID.geog
-00024990: 7261 7068 795f 7479 7065 2c0d 0a20 2020  raphy_type,..   
-000249a0: 2020 2020 2020 2020 2065 6e75 6d73 2e54           enums.T
-000249b0: 6167 4772 6f75 7049 442e 7265 6c65 6173  agGroupID.releas
-000249c0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000249d0: 656e 756d 732e 5461 6747 726f 7570 4944  enums.TagGroupID
-000249e0: 2e73 6561 736f 6e61 6c5f 6164 6a75 7374  .seasonal_adjust
-000249f0: 6d65 6e74 2c0d 0a20 2020 2020 2020 2020  ment,..         
-00024a00: 2020 2065 6e75 6d73 2e54 6167 4772 6f75     enums.TagGrou
-00024a10: 7049 442e 736f 7572 6365 0d0a 2020 2020  pID.source..    
-00024a20: 2020 2020 5d0d 0a0d 0a20 2020 2020 2020      ]....       
-00024a30: 2069 6620 6f72 6465 725f 6279 206e 6f74   if order_by not
-00024a40: 2069 6e20 616c 6c6f 7765 645f 6f72 6465   in allowed_orde
-00024a50: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
-00024a60: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00024a70: 7228 2756 6172 6961 626c 6520 6f72 6465  r('Variable orde
-00024a80: 725f 6279 2028 7b7d 2920 6973 206e 6f74  r_by ({}) is not
-00024a90: 206f 6e65 206f 6620 7468 6520 7661 6c75   one of the valu
-00024aa0: 6573 3a20 7b7d 272e 666f 726d 6174 286f  es: {}'.format(o
-00024ab0: 7264 6572 5f62 792c 2027 2c20 272e 6a6f  rder_by, ', '.jo
-00024ac0: 696e 286d 6170 2873 7472 2c20 616c 6c6f  in(map(str, allo
-00024ad0: 7765 645f 6f72 6465 7273 2929 2929 0d0a  wed_orders))))..
-00024ae0: 0d0a 2020 2020 2020 2020 6966 2074 6167  ..        if tag
-00024af0: 5f67 726f 7570 5f69 6420 6973 206e 6f74  _group_id is not
-00024b00: 204e 6f6e 6520 616e 6420 7461 675f 6772   None and tag_gr
-00024b10: 6f75 705f 6964 206e 6f74 2069 6e20 616c  oup_id not in al
-00024b20: 6c6f 7765 645f 7461 675f 6772 6f75 705f  lowed_tag_group_
-00024b30: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
-00024b40: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00024b50: 6f72 2827 5661 7269 6162 6c65 2074 6167  or('Variable tag
-00024b60: 5f67 726f 7570 5f69 6420 287b 7d29 2069  _group_id ({}) i
-00024b70: 7320 6e6f 7420 6f6e 6520 6f66 2074 6865  s not one of the
-00024b80: 2076 616c 7565 733a 207b 7d27 2e66 6f72   values: {}'.for
-00024b90: 6d61 7428 7461 675f 6772 6f75 705f 6964  mat(tag_group_id
-00024ba0: 2c20 272c 2027 2e6a 6f69 6e28 6d61 7028  , ', '.join(map(
-00024bb0: 7374 722c 2061 6c6c 6f77 6564 5f74 6167  str, allowed_tag
-00024bc0: 5f67 726f 7570 5f69 6473 2929 2929 0d0a  _group_ids))))..
-00024bd0: 0d0a 2020 2020 2020 2020 6966 2072 6561  ..        if rea
-00024be0: 6c74 696d 655f 7374 6172 7420 6973 206e  ltime_start is n
-00024bf0: 6f74 204e 6f6e 6520 616e 6420 7265 616c  ot None and real
-00024c00: 7469 6d65 5f73 7461 7274 203c 2064 6174  time_start < dat
-00024c10: 6528 3137 3736 2c20 372c 2034 293a 0d0a  e(1776, 7, 4):..
-00024c20: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00024c30: 6520 5661 6c75 6545 7272 6f72 2827 5661  e ValueError('Va
-00024c40: 7269 6162 6c65 2072 6561 6c74 696d 655f  riable realtime_
-00024c50: 7374 6172 7420 2822 7b7d 2229 2069 7320  start ("{}") is 
-00024c60: 6265 666f 7265 206d 696e 2064 6174 6520  before min date 
-00024c70: 3137 3736 2d30 372d 3034 2e27 2e66 6f72  1776-07-04.'.for
-00024c80: 6d61 7428 7265 616c 7469 6d65 5f73 7461  mat(realtime_sta
-00024c90: 7274 2929 0d0a 0d0a 2020 2020 2020 2020  rt))....        
-00024ca0: 6966 2072 6561 6c74 696d 655f 7374 6172  if realtime_star
-00024cb0: 7420 6973 206e 6f74 204e 6f6e 6520 616e  t is not None an
-00024cc0: 6420 7265 616c 7469 6d65 5f65 6e64 2069  d realtime_end i
-00024cd0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2072  s not None and r
-00024ce0: 6561 6c74 696d 655f 7374 6172 7420 3e20  ealtime_start > 
-00024cf0: 7265 616c 7469 6d65 5f65 6e64 3a0d 0a20  realtime_end:.. 
-00024d00: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00024d10: 2056 616c 7565 4572 726f 7228 2754 6865   ValueError('The
-00024d20: 2064 6174 6520 7365 7420 6279 2076 6172   date set by var
-00024d30: 6961 626c 6520 7265 616c 7469 6d65 5f73  iable realtime_s
-00024d40: 7461 7274 2028 227b 7d22 2920 6361 6e20  tart ("{}") can 
-00024d50: 6e6f 7420 6265 2061 6674 6572 2074 6865  not be after the
-00024d60: 2064 6174 6520 7365 7420 6279 2076 6172   date set by var
-00024d70: 6961 626c 6520 7265 616c 7469 6d65 5f65  iable realtime_e
-00024d80: 6e64 2028 227b 7d22 292e 272e 666f 726d  nd ("{}").'.form
-00024d90: 6174 2872 6561 6c74 696d 655f 7374 6172  at(realtime_star
-00024da0: 742c 2072 6561 6c74 696d 655f 656e 6429  t, realtime_end)
-00024db0: 290d 0a0d 0a20 2020 2020 2020 2064 6620  )....        df 
-00024dc0: 3d20 7064 2e44 6174 6146 7261 6d65 280d  = pd.DataFrame(.
-00024dd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00024de0: 662e 5f63 6c69 656e 742e 6765 7428 0d0a  f._client.get(..
-00024df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e00: 272f 6672 6564 2f72 656c 6174 6564 5f74  '/fred/related_t
-00024e10: 6167 7327 2c0d 0a20 2020 2020 2020 2020  ags',..         
-00024e20: 2020 2020 2020 2027 7461 6773 272c 0d0a         'tags',..
-00024e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e40: 6c69 6d69 743d 3130 3030 2c0d 0a20 2020  limit=1000,..   
-00024e50: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00024e60: 6c74 696d 655f 7374 6172 743d 7265 616c  ltime_start=real
-00024e70: 7469 6d65 5f73 7461 7274 2c0d 0a20 2020  time_start,..   
-00024e80: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00024e90: 6c74 696d 655f 656e 643d 7265 616c 7469  ltime_end=realti
-00024ea0: 6d65 5f65 6e64 2c0d 0a20 2020 2020 2020  me_end,..       
-00024eb0: 2020 2020 2020 2020 2074 6167 5f6e 616d           tag_nam
-00024ec0: 6573 3d74 6167 5f6e 616d 6573 2c0d 0a20  es=tag_names,.. 
-00024ed0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00024ee0: 7863 6c75 6465 5f74 6167 5f6e 616d 6573  xclude_tag_names
-00024ef0: 3d65 7863 6c75 6465 5f74 6167 5f6e 616d  =exclude_tag_nam
-00024f00: 6573 2c0d 0a20 2020 2020 2020 2020 2020  es,..           
-00024f10: 2020 2020 2074 6167 5f67 726f 7570 5f69       tag_group_i
-00024f20: 643d 7461 675f 6772 6f75 705f 6964 2c0d  d=tag_group_id,.
-00024f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024f40: 2073 6561 7263 685f 7465 7874 3d73 6561   search_text=sea
-00024f50: 7263 685f 7465 7874 2c0d 0a20 2020 2020  rch_text,..     
-00024f60: 2020 2020 2020 2020 2020 206f 7264 6572             order
-00024f70: 5f62 793d 6f72 6465 725f 6279 2c0d 0a20  _by=order_by,.. 
-00024f80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00024f90: 6f72 745f 6f72 6465 723d 736f 7274 5f6f  ort_order=sort_o
-00024fa0: 7264 6572 0d0a 2020 2020 2020 2020 2020  rder..          
-00024fb0: 2020 290d 0a20 2020 2020 2020 2029 0d0a    )..        )..
-00024fc0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00024fd0: 2064 662e 656d 7074 793a 0d0a 2020 2020   df.empty:..    
-00024fe0: 2020 2020 2020 2020 6466 2e63 7265 6174          df.creat
-00024ff0: 6564 203d 2070 642e 746f 5f64 6174 6574  ed = pd.to_datet
-00025000: 696d 6528 6466 2e63 7265 6174 6564 202b  ime(df.created +
-00025010: 2027 3030 272c 2075 7463 3d54 7275 652c   '00', utc=True,
-00025020: 2066 6f72 6d61 743d 2725 592d 256d 2d25   format='%Y-%m-%
-00025030: 6420 2548 3a25 4d3a 2553 257a 2729 0d0a  d %H:%M:%S%z')..
-00025040: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-00025050: 203d 2064 662e 6173 7479 7065 2864 7479   = df.astype(dty
-00025060: 7065 3d7b 0d0a 2020 2020 2020 2020 2020  pe={..          
-00025070: 2020 2020 2020 276e 616d 6527 3a20 2773        'name': 's
-00025080: 7472 696e 6727 2c0d 0a20 2020 2020 2020  tring',..       
-00025090: 2020 2020 2020 2020 2027 6e6f 7465 7327           'notes'
-000250a0: 3a20 2773 7472 696e 6727 2c0d 0a20 2020  : 'string',..   
-000250b0: 2020 2020 2020 2020 2020 2020 2027 6772               'gr
-000250c0: 6f75 705f 6964 273a 2027 6361 7465 676f  oup_id': 'catego
-000250d0: 7279 270d 0a20 2020 2020 2020 2020 2020  ry'..           
-000250e0: 207d 292e 7365 745f 696e 6465 7828 276e   }).set_index('n
-000250f0: 616d 6527 290d 0a0d 0a20 2020 2020 2020  ame')....       
-00025100: 2072 6574 7572 6e20 6466 0d0a 0d0a 2020   return df....  
-00025110: 2020 6465 6620 7461 6773 5f73 6572 6965    def tags_serie
-00025120: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-00025130: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-00025140: 2020 2074 6167 5f6e 616d 6573 3a20 4c69     tag_names: Li
-00025150: 7374 5b73 7472 5d20 3d20 4e6f 6e65 2c0d  st[str] = None,.
-00025160: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-00025170: 6c75 6465 5f74 6167 5f6e 616d 6573 3a20  lude_tag_names: 
-00025180: 4c69 7374 5b73 7472 5d20 3d20 4e6f 6e65  List[str] = None
-00025190: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-000251a0: 6561 6c74 696d 655f 7374 6172 743a 2064  ealtime_start: d
-000251b0: 6174 6520 3d20 4e6f 6e65 2c0d 0a20 2020  ate = None,..   
-000251c0: 2020 2020 2020 2020 2072 6561 6c74 696d           realtim
-000251d0: 655f 656e 643a 2064 6174 6520 3d20 4e6f  e_end: date = No
-000251e0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-000251f0: 206f 7264 6572 5f62 793a 2065 6e75 6d73   order_by: enums
-00025200: 2e4f 7264 6572 4279 203d 2065 6e75 6d73  .OrderBy = enums
-00025210: 2e4f 7264 6572 4279 2e73 6572 6965 735f  .OrderBy.series_
-00025220: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
-00025230: 2073 6f72 745f 6f72 6465 723a 2065 6e75   sort_order: enu
-00025240: 6d73 2e53 6f72 744f 7264 6572 203d 2065  ms.SortOrder = e
-00025250: 6e75 6d73 2e53 6f72 744f 7264 6572 2e61  nums.SortOrder.a
-00025260: 7363 0d0a 2020 2020 2920 2d3e 2070 642e  sc..    ) -> pd.
-00025270: 4461 7461 4672 616d 653a 0d0a 2020 2020  DataFrame:..    
-00025280: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00025290: 2023 2320 5061 7261 6d65 7465 7273 0d0a   ## Parameters..
-000252a0: 0d0a 2020 2020 2020 2020 6074 6167 5f6e  ..        `tag_n
-000252b0: 616d 6573 600d 0a20 2020 2020 2020 2054  ames`..        T
-000252c0: 7570 6c65 206f 6620 7461 6720 6e61 6d65  uple of tag name
-000252d0: 7320 7468 6174 2073 6572 6965 7320 6d61  s that series ma
-000252e0: 7463 6820 616c 6c20 6f66 2e0d 0a0d 0a20  tch all of..... 
-000252f0: 2020 2020 2020 2060 6578 636c 7564 655f         `exclude_
-00025300: 7461 675f 6e61 6d65 7360 0d0a 2020 2020  tag_names`..    
-00025310: 2020 2020 5475 706c 6520 6f66 2074 6167      Tuple of tag
-00025320: 206e 616d 6573 2074 6861 7420 7365 7269   names that seri
-00025330: 6573 206d 6174 6368 206e 6f6e 6520 6f66  es match none of
-00025340: 2e0d 0a0d 0a20 2020 2020 2020 2060 7265  .....        `re
-00025350: 616c 7469 6d65 5f73 7461 7274 600d 0a20  altime_start`.. 
-00025360: 2020 2020 2020 2054 6865 2073 7461 7274         The start
-00025370: 206f 6620 7468 6520 7265 616c 2d74 696d   of the real-tim
-00025380: 6520 7065 7269 6f64 2e20 466f 7220 6d6f  e period. For mo
-00025390: 7265 2069 6e66 6f72 6d61 7469 6f6e 2c20  re information, 
-000253a0: 7365 6520 5b52 6561 6c2d 5469 6d65 2050  see [Real-Time P
-000253b0: 6572 696f 6473 5d28 6874 7470 733a 2f2f  eriods](https://
-000253c0: 6672 6564 2e73 746c 6f75 6973 6665 642e  fred.stlouisfed.
-000253d0: 6f72 672f 646f 6373 2f61 7069 2f66 7265  org/docs/api/fre
-000253e0: 642f 7265 616c 7469 6d65 5f70 6572 696f  d/realtime_perio
-000253f0: 642e 6874 6d6c 292e 0d0a 0d0a 2020 2020  d.html).....    
-00025400: 2020 2020 6072 6561 6c74 696d 655f 656e      `realtime_en
-00025410: 6460 0d0a 2020 2020 2020 2020 5468 6520  d`..        The 
-00025420: 656e 6420 6f66 2074 6865 2072 6561 6c2d  end of the real-
-00025430: 7469 6d65 2070 6572 696f 642e 2046 6f72  time period. For
-00025440: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00025450: 6e2c 2073 6565 205b 5265 616c 2d54 696d  n, see [Real-Tim
-00025460: 6520 5065 7269 6f64 735d 2868 7474 7073  e Periods](https
-00025470: 3a2f 2f66 7265 642e 7374 6c6f 7569 7366  ://fred.stlouisf
-00025480: 6564 2e6f 7267 2f64 6f63 732f 6170 692f  ed.org/docs/api/
-00025490: 6672 6564 2f72 6561 6c74 696d 655f 7065  fred/realtime_pe
-000254a0: 7269 6f64 2e68 746d 6c29 2e0d 0a0d 0a20  riod.html)..... 
-000254b0: 2020 2020 2020 2060 6f72 6465 725f 6279         `order_by
-000254c0: 600d 0a20 2020 2020 2020 204f 7264 6572  `..        Order
-000254d0: 2072 6573 756c 7473 2062 7920 7661 6c75   results by valu
-000254e0: 6573 206f 6620 7468 6520 7370 6563 6966  es of the specif
-000254f0: 6965 6420 6174 7472 6962 7574 652e 0d0a  ied attribute...
-00025500: 0d0a 2020 2020 2020 2020 6073 6f72 745f  ..        `sort_
-00025510: 6f72 6465 7260 0d0a 2020 2020 2020 2020  order`..        
-00025520: 536f 7274 2072 6573 756c 7473 2069 7320  Sort results is 
-00025530: 6173 6365 6e64 696e 6720 6f72 2064 6573  ascending or des
-00025540: 6365 6e64 696e 6720 6f72 6465 7220 666f  cending order fo
-00025550: 7220 6174 7472 6962 7574 6520 7661 6c75  r attribute valu
-00025560: 6573 2073 7065 6369 6669 6564 2062 7920  es specified by 
-00025570: 6f72 6465 725f 6279 2e0d 0a0d 0a20 2020  order_by.....   
-00025580: 2020 2020 2023 2320 4465 7363 7269 7074       ## Descript
-00025590: 696f 6e0d 0a20 2020 2020 2020 2068 7474  ion..        htt
-000255a0: 7073 3a2f 2f66 7265 642e 7374 6c6f 7569  ps://fred.stloui
-000255b0: 7366 6564 2e6f 7267 2f64 6f63 732f 6170  sfed.org/docs/ap
-000255c0: 692f 6672 6564 2f74 6167 735f 7365 7269  i/fred/tags_seri
-000255d0: 6573 2e68 746d 6c0d 0a0d 0a20 2020 2020  es.html....     
-000255e0: 2020 2047 6574 2074 6865 2073 6572 6965     Get the serie
-000255f0: 7320 6d61 7463 6869 6e67 2061 6c6c 2074  s matching all t
-00025600: 6167 7320 696e 2074 6865 2074 6167 5f6e  ags in the tag_n
-00025610: 616d 6573 2070 6172 616d 6574 6572 2061  ames parameter a
-00025620: 6e64 206e 6f20 7461 6773 2069 6e20 7468  nd no tags in th
-00025630: 6520 6578 636c 7564 655f 7461 675f 6e61  e exclude_tag_na
-00025640: 6d65 7320 7061 7261 6d65 7465 722e 0d0a  mes parameter...
-00025650: 0d0a 2020 2020 2020 2020 2323 2041 5049  ..        ## API
-00025660: 2052 6571 7565 7374 2028 4854 5450 5320   Request (HTTPS 
-00025670: 4745 5429 0d0a 2020 2020 2020 2020 6874  GET)..        ht
-00025680: 7470 733a 2f2f 6170 692e 7374 6c6f 7569  tps://api.stloui
-00025690: 7366 6564 2e6f 7267 2f66 7265 642f 7461  sfed.org/fred/ta
-000256a0: 6773 2f73 6572 6965 733f 7461 675f 6e61  gs/series?tag_na
-000256b0: 6d65 733d 736c 6f76 656e 6961 3b66 6f6f  mes=slovenia;foo
-000256c0: 643b 6f65 6364 2661 7069 5f6b 6579 3d61  d;oecd&api_key=a
-000256d0: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
-000256e0: 7273 7475 7677 7879 7a31 3233 3435 3626  rstuvwxyz123456&
-000256f0: 6669 6c65 5f74 7970 653d 6a73 6f6e 0d0a  file_type=json..
-00025700: 0d0a 2020 2020 2020 2020 2323 2041 5049  ..        ## API
-00025710: 2052 6573 706f 6e73 650d 0a20 2020 2020   Response..     
-00025720: 2020 2060 6060 6a73 6f6e 0d0a 2020 2020     ```json..    
-00025730: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00025740: 2022 7265 616c 7469 6d65 5f73 7461 7274   "realtime_start
-00025750: 223a 2022 3230 3137 2d30 382d 3031 222c  ": "2017-08-01",
-00025760: 0d0a 2020 2020 2020 2020 2020 2272 6561  ..          "rea
-00025770: 6c74 696d 655f 656e 6422 3a20 2232 3031  ltime_end": "201
-00025780: 372d 3038 2d30 3122 2c0d 0a20 2020 2020  7-08-01",..     
-00025790: 2020 2020 2022 6f72 6465 725f 6279 223a       "order_by":
-000257a0: 2022 7365 7269 6573 5f69 6422 2c0d 0a20   "series_id",.. 
-000257b0: 2020 2020 2020 2020 2022 736f 7274 5f6f           "sort_o
-000257c0: 7264 6572 223a 2022 6173 6322 2c0d 0a20  rder": "asc",.. 
-000257d0: 2020 2020 2020 2020 2022 636f 756e 7422           "count"
-000257e0: 3a20 3138 2c0d 0a20 2020 2020 2020 2020  : 18,..         
-000257f0: 2022 6f66 6673 6574 223a 2030 2c0d 0a20   "offset": 0,.. 
-00025800: 2020 2020 2020 2020 2022 6c69 6d69 7422           "limit"
-00025810: 3a20 3130 3030 2c0d 0a20 2020 2020 2020  : 1000,..       
-00025820: 2020 2022 7365 7269 6573 7322 3a20 5b0d     "seriess": [.
-00025830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025840: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00025850: 2020 2020 2020 2269 6422 3a20 2243 5047        "id": "CPG
-00025860: 4446 4430 3253 4941 3635 374e 222c 0d0a  DFD02SIA657N",..
-00025870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025880: 2020 2272 6561 6c74 696d 655f 7374 6172    "realtime_star
-00025890: 7422 3a20 2232 3031 372d 3038 2d30 3122  t": "2017-08-01"
-000258a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000258b0: 2020 2020 2022 7265 616c 7469 6d65 5f65       "realtime_e
-000258c0: 6e64 223a 2022 3230 3137 2d30 382d 3031  nd": "2017-08-01
-000258d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000258e0: 2020 2020 2020 2274 6974 6c65 223a 2022        "title": "
-000258f0: 436f 6e73 756d 6572 2050 7269 6365 2049  Consumer Price I
-00025900: 6e64 6578 3a20 546f 7461 6c20 466f 6f64  ndex: Total Food
-00025910: 2045 7863 6c75 6469 6e67 2052 6573 7461   Excluding Resta
-00025920: 7572 616e 7473 2066 6f72 2053 6c6f 7665  urants for Slove
-00025930: 6e69 615c 7530 3061 3922 2c0d 0a20 2020  nia\u00a9",..   
-00025940: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00025950: 6f62 7365 7276 6174 696f 6e5f 7374 6172  observation_star
-00025960: 7422 3a20 2231 3939 362d 3031 2d30 3122  t": "1996-01-01"
-00025970: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00025980: 2020 2020 2022 6f62 7365 7276 6174 696f       "observatio
-00025990: 6e5f 656e 6422 3a20 2232 3031 362d 3031  n_end": "2016-01
-000259a0: 2d30 3122 2c0d 0a20 2020 2020 2020 2020  -01",..         
-000259b0: 2020 2020 2020 2020 2022 6672 6571 7565           "freque
-000259c0: 6e63 7922 3a20 2241 6e6e 7561 6c22 2c0d  ncy": "Annual",.
-000259d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000259e0: 2020 2022 6672 6571 7565 6e63 795f 7368     "frequency_sh
-000259f0: 6f72 7422 3a20 2241 222c 0d0a 2020 2020  ort": "A",..    
-00025a00: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00025a10: 6e69 7473 223a 2022 4772 6f77 7468 2052  nits": "Growth R
-00025a20: 6174 6520 5072 6576 696f 7573 2050 6572  ate Previous Per
-00025a30: 696f 6422 2c0d 0a20 2020 2020 2020 2020  iod",..         
-00025a40: 2020 2020 2020 2020 2022 756e 6974 735f           "units_
-00025a50: 7368 6f72 7422 3a20 2247 726f 7774 6820  short": "Growth 
-00025a60: 5261 7465 2050 7265 7669 6f75 7320 5065  Rate Previous Pe
-00025a70: 7269 6f64 222c 0d0a 2020 2020 2020 2020  riod",..        
-00025a80: 2020 2020 2020 2020 2020 2273 6561 736f            "seaso
-00025a90: 6e61 6c5f 6164 6a75 7374 6d65 6e74 223a  nal_adjustment":
-00025aa0: 2022 4e6f 7420 5365 6173 6f6e 616c 6c79   "Not Seasonally
-00025ab0: 2041 646a 7573 7465 6422 2c0d 0a20 2020   Adjusted",..   
-00025ac0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00025ad0: 7365 6173 6f6e 616c 5f61 646a 7573 746d  seasonal_adjustm
-00025ae0: 656e 745f 7368 6f72 7422 3a20 224e 5341  ent_short": "NSA
-00025af0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00025b00: 2020 2020 2020 226c 6173 745f 7570 6461        "last_upda
-00025b10: 7465 6422 3a20 2232 3031 372d 3034 2d32  ted": "2017-04-2
-00025b20: 3020 3030 3a34 383a 3335 2d30 3522 2c0d  0 00:48:35-05",.
-00025b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025b40: 2020 2022 706f 7075 6c61 7269 7479 223a     "popularity":
-00025b50: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
-00025b60: 2020 2020 2020 2022 6772 6f75 705f 706f         "group_po
-00025b70: 7075 6c61 7269 7479 223a 2030 2c0d 0a20  pularity": 0,.. 
-00025b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b90: 2022 6e6f 7465 7322 3a20 224f 4543 4420   "notes": "OECD 
-00025ba0: 6465 7363 7269 7074 6f72 2049 443a 2043  descriptor ID: C
-00025bb0: 5047 4446 4430 325c 5c6e 4f45 4344 2075  PGDFD02\\nOECD u
-00025bc0: 6e69 7420 4944 3a20 4750 5c5c 6e4f 4543  nit ID: GP\\nOEC
-00025bd0: 4420 636f 756e 7472 7920 4944 3a20 5356  D country ID: SV
-00025be0: 4e5c 5c6e 5c5c 6e41 6c6c 204f 4543 4420  N\\n\\nAll OECD 
-00025bf0: 6461 7461 2073 686f 756c 6420 6265 2063  data should be c
-00025c00: 6974 6564 2061 7320 666f 6c6c 6f77 733a  ited as follows:
-00025c10: 204f 4543 442c 205c 5c22 4d61 696e 2045   OECD, \\"Main E
-00025c20: 636f 6e6f 6d69 6320 496e 6469 6361 746f  conomic Indicato
-00025c30: 7273 202d 2063 6f6d 706c 6574 6520 6461  rs - complete da
-00025c40: 7461 6261 7365 5c5c 222c 204d 6169 6e20  tabase\\", Main 
-00025c50: 4563 6f6e 6f6d 6963 2049 6e64 6963 6174  Economic Indicat
-00025c60: 6f72 7320 2864 6174 6162 6173 6529 2c68  ors (database),h
-00025c70: 7474 703a 2f2f 6478 2e64 6f69 2e6f 7267  ttp://dx.doi.org
-00025c80: 2f31 302e 3137 3837 2f64 6174 612d 3030  /10.1787/data-00
-00025c90: 3035 322d 656e 2028 4163 6365 7373 6564  052-en (Accessed
-00025ca0: 206f 6e20 6461 7465 295c 5c6e 436f 7079   on date)\\nCopy
-00025cb0: 7269 6768 742c 2032 3031 362c 204f 4543  right, 2016, OEC
-00025cc0: 442e 2052 6570 7269 6e74 6564 2077 6974  D. Reprinted wit
-00025cd0: 6820 7065 726d 6973 7369 6f6e 2e22 0d0a  h permission."..
-00025ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025cf0: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00025d00: 2020 2020 2e2e 2e0d 0a20 2020 2020 2020      .....       
-00025d10: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-00025d20: 7d0d 0a20 2020 2020 2020 2060 6060 0d0a  }..        ```..
-00025d30: 0d0a 2020 2020 2020 2020 2323 2052 6574  ..        ## Ret
-00025d40: 7572 6e73 0d0a 2020 2020 2020 2020 6070  urns..        `p
-00025d50: 616e 6461 732e 4461 7461 4672 616d 6560  andas.DataFrame`
-00025d60: 0d0a 0d0a 2020 2020 2020 2020 2323 2045  ....        ## E
-00025d70: 7861 6d70 6c65 0d0a 2020 2020 2020 2020  xample..        
-00025d80: 6060 6070 7974 686f 6e0d 0a20 2020 2020  ```python..     
-00025d90: 2020 203e 3e3e 2066 7265 6420 3d20 4652     >>> fred = FR
-00025da0: 4544 2861 7069 5f6b 6579 3d27 6162 6364  ED(api_key='abcd
-00025db0: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
-00025dc0: 7576 7778 797a 3132 3334 3536 2729 0d0a  uvwxyz123456')..
-00025dd0: 2020 2020 2020 2020 3e3e 3e20 6672 6564          >>> fred
-00025de0: 2e74 6167 735f 7365 7269 6573 2874 6167  .tags_series(tag
-00025df0: 5f6e 616d 6573 3d5b 2766 6f6f 6427 2c20  _names=['food', 
-00025e00: 276f 6563 6427 5d29 2e68 6561 6428 290d  'oecd']).head().
-00025e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025e20: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00025e30: 6c74 696d 655f 7374 6172 7420 7265 616c  ltime_start real
-00025e40: 7469 6d65 5f65 6e64 2020 2020 2020 2020  time_end        
-00025e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025e70: 2020 2020 2020 7469 746c 6520 6f62 7365        title obse
-00025e80: 7276 6174 696f 6e5f 7374 6172 7420 6f62  rvation_start ob
-00025e90: 7365 7276 6174 696f 6e5f 656e 6420 2066  servation_end  f
-00025ea0: 7265 7175 656e 6379 2066 7265 7175 656e  requency frequen
-00025eb0: 6379 5f73 686f 7274 2020 2020 2020 2020  cy_short        
-00025ec0: 2020 2075 6e69 7473 2020 2020 2075 6e69     units     uni
-00025ed0: 7473 5f73 686f 7274 2020 2020 2020 7365  ts_short      se
-00025ee0: 6173 6f6e 616c 5f61 646a 7573 746d 656e  asonal_adjustmen
-00025ef0: 7420 7365 6173 6f6e 616c 5f61 646a 7573  t seasonal_adjus
-00025f00: 746d 656e 745f 7368 6f72 7420 2020 2020  tment_short     
-00025f10: 2020 2020 2020 2020 206c 6173 745f 7570           last_up
-00025f20: 6461 7465 6420 2070 6f70 756c 6172 6974  dated  popularit
-00025f30: 7920 2067 726f 7570 5f70 6f70 756c 6172  y  group_popular
-00025f40: 6974 7920 2020 2020 2020 2020 2020 2020  ity             
+000247d0: 2020 2020 2020 6d31 2020 2020 2020 2020        m1        
+000247e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000247f0: 2020 2020 2020 2020 2020 6765 6e20 204d            gen  M
+00024800: 3120 4d6f 6e65 7920 5374 6f63 6b20 3230  1 Money Stock 20
+00024810: 3132 2d30 322d 3237 2031 363a 3138 3a31  12-02-27 16:18:1
+00024820: 392b 3030 3a30 3020 2020 2020 2020 2020  9+00:00         
+00024830: 2034 3720 2020 2020 2020 2020 2020 2020   47             
+00024840: 320d 0a20 2020 2020 2020 2020 2020 206d  2..            m
+00024850: 3320 2020 2020 2020 2020 2020 2020 2020  3               
+00024860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024870: 2020 2067 656e 2020 4d33 204d 6f6e 6579     gen  M3 Money
+00024880: 2053 746f 636b 2032 3031 322d 3032 2d32   Stock 2012-02-2
+00024890: 3720 3136 3a31 383a 3139 2b30 303a 3030  7 16:18:19+00:00
+000248a0: 2020 2020 2020 2020 2020 3339 2020 2020            39    
+000248b0: 2020 2020 2020 2020 2032 0d0a 2020 2020           2..    
+000248c0: 2020 2020 6060 600d 0a20 2020 2020 2020      ```..       
+000248d0: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
+000248e0: 616c 6c6f 7765 645f 6f72 6465 7273 203d  allowed_orders =
+000248f0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+00024900: 656e 756d 732e 4f72 6465 7242 792e 7365  enums.OrderBy.se
+00024910: 7269 6573 5f63 6f75 6e74 2c0d 0a20 2020  ries_count,..   
+00024920: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
+00024930: 7264 6572 4279 2e70 6f70 756c 6172 6974  rderBy.popularit
+00024940: 792c 0d0a 2020 2020 2020 2020 2020 2020  y,..            
+00024950: 656e 756d 732e 4f72 6465 7242 792e 6372  enums.OrderBy.cr
+00024960: 6561 7465 642c 0d0a 2020 2020 2020 2020  eated,..        
+00024970: 2020 2020 656e 756d 732e 4f72 6465 7242      enums.OrderB
+00024980: 792e 6e61 6d65 2c0d 0a20 2020 2020 2020  y.name,..       
+00024990: 2020 2020 2065 6e75 6d73 2e4f 7264 6572       enums.Order
+000249a0: 4279 2e67 726f 7570 5f69 640d 0a20 2020  By.group_id..   
+000249b0: 2020 2020 205d 0d0a 0d0a 2020 2020 2020       ]....      
+000249c0: 2020 616c 6c6f 7765 645f 7461 675f 6772    allowed_tag_gr
+000249d0: 6f75 705f 6964 7320 3d20 5b0d 0a20 2020  oup_ids = [..   
+000249e0: 2020 2020 2020 2020 2065 6e75 6d73 2e54           enums.T
+000249f0: 6167 4772 6f75 7049 442e 6672 6571 7565  agGroupID.freque
+00024a00: 6e63 792c 0d0a 2020 2020 2020 2020 2020  ncy,..          
+00024a10: 2020 656e 756d 732e 5461 6747 726f 7570    enums.TagGroup
+00024a20: 4944 2e67 656e 6572 616c 5f6f 725f 636f  ID.general_or_co
+00024a30: 6e63 6570 742c 0d0a 2020 2020 2020 2020  ncept,..        
+00024a40: 2020 2020 656e 756d 732e 5461 6747 726f      enums.TagGro
+00024a50: 7570 4944 2e67 656f 6772 6170 6879 2c0d  upID.geography,.
+00024a60: 0a20 2020 2020 2020 2020 2020 2065 6e75  .            enu
+00024a70: 6d73 2e54 6167 4772 6f75 7049 442e 6765  ms.TagGroupID.ge
+00024a80: 6f67 7261 7068 795f 7479 7065 2c0d 0a20  ography_type,.. 
+00024a90: 2020 2020 2020 2020 2020 2065 6e75 6d73             enums
+00024aa0: 2e54 6167 4772 6f75 7049 442e 7265 6c65  .TagGroupID.rele
+00024ab0: 6173 652c 0d0a 2020 2020 2020 2020 2020  ase,..          
+00024ac0: 2020 656e 756d 732e 5461 6747 726f 7570    enums.TagGroup
+00024ad0: 4944 2e73 6561 736f 6e61 6c5f 6164 6a75  ID.seasonal_adju
+00024ae0: 7374 6d65 6e74 2c0d 0a20 2020 2020 2020  stment,..       
+00024af0: 2020 2020 2065 6e75 6d73 2e54 6167 4772       enums.TagGr
+00024b00: 6f75 7049 442e 736f 7572 6365 0d0a 2020  oupID.source..  
+00024b10: 2020 2020 2020 5d0d 0a0d 0a20 2020 2020        ]....     
+00024b20: 2020 2069 6620 6f72 6465 725f 6279 206e     if order_by n
+00024b30: 6f74 2069 6e20 616c 6c6f 7765 645f 6f72  ot in allowed_or
+00024b40: 6465 7273 3a0d 0a20 2020 2020 2020 2020  ders:..         
+00024b50: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00024b60: 726f 7228 2756 6172 6961 626c 6520 6f72  ror('Variable or
+00024b70: 6465 725f 6279 2028 7b7d 2920 6973 206e  der_by ({}) is n
+00024b80: 6f74 206f 6e65 206f 6620 7468 6520 7661  ot one of the va
+00024b90: 6c75 6573 3a20 7b7d 272e 666f 726d 6174  lues: {}'.format
+00024ba0: 286f 7264 6572 5f62 792c 2027 2c20 272e  (order_by, ', '.
+00024bb0: 6a6f 696e 286d 6170 2873 7472 2c20 616c  join(map(str, al
+00024bc0: 6c6f 7765 645f 6f72 6465 7273 2929 2929  lowed_orders))))
+00024bd0: 0d0a 0d0a 2020 2020 2020 2020 6966 2074  ....        if t
+00024be0: 6167 5f67 726f 7570 5f69 6420 6973 206e  ag_group_id is n
+00024bf0: 6f74 204e 6f6e 6520 616e 6420 7461 675f  ot None and tag_
+00024c00: 6772 6f75 705f 6964 206e 6f74 2069 6e20  group_id not in 
+00024c10: 616c 6c6f 7765 645f 7461 675f 6772 6f75  allowed_tag_grou
+00024c20: 705f 6964 733a 0d0a 2020 2020 2020 2020  p_ids:..        
+00024c30: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00024c40: 7272 6f72 2827 5661 7269 6162 6c65 2074  rror('Variable t
+00024c50: 6167 5f67 726f 7570 5f69 6420 287b 7d29  ag_group_id ({})
+00024c60: 2069 7320 6e6f 7420 6f6e 6520 6f66 2074   is not one of t
+00024c70: 6865 2076 616c 7565 733a 207b 7d27 2e66  he values: {}'.f
+00024c80: 6f72 6d61 7428 7461 675f 6772 6f75 705f  ormat(tag_group_
+00024c90: 6964 2c20 272c 2027 2e6a 6f69 6e28 6d61  id, ', '.join(ma
+00024ca0: 7028 7374 722c 2061 6c6c 6f77 6564 5f74  p(str, allowed_t
+00024cb0: 6167 5f67 726f 7570 5f69 6473 2929 2929  ag_group_ids))))
+00024cc0: 0d0a 0d0a 2020 2020 2020 2020 6966 2072  ....        if r
+00024cd0: 6561 6c74 696d 655f 7374 6172 7420 6973  ealtime_start is
+00024ce0: 206e 6f74 204e 6f6e 6520 616e 6420 7265   not None and re
+00024cf0: 616c 7469 6d65 5f73 7461 7274 203c 2064  altime_start < d
+00024d00: 6174 6528 3137 3736 2c20 372c 2034 293a  ate(1776, 7, 4):
+00024d10: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00024d20: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00024d30: 5661 7269 6162 6c65 2072 6561 6c74 696d  Variable realtim
+00024d40: 655f 7374 6172 7420 2822 7b7d 2229 2069  e_start ("{}") i
+00024d50: 7320 6265 666f 7265 206d 696e 2064 6174  s before min dat
+00024d60: 6520 3137 3736 2d30 372d 3034 2e27 2e66  e 1776-07-04.'.f
+00024d70: 6f72 6d61 7428 7265 616c 7469 6d65 5f73  ormat(realtime_s
+00024d80: 7461 7274 2929 0d0a 0d0a 2020 2020 2020  tart))....      
+00024d90: 2020 6966 2072 6561 6c74 696d 655f 7374    if realtime_st
+00024da0: 6172 7420 6973 206e 6f74 204e 6f6e 6520  art is not None 
+00024db0: 616e 6420 7265 616c 7469 6d65 5f65 6e64  and realtime_end
+00024dc0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00024dd0: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
+00024de0: 3e20 7265 616c 7469 6d65 5f65 6e64 3a0d  > realtime_end:.
+00024df0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00024e00: 7365 2056 616c 7565 4572 726f 7228 2754  se ValueError('T
+00024e10: 6865 2064 6174 6520 7365 7420 6279 2076  he date set by v
+00024e20: 6172 6961 626c 6520 7265 616c 7469 6d65  ariable realtime
+00024e30: 5f73 7461 7274 2028 227b 7d22 2920 6361  _start ("{}") ca
+00024e40: 6e20 6e6f 7420 6265 2061 6674 6572 2074  n not be after t
+00024e50: 6865 2064 6174 6520 7365 7420 6279 2076  he date set by v
+00024e60: 6172 6961 626c 6520 7265 616c 7469 6d65  ariable realtime
+00024e70: 5f65 6e64 2028 227b 7d22 292e 272e 666f  _end ("{}").'.fo
+00024e80: 726d 6174 2872 6561 6c74 696d 655f 7374  rmat(realtime_st
+00024e90: 6172 742c 2072 6561 6c74 696d 655f 656e  art, realtime_en
+00024ea0: 6429 290d 0a0d 0a20 2020 2020 2020 2064  d))....        d
+00024eb0: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+00024ec0: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+00024ed0: 656c 662e 5f63 6c69 656e 742e 6765 7428  elf._client.get(
+00024ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00024ef0: 2020 272f 6672 6564 2f72 656c 6174 6564    '/fred/related
+00024f00: 5f74 6167 7327 2c0d 0a20 2020 2020 2020  _tags',..       
+00024f10: 2020 2020 2020 2020 2027 7461 6773 272c           'tags',
+00024f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00024f30: 2020 6c69 6d69 743d 3130 3030 2c0d 0a20    limit=1000,.. 
+00024f40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00024f50: 6561 6c74 696d 655f 7374 6172 743d 7265  ealtime_start=re
+00024f60: 616c 7469 6d65 5f73 7461 7274 2c0d 0a20  altime_start,.. 
+00024f70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00024f80: 6561 6c74 696d 655f 656e 643d 7265 616c  ealtime_end=real
+00024f90: 7469 6d65 5f65 6e64 2c0d 0a20 2020 2020  time_end,..     
+00024fa0: 2020 2020 2020 2020 2020 2074 6167 5f6e             tag_n
+00024fb0: 616d 6573 3d74 6167 5f6e 616d 6573 2c0d  ames=tag_names,.
+00024fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024fd0: 2065 7863 6c75 6465 5f74 6167 5f6e 616d   exclude_tag_nam
+00024fe0: 6573 3d65 7863 6c75 6465 5f74 6167 5f6e  es=exclude_tag_n
+00024ff0: 616d 6573 2c0d 0a20 2020 2020 2020 2020  ames,..         
+00025000: 2020 2020 2020 2074 6167 5f67 726f 7570         tag_group
+00025010: 5f69 643d 7461 675f 6772 6f75 705f 6964  _id=tag_group_id
+00025020: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00025030: 2020 2073 6561 7263 685f 7465 7874 3d73     search_text=s
+00025040: 6561 7263 685f 7465 7874 2c0d 0a20 2020  earch_text,..   
+00025050: 2020 2020 2020 2020 2020 2020 206f 7264               ord
+00025060: 6572 5f62 793d 6f72 6465 725f 6279 2c0d  er_by=order_by,.
+00025070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025080: 2073 6f72 745f 6f72 6465 723d 736f 7274   sort_order=sort
+00025090: 5f6f 7264 6572 0d0a 2020 2020 2020 2020  _order..        
+000250a0: 2020 2020 290d 0a20 2020 2020 2020 2029      )..        )
+000250b0: 0d0a 0d0a 2020 2020 2020 2020 6966 206e  ....        if n
+000250c0: 6f74 2064 662e 656d 7074 793a 0d0a 2020  ot df.empty:..  
+000250d0: 2020 2020 2020 2020 2020 6466 2e63 7265            df.cre
+000250e0: 6174 6564 203d 2070 642e 746f 5f64 6174  ated = pd.to_dat
+000250f0: 6574 696d 6528 6466 2e63 7265 6174 6564  etime(df.created
+00025100: 202b 2027 3030 272c 2075 7463 3d54 7275   + '00', utc=Tru
+00025110: 652c 2066 6f72 6d61 743d 2725 592d 256d  e, format='%Y-%m
+00025120: 2d25 6420 2548 3a25 4d3a 2553 257a 2729  -%d %H:%M:%S%z')
+00025130: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00025140: 6466 203d 2064 662e 6173 7479 7065 2864  df = df.astype(d
+00025150: 7479 7065 3d7b 0d0a 2020 2020 2020 2020  type={..        
+00025160: 2020 2020 2020 2020 276e 616d 6527 3a20          'name': 
+00025170: 2773 7472 696e 6727 2c0d 0a20 2020 2020  'string',..     
+00025180: 2020 2020 2020 2020 2020 2027 6e6f 7465             'note
+00025190: 7327 3a20 2773 7472 696e 6727 2c0d 0a20  s': 'string',.. 
+000251a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000251b0: 6772 6f75 705f 6964 273a 2027 6361 7465  group_id': 'cate
+000251c0: 676f 7279 270d 0a20 2020 2020 2020 2020  gory'..         
+000251d0: 2020 207d 292e 7365 745f 696e 6465 7828     }).set_index(
+000251e0: 276e 616d 6527 290d 0a0d 0a20 2020 2020  'name')....     
+000251f0: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
+00025200: 2020 2020 6465 6620 7461 6773 5f73 6572      def tags_ser
+00025210: 6965 7328 0d0a 2020 2020 2020 2020 2020  ies(..          
+00025220: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00025230: 2020 2020 2074 6167 5f6e 616d 6573 3a20       tag_names: 
+00025240: 4c69 7374 5b73 7472 5d20 3d20 4e6f 6e65  List[str] = None
+00025250: 2c0d 0a20 2020 2020 2020 2020 2020 2065  ,..            e
+00025260: 7863 6c75 6465 5f74 6167 5f6e 616d 6573  xclude_tag_names
+00025270: 3a20 4c69 7374 5b73 7472 5d20 3d20 4e6f  : List[str] = No
+00025280: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+00025290: 2072 6561 6c74 696d 655f 7374 6172 743a   realtime_start:
+000252a0: 2064 6174 6520 3d20 4e6f 6e65 2c0d 0a20   date = None,.. 
+000252b0: 2020 2020 2020 2020 2020 2072 6561 6c74             realt
+000252c0: 696d 655f 656e 643a 2064 6174 6520 3d20  ime_end: date = 
+000252d0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+000252e0: 2020 206f 7264 6572 5f62 793a 2065 6e75     order_by: enu
+000252f0: 6d73 2e4f 7264 6572 4279 203d 2065 6e75  ms.OrderBy = enu
+00025300: 6d73 2e4f 7264 6572 4279 2e73 6572 6965  ms.OrderBy.serie
+00025310: 735f 6964 2c0d 0a20 2020 2020 2020 2020  s_id,..         
+00025320: 2020 2073 6f72 745f 6f72 6465 723a 2065     sort_order: e
+00025330: 6e75 6d73 2e53 6f72 744f 7264 6572 203d  nums.SortOrder =
+00025340: 2065 6e75 6d73 2e53 6f72 744f 7264 6572   enums.SortOrder
+00025350: 2e61 7363 0d0a 2020 2020 2920 2d3e 2070  .asc..    ) -> p
+00025360: 642e 4461 7461 4672 616d 653a 0d0a 2020  d.DataFrame:..  
+00025370: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00025380: 2020 2023 2320 5061 7261 6d65 7465 7273     ## Parameters
+00025390: 0d0a 0d0a 2020 2020 2020 2020 6074 6167  ....        `tag
+000253a0: 5f6e 616d 6573 600d 0a20 2020 2020 2020  _names`..       
+000253b0: 2054 7570 6c65 206f 6620 7461 6720 6e61   Tuple of tag na
+000253c0: 6d65 7320 7468 6174 2073 6572 6965 7320  mes that series 
+000253d0: 6d61 7463 6820 616c 6c20 6f66 2e0d 0a0d  match all of....
+000253e0: 0a20 2020 2020 2020 2060 6578 636c 7564  .        `exclud
+000253f0: 655f 7461 675f 6e61 6d65 7360 0d0a 2020  e_tag_names`..  
+00025400: 2020 2020 2020 5475 706c 6520 6f66 2074        Tuple of t
+00025410: 6167 206e 616d 6573 2074 6861 7420 7365  ag names that se
+00025420: 7269 6573 206d 6174 6368 206e 6f6e 6520  ries match none 
+00025430: 6f66 2e0d 0a0d 0a20 2020 2020 2020 2060  of.....        `
+00025440: 7265 616c 7469 6d65 5f73 7461 7274 600d  realtime_start`.
+00025450: 0a20 2020 2020 2020 2054 6865 2073 7461  .        The sta
+00025460: 7274 206f 6620 7468 6520 7265 616c 2d74  rt of the real-t
+00025470: 696d 6520 7065 7269 6f64 2e20 466f 7220  ime period. For 
+00025480: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00025490: 2c20 7365 6520 5b52 6561 6c2d 5469 6d65  , see [Real-Time
+000254a0: 2050 6572 696f 6473 5d28 6874 7470 733a   Periods](https:
+000254b0: 2f2f 6672 6564 2e73 746c 6f75 6973 6665  //fred.stlouisfe
+000254c0: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
+000254d0: 7265 642f 7265 616c 7469 6d65 5f70 6572  red/realtime_per
+000254e0: 696f 642e 6874 6d6c 292e 0d0a 0d0a 2020  iod.html).....  
+000254f0: 2020 2020 2020 6072 6561 6c74 696d 655f        `realtime_
+00025500: 656e 6460 0d0a 2020 2020 2020 2020 5468  end`..        Th
+00025510: 6520 656e 6420 6f66 2074 6865 2072 6561  e end of the rea
+00025520: 6c2d 7469 6d65 2070 6572 696f 642e 2046  l-time period. F
+00025530: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00025540: 696f 6e2c 2073 6565 205b 5265 616c 2d54  ion, see [Real-T
+00025550: 696d 6520 5065 7269 6f64 735d 2868 7474  ime Periods](htt
+00025560: 7073 3a2f 2f66 7265 642e 7374 6c6f 7569  ps://fred.stloui
+00025570: 7366 6564 2e6f 7267 2f64 6f63 732f 6170  sfed.org/docs/ap
+00025580: 692f 6672 6564 2f72 6561 6c74 696d 655f  i/fred/realtime_
+00025590: 7065 7269 6f64 2e68 746d 6c29 2e0d 0a0d  period.html)....
+000255a0: 0a20 2020 2020 2020 2060 6f72 6465 725f  .        `order_
+000255b0: 6279 600d 0a20 2020 2020 2020 204f 7264  by`..        Ord
+000255c0: 6572 2072 6573 756c 7473 2062 7920 7661  er results by va
+000255d0: 6c75 6573 206f 6620 7468 6520 7370 6563  lues of the spec
+000255e0: 6966 6965 6420 6174 7472 6962 7574 652e  ified attribute.
+000255f0: 0d0a 0d0a 2020 2020 2020 2020 6073 6f72  ....        `sor
+00025600: 745f 6f72 6465 7260 0d0a 2020 2020 2020  t_order`..      
+00025610: 2020 536f 7274 2072 6573 756c 7473 2069    Sort results i
+00025620: 7320 6173 6365 6e64 696e 6720 6f72 2064  s ascending or d
+00025630: 6573 6365 6e64 696e 6720 6f72 6465 7220  escending order 
+00025640: 666f 7220 6174 7472 6962 7574 6520 7661  for attribute va
+00025650: 6c75 6573 2073 7065 6369 6669 6564 2062  lues specified b
+00025660: 7920 6f72 6465 725f 6279 2e0d 0a0d 0a20  y order_by..... 
+00025670: 2020 2020 2020 2023 2320 4465 7363 7269         ## Descri
+00025680: 7074 696f 6e0d 0a20 2020 2020 2020 2068  ption..        h
+00025690: 7474 7073 3a2f 2f66 7265 642e 7374 6c6f  ttps://fred.stlo
+000256a0: 7569 7366 6564 2e6f 7267 2f64 6f63 732f  uisfed.org/docs/
+000256b0: 6170 692f 6672 6564 2f74 6167 735f 7365  api/fred/tags_se
+000256c0: 7269 6573 2e68 746d 6c0d 0a0d 0a20 2020  ries.html....   
+000256d0: 2020 2020 2047 6574 2074 6865 2073 6572       Get the ser
+000256e0: 6965 7320 6d61 7463 6869 6e67 2061 6c6c  ies matching all
+000256f0: 2074 6167 7320 696e 2074 6865 2074 6167   tags in the tag
+00025700: 5f6e 616d 6573 2070 6172 616d 6574 6572  _names parameter
+00025710: 2061 6e64 206e 6f20 7461 6773 2069 6e20   and no tags in 
+00025720: 7468 6520 6578 636c 7564 655f 7461 675f  the exclude_tag_
+00025730: 6e61 6d65 7320 7061 7261 6d65 7465 722e  names parameter.
+00025740: 0d0a 0d0a 2020 2020 2020 2020 2323 2041  ....        ## A
+00025750: 5049 2052 6571 7565 7374 2028 4854 5450  PI Request (HTTP
+00025760: 5320 4745 5429 0d0a 2020 2020 2020 2020  S GET)..        
+00025770: 6874 7470 733a 2f2f 6170 692e 7374 6c6f  https://api.stlo
+00025780: 7569 7366 6564 2e6f 7267 2f66 7265 642f  uisfed.org/fred/
+00025790: 7461 6773 2f73 6572 6965 733f 7461 675f  tags/series?tag_
+000257a0: 6e61 6d65 733d 736c 6f76 656e 6961 3b66  names=slovenia;f
+000257b0: 6f6f 643b 6f65 6364 2661 7069 5f6b 6579  ood;oecd&api_key
+000257c0: 3d61 6263 6465 6667 6869 6a6b 6c6d 6e6f  =abcdefghijklmno
+000257d0: 7071 7273 7475 7677 7879 7a31 3233 3435  pqrstuvwxyz12345
+000257e0: 3626 6669 6c65 5f74 7970 653d 6a73 6f6e  6&file_type=json
+000257f0: 0d0a 0d0a 2020 2020 2020 2020 2323 2041  ....        ## A
+00025800: 5049 2052 6573 706f 6e73 650d 0a20 2020  PI Response..   
+00025810: 2020 2020 2060 6060 6a73 6f6e 0d0a 2020       ```json..  
+00025820: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00025830: 2020 2022 7265 616c 7469 6d65 5f73 7461     "realtime_sta
+00025840: 7274 223a 2022 3230 3137 2d30 382d 3031  rt": "2017-08-01
+00025850: 222c 0d0a 2020 2020 2020 2020 2020 2272  ",..          "r
+00025860: 6561 6c74 696d 655f 656e 6422 3a20 2232  ealtime_end": "2
+00025870: 3031 372d 3038 2d30 3122 2c0d 0a20 2020  017-08-01",..   
+00025880: 2020 2020 2020 2022 6f72 6465 725f 6279         "order_by
+00025890: 223a 2022 7365 7269 6573 5f69 6422 2c0d  ": "series_id",.
+000258a0: 0a20 2020 2020 2020 2020 2022 736f 7274  .          "sort
+000258b0: 5f6f 7264 6572 223a 2022 6173 6322 2c0d  _order": "asc",.
+000258c0: 0a20 2020 2020 2020 2020 2022 636f 756e  .          "coun
+000258d0: 7422 3a20 3138 2c0d 0a20 2020 2020 2020  t": 18,..       
+000258e0: 2020 2022 6f66 6673 6574 223a 2030 2c0d     "offset": 0,.
+000258f0: 0a20 2020 2020 2020 2020 2022 6c69 6d69  .          "limi
+00025900: 7422 3a20 3130 3030 2c0d 0a20 2020 2020  t": 1000,..     
+00025910: 2020 2020 2022 7365 7269 6573 7322 3a20       "seriess": 
+00025920: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00025930: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00025940: 2020 2020 2020 2020 2269 6422 3a20 2243          "id": "C
+00025950: 5047 4446 4430 3253 4941 3635 374e 222c  PGDFD02SIA657N",
+00025960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025970: 2020 2020 2272 6561 6c74 696d 655f 7374      "realtime_st
+00025980: 6172 7422 3a20 2232 3031 372d 3038 2d30  art": "2017-08-0
+00025990: 3122 2c0d 0a20 2020 2020 2020 2020 2020  1",..           
+000259a0: 2020 2020 2020 2022 7265 616c 7469 6d65         "realtime
+000259b0: 5f65 6e64 223a 2022 3230 3137 2d30 382d  _end": "2017-08-
+000259c0: 3031 222c 0d0a 2020 2020 2020 2020 2020  01",..          
+000259d0: 2020 2020 2020 2020 2274 6974 6c65 223a          "title":
+000259e0: 2022 436f 6e73 756d 6572 2050 7269 6365   "Consumer Price
+000259f0: 2049 6e64 6578 3a20 546f 7461 6c20 466f   Index: Total Fo
+00025a00: 6f64 2045 7863 6c75 6469 6e67 2052 6573  od Excluding Res
+00025a10: 7461 7572 616e 7473 2066 6f72 2053 6c6f  taurants for Slo
+00025a20: 7665 6e69 615c 7530 3061 3922 2c0d 0a20  venia\u00a9",.. 
+00025a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a40: 2022 6f62 7365 7276 6174 696f 6e5f 7374   "observation_st
+00025a50: 6172 7422 3a20 2231 3939 362d 3031 2d30  art": "1996-01-0
+00025a60: 3122 2c0d 0a20 2020 2020 2020 2020 2020  1",..           
+00025a70: 2020 2020 2020 2022 6f62 7365 7276 6174         "observat
+00025a80: 696f 6e5f 656e 6422 3a20 2232 3031 362d  ion_end": "2016-
+00025a90: 3031 2d30 3122 2c0d 0a20 2020 2020 2020  01-01",..       
+00025aa0: 2020 2020 2020 2020 2020 2022 6672 6571             "freq
+00025ab0: 7565 6e63 7922 3a20 2241 6e6e 7561 6c22  uency": "Annual"
+00025ac0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00025ad0: 2020 2020 2022 6672 6571 7565 6e63 795f       "frequency_
+00025ae0: 7368 6f72 7422 3a20 2241 222c 0d0a 2020  short": "A",..  
+00025af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b00: 2275 6e69 7473 223a 2022 4772 6f77 7468  "units": "Growth
+00025b10: 2052 6174 6520 5072 6576 696f 7573 2050   Rate Previous P
+00025b20: 6572 696f 6422 2c0d 0a20 2020 2020 2020  eriod",..       
+00025b30: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
+00025b40: 735f 7368 6f72 7422 3a20 2247 726f 7774  s_short": "Growt
+00025b50: 6820 5261 7465 2050 7265 7669 6f75 7320  h Rate Previous 
+00025b60: 5065 7269 6f64 222c 0d0a 2020 2020 2020  Period",..      
+00025b70: 2020 2020 2020 2020 2020 2020 2273 6561              "sea
+00025b80: 736f 6e61 6c5f 6164 6a75 7374 6d65 6e74  sonal_adjustment
+00025b90: 223a 2022 4e6f 7420 5365 6173 6f6e 616c  ": "Not Seasonal
+00025ba0: 6c79 2041 646a 7573 7465 6422 2c0d 0a20  ly Adjusted",.. 
+00025bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025bc0: 2022 7365 6173 6f6e 616c 5f61 646a 7573   "seasonal_adjus
+00025bd0: 746d 656e 745f 7368 6f72 7422 3a20 224e  tment_short": "N
+00025be0: 5341 222c 0d0a 2020 2020 2020 2020 2020  SA",..          
+00025bf0: 2020 2020 2020 2020 226c 6173 745f 7570          "last_up
+00025c00: 6461 7465 6422 3a20 2232 3031 372d 3034  dated": "2017-04
+00025c10: 2d32 3020 3030 3a34 383a 3335 2d30 3522  -20 00:48:35-05"
+00025c20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00025c30: 2020 2020 2022 706f 7075 6c61 7269 7479       "popularity
+00025c40: 223a 2030 2c0d 0a20 2020 2020 2020 2020  ": 0,..         
+00025c50: 2020 2020 2020 2020 2022 6772 6f75 705f           "group_
+00025c60: 706f 7075 6c61 7269 7479 223a 2030 2c0d  popularity": 0,.
+00025c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025c80: 2020 2022 6e6f 7465 7322 3a20 224f 4543     "notes": "OEC
+00025c90: 4420 6465 7363 7269 7074 6f72 2049 443a  D descriptor ID:
+00025ca0: 2043 5047 4446 4430 325c 5c6e 4f45 4344   CPGDFD02\\nOECD
+00025cb0: 2075 6e69 7420 4944 3a20 4750 5c5c 6e4f   unit ID: GP\\nO
+00025cc0: 4543 4420 636f 756e 7472 7920 4944 3a20  ECD country ID: 
+00025cd0: 5356 4e5c 5c6e 5c5c 6e41 6c6c 204f 4543  SVN\\n\\nAll OEC
+00025ce0: 4420 6461 7461 2073 686f 756c 6420 6265  D data should be
+00025cf0: 2063 6974 6564 2061 7320 666f 6c6c 6f77   cited as follow
+00025d00: 733a 204f 4543 442c 205c 5c22 4d61 696e  s: OECD, \\"Main
+00025d10: 2045 636f 6e6f 6d69 6320 496e 6469 6361   Economic Indica
+00025d20: 746f 7273 202d 2063 6f6d 706c 6574 6520  tors - complete 
+00025d30: 6461 7461 6261 7365 5c5c 222c 204d 6169  database\\", Mai
+00025d40: 6e20 4563 6f6e 6f6d 6963 2049 6e64 6963  n Economic Indic
+00025d50: 6174 6f72 7320 2864 6174 6162 6173 6529  ators (database)
+00025d60: 2c68 7474 703a 2f2f 6478 2e64 6f69 2e6f  ,http://dx.doi.o
+00025d70: 7267 2f31 302e 3137 3837 2f64 6174 612d  rg/10.1787/data-
+00025d80: 3030 3035 322d 656e 2028 4163 6365 7373  00052-en (Access
+00025d90: 6564 206f 6e20 6461 7465 295c 5c6e 436f  ed on date)\\nCo
+00025da0: 7079 7269 6768 742c 2032 3031 362c 204f  pyright, 2016, O
+00025db0: 4543 442e 2052 6570 7269 6e74 6564 2077  ECD. Reprinted w
+00025dc0: 6974 6820 7065 726d 6973 7369 6f6e 2e22  ith permission."
+00025dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025de0: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
+00025df0: 2020 2020 2020 2e2e 2e0d 0a20 2020 2020        .....     
+00025e00: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+00025e10: 2020 7d0d 0a20 2020 2020 2020 2060 6060    }..        ```
+00025e20: 0d0a 0d0a 2020 2020 2020 2020 2323 2052  ....        ## R
+00025e30: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
+00025e40: 6070 616e 6461 732e 4461 7461 4672 616d  `pandas.DataFram
+00025e50: 6560 0d0a 0d0a 2020 2020 2020 2020 2323  e`....        ##
+00025e60: 2045 7861 6d70 6c65 0d0a 2020 2020 2020   Example..      
+00025e70: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
+00025e80: 2020 2020 203e 3e3e 2066 7265 6420 3d20       >>> fred = 
+00025e90: 4652 4544 2861 7069 5f6b 6579 3d27 6162  FRED(api_key='ab
+00025ea0: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
+00025eb0: 7374 7576 7778 797a 3132 3334 3536 2729  stuvwxyz123456')
+00025ec0: 0d0a 2020 2020 2020 2020 3e3e 3e20 6672  ..        >>> fr
+00025ed0: 6564 2e74 6167 735f 7365 7269 6573 2874  ed.tags_series(t
+00025ee0: 6167 5f6e 616d 6573 3d5b 2766 6f6f 6427  ag_names=['food'
+00025ef0: 2c20 276f 6563 6427 5d29 2e68 6561 6428  , 'oecd']).head(
+00025f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00025f10: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00025f20: 6561 6c74 696d 655f 7374 6172 7420 7265  ealtime_start re
+00025f30: 616c 7469 6d65 5f65 6e64 2020 2020 2020  altime_end      
+00025f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00025f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f70: 206e 6f74 6573 0d0a 2020 2020 2020 2020   notes..        
-00025f80: 2020 2020 6964 0d0a 2020 2020 2020 2020      id..        
-00025f90: 2020 2020 4155 5343 5049 434f 5241 494e      AUSCPICORAIN
-00025fa0: 4d45 4920 2020 2020 3230 3232 2d30 322d  MEI     2022-02-
-00025fb0: 3035 2020 2032 3032 322d 3032 2d30 3520  05   2022-02-05 
-00025fc0: 2043 6f6e 7375 6d65 7220 5072 6963 6520   Consumer Price 
-00025fd0: 496e 6465 783a 2041 6c6c 2049 7465 6d73  Index: All Items
-00025fe0: 2045 7863 6c75 6469 6e67 2046 6f6f 642e   Excluding Food.
-00025ff0: 2e2e 2020 2020 2020 2020 3139 3732 2d30  ..        1972-0
-00026000: 312d 3031 2020 2020 2020 3230 3230 2d30  1-01      2020-0
-00026010: 312d 3031 2020 2020 2041 6e6e 7561 6c20  1-01     Annual 
-00026020: 2020 2020 2020 2020 2020 2020 2020 4120                A 
-00026030: 2049 6e64 6578 2032 3031 353d 3130 3020   Index 2015=100 
-00026040: 2049 6e64 6578 2032 3031 353d 3130 3020   Index 2015=100 
-00026050: 204e 6f74 2053 6561 736f 6e61 6c6c 7920   Not Seasonally 
-00026060: 4164 6a75 7374 6564 2020 2020 2020 2020  Adjusted        
-00026070: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-00026080: 5341 2032 3032 312d 3032 2d31 3720 3138  SA 2021-02-17 18
-00026090: 3a32 373a 3339 2b30 303a 3030 2020 2020  :27:39+00:00    
-000260a0: 2020 2020 2020 2031 2020 2020 2020 2020         1        
-000260b0: 2020 2020 2020 2020 3132 2020 436f 7079          12  Copy
-000260c0: 7269 6768 742c 2032 3031 362c 204f 4543  right, 2016, OEC
-000260d0: 442e 2052 6570 7269 6e74 6564 2077 6974  D. Reprinted wit
-000260e0: 6820 7065 726d 6973 7369 2e2e 2e0d 0a20  h permissi..... 
-000260f0: 2020 2020 2020 2020 2020 2041 5553 4350             AUSCP
-00026100: 4943 4f52 5149 4e4d 4549 2020 2020 2032  ICORQINMEI     2
-00026110: 3032 322d 3032 2d30 3520 2020 3230 3232  022-02-05   2022
-00026120: 2d30 322d 3035 2020 436f 6e73 756d 6572  -02-05  Consumer
-00026130: 2050 7269 6365 2049 6e64 6578 3a20 416c   Price Index: Al
-00026140: 6c20 4974 656d 7320 4578 636c 7564 696e  l Items Excludin
-00026150: 6720 466f 6f64 2e2e 2e20 2020 2020 2020  g Food...       
-00026160: 2031 3937 312d 3034 2d30 3120 2020 2020   1971-04-01     
-00026170: 2032 3032 312d 3037 2d30 3120 2051 7561   2021-07-01  Qua
-00026180: 7274 6572 6c79 2020 2020 2020 2020 2020  rterly          
-00026190: 2020 2020 2051 2020 496e 6465 7820 3230       Q  Index 20
-000261a0: 3135 3d31 3030 2020 496e 6465 7820 3230  15=100  Index 20
-000261b0: 3135 3d31 3030 2020 4e6f 7420 5365 6173  15=100  Not Seas
-000261c0: 6f6e 616c 6c79 2041 646a 7573 7465 6420  onally Adjusted 
-000261d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000261e0: 2020 2020 2020 4e53 4120 3230 3231 2d31        NSA 2021-1
-000261f0: 322d 3134 2032 313a 3537 3a30 342b 3030  2-14 21:57:04+00
-00026200: 3a30 3020 2020 2020 2020 2020 2031 3220  :00          12 
-00026210: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00026220: 3220 2043 6f70 7972 6967 6874 2c20 3230  2  Copyright, 20
-00026230: 3136 2c20 4f45 4344 2e20 5265 7072 696e  16, OECD. Reprin
-00026240: 7465 6420 7769 7468 2070 6572 6d69 7373  ted with permiss
-00026250: 692e 2e2e 0d0a 2020 2020 2020 2020 2020  i.....          
-00026260: 2020 4155 5343 5049 464f 4441 494e 4d45    AUSCPIFODAINME
-00026270: 4920 2020 2020 3230 3232 2d30 322d 3035  I     2022-02-05
-00026280: 2020 2032 3032 322d 3032 2d30 3520 2020     2022-02-05   
-00026290: 2020 2020 2020 2020 436f 6e73 756d 6572          Consumer
-000262a0: 2050 7269 6365 2049 6e64 6578 3a20 466f   Price Index: Fo
-000262b0: 6f64 2066 6f72 2041 7573 7472 616c 6961  od for Australia
-000262c0: 2020 2020 2020 2020 3139 3737 2d30 312d          1977-01-
-000262d0: 3031 2020 2020 2020 3230 3137 2d30 312d  01      2017-01-
-000262e0: 3031 2020 2020 2041 6e6e 7561 6c20 2020  01     Annual   
-000262f0: 2020 2020 2020 2020 2020 2020 4120 2049              A  I
-00026300: 6e64 6578 2032 3031 303d 3130 3020 2049  ndex 2010=100  I
-00026310: 6e64 6578 2032 3031 303d 3130 3020 204e  ndex 2010=100  N
-00026320: 6f74 2053 6561 736f 6e61 6c6c 7920 4164  ot Seasonally Ad
-00026330: 6a75 7374 6564 2020 2020 2020 2020 2020  justed          
-00026340: 2020 2020 2020 2020 2020 2020 204e 5341               NSA
-00026350: 2032 3031 382d 3033 2d30 3920 3231 3a31   2018-03-09 21:1
-00026360: 323a 3039 2b30 303a 3030 2020 2020 2020  2:09+00:00      
-00026370: 2020 2020 2031 2020 2020 2020 2020 2020       1          
-00026380: 2020 2020 2020 2032 2020 436f 7079 7269         2  Copyri
-00026390: 6768 742c 2032 3031 362c 204f 4543 442e  ght, 2016, OECD.
-000263a0: 2052 6570 7269 6e74 6564 2077 6974 6820   Reprinted with 
-000263b0: 7065 726d 6973 7369 2e2e 2e0d 0a20 2020  permissi.....   
-000263c0: 2020 2020 2020 2020 2041 5553 4350 4946           AUSCPIF
-000263d0: 4f44 5149 4e4d 4549 2020 2020 2032 3032  ODQINMEI     202
-000263e0: 322d 3032 2d30 3520 2020 3230 3232 2d30  2-02-05   2022-0
-000263f0: 322d 3035 2020 2020 2020 2020 2020 2043  2-05           C
-00026400: 6f6e 7375 6d65 7220 5072 6963 6520 496e  onsumer Price In
-00026410: 6465 783a 2046 6f6f 6420 666f 7220 4175  dex: Food for Au
-00026420: 7374 7261 6c69 6120 2020 2020 2020 2031  stralia        1
-00026430: 3937 362d 3037 2d30 3120 2020 2020 2032  976-07-01      2
-00026440: 3031 382d 3031 2d30 3120 2051 7561 7274  018-01-01  Quart
-00026450: 6572 6c79 2020 2020 2020 2020 2020 2020  erly            
-00026460: 2020 2051 2020 496e 6465 7820 3230 3130     Q  Index 2010
-00026470: 3d31 3030 2020 496e 6465 7820 3230 3130  =100  Index 2010
-00026480: 3d31 3030 2020 4e6f 7420 5365 6173 6f6e  =100  Not Season
-00026490: 616c 6c79 2041 646a 7573 7465 6420 2020  ally Adjusted   
-000264a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000264b0: 2020 2020 4e53 4120 3230 3138 2d30 342d      NSA 2018-04-
-000264c0: 3234 2031 393a 3531 3a30 342b 3030 3a30  24 19:51:04+00:0
-000264d0: 3020 2020 2020 2020 2020 2020 3220 2020  0           2   
-000264e0: 2020 2020 2020 2020 2020 2020 2020 3220                2 
-000264f0: 2043 6f70 7972 6967 6874 2c20 3230 3136   Copyright, 2016
-00026500: 2c20 4f45 4344 2e20 5265 7072 696e 7465  , OECD. Reprinte
-00026510: 6420 7769 7468 2070 6572 6d69 7373 692e  d with permissi.
-00026520: 2e2e 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00026530: 4155 5443 5049 434f 5241 494e 4d45 4920  AUTCPICORAINMEI 
-00026540: 2020 2020 3230 3232 2d30 322d 3035 2020      2022-02-05  
-00026550: 2032 3032 322d 3032 2d30 3520 2043 6f6e   2022-02-05  Con
-00026560: 7375 6d65 7220 5072 6963 6520 496e 6465  sumer Price Inde
-00026570: 783a 2041 6c6c 2049 7465 6d73 2045 7863  x: All Items Exc
-00026580: 6c75 6469 6e67 2046 6f6f 642e 2e2e 2020  luding Food...  
-00026590: 2020 2020 2020 3139 3636 2d30 312d 3031        1966-01-01
-000265a0: 2020 2020 2020 3230 3230 2d30 312d 3031        2020-01-01
-000265b0: 2020 2020 2041 6e6e 7561 6c20 2020 2020       Annual     
-000265c0: 2020 2020 2020 2020 2020 4120 2049 6e64            A  Ind
-000265d0: 6578 2032 3031 353d 3130 3020 2049 6e64  ex 2015=100  Ind
-000265e0: 6578 2032 3031 353d 3130 3020 204e 6f74  ex 2015=100  Not
-000265f0: 2053 6561 736f 6e61 6c6c 7920 4164 6a75   Seasonally Adju
-00026600: 7374 6564 2020 2020 2020 2020 2020 2020  sted            
-00026610: 2020 2020 2020 2020 2020 204e 5341 2032             NSA 2
-00026620: 3032 312d 3033 2d31 3620 3232 3a33 373a  021-03-16 22:37:
-00026630: 3537 2b30 303a 3030 2020 2020 2020 2020  57+00:00        
-00026640: 2020 2030 2020 2020 2020 2020 2020 2020     0            
-00026650: 2020 2020 2031 2020 436f 7079 7269 6768       1  Copyrigh
-00026660: 742c 2032 3031 362c 204f 4543 442e 2052  t, 2016, OECD. R
-00026670: 6570 7269 6e74 6564 2077 6974 6820 7065  eprinted with pe
-00026680: 726d 6973 7369 2e2e 2e0d 0a20 2020 2020  rmissi.....     
-00026690: 2020 2060 6060 0d0a 2020 2020 2020 2020     ```..        
-000266a0: 2222 220d 0a0d 0a20 2020 2020 2020 2061  """....        a
-000266b0: 6c6c 6f77 6564 5f6f 7264 6572 7320 3d20  llowed_orders = 
-000266c0: 5b0d 0a20 2020 2020 2020 2020 2020 2065  [..            e
-000266d0: 6e75 6d73 2e4f 7264 6572 4279 2e73 6572  nums.OrderBy.ser
-000266e0: 6965 735f 6964 2c0d 0a20 2020 2020 2020  ies_id,..       
-000266f0: 2020 2020 2065 6e75 6d73 2e4f 7264 6572       enums.Order
-00026700: 4279 2e74 6974 6c65 2c0d 0a20 2020 2020  By.title,..     
-00026710: 2020 2020 2020 2065 6e75 6d73 2e4f 7264         enums.Ord
-00026720: 6572 4279 2e75 6e69 7473 2c0d 0a20 2020  erBy.units,..   
-00026730: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
-00026740: 7264 6572 4279 2e66 7265 7175 656e 6379  rderBy.frequency
-00026750: 2c0d 0a20 2020 2020 2020 2020 2020 2065  ,..            e
-00026760: 6e75 6d73 2e4f 7264 6572 4279 2e73 6561  nums.OrderBy.sea
-00026770: 736f 6e61 6c5f 6164 6a75 7374 6d65 6e74  sonal_adjustment
-00026780: 2c0d 0a20 2020 2020 2020 2020 2020 2065  ,..            e
-00026790: 6e75 6d73 2e4f 7264 6572 4279 2e72 6561  nums.OrderBy.rea
-000267a0: 6c74 696d 655f 7374 6172 742c 0d0a 2020  ltime_start,..  
-000267b0: 2020 2020 2020 2020 2020 656e 756d 732e            enums.
-000267c0: 4f72 6465 7242 792e 7265 616c 7469 6d65  OrderBy.realtime
-000267d0: 5f65 6e64 2c0d 0a20 2020 2020 2020 2020  _end,..         
-000267e0: 2020 2065 6e75 6d73 2e4f 7264 6572 4279     enums.OrderBy
-000267f0: 2e6c 6173 745f 7570 6461 7465 642c 0d0a  .last_updated,..
-00026800: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-00026810: 732e 4f72 6465 7242 792e 6f62 7365 7276  s.OrderBy.observ
-00026820: 6174 696f 6e5f 7374 6172 742c 0d0a 2020  ation_start,..  
-00026830: 2020 2020 2020 2020 2020 656e 756d 732e            enums.
-00026840: 4f72 6465 7242 792e 6f62 7365 7276 6174  OrderBy.observat
-00026850: 696f 6e5f 656e 642c 0d0a 2020 2020 2020  ion_end,..      
-00026860: 2020 2020 2020 656e 756d 732e 4f72 6465        enums.Orde
-00026870: 7242 792e 706f 7075 6c61 7269 7479 2c0d  rBy.popularity,.
-00026880: 0a20 2020 2020 2020 2020 2020 2065 6e75  .            enu
-00026890: 6d73 2e4f 7264 6572 4279 2e67 726f 7570  ms.OrderBy.group
-000268a0: 5f70 6f70 756c 6172 6974 792c 0d0a 2020  _popularity,..  
-000268b0: 2020 2020 2020 5d0d 0a0d 0a20 2020 2020        ]....     
-000268c0: 2020 2069 6620 6f72 6465 725f 6279 206e     if order_by n
-000268d0: 6f74 2069 6e20 616c 6c6f 7765 645f 6f72  ot in allowed_or
-000268e0: 6465 7273 3a0d 0a20 2020 2020 2020 2020  ders:..         
-000268f0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00026900: 726f 7228 2756 6172 6961 626c 6520 6f72  ror('Variable or
-00026910: 6465 725f 6279 2028 7b7d 2920 6973 206e  der_by ({}) is n
-00026920: 6f74 206f 6e65 206f 6620 7468 6520 7661  ot one of the va
-00026930: 6c75 6573 3a20 7b7d 272e 666f 726d 6174  lues: {}'.format
-00026940: 286f 7264 6572 5f62 792c 2027 2c20 272e  (order_by, ', '.
-00026950: 6a6f 696e 286d 6170 2873 7472 2c20 616c  join(map(str, al
-00026960: 6c6f 7765 645f 6f72 6465 7273 2929 2929  lowed_orders))))
-00026970: 0d0a 0d0a 2020 2020 2020 2020 6966 2072  ....        if r
-00026980: 6561 6c74 696d 655f 7374 6172 7420 6973  ealtime_start is
-00026990: 206e 6f74 204e 6f6e 6520 616e 6420 7265   not None and re
-000269a0: 616c 7469 6d65 5f73 7461 7274 203c 2064  altime_start < d
-000269b0: 6174 6528 3137 3736 2c20 372c 2034 293a  ate(1776, 7, 4):
-000269c0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-000269d0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-000269e0: 5661 7269 6162 6c65 2072 6561 6c74 696d  Variable realtim
-000269f0: 655f 7374 6172 7420 2822 7b7d 2229 2069  e_start ("{}") i
-00026a00: 7320 6265 666f 7265 206d 696e 2064 6174  s before min dat
-00026a10: 6520 3137 3736 2d30 372d 3034 2e27 2e66  e 1776-07-04.'.f
-00026a20: 6f72 6d61 7428 7265 616c 7469 6d65 5f73  ormat(realtime_s
-00026a30: 7461 7274 2929 0d0a 0d0a 2020 2020 2020  tart))....      
-00026a40: 2020 6966 2072 6561 6c74 696d 655f 7374    if realtime_st
-00026a50: 6172 7420 6973 206e 6f74 204e 6f6e 6520  art is not None 
-00026a60: 616e 6420 7265 616c 7469 6d65 5f65 6e64  and realtime_end
-00026a70: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00026a80: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
-00026a90: 3e20 7265 616c 7469 6d65 5f65 6e64 3a0d  > realtime_end:.
-00026aa0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00026ab0: 7365 2056 616c 7565 4572 726f 7228 2754  se ValueError('T
-00026ac0: 6865 2064 6174 6520 7365 7420 6279 2076  he date set by v
-00026ad0: 6172 6961 626c 6520 7265 616c 7469 6d65  ariable realtime
-00026ae0: 5f73 7461 7274 2028 227b 7d22 2920 6361  _start ("{}") ca
-00026af0: 6e20 6e6f 7420 6265 2061 6674 6572 2074  n not be after t
-00026b00: 6865 2064 6174 6520 7365 7420 6279 2076  he date set by v
-00026b10: 6172 6961 626c 6520 7265 616c 7469 6d65  ariable realtime
-00026b20: 5f65 6e64 2028 227b 7d22 292e 272e 666f  _end ("{}").'.fo
-00026b30: 726d 6174 2872 6561 6c74 696d 655f 7374  rmat(realtime_st
-00026b40: 6172 742c 2072 6561 6c74 696d 655f 656e  art, realtime_en
-00026b50: 6429 290d 0a0d 0a20 2020 2020 2020 2064  d))....        d
-00026b60: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
-00026b70: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-00026b80: 656c 662e 5f63 6c69 656e 742e 6765 7428  elf._client.get(
-00026b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00026ba0: 2020 272f 6672 6564 2f74 6167 732f 7365    '/fred/tags/se
-00026bb0: 7269 6573 272c 0d0a 2020 2020 2020 2020  ries',..        
-00026bc0: 2020 2020 2020 2020 2773 6572 6965 7373          'seriess
-00026bd0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00026be0: 2020 2020 6c69 6d69 743d 3130 3030 2c0d      limit=1000,.
-00026bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026c00: 2074 6167 5f6e 616d 6573 3d74 6167 5f6e   tag_names=tag_n
-00026c10: 616d 6573 2c0d 0a20 2020 2020 2020 2020  ames,..         
-00026c20: 2020 2020 2020 2065 7863 6c75 6465 5f74         exclude_t
-00026c30: 6167 5f6e 616d 6573 3d65 7863 6c75 6465  ag_names=exclude
-00026c40: 5f74 6167 5f6e 616d 6573 2c0d 0a20 2020  _tag_names,..   
-00026c50: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00026c60: 6c74 696d 655f 7374 6172 743d 7265 616c  ltime_start=real
-00026c70: 7469 6d65 5f73 7461 7274 2c0d 0a20 2020  time_start,..   
-00026c80: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00026c90: 6c74 696d 655f 656e 643d 7265 616c 7469  ltime_end=realti
-00026ca0: 6d65 5f65 6e64 2c0d 0a20 2020 2020 2020  me_end,..       
-00026cb0: 2020 2020 2020 2020 206f 7264 6572 5f62           order_b
-00026cc0: 793d 6f72 6465 725f 6279 2c0d 0a20 2020  y=order_by,..   
-00026cd0: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
-00026ce0: 745f 6f72 6465 723d 736f 7274 5f6f 7264  t_order=sort_ord
-00026cf0: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
-00026d00: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
-00026d10: 2020 2020 2020 2020 6461 7465 5f63 6f6c          date_col
-00026d20: 756d 6e73 203d 205b 0d0a 2020 2020 2020  umns = [..      
-00026d30: 2020 2020 2020 2772 6561 6c74 696d 655f        'realtime_
-00026d40: 7374 6172 7427 2c20 2772 6561 6c74 696d  start', 'realtim
-00026d50: 655f 656e 6427 2c0d 0a20 2020 2020 2020  e_end',..       
-00026d60: 2020 2020 2027 6f62 7365 7276 6174 696f       'observatio
-00026d70: 6e5f 7374 6172 7427 2c20 276f 6273 6572  n_start', 'obser
-00026d80: 7661 7469 6f6e 5f65 6e64 272c 0d0a 2020  vation_end',..  
-00026d90: 2020 2020 2020 5d0d 0a0d 0a20 2020 2020        ]....     
-00026da0: 2020 2069 6620 6e6f 7420 6466 2e65 6d70     if not df.emp
-00026db0: 7479 3a0d 0a20 2020 2020 2020 2020 2020  ty:..           
-00026dc0: 2064 665b 6461 7465 5f63 6f6c 756d 6e73   df[date_columns
-00026dd0: 5d20 3d20 6466 5b64 6174 655f 636f 6c75  ] = df[date_colu
-00026de0: 6d6e 735d 2e61 7070 6c79 2870 642e 746f  mns].apply(pd.to
-00026df0: 5f64 6174 6574 696d 652c 2066 6f72 6d61  _datetime, forma
-00026e00: 743d 2725 592d 256d 2d25 6427 290d 0a20  t='%Y-%m-%d').. 
-00026e10: 2020 2020 2020 2020 2020 2064 662e 6c61             df.la
-00026e20: 7374 5f75 7064 6174 6564 203d 2070 642e  st_updated = pd.
-00026e30: 746f 5f64 6174 6574 696d 6528 6466 2e6c  to_datetime(df.l
-00026e40: 6173 745f 7570 6461 7465 6420 2b20 2730  ast_updated + '0
-00026e50: 3027 2c20 7574 633d 5472 7565 2c20 666f  0', utc=True, fo
-00026e60: 726d 6174 3d27 2559 2d25 6d2d 2564 2025  rmat='%Y-%m-%d %
-00026e70: 483a 254d 3a25 5325 7a27 290d 0a0d 0a20  H:%M:%S%z').... 
-00026e80: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
-00026e90: 6466 2e61 7374 7970 6528 6474 7970 653d  df.astype(dtype=
-00026ea0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00026eb0: 2020 2027 6964 273a 2027 7374 7269 6e67     'id': 'string
-00026ec0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00026ed0: 2020 2020 276e 6f74 6573 273a 2027 7374      'notes': 'st
-00026ee0: 7269 6e67 272c 0d0a 2020 2020 2020 2020  ring',..        
-00026ef0: 2020 2020 2020 2020 2774 6974 6c65 273a          'title':
-00026f00: 2027 7374 7269 6e67 272c 0d0a 2020 2020   'string',..    
-00026f10: 2020 2020 2020 2020 2020 2020 2766 7265              'fre
-00026f20: 7175 656e 6379 273a 2027 6361 7465 676f  quency': 'catego
-00026f30: 7279 272c 0d0a 2020 2020 2020 2020 2020  ry',..          
-00026f40: 2020 2020 2020 2766 7265 7175 656e 6379        'frequency
-00026f50: 5f73 686f 7274 273a 2027 6361 7465 676f  _short': 'catego
-00026f60: 7279 272c 0d0a 2020 2020 2020 2020 2020  ry',..          
-00026f70: 2020 2020 2020 2775 6e69 7473 5f73 686f        'units_sho
-00026f80: 7274 273a 2027 6361 7465 676f 7279 272c  rt': 'category',
-00026f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00026fa0: 2020 2775 6e69 7473 273a 2027 6361 7465    'units': 'cate
-00026fb0: 676f 7279 272c 0d0a 2020 2020 2020 2020  gory',..        
-00026fc0: 2020 2020 2020 2020 2773 6561 736f 6e61          'seasona
-00026fd0: 6c5f 6164 6a75 7374 6d65 6e74 273a 2027  l_adjustment': '
-00026fe0: 6361 7465 676f 7279 272c 0d0a 2020 2020  category',..    
-00026ff0: 2020 2020 2020 2020 2020 2020 2773 6561              'sea
-00027000: 736f 6e61 6c5f 6164 6a75 7374 6d65 6e74  sonal_adjustment
-00027010: 5f73 686f 7274 273a 2027 6361 7465 676f  _short': 'catego
-00027020: 7279 270d 0a20 2020 2020 2020 2020 2020  ry'..           
-00027030: 207d 292e 7365 745f 696e 6465 7828 2769   }).set_index('i
-00027040: 6427 290d 0a0d 0a20 2020 2020 2020 2072  d')....        r
-00027050: 6574 7572 6e20 6466 0d0a 0d0a 0d0a 636c  eturn df......cl
-00027060: 6173 7320 414c 4652 4544 2846 5245 4429  ass ALFRED(FRED)
-00027070: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-00027080: 414c 4652 4544 2073 7461 6e64 7320 666f  ALFRED stands fo
-00027090: 7220 4172 6368 6976 616c 2046 6564 6572  r Archival Feder
-000270a0: 616c 2052 6573 6572 7665 2045 636f 6e6f  al Reserve Econo
-000270b0: 6d69 6320 4461 7461 2e0d 0a20 2020 2041  mic Data...    A
-000270c0: 4c46 5245 4420 6172 6368 6976 6573 2046  LFRED archives F
-000270d0: 5245 4420 6461 7461 2062 7920 6164 6469  RED data by addi
-000270e0: 6e67 2074 6865 2072 6561 6c2d 7469 6d65  ng the real-time
-000270f0: 2070 6572 696f 6420 7768 656e 2076 616c   period when val
-00027100: 7565 7320 7765 7265 206f 7269 6769 6e61  ues were origina
-00027110: 6c6c 7920 7265 6c65 6173 6564 2061 6e64  lly released and
-00027120: 206c 6174 6572 2072 6576 6973 6564 2e20   later revised. 
-00027130: 466f 7220 696e 7374 616e 6365 206f 6e20  For instance on 
-00027140: 4665 6272 7561 7279 2032 2c20 3139 3930  February 2, 1990
-00027150: 2c20 7468 6520 5553 2042 7572 6561 7520  , the US Bureau 
-00027160: 6f66 204c 6162 6f72 2053 7461 7469 7374  of Labor Statist
-00027170: 6963 7320 7265 706f 7274 6564 2074 6865  ics reported the
-00027180: 2055 5320 756e 656d 706c 6f79 6d65 6e74   US unemployment
-00027190: 2072 6174 6520 666f 7220 7468 6520 6d6f   rate for the mo
-000271a0: 6e74 6820 6f66 204a 616e 7561 7279 2c20  nth of January, 
-000271b0: 3139 3930 2061 7320 352e 3320 7065 7263  1990 as 5.3 perc
-000271c0: 656e 742e 0d0a 2020 2020 4f76 6572 2036  ent...    Over 6
-000271d0: 2079 6561 7273 206c 6174 6572 206f 6e20   years later on 
-000271e0: 4d61 7263 6820 382c 2031 3939 362c 2074  March 8, 1996, t
-000271f0: 6865 2055 5320 756e 656d 706c 6f79 6d65  he US unemployme
-00027200: 6e74 2072 6174 6520 666f 7220 7468 6520  nt rate for the 
-00027210: 7361 6d65 206d 6f6e 7468 204a 616e 7561  same month Janua
-00027220: 7279 2c20 3139 3930 2077 6173 2072 6576  ry, 1990 was rev
-00027230: 6973 6564 2074 6f20 352e 3420 7065 7263  ised to 5.4 perc
-00027240: 656e 742e 0d0a 0d0a 2020 2020 6874 7470  ent.....    http
-00027250: 733a 2f2f 616c 6672 6564 2e73 746c 6f75  s://alfred.stlou
-00027260: 6973 6665 642e 6f72 672f 0d0a 0d0a 2020  isfed.org/....  
-00027270: 2020 6874 7470 733a 2f2f 6672 6564 2e73    https://fred.s
-00027280: 746c 6f75 6973 6665 642e 6f72 672f 646f  tlouisfed.org/do
-00027290: 6373 2f61 7069 2f66 7265 642f 616c 6672  cs/api/fred/alfr
-000272a0: 6564 2e68 746d 6c0d 0a20 2020 2022 2222  ed.html..    """
-000272b0: 0d0a 0d0a 0d0a 636c 6173 7320 4765 6f46  ......class GeoF
-000272c0: 5245 443a 0d0a 2020 2020 2222 220d 0a20  RED:..    """.. 
-000272d0: 2020 2054 6865 2047 656f 4652 4544 2041     The GeoFRED A
-000272e0: 5049 2069 7320 6120 7765 6220 7365 7276  PI is a web serv
-000272f0: 6963 6520 7468 6174 2061 6c6c 6f77 7320  ice that allows 
-00027300: 6465 7665 6c6f 7065 7273 2074 6f20 7772  developers to wr
-00027310: 6974 6520 7072 6f67 7261 6d73 2061 6e64  ite programs and
-00027320: 2062 7569 6c64 2061 7070 6c69 6361 7469   build applicati
-00027330: 6f6e 7320 746f 2068 6172 7665 7374 2064  ons to harvest d
-00027340: 6174 6120 616e 6420 7368 6170 6520 6669  ata and shape fi
-00027350: 6c65 7320 666f 756e 6420 696e 2047 656f  les found in Geo
-00027360: 4652 4544 2077 6562 7369 7465 2068 6f73  FRED website hos
-00027370: 7465 6420 6279 2074 6865 2045 636f 6e6f  ted by the Econo
-00027380: 6d69 6320 5265 7365 6172 6368 2044 6976  mic Research Div
-00027390: 6973 696f 6e20 6f66 2074 6865 2046 6564  ision of the Fed
-000273a0: 6572 616c 2052 6573 6572 7665 2042 616e  eral Reserve Ban
-000273b0: 6b20 6f66 2053 742e 204c 6f75 6973 2e0d  k of St. Louis..
-000273c0: 0a0d 0a20 2020 2068 7474 7073 3a2f 2f67  ...    https://g
-000273d0: 656f 6672 6564 2e73 746c 6f75 6973 6665  eofred.stlouisfe
-000273e0: 642e 6f72 672f 0d0a 0d0a 2020 2020 6874  d.org/....    ht
-000273f0: 7470 733a 2f2f 6765 6f66 7265 642e 7374  tps://geofred.st
-00027400: 6c6f 7569 7366 6564 2e6f 7267 2f64 6f63  louisfed.org/doc
-00027410: 732f 6170 692f 6765 6f66 7265 642f 0d0a  s/api/geofred/..
-00027420: 2020 2020 2222 220d 0a20 2020 2045 4d50      """..    EMP
-00027430: 5459 5f56 414c 5545 203d 2027 2e27 0d0a  TY_VALUE = '.'..
-00027440: 0d0a 2020 2020 2222 220d 0a20 2020 2068  ..    """..    h
-00027450: 7474 7073 3a2f 2f67 656f 6672 6564 2e73  ttps://geofred.s
-00027460: 746c 6f75 6973 6665 642e 6f72 672f 0d0a  tlouisfed.org/..
-00027470: 2020 2020 6874 7470 733a 2f2f 6765 6f66      https://geof
-00027480: 7265 642e 7374 6c6f 7569 7366 6564 2e6f  red.stlouisfed.o
-00027490: 7267 2f64 6f63 732f 6170 692f 6765 6f66  rg/docs/api/geof
-000274a0: 7265 642f 0d0a 2020 2020 2222 220d 0a0d  red/..    """...
-000274b0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000274c0: 5f28 7365 6c66 2c20 6170 695f 6b65 793a  _(self, api_key:
-000274d0: 2073 7472 2c20 7261 7465 6c69 6d69 7465   str, ratelimite
-000274e0: 725f 656e 6162 6c65 643a 2062 6f6f 6c20  r_enabled: bool 
-000274f0: 3d20 4661 6c73 652c 2072 6174 656c 696d  = False, ratelim
-00027500: 6974 6572 5f6d 6178 5f63 616c 6c73 3a20  iter_max_calls: 
-00027510: 696e 7420 3d20 322c 2072 6174 656c 696d  int = 2, ratelim
-00027520: 6974 6572 5f70 6572 696f 643a 2069 6e74  iter_period: int
-00027530: 203d 2031 2c20 7265 7175 6573 745f 7061   = 1, request_pa
-00027540: 7261 6d73 3a20 6469 6374 203d 204e 6f6e  rams: dict = Non
-00027550: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
-00027560: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00027570: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-00027580: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00027590: 2020 6170 695f 6b65 793a 2073 7472 0d0a    api_key: str..
-000275a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000275b0: 3332 2063 6861 7261 6374 6572 2061 6c70  32 character alp
-000275c0: 6861 2d6e 756d 6572 6963 206c 6f77 6572  ha-numeric lower
-000275d0: 6361 7365 2073 7472 696e 670d 0a20 2020  case string..   
-000275e0: 2020 2020 2072 6174 656c 696d 6974 6572       ratelimiter
-000275f0: 5f65 6e61 626c 6564 3a20 626f 6f6c 0d0a  _enabled: bool..
-00027600: 2020 2020 2020 2020 7261 7465 6c69 6d69          ratelimi
-00027610: 7465 725f 6d61 785f 6361 6c6c 733a 2069  ter_max_calls: i
-00027620: 6e74 0d0a 2020 2020 2020 2020 7261 7465  nt..        rate
-00027630: 6c69 6d69 7465 725f 7065 7269 6f64 3a20  limiter_period: 
-00027640: 696e 740d 0a20 2020 2020 2020 2072 6571  int..        req
-00027650: 7565 7374 5f70 6172 616d 733a 2064 6963  uest_params: dic
-00027660: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-00027670: 2020 2048 5454 5020 4745 5420 6d65 7468     HTTP GET meth
-00027680: 6f64 2070 6172 616d 6574 6572 732c 2073  od parameters, s
-00027690: 6565 2068 7474 7073 3a2f 2f64 6f63 732e  ee https://docs.
-000276a0: 7079 7468 6f6e 2d72 6571 7565 7374 732e  python-requests.
-000276b0: 6f72 672f 656e 2f6c 6174 6573 742f 6170  org/en/latest/ap
-000276c0: 692f 2372 6571 7565 7374 732e 7265 7175  i/#requests.requ
-000276d0: 6573 740d 0a20 2020 2020 2020 2022 2222  est..        """
-000276e0: 0d0a 0d0a 2020 2020 2020 2020 6966 2061  ....        if a
-000276f0: 7069 5f6b 6579 2069 7320 4e6f 6e65 206f  pi_key is None o
-00027700: 7220 6c65 6e28 6170 695f 6b65 7929 2021  r len(api_key) !
-00027710: 3d20 3332 3a0d 0a20 2020 2020 2020 2020  = 32:..         
-00027720: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
-00027730: 6f6e 2827 5661 7269 6162 6c65 2061 7069  on('Variable api
-00027740: 5f6b 6579 206d 7573 7420 6265 2033 3220  _key must be 32 
-00027750: 6368 6172 6163 7465 7220 6c65 6e67 7468  character length
-00027760: 2061 6c70 6861 6e75 6d65 7269 6320 7374   alphanumeric st
-00027770: 7269 6e67 2e27 290d 0a0d 0a20 2020 2020  ring.')....     
-00027780: 2020 2073 656c 662e 5f63 6c69 656e 7420     self._client 
-00027790: 3d20 436c 6965 6e74 280d 0a20 2020 2020  = Client(..     
-000277a0: 2020 2020 2020 206b 6579 3d61 7069 5f6b         key=api_k
-000277b0: 6579 2e6c 6f77 6572 2829 2c0d 0a20 2020  ey.lower(),..   
-000277c0: 2020 2020 2020 2020 2072 6174 656c 696d           ratelim
-000277d0: 6974 6572 5f65 6e61 626c 6564 3d72 6174  iter_enabled=rat
-000277e0: 656c 696d 6974 6572 5f65 6e61 626c 6564  elimiter_enabled
-000277f0: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-00027800: 6174 656c 696d 6974 6572 5f6d 6178 5f63  atelimiter_max_c
-00027810: 616c 6c73 3d72 6174 656c 696d 6974 6572  alls=ratelimiter
-00027820: 5f6d 6178 5f63 616c 6c73 2c0d 0a20 2020  _max_calls,..   
-00027830: 2020 2020 2020 2020 2072 6174 656c 696d           ratelim
-00027840: 6974 6572 5f70 6572 696f 643d 7261 7465  iter_period=rate
-00027850: 6c69 6d69 7465 725f 7065 7269 6f64 2c0d  limiter_period,.
-00027860: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00027870: 7565 7374 5f70 6172 616d 733d 7265 7175  uest_params=requ
-00027880: 6573 745f 7061 7261 6d73 0d0a 2020 2020  est_params..    
-00027890: 2020 2020 290d 0a0d 0a20 2020 2040 7072      )....    @pr
-000278a0: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-000278b0: 7261 7465 5f6c 696d 6974 2873 656c 6629  rate_limit(self)
-000278c0: 202d 3e20 696e 743a 0d0a 2020 2020 2020   -> int:..      
-000278d0: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
-000278e0: 6c69 656e 742e 7261 7465 5f6c 696d 6974  lient.rate_limit
-000278f0: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
-00027900: 790d 0a20 2020 2064 6566 2072 6174 655f  y..    def rate_
-00027910: 6c69 6d69 745f 7265 6d61 696e 696e 6728  limit_remaining(
-00027920: 7365 6c66 2920 2d3e 2069 6e74 3a0d 0a20  self) -> int:.. 
-00027930: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00027940: 6c66 2e5f 636c 6965 6e74 2e72 6174 655f  lf._client.rate_
-00027950: 6c69 6d69 745f 7265 6d61 696e 696e 670d  limit_remaining.
-00027960: 0a0d 0a20 2020 2064 6566 2073 6861 7065  ...    def shape
-00027970: 7328 7365 6c66 2c20 7368 6170 653a 2065  s(self, shape: e
-00027980: 6e75 6d73 2e53 6861 7065 5479 7065 2920  nums.ShapeType) 
-00027990: 2d3e 204c 6973 745b 6d6f 6465 6c73 2e53  -> List[models.S
-000279a0: 6861 7065 5d3a 0d0a 2020 2020 2020 2020  hape]:..        
-000279b0: 2222 220d 0a20 2020 2020 2020 2068 7474  """..        htt
-000279c0: 7073 3a2f 2f67 656f 6672 6564 2e73 746c  ps://geofred.stl
-000279d0: 6f75 6973 6665 642e 6f72 672f 646f 6373  ouisfed.org/docs
-000279e0: 2f61 7069 2f67 656f 6672 6564 2f73 6861  /api/geofred/sha
-000279f0: 7065 732e 6874 6d6c 0d0a 0d0a 2020 2020  pes.html....    
-00027a00: 2020 2020 2323 2044 6573 6372 6970 7469      ## Descripti
-00027a10: 6f6e 0d0a 2020 2020 2020 2020 5468 6973  on..        This
-00027a20: 2072 6571 7565 7374 2072 6574 7572 6e73   request returns
-00027a30: 2073 6861 7065 2066 696c 6573 2066 726f   shape files fro
-00027a40: 6d20 4765 6f46 5245 4420 696e 2057 656c  m GeoFRED in Wel
-00027a50: 6c2d 6b6e 6f77 6e20 7465 7874 2028 574b  l-known text (WK
-00027a60: 5429 2066 6f72 6d61 742e 0d0a 0d0a 2020  T) format.....  
-00027a70: 2020 2020 2020 2323 2041 5049 2052 6571        ## API Req
-00027a80: 7565 7374 2028 4854 5450 5320 4745 5429  uest (HTTPS GET)
-00027a90: 0d0a 2020 2020 2020 2020 6874 7470 733a  ..        https:
-00027aa0: 2f2f 6170 692e 7374 6c6f 7569 7366 6564  //api.stlouisfed
-00027ab0: 2e6f 7267 2f67 656f 6672 6564 2f73 6861  .org/geofred/sha
-00027ac0: 7065 732f 6669 6c65 3f73 6861 7065 3d62  pes/file?shape=b
-00027ad0: 6561 2661 7069 5f6b 6579 3d61 6263 6465  ea&api_key=abcde
-00027ae0: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
-00027af0: 7677 7879 7a31 3233 3435 360d 0a0d 0a20  vwxyz123456.... 
-00027b00: 2020 2020 2020 2023 2320 4150 4920 5265         ## API Re
-00027b10: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
-00027b20: 6060 606a 736f 6e0d 0a20 2020 2020 2020  ```json..       
-00027b30: 207b 0d0a 2020 2020 2020 2020 2020 2262   {..          "b
-00027b40: 6561 223a 205b 0d0a 2020 2020 2020 2020  ea": [..        
-00027b50: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00027b60: 2020 2020 2022 6e61 6d65 223a 2022 4661       "name": "Fa
-00027b70: 7220 5765 7374 222c 0d0a 2020 2020 2020  r West",..      
-00027b80: 2020 2020 2020 2020 2263 6f64 6522 3a20          "code": 
-00027b90: 2238 222c 0d0a 2020 2020 2020 2020 2020  "8",..          
-00027ba0: 2020 2020 2263 656e 7472 6f69 6422 3a20      "centroid": 
-00027bb0: 2250 4f49 4e54 282d 3134 322e 3336 3239  "POINT(-142.3629
-00027bc0: 3438 3337 3834 3332 2035 372e 3134 3738  48378432 57.1478
-00027bd0: 3733 3438 3239 3038 3529 222c 0d0a 2020  734829085)",..  
-00027be0: 2020 2020 2020 2020 2020 2020 2267 656f              "geo
-00027bf0: 6d65 7472 7922 3a20 224d 554c 5449 504f  metry": "MULTIPO
-00027c00: 4c59 474f 4e28 2828 2d31 3535 2e37 3738  LYGON(((-155.778
-00027c10: 3233 3420 3230 2e32 3435 3734 332c 2d31  234 20.245743,-1
-00027c20: 3535 2e37 3732 3733 3420 2e2e 2e29 2929  55.772734 ...)))
-00027c30: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00027c40: 2020 2272 6570 6f72 7420 6e61 6d65 223a    "report name":
-00027c50: 2022 4e6f 7274 6820 4164 616d 732c 204d   "North Adams, M
-00027c60: 412d 5654 220d 0a20 2020 2020 2020 2020  A-VT"..         
-00027c70: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
-00027c80: 2020 2e2e 2e0d 0a20 2020 2020 2020 2020    .....         
-00027c90: 205d 0d0a 2020 2020 2020 2020 7d0d 0a20   ]..        }.. 
-00027ca0: 2020 2020 2020 2060 6060 0d0a 0d0a 2020         ```....  
-00027cb0: 2020 2020 2020 2323 2052 6574 7572 6e73        ## Returns
-00027cc0: 0d0a 2020 2020 2020 2020 604c 6973 745b  ..        `List[
-00027cd0: 7079 7374 6c6f 7569 7366 6564 2e6d 6f64  pystlouisfed.mod
-00027ce0: 656c 732e 5368 6170 655d 600d 0a0d 0a20  els.Shape]`.... 
-00027cf0: 2020 2020 2020 2023 2320 4578 616d 706c         ## Exampl
-00027d00: 650d 0a20 2020 2020 2020 2060 6060 7079  e..        ```py
-00027d10: 7468 6f6e 0d0a 2020 2020 2020 2020 2020  thon..          
-00027d20: 2020 696d 706f 7274 206d 6174 706c 6f74    import matplot
-00027d30: 6c69 622e 7079 706c 6f74 2061 7320 706c  lib.pyplot as pl
-00027d40: 740d 0a20 2020 2020 2020 2020 2020 2066  t..            f
-00027d50: 726f 6d20 6465 7363 6172 7465 7320 696d  rom descartes im
-00027d60: 706f 7274 2050 6f6c 7967 6f6e 5061 7463  port PolygonPatc
-00027d70: 680d 0a20 2020 2020 2020 2020 2020 2066  h..            f
-00027d80: 726f 6d20 7079 7374 6c6f 7569 7366 6564  rom pystlouisfed
-00027d90: 2e63 6c69 656e 7420 696d 706f 7274 2047  .client import G
-00027da0: 656f 4652 4544 2c20 5368 6170 6554 7970  eoFRED, ShapeTyp
-00027db0: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-00027dc0: 2070 6c74 2e66 6967 7572 6528 290d 0a20   plt.figure().. 
-00027dd0: 2020 2020 2020 2020 2020 2061 7820 3d20             ax = 
-00027de0: 706c 742e 6178 6573 2829 0d0a 2020 2020  plt.axes()..    
-00027df0: 2020 2020 2020 2020 6765 6f5f 6672 6564          geo_fred
-00027e00: 203d 2047 656f 4652 4544 2861 7069 5f6b   = GeoFRED(api_k
-00027e10: 6579 3d27 6162 6364 6566 6768 696a 6b6c  ey='abcdefghijkl
-00027e20: 6d6e 6f70 7172 7374 7576 7778 797a 3132  mnopqrstuvwxyz12
-00027e30: 3334 3536 2729 0d0a 0d0a 2020 2020 2020  3456')....      
-00027e40: 2020 2020 2020 666f 7220 636f 756e 7472        for countr
-00027e50: 795f 7368 6170 6520 696e 2067 656f 5f66  y_shape in geo_f
-00027e60: 7265 642e 7368 6170 6573 2873 6861 7065  red.shapes(shape
-00027e70: 3d53 6861 7065 5479 7065 2e63 6f75 6e74  =ShapeType.count
-00027e80: 7279 293a 0d0a 2020 2020 2020 2020 2020  ry):..          
-00027e90: 2020 2020 2020 6178 2e61 6464 5f70 6174        ax.add_pat
-00027ea0: 6368 2850 6f6c 7967 6f6e 5061 7463 6828  ch(PolygonPatch(
-00027eb0: 636f 756e 7472 795f 7368 6170 652e 6765  country_shape.ge
-00027ec0: 6f6d 6574 7279 2c20 6563 3d27 2339 3939  ometry, ec='#999
-00027ed0: 3939 3927 2c20 6663 3d27 2336 3639 3963  999', fc='#6699c
-00027ee0: 6327 2c20 616c 7068 613d 302e 352c 207a  c', alpha=0.5, z
-00027ef0: 6f72 6465 723d 3229 290d 0a20 2020 2020  order=2))..     
-00027f00: 2020 2020 2020 2061 782e 6178 6973 2827         ax.axis('
-00027f10: 7363 616c 6564 2729 0d0a 2020 2020 2020  scaled')..      
-00027f20: 2020 2020 2020 706c 742e 7368 6f77 2829        plt.show()
-00027f30: 0d0a 2020 2020 2020 2020 6060 600d 0a20  ..        ```.. 
-00027f40: 2020 2020 2020 202e 2e20 696d 6167 653a         .. image:
-00027f50: 3a20 6765 6f66 7265 645f 7368 6170 655f  : geofred_shape_
-00027f60: 6d61 702e 706e 670d 0a20 2020 2020 2020  map.png..       
-00027f70: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-00027f80: 776b 745f 6c69 7374 203d 2073 656c 662e  wkt_list = self.
-00027f90: 5f63 6c69 656e 742e 6765 7428 0d0a 2020  _client.get(..  
-00027fa0: 2020 2020 2020 2020 2020 272f 6765 6f66            '/geof
-00027fb0: 7265 642f 7368 6170 6573 2f66 696c 6527  red/shapes/file'
-00027fc0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00027fd0: 6861 7065 2e76 616c 7565 2c0d 0a20 2020  hape.value,..   
-00027fe0: 2020 2020 2020 2020 2073 6861 7065 3d73           shape=s
-00027ff0: 6861 7065 0d0a 2020 2020 2020 2020 290d  hape..        ).
-00028000: 0a0d 0a20 2020 2020 2020 2023 2072 6570  ...        # rep
-00028010: 6c61 6365 2077 6869 7465 7370 6163 6573  lace whitespaces
-00028020: 2069 6e20 6469 6374 206b 6579 730d 0a20   in dict keys.. 
-00028030: 2020 2020 2020 2066 6f72 2077 6b74 2069         for wkt i
-00028040: 6e20 776b 745f 6c69 7374 3a0d 0a20 2020  n wkt_list:..   
-00028050: 2020 2020 2020 2020 2066 6f72 206b 6579           for key
-00028060: 2069 6e20 6c69 7374 2877 6b74 2e6b 6579   in list(wkt.key
-00028070: 7328 2929 3a0d 0a20 2020 2020 2020 2020  s()):..         
-00028080: 2020 2020 2020 2077 6b74 5b6b 6579 2e72         wkt[key.r
-00028090: 6570 6c61 6365 2827 2027 2c20 275f 2729  eplace(' ', '_')
-000280a0: 5d20 3d20 776b 742e 706f 7028 6b65 7929  ] = wkt.pop(key)
-000280b0: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-000280c0: 726e 206c 6973 7428 6d61 7028 6c61 6d62  rn list(map(lamb
-000280d0: 6461 2077 6b74 3a20 6d6f 6465 6c73 2e53  da wkt: models.S
-000280e0: 6861 7065 282a 2a77 6b74 292c 2077 6b74  hape(**wkt), wkt
-000280f0: 5f6c 6973 7429 290d 0a0d 0a20 2020 2064  _list))....    d
-00028100: 6566 2073 6572 6965 735f 6772 6f75 7028  ef series_group(
-00028110: 7365 6c66 2c20 7365 7269 6573 5f69 643a  self, series_id:
-00028120: 2073 7472 2920 2d3e 206d 6f64 656c 732e   str) -> models.
-00028130: 5365 7269 6573 4772 6f75 703a 0d0a 2020  SeriesGroup:..  
-00028140: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00028150: 2020 2068 7474 7073 3a2f 2f67 656f 6672     https://geofr
-00028160: 6564 2e73 746c 6f75 6973 6665 642e 6f72  ed.stlouisfed.or
-00028170: 672f 646f 6373 2f61 7069 2f67 656f 6672  g/docs/api/geofr
-00028180: 6564 2f73 6572 6965 735f 6772 6f75 702e  ed/series_group.
-00028190: 6874 6d6c 0d0a 0d0a 2020 2020 2020 2020  html....        
-000281a0: 2323 2044 6573 6372 6970 7469 6f6e 0d0a  ## Description..
-000281b0: 2020 2020 2020 2020 5468 6973 2072 6571          This req
-000281c0: 7565 7374 2072 6574 7572 6e73 2074 6865  uest returns the
-000281d0: 206d 6574 6120 696e 666f 726d 6174 696f   meta informatio
-000281e0: 6e20 6e65 6564 6564 2074 6f20 6d61 6b65  n needed to make
-000281f0: 2072 6571 7565 7374 7320 666f 7220 4765   requests for Ge
-00028200: 6f46 5245 4420 6461 7461 2e0d 0a20 2020  oFRED data...   
-00028210: 2020 2020 204d 696e 696d 756d 2061 6e64       Minimum and
-00028220: 206d 6178 696d 756d 2064 6174 6520 6172   maximum date ar
-00028230: 6520 616c 736f 2073 7570 706c 6965 6420  e also supplied 
-00028240: 666f 7220 7468 6520 6461 7461 2072 616e  for the data ran
-00028250: 6765 2061 7661 696c 6162 6c65 2e0d 0a0d  ge available....
-00028260: 0a20 2020 2020 2020 2023 2320 4150 4920  .        ## API 
-00028270: 5265 7175 6573 7420 2848 5454 5053 2047  Request (HTTPS G
-00028280: 4554 290d 0a20 2020 2020 2020 2068 7474  ET)..        htt
-00028290: 7073 3a2f 2f61 7069 2e73 746c 6f75 6973  ps://api.stlouis
-000282a0: 6665 642e 6f72 672f 6765 6f66 7265 642f  fed.org/geofred/
-000282b0: 7365 7269 6573 2f67 726f 7570 3f73 6572  series/group?ser
-000282c0: 6965 735f 6964 3d53 4d55 3536 3030 3030  ies_id=SMU560000
-000282d0: 3030 3530 3030 3030 3030 3161 2661 7069  00500000001a&api
-000282e0: 5f6b 6579 3d61 6263 6465 6667 6869 6a6b  _key=abcdefghijk
-000282f0: 6c6d 6e6f 7071 7273 7475 7677 7879 7a31  lmnopqrstuvwxyz1
-00028300: 3233 3435 360d 0a0d 0a20 2020 2020 2020  23456....       
-00028310: 2023 2320 4150 4920 5265 7370 6f6e 7365   ## API Response
-00028320: 0d0a 2020 2020 2020 2020 6060 606a 736f  ..        ```jso
-00028330: 6e0d 0a20 2020 2020 2020 207b 0d0a 2020  n..        {..  
-00028340: 2020 2020 2020 2020 2273 6572 6965 735f          "series_
-00028350: 6772 6f75 7022 3a20 5b0d 0a20 2020 2020  group": [..     
-00028360: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00028370: 2020 2020 2020 2020 2274 6974 6c65 223a          "title":
-00028380: 2022 416c 6c20 456d 706c 6f79 6565 733a   "All Employees:
-00028390: 2054 6f74 616c 2050 7269 7661 7465 222c   Total Private",
-000283a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000283b0: 2267 656f 6d5f 7479 7065 223a 2022 7374  "geom_type": "st
-000283c0: 6174 6522 2c0d 0a20 2020 2020 2020 2020  ate",..         
-000283d0: 2020 2020 2022 6772 6f75 705f 6964 223a       "group_id":
-000283e0: 2022 3139 3222 2c0d 0a20 2020 2020 2020   "192",..       
-000283f0: 2020 2020 2020 2022 7365 6173 6f6e 223a         "season":
-00028400: 2022 4e53 4122 2c0d 0a20 2020 2020 2020   "NSA",..       
-00028410: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
-00028420: 2254 686f 7573 616e 6473 206f 6620 5065  "Thousands of Pe
-00028430: 7273 6f6e 7322 2c0d 0a20 2020 2020 2020  rsons",..       
-00028440: 2020 2020 2020 2022 6672 6571 7565 6e63         "frequenc
-00028450: 7922 3a20 226d 222c 0d0a 2020 2020 2020  y": "m",..      
-00028460: 2020 2020 2020 2020 226d 696e 5f73 7461          "min_sta
-00028470: 7274 5f64 6174 6522 3a20 2231 3939 302d  rt_date": "1990-
-00028480: 3031 2d30 3122 2c0d 0a20 2020 2020 2020  01-01",..       
-00028490: 2020 2020 2020 2022 6d61 785f 7374 6172         "max_star
-000284a0: 745f 6461 7465 223a 2022 3230 3135 2d30  t_date": "2015-0
-000284b0: 362d 3031 220d 0a20 2020 2020 2020 2020  6-01"..         
-000284c0: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
-000284d0: 5d0d 0a20 2020 2020 2020 207d 0d0a 2020  ]..        }..  
-000284e0: 2020 2020 2020 6060 600d 0a0d 0a20 2020        ```....   
-000284f0: 2020 2020 2023 2320 5265 7475 726e 730d       ## Returns.
-00028500: 0a20 2020 2020 2020 2060 6d6f 6465 6c73  .        `models
-00028510: 2e53 6572 6965 7347 726f 7570 600d 0a0d  .SeriesGroup`...
-00028520: 0a20 2020 2020 2020 2023 2320 4578 616d  .        ## Exam
-00028530: 706c 650d 0a20 2020 2020 2020 2060 6060  ple..        ```
-00028540: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
-00028550: 2020 2020 3e3e 3e20 6765 6f5f 6672 6564      >>> geo_fred
-00028560: 203d 2047 656f 4652 4544 2861 7069 5f6b   = GeoFRED(api_k
-00028570: 6579 3d27 6162 6364 6566 6768 696a 6b6c  ey='abcdefghijkl
-00028580: 6d6e 6f70 7172 7374 7576 7778 797a 3132  mnopqrstuvwxyz12
-00028590: 3334 3536 2729 0d0a 2020 2020 2020 2020  3456')..        
-000285a0: 2020 2020 3e3e 3e20 7072 696e 7428 6765      >>> print(ge
-000285b0: 6f5f 6672 6564 2e73 6572 6965 735f 6772  o_fred.series_gr
-000285c0: 6f75 7028 7365 7269 6573 5f69 643d 2753  oup(series_id='S
-000285d0: 4d55 3536 3030 3030 3030 3530 3030 3030  MU56000000500000
-000285e0: 3030 3161 2729 290d 0a20 2020 2020 2020  001a'))..       
-000285f0: 2020 2020 2053 6572 6965 7347 726f 7570       SeriesGroup
-00028600: 2874 6974 6c65 3d27 416c 6c20 456d 706c  (title='All Empl
-00028610: 6f79 6565 733a 2054 6f74 616c 2050 7269  oyees: Total Pri
-00028620: 7661 7465 272c 2072 6567 696f 6e5f 7479  vate', region_ty
-00028630: 7065 3d27 7374 6174 6527 2c20 7365 7269  pe='state', seri
-00028640: 6573 5f67 726f 7570 3d27 3132 3233 272c  es_group='1223',
-00028650: 2073 6561 736f 6e3d 274e 5341 272c 2075   season='NSA', u
-00028660: 6e69 7473 3d27 5468 6f75 7361 6e64 7320  nits='Thousands 
-00028670: 6f66 2050 6572 736f 6e73 272c 2066 7265  of Persons', fre
-00028680: 7175 656e 6379 3d27 6127 2c20 6d69 6e5f  quency='a', min_
-00028690: 6461 7465 3d64 6174 6574 696d 652e 6461  date=datetime.da
-000286a0: 7465 2831 3939 302c 2031 2c20 3129 2c20  te(1990, 1, 1), 
-000286b0: 6d61 785f 6461 7465 3d64 6174 6574 696d  max_date=datetim
-000286c0: 652e 6461 7465 2832 3032 302c 2031 2c20  e.date(2020, 1, 
-000286d0: 3129 290d 0a20 2020 2020 2020 2060 6060  1))..        ```
-000286e0: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
-000286f0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00028700: 7365 6c66 2e5f 636c 6965 6e74 2e67 6574  self._client.get
-00028710: 280d 0a20 2020 2020 2020 2020 2020 2027  (..            '
-00028720: 2f67 656f 6672 6564 2f73 6572 6965 732f  /geofred/series/
-00028730: 6772 6f75 7027 2c0d 0a20 2020 2020 2020  group',..       
-00028740: 2020 2020 2027 7365 7269 6573 5f67 726f       'series_gro
-00028750: 7570 272c 0d0a 2020 2020 2020 2020 2020  up',..          
-00028760: 2020 7365 7269 6573 5f69 643d 7365 7269    series_id=seri
-00028770: 6573 5f69 640d 0a20 2020 2020 2020 2029  es_id..        )
-00028780: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-00028790: 726e 206d 6f64 656c 732e 5365 7269 6573  rn models.Series
-000287a0: 4772 6f75 7028 2a2a 6461 7461 5b30 5d29  Group(**data[0])
-000287b0: 0d0a 0d0a 2020 2020 6465 6620 7365 7269  ....    def seri
-000287c0: 6573 5f64 6174 6128 7365 6c66 2c20 7365  es_data(self, se
-000287d0: 7269 6573 5f69 643a 2073 7472 2c20 6461  ries_id: str, da
-000287e0: 7465 3a20 6461 7465 203d 204e 6f6e 652c  te: date = None,
-000287f0: 2073 7461 7274 5f64 6174 653a 2064 6174   start_date: dat
-00028800: 6520 3d20 4e6f 6e65 2920 2d3e 2070 642e  e = None) -> pd.
-00028810: 4461 7461 4672 616d 653a 0d0a 2020 2020  DataFrame:..    
-00028820: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00028830: 2023 2320 5061 7261 6d65 7465 7273 0d0a   ## Parameters..
-00028840: 0d0a 2020 2020 2020 2020 6073 6572 6965  ..        `serie
-00028850: 735f 6964 600d 0a20 2020 2020 2020 2054  s_id`..        T
-00028860: 6865 2046 5245 4420 7365 7269 6573 5f69  he FRED series_i
-00028870: 6420 796f 7520 7761 6e74 2074 6f20 7265  d you want to re
-00028880: 7175 6573 7420 4765 6f46 5245 4420 6461  quest GeoFRED da
-00028890: 7461 2066 6f72 2e20 4e6f 7420 616c 6c20  ta for. Not all 
-000288a0: 7365 7269 6573 2074 6861 7420 6172 6520  series that are 
-000288b0: 696e 2046 5245 4420 6861 7665 2067 656f  in FRED have geo
-000288c0: 6772 6170 6869 6361 6c20 6461 7461 2e0d  graphical data..
-000288d0: 0a0d 0a20 2020 2020 2020 2060 6461 7465  ...        `date
-000288e0: 600d 0a20 2020 2020 2020 2054 6865 2064  `..        The d
-000288f0: 6174 6520 796f 7520 7761 6e74 2074 6f20  ate you want to 
-00028900: 7265 7175 6573 7420 7365 7269 6573 2067  request series g
-00028910: 726f 7570 2064 6174 6120 6672 6f6d 2e0d  roup data from..
-00028920: 0a0d 0a20 2020 2020 2020 2060 7374 6172  ...        `star
-00028930: 745f 6461 7465 600d 0a20 2020 2020 2020  t_date`..       
-00028940: 2054 6865 2073 7461 7274 2064 6174 6520   The start date 
-00028950: 796f 7520 7761 6e74 2074 6f20 7265 7175  you want to requ
-00028960: 6573 7420 7365 7269 6573 2067 726f 7570  est series group
-00028970: 2064 6174 6120 6672 6f6d 2e20 5468 6973   data from. This
-00028980: 2061 6c6c 6f77 7320 796f 7520 746f 2070   allows you to p
-00028990: 756c 6c20 6120 7261 6e67 6520 6f66 2064  ull a range of d
-000289a0: 6174 610d 0a0d 0a20 2020 2020 2020 2023  ata....        #
-000289b0: 2320 4465 7363 7269 7074 696f 6e0d 0a20  # Description.. 
-000289c0: 2020 2020 2020 2068 7474 7073 3a2f 2f67         https://g
-000289d0: 656f 6672 6564 2e73 746c 6f75 6973 6665  eofred.stlouisfe
-000289e0: 642e 6f72 672f 646f 6373 2f61 7069 2f67  d.org/docs/api/g
-000289f0: 656f 6672 6564 2f73 6572 6965 735f 6461  eofred/series_da
-00028a00: 7461 2e68 746d 6c0d 0a0d 0a20 2020 2020  ta.html....     
-00028a10: 2020 2054 6869 7320 7265 7175 6573 7420     This request 
-00028a20: 7265 7475 726e 7320 6120 6372 6f73 7320  returns a cross 
-00028a30: 7365 6374 696f 6e20 6f66 2072 6567 696f  section of regio
-00028a40: 6e61 6c20 6461 7461 2066 6f72 2061 2073  nal data for a s
-00028a50: 7065 6369 6669 6564 2072 656c 6561 7365  pecified release
-00028a60: 2064 6174 652e 0d0a 2020 2020 2020 2020   date...        
-00028a70: 4966 206e 6f20 6461 7465 2069 7320 7370  If no date is sp
-00028a80: 6563 6966 6965 642c 2074 6865 206d 6f73  ecified, the mos
-00028a90: 7420 7265 6365 6e74 2064 6174 6120 6176  t recent data av
-00028aa0: 6169 6c61 626c 6520 6172 6520 7265 7475  ailable are retu
-00028ab0: 726e 6564 2e0d 0a0d 0a20 2020 2020 2020  rned.....       
-00028ac0: 2023 2320 4150 4920 5265 7175 6573 7420   ## API Request 
-00028ad0: 2848 5454 5053 2047 4554 290d 0a20 2020  (HTTPS GET)..   
-00028ae0: 2020 2020 2068 7474 7073 3a2f 2f61 7069       https://api
-00028af0: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
-00028b00: 6765 6f66 7265 642f 7365 7269 6573 2f64  geofred/series/d
-00028b10: 6174 613f 7365 7269 6573 5f69 643d 5749  ata?series_id=WI
-00028b20: 5043 5049 2661 7069 5f6b 6579 3d61 6263  PCPI&api_key=abc
-00028b30: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
-00028b40: 7475 7677 7879 7a31 3233 3435 3626 6461  tuvwxyz123456&da
-00028b50: 7465 3d32 3031 322d 3031 2d30 310d 0a0d  te=2012-01-01...
-00028b60: 0a20 2020 2020 2020 2023 2320 4150 4920  .        ## API 
-00028b70: 5265 7370 6f6e 7365 0d0a 2020 2020 2020  Response..      
-00028b80: 2020 6060 606a 736f 6e0d 0a20 2020 2020    ```json..     
-00028b90: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00028ba0: 226d 6574 6122 3a20 7b0d 0a20 2020 2020  "meta": {..     
-00028bb0: 2020 2020 2020 2022 7469 746c 6522 3a20         "title": 
-00028bc0: 2250 6572 2043 6170 6974 6120 5065 7273  "Per Capita Pers
-00028bd0: 6f6e 616c 2049 6e63 6f6d 6520 6279 2053  onal Income by S
-00028be0: 7461 7465 2028 446f 6c6c 6172 7329 222c  tate (Dollars)",
-00028bf0: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-00028c00: 6567 696f 6e22 3a20 2273 7461 7465 222c  egion": "state",
-00028c10: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
-00028c20: 6561 736f 6e61 6c69 7479 223a 2022 4e6f  easonality": "No
-00028c30: 7420 5365 6173 6f6e 616c 6c79 2041 646a  t Seasonally Adj
-00028c40: 7573 7465 6422 2c0d 0a20 2020 2020 2020  usted",..       
-00028c50: 2020 2020 2022 756e 6974 7322 3a20 2244       "units": "D
-00028c60: 6f6c 6c61 7273 222c 0d0a 2020 2020 2020  ollars",..      
-00028c70: 2020 2020 2020 2266 7265 7175 656e 6379        "frequency
-00028c80: 223a 2022 416e 6e75 616c 222c 0d0a 2020  ": "Annual",..  
-00028c90: 2020 2020 2020 2020 2020 2264 6174 6522            "date"
-00028ca0: 3a20 2232 3031 322d 3031 2d30 3122 2c0d  : "2012-01-01",.
-00028cb0: 0a20 2020 2020 2020 2020 2020 2022 6461  .            "da
-00028cc0: 7461 223a 207b 0d0a 2020 2020 2020 2020  ta": {..        
-00028cd0: 2020 2020 2020 2232 3032 3022 3a20 5b0d        "2020": [.
-00028ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028cf0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00028d00: 2020 2020 2020 2272 6567 696f 6e22 3a20        "region": 
-00028d10: 2241 6c61 6261 6d61 222c 0d0a 2020 2020  "Alabama",..    
-00028d20: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00028d30: 6f64 6522 3a20 2230 3122 2c0d 0a20 2020  ode": "01",..   
-00028d40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00028d50: 7661 6c75 6522 3a20 2234 3634 3739 2e30  value": "46479.0
-00028d60: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00028d70: 2020 2020 2020 2273 6572 6965 735f 6964        "series_id
-00028d80: 223a 2022 414c 5043 5049 220d 0a20 2020  ": "ALPCPI"..   
-00028d90: 2020 2020 2020 2020 2020 2020 207d 2c0d               },.
-00028da0: 0a20 2020 2020 2020 2020 2020 2020 202e  .              .
-00028db0: 2e2e 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00028dc0: 5d0d 0a20 2020 2020 2020 2020 207d 0d0a  ]..          }..
-00028dd0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00028de0: 2020 2060 6060 0d0a 0d0a 2020 2020 2020     ```....      
-00028df0: 2020 2323 2052 6574 7572 6e73 0d0a 2020    ## Returns..  
-00028e00: 2020 2020 2020 6070 616e 6461 732e 4461        `pandas.Da
-00028e10: 7461 4672 616d 6560 0d0a 0d0a 2020 2020  taFrame`....    
-00028e20: 2020 2020 2323 2045 7861 6d70 6c65 2028      ## Example (
-00028e30: 6070 616e 6461 732e 4461 7461 4672 616d  `pandas.DataFram
-00028e40: 6560 290d 0a20 2020 2020 2020 2060 6060  e`)..        ```
-00028e50: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
-00028e60: 3e3e 3e20 6765 6f5f 6672 6564 203d 2047  >>> geo_fred = G
-00028e70: 656f 4652 4544 2861 7069 5f6b 6579 3d27  eoFRED(api_key='
-00028e80: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
-00028e90: 7172 7374 7576 7778 797a 3132 3334 3536  qrstuvwxyz123456
-00028ea0: 2729 0d0a 2020 2020 2020 2020 3e3e 3e20  ')..        >>> 
-00028eb0: 6765 6f5f 6672 6564 2e73 6572 6965 735f  geo_fred.series_
-00028ec0: 6461 7461 2873 6572 6965 735f 6964 3d27  data(series_id='
-00028ed0: 5749 5043 5049 2729 0d0a 2020 2020 2020  WIPCPI')..      
-00028ee0: 2020 2020 2020 2020 2072 6567 696f 6e20           region 
-00028ef0: 636f 6465 2020 2020 7661 6c75 6520 7365  code    value se
-00028f00: 7269 6573 5f69 6420 2079 6561 720d 0a20  ries_id  year.. 
-00028f10: 2020 2020 2020 2030 2020 2020 2041 6c61         0     Ala
-00028f20: 6261 6d61 2020 2030 3120 2034 3634 3739  bama   01  46479
-00028f30: 2e30 2020 2020 414c 5043 5049 2020 3230  .0    ALPCPI  20
-00028f40: 3230 0d0a 2020 2020 2020 2020 3120 2020  20..        1   
-00028f50: 2020 2041 6c61 736b 6120 2020 3032 2020     Alaska   02  
-00028f60: 3633 3530 322e 3020 2020 2041 4b50 4350  63502.0    AKPCP
-00028f70: 4920 2032 3032 300d 0a20 2020 2020 2020  I  2020..       
-00028f80: 2032 2020 2020 2041 7269 7a6f 6e61 2020   2     Arizona  
-00028f90: 2030 3420 2034 3936 3438 2e30 2020 2020   04  49648.0    
-00028fa0: 415a 5043 5049 2020 3230 3230 0d0a 2020  AZPCPI  2020..  
-00028fb0: 2020 2020 2020 3320 2020 2041 726b 616e        3    Arkan
-00028fc0: 7361 7320 2020 3035 2020 3437 3233 352e  sas   05  47235.
-00028fd0: 3020 2020 2041 5250 4350 4920 2032 3032  0    ARPCPI  202
-00028fe0: 300d 0a20 2020 2020 2020 2034 2020 4361  0..        4  Ca
-00028ff0: 6c69 666f 726e 6961 2020 2030 3620 2037  lifornia   06  7
-00029000: 3031 3932 2e30 2020 2020 4341 5043 5049  0192.0    CAPCPI
-00029010: 2020 3230 3230 0d0a 2020 2020 2020 2020    2020..        
-00029020: 6060 600d 0a20 2020 2020 2020 2022 2222  ```..        """
-00029030: 0d0a 0d0a 2020 2020 2020 2020 7965 6172  ....        year
-00029040: 7320 3d20 7365 6c66 2e5f 636c 6965 6e74  s = self._client
-00029050: 2e67 6574 280d 0a20 2020 2020 2020 2020  .get(..         
-00029060: 2020 2027 2f67 656f 6672 6564 2f73 6572     '/geofred/ser
-00029070: 6965 732f 6461 7461 272c 0d0a 2020 2020  ies/data',..    
-00029080: 2020 2020 2020 2020 276d 6574 612e 6461          'meta.da
-00029090: 7461 272c 0d0a 2020 2020 2020 2020 2020  ta',..          
-000290a0: 2020 7365 7269 6573 5f69 643d 7365 7269    series_id=seri
-000290b0: 6573 5f69 642c 0d0a 2020 2020 2020 2020  es_id,..        
-000290c0: 2020 2020 6461 7465 3d64 6174 652c 0d0a      date=date,..
-000290d0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-000290e0: 745f 6461 7465 3d73 7461 7274 5f64 6174  t_date=start_dat
-000290f0: 650d 0a20 2020 2020 2020 2029 0d0a 0d0a  e..        )....
-00029100: 2020 2020 2020 2020 6466 203d 2070 642e          df = pd.
-00029110: 4461 7461 4672 616d 6528 0d0a 2020 2020  DataFrame(..    
-00029120: 2020 2020 2020 2020 7365 6c66 2e5f 6164          self._ad
-00029130: 645f 7965 6172 7328 7965 6172 735b 305d  d_years(years[0]
-00029140: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
-00029150: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
-00029160: 662e 656d 7074 793a 0d0a 2020 2020 2020  f.empty:..      
-00029170: 2020 2020 2020 6466 2e76 616c 7565 203d        df.value =
-00029180: 2064 662e 7661 6c75 652e 7265 706c 6163   df.value.replac
-00029190: 6528 7365 6c66 2e45 4d50 5459 5f56 414c  e(self.EMPTY_VAL
-000291a0: 5545 2c20 6e70 2e6e 616e 290d 0a0d 0a20  UE, np.nan).... 
-000291b0: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
-000291c0: 6466 2e61 7374 7970 6528 6474 7970 653d  df.astype(dtype=
-000291d0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-000291e0: 2020 2027 7661 6c75 6527 3a20 2766 6c6f     'value': 'flo
-000291f0: 6174 3634 272c 0d0a 2020 2020 2020 2020  at64',..        
-00029200: 2020 2020 2020 2020 2779 6561 7227 3a20          'year': 
-00029210: 2769 6e74 3634 270d 0a20 2020 2020 2020  'int64'..       
-00029220: 2020 2020 207d 290d 0a0d 0a20 2020 2020       })....     
-00029230: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
-00029240: 2020 2020 6465 6620 7265 6769 6f6e 616c      def regional
-00029250: 5f64 6174 6128 0d0a 2020 2020 2020 2020  _data(..        
-00029260: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-00029270: 2020 2020 2020 2073 6572 6965 735f 6772         series_gr
-00029280: 6f75 703a 2073 7472 2c0d 0a20 2020 2020  oup: str,..     
-00029290: 2020 2020 2020 2072 6567 696f 6e5f 7479         region_ty
-000292a0: 7065 3a20 656e 756d 732e 5265 6769 6f6e  pe: enums.Region
-000292b0: 5479 7065 2c0d 0a20 2020 2020 2020 2020  Type,..         
-000292c0: 2020 2064 6174 653a 2064 6174 652c 0d0a     date: date,..
-000292d0: 2020 2020 2020 2020 2020 2020 7365 6173              seas
-000292e0: 6f6e 3a20 656e 756d 732e 5365 6173 6f6e  on: enums.Season
-000292f0: 616c 6974 792c 0d0a 2020 2020 2020 2020  ality,..        
-00029300: 2020 2020 756e 6974 733a 2073 7472 203d      units: str =
-00029310: 2027 446f 6c6c 6172 7327 2c20 2023 2044   'Dollars',  # D
-00029320: 6f63 756d 656e 7461 7469 6f6e 2069 7320  ocumentation is 
-00029330: 6d69 7373 696e 670d 0a20 2020 2020 2020  missing..       
-00029340: 2020 2020 2073 7461 7274 5f64 6174 653a       start_date:
-00029350: 2064 6174 6520 3d20 4e6f 6e65 2c0d 0a20   date = None,.. 
-00029360: 2020 2020 2020 2020 2020 2066 7265 7175             frequ
-00029370: 656e 6379 3a20 656e 756d 732e 4672 6571  ency: enums.Freq
-00029380: 7565 6e63 7920 3d20 4e6f 6e65 2c0d 0a20  uency = None,.. 
-00029390: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-000293a0: 666f 726d 6174 696f 6e3a 2065 6e75 6d73  formation: enums
-000293b0: 2e55 6e69 7420 3d20 656e 756d 732e 556e  .Unit = enums.Un
-000293c0: 6974 2e6c 696e 2c0d 0a20 2020 2020 2020  it.lin,..       
-000293d0: 2020 2020 2061 6767 7265 6761 7469 6f6e       aggregation
-000293e0: 5f6d 6574 686f 643a 2065 6e75 6d73 2e41  _method: enums.A
-000293f0: 6767 7265 6761 7469 6f6e 4d65 7468 6f64  ggregationMethod
-00029400: 203d 2065 6e75 6d73 2e41 6767 7265 6761   = enums.Aggrega
-00029410: 7469 6f6e 4d65 7468 6f64 2e61 7665 7261  tionMethod.avera
-00029420: 6765 0d0a 2020 2020 2920 2d3e 2070 642e  ge..    ) -> pd.
-00029430: 4461 7461 4672 616d 653a 0d0a 2020 2020  DataFrame:..    
-00029440: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00029450: 2023 2320 5061 7261 6d65 7465 7273 0d0a   ## Parameters..
-00029460: 0d0a 2020 2020 2020 2020 6073 6572 6965  ..        `serie
-00029470: 735f 6772 6f75 7060 0d0a 2020 2020 2020  s_group`..      
-00029480: 2020 5468 6520 4944 2066 6f72 2061 2067    The ID for a g
-00029490: 726f 7570 206f 6620 7365 7269 6573 7320  roup of seriess 
-000294a0: 666f 756e 6420 696e 2047 656f 4652 4544  found in GeoFRED
-000294b0: 2e0d 0a0d 0a20 2020 2020 2020 2060 7265  .....        `re
-000294c0: 6769 6f6e 5f74 7970 6560 0d0a 2020 2020  gion_type`..    
-000294d0: 2020 2020 5468 6520 7265 6769 6f6e 2079      The region y
-000294e0: 6f75 2077 616e 7420 7761 6e74 2074 6f20  ou want want to 
-000294f0: 7075 6c6c 2064 6174 6120 666f 722e 0d0a  pull data for...
-00029500: 0d0a 2020 2020 2020 2020 6064 6174 650d  ..        `date.
-00029510: 0a20 2020 2020 2020 2054 6865 2064 6174  .        The dat
-00029520: 6520 796f 7520 7761 6e74 2074 6f20 7075  e you want to pu
-00029530: 6c6c 2061 2073 6572 6965 7320 6772 6f75  ll a series grou
-00029540: 7020 6461 7461 2066 726f 6d2e 0d0a 0d0a  p data from.....
-00029550: 2020 2020 2020 2020 6073 7461 7274 5f64          `start_d
-00029560: 6174 6560 0d0a 2020 2020 2020 2020 5468  ate`..        Th
-00029570: 6520 7374 6172 7420 6461 7465 2079 6f75  e start date you
-00029580: 2077 616e 7420 746f 2072 6571 7565 7374   want to request
-00029590: 2073 6572 6965 7320 6772 6f75 7020 6461   series group da
-000295a0: 7461 2066 726f 6d2e 0d0a 2020 2020 2020  ta from...      
-000295b0: 2020 5468 6973 2061 6c6c 6f77 7320 796f    This allows yo
-000295c0: 7520 746f 2070 756c 6c20 6120 7261 6e67  u to pull a rang
-000295d0: 6520 6f66 2064 6174 610d 0a0d 0a20 2020  e of data....   
-000295e0: 2020 2020 2060 756e 6974 7360 0d0a 2020       `units`..  
-000295f0: 2020 2020 2020 5468 6520 756e 6974 7320        The units 
-00029600: 6f66 2074 6865 2073 6572 6965 7320 796f  of the series yo
-00029610: 7520 7761 6e74 2074 6f20 7075 6c6c 2e0d  u want to pull..
-00029620: 0a0d 0a20 2020 2020 2020 2060 7365 6173  ...        `seas
-00029630: 6f6e 600d 0a20 2020 2020 2020 2054 6865  on`..        The
-00029640: 2073 6561 736f 6e61 6c69 7479 206f 6620   seasonality of 
-00029650: 7468 6520 7365 7269 6573 2067 726f 7570  the series group
-00029660: 2e0d 0a0d 0a20 2020 2020 2020 2060 6672  .....        `fr
-00029670: 6571 7565 6e63 7960 0d0a 2020 2020 2020  equency`..      
-00029680: 2020 416e 206f 7074 696f 6e61 6c20 7061    An optional pa
-00029690: 7261 6d65 7465 7220 7468 6174 2069 6e64  rameter that ind
-000296a0: 6963 6174 6573 2061 206c 6f77 6572 2066  icates a lower f
-000296b0: 7265 7175 656e 6379 2074 6f20 6167 6772  requency to aggr
-000296c0: 6567 6174 6520 7661 6c75 6573 2074 6f2e  egate values to.
-000296d0: 0d0a 2020 2020 2020 2020 5468 6520 4765  ..        The Ge
-000296e0: 6f46 5245 4420 6672 6571 7565 6e63 7920  oFRED frequency 
-000296f0: 6167 6772 6567 6174 696f 6e20 6665 6174  aggregation feat
-00029700: 7572 6520 636f 6e76 6572 7473 2068 6967  ure converts hig
-00029710: 6865 7220 6672 6571 7565 6e63 7920 6461  her frequency da
-00029720: 7461 2073 6572 6965 7320 696e 746f 206c  ta series into l
-00029730: 6f77 6572 2066 7265 7175 656e 6379 2064  ower frequency d
-00029740: 6174 6120 7365 7269 6573 2028 652e 672e  ata series (e.g.
-00029750: 2063 6f6e 7665 7274 7320 6120 6d6f 6e74   converts a mont
-00029760: 686c 7920 6461 7461 2073 6572 6965 7320  hly data series 
-00029770: 696e 746f 2061 6e20 616e 6e75 616c 2064  into an annual d
-00029780: 6174 6120 7365 7269 6573 292e 0d0a 2020  ata series)...  
-00029790: 2020 2020 2020 496e 2047 656f 4652 4544        In GeoFRED
-000297a0: 2c20 7468 6520 6869 6768 6573 7420 6672  , the highest fr
-000297b0: 6571 7565 6e63 7920 6461 7461 2069 7320  equency data is 
-000297c0: 6461 696c 792c 2061 6e64 2074 6865 206c  daily, and the l
-000297d0: 6f77 6573 7420 6672 6571 7565 6e63 7920  owest frequency 
-000297e0: 6461 7461 2069 7320 616e 6e75 616c 2e0d  data is annual..
-000297f0: 0a20 2020 2020 2020 2054 6865 7265 2061  .        There a
-00029800: 7265 2033 2061 6767 7265 6761 7469 6f6e  re 3 aggregation
-00029810: 206d 6574 686f 6473 2061 7661 696c 6162   methods availab
-00029820: 6c65 2d20 6176 6572 6167 652c 2073 756d  le- average, sum
-00029830: 2c20 616e 6420 656e 6420 6f66 2070 6572  , and end of per
-00029840: 696f 642e 0d0a 2020 2020 2020 2020 5365  iod...        Se
-00029850: 6520 7468 6520 6167 6772 6567 6174 696f  e the aggregatio
-00029860: 6e5f 6d65 7468 6f64 2070 6172 616d 6574  n_method paramet
-00029870: 6572 2e0d 0a0d 0a20 2020 2020 2020 2060  er.....        `
-00029880: 7472 616e 7366 6f72 6d61 7469 6f6e 600d  transformation`.
-00029890: 0a20 2020 2020 2020 2041 206b 6579 2074  .        A key t
-000298a0: 6861 7420 696e 6469 6361 7465 7320 6120  hat indicates a 
-000298b0: 6461 7461 2076 616c 7565 2074 7261 6e73  data value trans
-000298c0: 666f 726d 6174 696f 6e2e 0d0a 0d0a 2020  formation.....  
-000298d0: 2020 2020 2020 2323 2044 6573 6372 6970        ## Descrip
-000298e0: 7469 6f6e 0d0a 2020 2020 2020 2020 6874  tion..        ht
-000298f0: 7470 733a 2f2f 6765 6f66 7265 642e 7374  tps://geofred.st
-00029900: 6c6f 7569 7366 6564 2e6f 7267 2f64 6f63  louisfed.org/doc
-00029910: 732f 6170 692f 6765 6f66 7265 642f 7265  s/api/geofred/re
-00029920: 6769 6f6e 616c 5f64 6174 612e 6874 6d6c  gional_data.html
-00029930: 0d0a 0d0a 2020 2020 2020 2020 5468 6973  ....        This
-00029940: 2072 6571 7565 7374 2072 6574 7572 6e73   request returns
-00029950: 2061 2063 726f 7373 2073 6563 7469 6f6e   a cross section
-00029960: 206f 6620 7265 6769 6f6e 616c 2064 6174   of regional dat
-00029970: 610d 0a0d 0a20 2020 2020 2020 2023 2320  a....        ## 
-00029980: 4150 4920 5265 7175 6573 7420 2848 5454  API Request (HTT
-00029990: 5053 2047 4554 290d 0a20 2020 2020 2020  PS GET)..       
-000299a0: 2068 7474 7073 3a2f 2f61 7069 2e73 746c   https://api.stl
-000299b0: 6f75 6973 6665 642e 6f72 672f 6765 6f66  ouisfed.org/geof
-000299c0: 7265 642f 7265 6769 6f6e 616c 2f64 6174  red/regional/dat
-000299d0: 613f 6170 695f 6b65 793d 6162 6364 6566  a?api_key=abcdef
-000299e0: 6768 696a 6b6c 6d6e 6f70 7172 7374 7576  ghijklmnopqrstuv
-000299f0: 7778 797a 3132 3334 3536 2673 6572 6965  wxyz123456&serie
-00029a00: 735f 6772 6f75 703d 3838 3226 6461 7465  s_group=882&date
-00029a10: 3d32 3031 332d 3031 2d30 3126 7265 6769  =2013-01-01&regi
-00029a20: 6f6e 5f74 7970 653d 7374 6174 6526 756e  on_type=state&un
-00029a30: 6974 733d 446f 6c6c 6172 7326 6672 6571  its=Dollars&freq
-00029a40: 7565 6e63 793d 6126 7365 6173 6f6e 3d4e  uency=a&season=N
-00029a50: 5341 0d0a 2020 2020 2020 2020 2323 2041  SA..        ## A
-00029a60: 5049 2052 6573 706f 6e73 650d 0a20 2020  PI Response..   
-00029a70: 2020 2020 2060 6060 6a73 6f6e 0d0a 2020       ```json..  
-00029a80: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00029a90: 2020 2022 6d65 7461 223a 207b 0d0a 2020     "meta": {..  
-00029aa0: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
-00029ab0: 223a 2022 5065 7220 4361 7069 7461 2050  ": "Per Capita P
-00029ac0: 6572 736f 6e61 6c20 496e 636f 6d65 2062  ersonal Income b
-00029ad0: 7920 5374 6174 6520 2844 6f6c 6c61 7273  y State (Dollars
-00029ae0: 2922 2c0d 0a20 2020 2020 2020 2020 2020  )",..           
-00029af0: 2022 7265 6769 6f6e 223a 2022 7374 6174   "region": "stat
-00029b00: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-00029b10: 2022 7365 6173 6f6e 616c 6974 7922 3a20   "seasonality": 
-00029b20: 224e 6f74 2053 6561 736f 6e61 6c6c 7920  "Not Seasonally 
-00029b30: 4164 6a75 7374 6564 222c 0d0a 2020 2020  Adjusted",..    
-00029b40: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-00029b50: 2022 446f 6c6c 6172 7322 2c0d 0a20 2020   "Dollars",..   
-00029b60: 2020 2020 2020 2020 2022 6672 6571 7565           "freque
-00029b70: 6e63 7922 3a20 2241 6e6e 7561 6c22 2c0d  ncy": "Annual",.
-00029b80: 0a20 2020 2020 2020 2020 2020 2022 6461  .            "da
-00029b90: 7461 223a 207b 0d0a 2020 2020 2020 2020  ta": {..        
-00029ba0: 2020 2020 2020 2232 3031 3322 3a20 5b0d        "2013": [.
-00029bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029bc0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00029bd0: 2020 2020 2020 2272 6567 696f 6e22 3a20        "region": 
-00029be0: 2241 6c61 6261 6d61 222c 0d0a 2020 2020  "Alabama",..    
-00029bf0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00029c00: 6f64 6522 3a20 2230 3122 2c0d 0a20 2020  ode": "01",..   
-00029c10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00029c20: 7661 6c75 6522 3a20 2233 3632 3538 2e30  value": "36258.0
-00029c30: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00029c40: 2020 2020 2020 2273 6572 6965 735f 6964        "series_id
-00029c50: 223a 2022 414c 5043 5049 220d 0a20 2020  ": "ALPCPI"..   
-00029c60: 2020 2020 2020 2020 2020 2020 207d 2c0d               },.
-00029c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029c80: 202e 2e2e 0d0a 2020 2020 2020 2020 2020   .....          
-00029c90: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
-00029ca0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00029cb0: 2020 7d0d 0a20 2020 2020 2020 207d 0d0a    }..        }..
-00029cc0: 2020 2020 2020 2020 6060 600d 0a0d 0a20          ```.... 
-00029cd0: 2020 2020 2020 2023 2320 5265 7475 726e         ## Return
-00029ce0: 730d 0a20 2020 2020 2020 2060 7061 6e64  s..        `pand
-00029cf0: 6173 2e44 6174 6146 7261 6d65 600d 0a0d  as.DataFrame`...
-00029d00: 0a20 2020 2020 2020 2023 2320 4578 616d  .        ## Exam
-00029d10: 706c 6520 2860 7061 6e64 6173 2e44 6174  ple (`pandas.Dat
-00029d20: 6146 7261 6d65 6029 0d0a 2020 2020 2020  aFrame`)..      
-00029d30: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
-00029d40: 2020 2020 203e 3e3e 2067 656f 5f66 7265       >>> geo_fre
-00029d50: 6420 3d20 4765 6f46 5245 4428 6170 695f  d = GeoFRED(api_
-00029d60: 6b65 793d 2761 6263 6465 6667 6869 6a6b  key='abcdefghijk
-00029d70: 6c6d 6e6f 7071 7273 7475 7677 7879 7a31  lmnopqrstuvwxyz1
-00029d80: 3233 3435 3627 290d 0a20 2020 2020 2020  23456')..       
-00029d90: 203e 3e3e 2067 656f 5f66 7265 642e 7265   >>> geo_fred.re
-00029da0: 6769 6f6e 616c 5f64 6174 6128 7365 7269  gional_data(seri
-00029db0: 6573 5f67 726f 7570 3d27 3838 3227 2c20  es_group='882', 
-00029dc0: 6461 7465 3d64 6174 6528 3230 3133 2c20  date=date(2013, 
-00029dd0: 312c 2031 292c 2072 6567 696f 6e5f 7479  1, 1), region_ty
-00029de0: 7065 3d52 6567 696f 6e54 7970 652e 7374  pe=RegionType.st
-00029df0: 6174 652c 2066 7265 7175 656e 6379 3d46  ate, frequency=F
-00029e00: 7265 7175 656e 6379 2e61 6e75 616c 2c20  requency.anual, 
-00029e10: 7365 6173 6f6e 3d53 6561 736f 6e61 6c69  season=Seasonali
-00029e20: 7479 2e6e 6f74 5f73 6561 736f 6e61 6c6c  ty.not_seasonall
-00029e30: 795f 6164 6a75 7374 6564 290d 0a20 2020  y_adjusted)..   
-00029e40: 2020 2020 2020 2020 2020 2020 7265 6769              regi
-00029e50: 6f6e 2063 6f64 6520 2020 2076 616c 7565  on code    value
-00029e60: 2073 6572 6965 735f 6964 2020 7965 6172   series_id  year
-00029e70: 0d0a 2020 2020 2020 2020 3020 2020 2020  ..        0     
-00029e80: 416c 6162 616d 6120 2020 3031 2020 3336  Alabama   01  36
-00029e90: 3235 382e 3020 2020 2041 4c50 4350 4920  258.0    ALPCPI 
-00029ea0: 2032 3031 330d 0a20 2020 2020 2020 2031   2013..        1
-00029eb0: 2020 2020 2020 416c 6173 6b61 2020 2030        Alaska   0
-00029ec0: 3220 2035 3238 3433 2e30 2020 2020 414b  2  52843.0    AK
-00029ed0: 5043 5049 2020 3230 3133 0d0a 2020 2020  PCPI  2013..    
-00029ee0: 2020 2020 3220 2020 2020 4172 697a 6f6e      2     Arizon
-00029ef0: 6120 2020 3034 2020 3336 3733 392e 3020  a   04  36739.0 
-00029f00: 2020 2041 5a50 4350 4920 2032 3031 330d     AZPCPI  2013.
-00029f10: 0a20 2020 2020 2020 2033 2020 2020 4172  .        3    Ar
-00029f20: 6b61 6e73 6173 2020 2030 3520 2033 3636  kansas   05  366
-00029f30: 3035 2e30 2020 2020 4152 5043 5049 2020  05.0    ARPCPI  
-00029f40: 3230 3133 0d0a 2020 2020 2020 2020 3420  2013..        4 
-00029f50: 2043 616c 6966 6f72 6e69 6120 2020 3036   California   06
-00029f60: 2020 3438 3534 392e 3020 2020 2043 4150    48549.0    CAP
-00029f70: 4350 4920 2032 3031 330d 0a20 2020 2020  CPI  2013..     
-00029f80: 2020 2060 6060 0d0a 2020 2020 2020 2020     ```..        
-00029f90: 2222 220d 0a0d 0a20 2020 2020 2020 2069  """....        i
-00029fa0: 6620 6672 6571 7565 6e63 7920 6973 206e  f frequency is n
-00029fb0: 6f74 204e 6f6e 6520 616e 6420 6672 6571  ot None and freq
-00029fc0: 7565 6e63 7920 6e6f 7420 696e 2065 6e75  uency not in enu
-00029fd0: 6d73 2e46 7265 7175 656e 6379 3a0d 0a20  ms.Frequency:.. 
-00029fe0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00029ff0: 2056 616c 7565 4572 726f 7228 2756 6172   ValueError('Var
-0002a000: 6961 626c 6520 6672 6571 7565 6e63 7920  iable frequency 
-0002a010: 6973 206e 6f74 206f 6e65 206f 6620 7468  is not one of th
-0002a020: 6520 7661 6c75 6573 3a20 7b7d 272e 666f  e values: {}'.fo
-0002a030: 726d 6174 2827 2c20 272e 6a6f 696e 286d  rmat(', '.join(m
-0002a040: 6170 2873 7472 2c20 656e 756d 732e 4672  ap(str, enums.Fr
-0002a050: 6571 7565 6e63 7929 2929 290d 0a0d 0a20  equency)))).... 
-0002a060: 2020 2020 2020 2069 6620 6167 6772 6567         if aggreg
-0002a070: 6174 696f 6e5f 6d65 7468 6f64 206e 6f74  ation_method not
-0002a080: 2069 6e20 656e 756d 732e 4167 6772 6567   in enums.Aggreg
-0002a090: 6174 696f 6e4d 6574 686f 643a 0d0a 2020  ationMethod:..  
-0002a0a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0002a0b0: 5661 6c75 6545 7272 6f72 2827 5661 7269  ValueError('Vari
-0002a0c0: 6162 6c65 2061 6767 7265 6761 7469 6f6e  able aggregation
-0002a0d0: 5f6d 6574 686f 6420 6973 206e 6f74 206f  _method is not o
-0002a0e0: 6e65 206f 6620 7468 6520 7661 6c75 6573  ne of the values
-0002a0f0: 3a20 7b7d 272e 666f 726d 6174 2827 2c20  : {}'.format(', 
-0002a100: 272e 6a6f 696e 286d 6170 2873 7472 2c20  '.join(map(str, 
-0002a110: 656e 756d 732e 4167 6772 6567 6174 696f  enums.Aggregatio
-0002a120: 6e4d 6574 686f 6429 2929 290d 0a0d 0a20  nMethod)))).... 
-0002a130: 2020 2020 2020 2069 6620 7472 616e 7366         if transf
-0002a140: 6f72 6d61 7469 6f6e 206e 6f74 2069 6e20  ormation not in 
-0002a150: 656e 756d 732e 556e 6974 3a0d 0a20 2020  enums.Unit:..   
-0002a160: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0002a170: 616c 7565 4572 726f 7228 2756 6172 6961  alueError('Varia
-0002a180: 626c 6520 7472 616e 7366 6f72 6d61 7469  ble transformati
-0002a190: 6f6e 2069 7320 6e6f 7420 6f6e 6520 6f66  on is not one of
-0002a1a0: 2074 6865 2076 616c 7565 733a 207b 7d27   the values: {}'
-0002a1b0: 2e66 6f72 6d61 7428 272c 2027 2e6a 6f69  .format(', '.joi
-0002a1c0: 6e28 6d61 7028 7374 722c 2065 6e75 6d73  n(map(str, enums
-0002a1d0: 2e55 6e69 7429 2929 290d 0a0d 0a20 2020  .Unit))))....   
-0002a1e0: 2020 2020 2079 6561 7273 203d 2073 656c       years = sel
-0002a1f0: 662e 5f63 6c69 656e 742e 6765 7428 0d0a  f._client.get(..
-0002a200: 2020 2020 2020 2020 2020 2020 272f 6765              '/ge
-0002a210: 6f66 7265 642f 7265 6769 6f6e 616c 2f64  ofred/regional/d
-0002a220: 6174 6127 2c0d 0a20 2020 2020 2020 2020  ata',..         
-0002a230: 2020 2027 6d65 7461 2e64 6174 6127 2c0d     'meta.data',.
-0002a240: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
-0002a250: 6965 735f 6772 6f75 703d 7365 7269 6573  ies_group=series
-0002a260: 5f67 726f 7570 2c0d 0a20 2020 2020 2020  _group,..       
-0002a270: 2020 2020 2072 6567 696f 6e5f 7479 7065       region_type
-0002a280: 3d72 6567 696f 6e5f 7479 7065 2c0d 0a20  =region_type,.. 
-0002a290: 2020 2020 2020 2020 2020 2064 6174 653d             date=
-0002a2a0: 6461 7465 2c0d 0a20 2020 2020 2020 2020  date,..         
-0002a2b0: 2020 2075 6e69 7473 3d75 6e69 7473 2c0d     units=units,.
-0002a2c0: 0a20 2020 2020 2020 2020 2020 2073 6561  .            sea
-0002a2d0: 736f 6e3d 7365 6173 6f6e 2c0d 0a20 2020  son=season,..   
-0002a2e0: 2020 2020 2020 2020 2073 7461 7274 5f64           start_d
-0002a2f0: 6174 653d 7374 6172 745f 6461 7465 2c0d  ate=start_date,.
-0002a300: 0a20 2020 2020 2020 2020 2020 2066 7265  .            fre
-0002a310: 7175 656e 6379 3d66 7265 7175 656e 6379  quency=frequency
-0002a320: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-0002a330: 7261 6e73 666f 726d 6174 696f 6e3d 7472  ransformation=tr
-0002a340: 616e 7366 6f72 6d61 7469 6f6e 2c0d 0a20  ansformation,.. 
-0002a350: 2020 2020 2020 2020 2020 2061 6767 7265             aggre
-0002a360: 6761 7469 6f6e 5f6d 6574 686f 643d 6167  gation_method=ag
-0002a370: 6772 6567 6174 696f 6e5f 6d65 7468 6f64  gregation_method
-0002a380: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
-0002a390: 2020 2020 2020 2064 6620 3d20 7064 2e44         df = pd.D
-0002a3a0: 6174 6146 7261 6d65 280d 0a20 2020 2020  ataFrame(..     
-0002a3b0: 2020 2020 2020 2073 656c 662e 5f61 6464         self._add
-0002a3c0: 5f79 6561 7273 2879 6561 7273 5b30 5d29  _years(years[0])
-0002a3d0: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
-0002a3e0: 2020 2020 2020 2069 6620 6e6f 7420 6466         if not df
-0002a3f0: 2e65 6d70 7479 3a0d 0a20 2020 2020 2020  .empty:..       
-0002a400: 2020 2020 2064 662e 7661 6c75 6520 3d20       df.value = 
-0002a410: 6466 2e76 616c 7565 2e72 6570 6c61 6365  df.value.replace
-0002a420: 2873 656c 662e 454d 5054 595f 5641 4c55  (self.EMPTY_VALU
-0002a430: 452c 206e 702e 6e61 6e29 0d0a 0d0a 2020  E, np.nan)....  
-0002a440: 2020 2020 2020 2020 2020 6466 203d 2064            df = d
-0002a450: 662e 6173 7479 7065 2864 7479 7065 3d7b  f.astype(dtype={
-0002a460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0002a470: 2020 2776 616c 7565 273a 2027 666c 6f61    'value': 'floa
-0002a480: 7436 3427 2c0d 0a20 2020 2020 2020 2020  t64',..         
-0002a490: 2020 2020 2020 2027 7965 6172 273a 2027         'year': '
-0002a4a0: 696e 7436 3427 0d0a 2020 2020 2020 2020  int64'..        
-0002a4b0: 2020 2020 7d29 0d0a 0d0a 2020 2020 2020      })....      
-0002a4c0: 2020 7265 7475 726e 2064 660d 0a0d 0a20    return df.... 
-0002a4d0: 2020 2064 6566 205f 6164 645f 7965 6172     def _add_year
-0002a4e0: 7328 7365 6c66 2c20 6461 7461 3a20 6469  s(self, data: di
-0002a4f0: 6374 2920 2d3e 2047 656e 6572 6174 6f72  ct) -> Generator
-0002a500: 5b64 6963 742c 204e 6f6e 652c 204e 6f6e  [dict, None, Non
-0002a510: 655d 3a0d 0a20 2020 2020 2020 2022 2222  e]:..        """
-0002a520: 0d0a 2020 2020 2020 2020 7472 616e 7366  ..        transf
-0002a530: 6f72 6d20 6469 6374 2069 6e64 6578 6564  orm dict indexed
-0002a540: 2062 7920 7965 6172 2066 726f 6d3a 0d0a   by year from:..
-0002a550: 2020 2020 2020 2020 6060 606a 736f 6e0d          ```json.
-0002a560: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-0002a570: 2020 2020 2020 2232 3032 3022 3a20 5b0d        "2020": [.
-0002a580: 0a20 2020 2020 2020 2020 2020 207b 0d0a  .            {..
-0002a590: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-0002a5a0: 6567 696f 6e22 3a20 2241 6c61 6261 6d61  egion": "Alabama
-0002a5b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0002a5c0: 2020 2263 6f64 6522 3a20 2230 3122 2c0d    "code": "01",.
-0002a5d0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-0002a5e0: 7661 6c75 6522 3a20 2234 3634 3739 2e30  value": "46479.0
-0002a5f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0002a600: 2020 2273 6572 6965 735f 6964 223a 2022    "series_id": "
-0002a610: 414c 5043 5049 220d 0a20 2020 2020 2020  ALPCPI"..       
-0002a620: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-0002a630: 2020 2020 202e 2e2e 0d0a 2020 2020 2020       .....      
-0002a640: 2020 2020 5d0d 0a20 2020 2020 2020 207d      ]..        }
-0002a650: 0d0a 2020 2020 2020 2020 6060 600d 0a20  ..        ```.. 
-0002a660: 2020 2020 2020 2074 6f0d 0a20 2020 2020         to..     
-0002a670: 2020 2060 6060 6a73 6f6e 0d0a 2020 2020     ```json..    
-0002a680: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
-0002a690: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-0002a6a0: 2272 6567 696f 6e22 3a20 2241 6c61 6261  "region": "Alaba
-0002a6b0: 6d61 222c 0d0a 2020 2020 2020 2020 2020  ma",..          
-0002a6c0: 2020 2263 6f64 6522 3a20 2230 3122 2c0d    "code": "01",.
-0002a6d0: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
-0002a6e0: 6c75 6522 3a20 2234 3634 3739 2e30 222c  lue": "46479.0",
-0002a6f0: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
-0002a700: 6572 6965 735f 6964 223a 2022 414c 5043  eries_id": "ALPC
-0002a710: 5049 222c 0d0a 2020 2020 2020 2020 2020  PI",..          
-0002a720: 2020 2279 6561 7222 3a20 2232 3032 3022    "year": "2020"
-0002a730: 0d0a 2020 2020 2020 2020 2020 7d2c 0d0a  ..          },..
-0002a740: 2020 2020 2020 2020 2020 2e2e 2e0d 0a20            ..... 
-0002a750: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
-0002a760: 2020 6060 600d 0a20 2020 2020 2020 2022    ```..        "
-0002a770: 2222 0d0a 2020 2020 2020 2020 666f 7220  ""..        for 
-0002a780: 7965 6172 2c20 726f 7773 2069 6e20 6461  year, rows in da
-0002a790: 7461 2e69 7465 6d73 2829 3a0d 0a20 2020  ta.items():..   
-0002a7a0: 2020 2020 2020 2020 2066 6f72 2072 6f77           for row
-0002a7b0: 2069 6e20 726f 7773 3a0d 0a20 2020 2020   in rows:..     
-0002a7c0: 2020 2020 2020 2020 2020 2072 6f77 5b27             row['
-0002a7d0: 7965 6172 275d 203d 2079 6561 720d 0a20  year'] = year.. 
-0002a7e0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-0002a7f0: 6965 6c64 2072 6f77 0d0a 0d0a 0d0a 636c  ield row......cl
-0002a800: 6173 7320 4652 4153 4552 3a0d 0a20 2020  ass FRASER:..   
-0002a810: 2022 2222 0d0a 2020 2020 4652 4153 4552   """..    FRASER
-0002a820: 2069 7320 6120 6469 6769 7461 6c20 6c69   is a digital li
-0002a830: 6272 6172 7920 6f66 2055 2e53 2e20 6563  brary of U.S. ec
-0002a840: 6f6e 6f6d 6963 2c20 6669 6e61 6e63 6961  onomic, financia
-0002a850: 6c2c 2061 6e64 2062 616e 6b69 6e67 2068  l, and banking h
-0002a860: 6973 746f 7279 e280 9470 6172 7469 6375  istory...particu
-0002a870: 6c61 726c 7920 7468 6520 6869 7374 6f72  larly the histor
-0002a880: 7920 6f66 2074 6865 2046 6564 6572 616c  y of the Federal
-0002a890: 2052 6573 6572 7665 2053 7973 7465 6d2e   Reserve System.
-0002a8a0: 0d0a 0d0a 2020 2020 5072 6f76 6964 696e  ....    Providin
-0002a8b0: 6720 6563 6f6e 6f6d 6963 2069 6e66 6f72  g economic infor
-0002a8c0: 6d61 7469 6f6e 2061 6e64 2064 6174 6120  mation and data 
-0002a8d0: 746f 2074 6865 2070 7562 6c69 6320 6973  to the public is
-0002a8e0: 2061 6e20 696d 706f 7274 616e 7420 6d69   an important mi
-0002a8f0: 7373 696f 6e20 666f 7220 7468 6520 5374  ssion for the St
-0002a900: 2e20 4c6f 7569 7320 4665 6420 7374 6172  . Louis Fed star
-0002a910: 7465 6420 6279 2066 6f72 6d65 7220 5374  ted by former St
-0002a920: 2e20 4c6f 7569 7320 4665 6420 5265 7365  . Louis Fed Rese
-0002a930: 6172 6368 2044 6972 6563 746f 7220 486f  arch Director Ho
-0002a940: 6d65 7220 4a6f 6e65 7320 696e 2031 3935  mer Jones in 195
-0002a950: 382e 0d0a 2020 2020 4652 4153 4552 2062  8...    FRASER b
-0002a960: 6567 616e 2061 7320 6120 6461 7461 2070  egan as a data p
-0002a970: 7265 7365 7276 6174 696f 6e20 616e 6420  reservation and 
-0002a980: 6163 6365 7373 6962 696c 6974 7920 7072  accessibility pr
-0002a990: 6f6a 6563 7420 6f66 2074 6865 2046 6564  oject of the Fed
-0002a9a0: 6572 616c 2052 6573 6572 7665 2042 616e  eral Reserve Ban
-0002a9b0: 6b20 6f66 2053 742e 204c 6f75 6973 2069  k of St. Louis i
-0002a9c0: 6e20 3230 3034 2061 6e64 206e 6f77 2070  n 2004 and now p
-0002a9d0: 726f 7669 6465 7320 6163 6365 7373 2074  rovides access t
-0002a9e0: 6f20 6461 7461 2061 6e64 2070 6f6c 6963  o data and polic
-0002a9f0: 7920 646f 6375 6d65 6e74 7320 6672 6f6d  y documents from
-0002aa00: 2074 6865 2046 6564 6572 616c 2052 6573   the Federal Res
-0002aa10: 6572 7665 2053 7973 7465 6d20 616e 6420  erve System and 
-0002aa20: 6d61 6e79 206f 7468 6572 2069 6e73 7469  many other insti
-0002aa30: 7475 7469 6f6e 732e 0d0a 0d0a 2020 2020  tutions.....    
-0002aa40: 6874 7470 733a 2f2f 6672 6173 6572 2e73  https://fraser.s
-0002aa50: 746c 6f75 6973 6665 642e 6f72 672f 0d0a  tlouisfed.org/..
-0002aa60: 2020 2020 6874 7470 733a 2f2f 7265 7365      https://rese
-0002aa70: 6172 6368 2e73 746c 6f75 6973 6665 642e  arch.stlouisfed.
-0002aa80: 6f72 672f 646f 6373 2f61 7069 2f66 7261  org/docs/api/fra
-0002aa90: 7365 722f 0d0a 2020 2020 2222 220d 0a0d  ser/..    """...
-0002aaa0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0002aab0: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
-0002aac0: 2020 7365 6c66 2e5f 7369 636b 6c65 203d    self._sickle =
-0002aad0: 2073 6963 6b6c 652e 5369 636b 6c65 2827   sickle.Sickle('
-0002aae0: 6874 7470 733a 2f2f 6672 6173 6572 2e73  https://fraser.s
-0002aaf0: 746c 6f75 6973 6665 642e 6f72 672f 6f61  tlouisfed.org/oa
-0002ab00: 6927 290d 0a0d 0a20 2020 2064 6566 206c  i')....    def l
-0002ab10: 6973 745f 7265 636f 7264 7328 7365 6c66  ist_records(self
-0002ab20: 2c20 6967 6e6f 7265 5f64 656c 6574 6564  , ignore_deleted
-0002ab30: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
-0002ab40: 7365 743a 2073 7472 203d 204e 6f6e 6529  set: str = None)
-0002ab50: 202d 3e20 7369 636b 6c65 2e69 7465 7261   -> sickle.itera
-0002ab60: 746f 722e 4261 7365 4f41 4949 7465 7261  tor.BaseOAIItera
-0002ab70: 746f 723a 0d0a 2020 2020 2020 2020 2222  tor:..        ""
-0002ab80: 220d 0a20 2020 2020 2020 2023 2320 5061  "..        ## Pa
-0002ab90: 7261 6d65 7465 7273 0d0a 0d0a 2020 2020  rameters....    
-0002aba0: 2020 2020 6073 6574 600d 0a20 2020 2020      `set`..     
-0002abb0: 2020 2054 6869 7320 7061 7261 6d65 7465     This paramete
-0002abc0: 7220 7370 6563 6966 6965 7320 7468 6520  r specifies the 
-0002abd0: 7365 7453 7065 6320 7661 6c75 6520 616e  setSpec value an
-0002abe0: 6420 6c69 6d69 7473 2074 6865 2072 6563  d limits the rec
-0002abf0: 6f72 6473 2074 6861 7420 6172 6520 7265  ords that are re
-0002ac00: 7472 6965 7665 6420 746f 206f 6e6c 7920  trieved to only 
-0002ac10: 7468 6f73 6520 696e 2074 6865 2073 7065  those in the spe
-0002ac20: 6369 6669 6564 2073 6574 2e0d 0a20 2020  cified set...   
-0002ac30: 2020 2020 2049 676e 6f72 6520 7468 6973       Ignore this
-0002ac40: 2070 6172 616d 6574 6572 2074 6f20 7265   parameter to re
-0002ac50: 7475 726e 2061 6c6c 2072 6563 6f72 6473  turn all records
-0002ac60: 2e0d 0a0d 0a20 2020 2020 2020 2023 2320  .....        ## 
-0002ac70: 4465 7363 7269 7074 696f 6e0d 0a20 2020  Description..   
-0002ac80: 2020 2020 2068 7474 7073 3a2f 2f72 6573       https://res
-0002ac90: 6561 7263 682e 7374 6c6f 7569 7366 6564  earch.stlouisfed
-0002aca0: 2e6f 7267 2f64 6f63 732f 6170 692f 6672  .org/docs/api/fr
-0002acb0: 6173 6572 2f6c 6973 7452 6563 6f72 6473  aser/listRecords
-0002acc0: 2e68 746d 6c0d 0a0d 0a20 2020 2020 2020  .html....       
-0002acd0: 2054 6869 7320 7265 7175 6573 7420 7265   This request re
-0002ace0: 7475 726e 7320 7469 746c 6520 7265 636f  turns title reco
-0002acf0: 7264 7320 6672 6f6d 2074 6865 2046 5241  rds from the FRA
-0002ad00: 5345 5220 7265 706f 7369 746f 7279 2e0d  SER repository..
-0002ad10: 0a20 2020 2020 2020 2041 2072 6573 756d  .        A resum
-0002ad20: 7074 696f 6e54 6f6b 656e 2063 616e 2062  ptionToken can b
-0002ad30: 6520 7573 6564 2074 6f20 7265 7472 6965  e used to retrie
-0002ad40: 7665 2061 6c6c 2072 6563 6f72 6473 2075  ve all records u
-0002ad50: 7369 6e67 206d 756c 7469 706c 6520 7265  sing multiple re
-0002ad60: 7175 6573 7473 2e0d 0a0d 0a20 2020 2020  quests.....     
-0002ad70: 2020 2041 6464 6974 696f 6e61 6c20 696e     Additional in
-0002ad80: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
-0002ad90: 616e 2069 6e64 6976 6964 7561 6c20 7469  an individual ti
-0002ada0: 746c 652c 2069 6e63 6c75 6469 6e67 2074  tle, including t
-0002adb0: 6865 2074 6974 6c65 2773 2063 6869 6c64  he title's child
-0002adc0: 2072 6563 6f72 6473 2c20 6361 6e20 6265   records, can be
-0002add0: 2072 6574 7269 6576 6564 2075 7369 6e67   retrieved using
-0002ade0: 2074 6865 2047 6574 5265 636f 7264 2072   the GetRecord r
-0002adf0: 6571 7565 7374 2e0d 0a0d 0a20 2020 2020  equest.....     
-0002ae00: 2020 2023 2320 4150 4920 5265 7175 6573     ## API Reques
-0002ae10: 7420 2848 5454 5053 2047 4554 290d 0a20  t (HTTPS GET).. 
-0002ae20: 2020 2020 2020 2068 7474 7073 3a2f 2f66         https://f
-0002ae30: 7261 7365 722e 7374 6c6f 7569 7366 6564  raser.stlouisfed
-0002ae40: 2e6f 7267 2f6f 6169 2f3f 7665 7262 3d4c  .org/oai/?verb=L
-0002ae50: 6973 7452 6563 6f72 6473 266d 6574 6164  istRecords&metad
-0002ae60: 6174 6150 7265 6669 783d 6d6f 6473 2672  ataPrefix=mods&r
-0002ae70: 6573 756d 7074 696f 6e54 6f6b 656e 3d31  esumptionToken=1
-0002ae80: 3436 3932 3939 3539 383a 300d 0a0d 0a20  469299598:0.... 
-0002ae90: 2020 2020 2020 2023 2320 5265 7475 726e         ## Return
-0002aea0: 730d 0a20 2020 2020 2020 2060 7369 636b  s..        `sick
-0002aeb0: 6c65 2e69 7465 7261 746f 722e 4261 7365  le.iterator.Base
-0002aec0: 4f41 4949 7465 7261 746f 7260 0d0a 0d0a  OAIIterator`....
-0002aed0: 2020 2020 2020 2020 2323 2045 7861 6d70          ## Examp
-0002aee0: 6c65 2028 6070 616e 6461 732e 4461 7461  le (`pandas.Data
-0002aef0: 4672 616d 6560 290d 0a20 2020 2020 2020  Frame`)..       
-0002af00: 2060 6060 7079 7468 6f6e 0d0a 2020 2020   ```python..    
-0002af10: 2020 2020 2020 2020 6672 6f6d 2070 7973          from pys
-0002af20: 746c 6f75 6973 6665 6420 696d 706f 7274  tlouisfed import
-0002af30: 2046 5241 5345 520d 0a0d 0a20 2020 2020   FRASER....     
-0002af40: 2020 2020 2020 2066 6f72 2072 6563 6f72         for recor
-0002af50: 6420 696e 2046 5241 5345 5228 292e 6c69  d in FRASER().li
-0002af60: 7374 5f72 6563 6f72 6473 2829 3a0d 0a20  st_records():.. 
-0002af70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0002af80: 7269 6e74 2872 6563 6f72 642e 6765 745f  rint(record.get_
-0002af90: 6d65 7461 6461 7461 2829 290d 0a20 2020  metadata())..   
-0002afa0: 2020 2020 2060 6060 0d0a 2020 2020 2020       ```..      
-0002afb0: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
-0002afc0: 2072 6574 7572 6e20 7365 6c66 2e5f 7369   return self._si
-0002afd0: 636b 6c65 2e4c 6973 7452 6563 6f72 6473  ckle.ListRecords
-0002afe0: 286d 6574 6164 6174 6150 7265 6669 783d  (metadataPrefix=
-0002aff0: 276d 6f64 7327 2c20 6967 6e6f 7265 5f64  'mods', ignore_d
-0002b000: 656c 6574 6564 3d69 676e 6f72 655f 6465  eleted=ignore_de
-0002b010: 6c65 7465 642c 2073 6574 3d73 6574 290d  leted, set=set).
-0002b020: 0a0d 0a20 2020 2064 6566 206c 6973 745f  ...    def list_
-0002b030: 7365 7473 2873 656c 6629 202d 3e20 7369  sets(self) -> si
-0002b040: 636b 6c65 2e69 7465 7261 746f 722e 4261  ckle.iterator.Ba
-0002b050: 7365 4f41 4949 7465 7261 746f 723a 0d0a  seOAIIterator:..
-0002b060: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0002b070: 2020 2020 2023 2320 4465 7363 7269 7074       ## Descript
-0002b080: 696f 6e0d 0a20 2020 2020 2020 2068 7474  ion..        htt
-0002b090: 7073 3a2f 2f72 6573 6561 7263 682e 7374  ps://research.st
-0002b0a0: 6c6f 7569 7366 6564 2e6f 7267 2f64 6f63  louisfed.org/doc
-0002b0b0: 732f 6170 692f 6672 6173 6572 2f6c 6973  s/api/fraser/lis
-0002b0c0: 7453 6574 732e 6874 6d6c 0d0a 0d0a 2020  tSets.html....  
-0002b0d0: 2020 2020 2020 5468 6973 2072 6571 7565        This reque
-0002b0e0: 7374 2072 6574 7572 6e73 2074 6865 2073  st returns the s
-0002b0f0: 6574 2073 7472 7563 7475 7265 2066 6f72  et structure for
-0002b100: 2072 6563 6f72 6473 2069 6e20 7468 6520   records in the 
-0002b110: 4652 4153 4552 2072 6570 6f73 6974 6f72  FRASER repositor
-0002b120: 792e 0d0a 2020 2020 2020 2020 4120 7265  y...        A re
-0002b130: 7375 6d70 7469 6f6e 546f 6b65 6e20 6361  sumptionToken ca
-0002b140: 6e20 6265 2075 7365 6420 746f 2072 6574  n be used to ret
-0002b150: 7269 6576 6520 7468 6520 636f 6d70 6c65  rieve the comple
-0002b160: 7465 2073 6574 2073 7472 7563 7475 7265  te set structure
-0002b170: 2075 7369 6e67 206d 756c 7469 706c 6520   using multiple 
-0002b180: 7265 7175 6573 7473 2e0d 0a0d 0a20 2020  requests.....   
-0002b190: 2020 2020 2023 2320 4150 4920 5265 7175       ## API Requ
-0002b1a0: 6573 7420 2848 5454 5053 2047 4554 290d  est (HTTPS GET).
-0002b1b0: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
-0002b1c0: 2f66 7261 7365 722e 7374 6c6f 7569 7366  /fraser.stlouisf
-0002b1d0: 6564 2e6f 7267 2f6f 6169 2f3f 7665 7262  ed.org/oai/?verb
-0002b1e0: 3d4c 6973 7453 6574 7326 7265 7375 6d70  =ListSets&resump
-0002b1f0: 7469 6f6e 546f 6b65 6e3d 3134 3738 3730  tionToken=147870
-0002b200: 3736 3338 3a30 0d0a 0d0a 2020 2020 2020  7638:0....      
-0002b210: 2020 2323 2052 6574 7572 6e73 0d0a 2020    ## Returns..  
-0002b220: 2020 2020 2020 6073 6963 6b6c 652e 6974        `sickle.it
-0002b230: 6572 6174 6f72 2e42 6173 654f 4149 4974  erator.BaseOAIIt
-0002b240: 6572 6174 6f72 600d 0a0d 0a20 2020 2020  erator`....     
-0002b250: 2020 2023 2320 4578 616d 706c 6520 2860     ## Example (`
-0002b260: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
-0002b270: 6029 0d0a 2020 2020 2020 2020 6060 6070  `)..        ```p
-0002b280: 7974 686f 6e0d 0a20 2020 2020 2020 2020  ython..         
-0002b290: 2020 2066 726f 6d20 7079 7374 6c6f 7569     from pystloui
-0002b2a0: 7366 6564 2069 6d70 6f72 7420 4652 4153  sfed import FRAS
-0002b2b0: 4552 0d0a 0d0a 2020 2020 2020 2020 2020  ER....          
-0002b2c0: 2020 666f 7220 7365 7420 696e 2046 5241    for set in FRA
-0002b2d0: 5345 5228 292e 6c69 7374 5f73 6574 7328  SER().list_sets(
-0002b2e0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0002b2f0: 2020 2020 7072 696e 7428 7365 7429 0d0a      print(set)..
-0002b300: 2020 2020 2020 2020 6060 600d 0a20 2020          ```..   
-0002b310: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
-0002b320: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0002b330: 5f73 6963 6b6c 652e 4c69 7374 5365 7473  _sickle.ListSets
-0002b340: 2829 0d0a 0d0a 2020 2020 6465 6620 6c69  ()....    def li
-0002b350: 7374 5f69 6465 6e74 6966 6965 7273 2873  st_identifiers(s
-0002b360: 656c 662c 2069 676e 6f72 655f 6465 6c65  elf, ignore_dele
-0002b370: 7465 643a 2062 6f6f 6c20 3d20 4661 6c73  ted: bool = Fals
-0002b380: 652c 2073 6574 3a20 7374 7220 3d20 4e6f  e, set: str = No
-0002b390: 6e65 2920 2d3e 2073 6963 6b6c 652e 6974  ne) -> sickle.it
-0002b3a0: 6572 6174 6f72 2e42 6173 654f 4149 4974  erator.BaseOAIIt
-0002b3b0: 6572 6174 6f72 3a0d 0a20 2020 2020 2020  erator:..       
-0002b3c0: 2022 2222 0d0a 2020 2020 2020 2020 2323   """..        ##
-0002b3d0: 2050 6172 616d 6574 6572 730d 0a0d 0a20   Parameters.... 
-0002b3e0: 2020 2020 2020 2060 7365 7460 0d0a 2020         `set`..  
-0002b3f0: 2020 2020 2020 5468 6973 2070 6172 616d        This param
-0002b400: 6574 6572 2073 7065 6369 6669 6573 2074  eter specifies t
-0002b410: 6865 2073 6574 5370 6563 2076 616c 7565  he setSpec value
-0002b420: 2061 6e64 206c 696d 6974 7320 7468 6520   and limits the 
-0002b430: 7265 636f 7264 7320 7468 6174 2061 7265  records that are
-0002b440: 2072 6574 7269 6576 6564 2074 6f20 6f6e   retrieved to on
-0002b450: 6c79 2074 686f 7365 2069 6e20 7468 6520  ly those in the 
-0002b460: 7370 6563 6966 6965 6420 7365 7420 4967  specified set Ig
-0002b470: 6e6f 7265 2074 6869 7320 7061 7261 6d65  nore this parame
-0002b480: 7465 7220 746f 2072 6574 7572 6e20 616c  ter to return al
-0002b490: 6c20 7265 636f 7264 732e 0d0a 0d0a 2020  l records.....  
-0002b4a0: 2020 2020 2020 2323 2044 6573 6372 6970        ## Descrip
-0002b4b0: 7469 6f6e 0d0a 2020 2020 2020 2020 6874  tion..        ht
-0002b4c0: 7470 733a 2f2f 7265 7365 6172 6368 2e73  tps://research.s
-0002b4d0: 746c 6f75 6973 6665 642e 6f72 672f 646f  tlouisfed.org/do
-0002b4e0: 6373 2f61 7069 2f66 7261 7365 722f 6c69  cs/api/fraser/li
-0002b4f0: 7374 4964 656e 7469 6669 6572 732e 6874  stIdentifiers.ht
-0002b500: 6d6c 0d0a 0d0a 2020 2020 2020 2020 5468  ml....        Th
-0002b510: 6973 2072 6571 7565 7374 2072 6574 7572  is request retur
-0002b520: 6e73 2068 6561 6465 7273 2066 6f72 2072  ns headers for r
-0002b530: 6563 6f72 6473 2069 6e20 7468 6520 4652  ecords in the FR
-0002b540: 4153 4552 2072 6570 6f73 6974 6f72 792e  ASER repository.
-0002b550: 0d0a 2020 2020 2020 2020 4120 7265 7375  ..        A resu
-0002b560: 6d70 7469 6f6e 546f 6b65 6e20 6361 6e20  mptionToken can 
-0002b570: 6265 2075 7365 6420 746f 2072 6574 7269  be used to retri
-0002b580: 6576 6520 616c 6c20 7265 636f 7264 7320  eve all records 
-0002b590: 7573 696e 6720 6d75 6c74 6970 6c65 2072  using multiple r
-0002b5a0: 6571 7565 7374 732e 0d0a 0d0a 2020 2020  equests.....    
-0002b5b0: 2020 2020 2323 2041 5049 2052 6571 7565      ## API Reque
-0002b5c0: 7374 2028 4854 5450 5320 4745 5429 0d0a  st (HTTPS GET)..
-0002b5d0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-0002b5e0: 6672 6173 6572 2e73 746c 6f75 6973 6665  fraser.stlouisfe
-0002b5f0: 642e 6f72 672f 6f61 692f 3f76 6572 623d  d.org/oai/?verb=
-0002b600: 4c69 7374 4964 656e 7469 6669 6572 7326  ListIdentifiers&
-0002b610: 7265 7375 6d70 7469 6f6e 546f 6b65 6e3d  resumptionToken=
-0002b620: 3134 3639 3330 3034 3531 3a30 0d0a 0d0a  1469300451:0....
-0002b630: 2020 2020 2020 2020 2323 2052 6574 7572          ## Retur
-0002b640: 6e73 0d0a 2020 2020 2020 2020 6073 6963  ns..        `sic
-0002b650: 6b6c 652e 6974 6572 6174 6f72 2e42 6173  kle.iterator.Bas
-0002b660: 654f 4149 4974 6572 6174 6f72 600d 0a0d  eOAIIterator`...
-0002b670: 0a20 2020 2020 2020 2023 2320 4578 616d  .        ## Exam
-0002b680: 706c 6520 2860 7061 6e64 6173 2e44 6174  ple (`pandas.Dat
-0002b690: 6146 7261 6d65 6029 0d0a 2020 2020 2020  aFrame`)..      
-0002b6a0: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
-0002b6b0: 2020 2020 2020 2020 2066 726f 6d20 7079           from py
-0002b6c0: 7374 6c6f 7569 7366 6564 2069 6d70 6f72  stlouisfed impor
-0002b6d0: 7420 4652 4153 4552 0d0a 0d0a 2020 2020  t FRASER....    
-0002b6e0: 2020 2020 2020 2020 666f 7220 6865 6164          for head
-0002b6f0: 6572 2069 6e20 4652 4153 4552 2829 2e6c  er in FRASER().l
-0002b700: 6973 745f 6964 656e 7469 6669 6572 7328  ist_identifiers(
-0002b710: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0002b720: 2020 2020 7072 696e 7428 6865 6164 6572      print(header
-0002b730: 2e69 6465 6e74 6966 6965 7229 0d0a 2020  .identifier)..  
-0002b740: 2020 2020 2020 6060 600d 0a20 2020 2020        ```..     
-0002b750: 2020 2022 2222 0d0a 0d0a 2020 2020 2020     """....      
-0002b760: 2020 7265 7475 726e 2073 656c 662e 5f73    return self._s
-0002b770: 6963 6b6c 652e 4c69 7374 4964 656e 7469  ickle.ListIdenti
-0002b780: 6669 6572 7328 6d65 7461 6461 7461 5072  fiers(metadataPr
-0002b790: 6566 6978 3d27 6d6f 6473 272c 2069 676e  efix='mods', ign
-0002b7a0: 6f72 655f 6465 6c65 7465 643d 6967 6e6f  ore_deleted=igno
-0002b7b0: 7265 5f64 656c 6574 6564 2c20 7365 743d  re_deleted, set=
-0002b7c0: 7365 7429 0d0a 0d0a 2020 2020 6465 6620  set)....    def 
-0002b7d0: 6765 745f 7265 636f 7264 2873 656c 662c  get_record(self,
-0002b7e0: 2069 6465 6e74 6966 6965 723a 2073 7472   identifier: str
-0002b7f0: 2920 2d3e 2073 6963 6b6c 652e 6d6f 6465  ) -> sickle.mode
-0002b800: 6c73 2e52 6563 6f72 643a 0d0a 2020 2020  ls.Record:..    
-0002b810: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0002b820: 2023 2320 4465 7363 7269 7074 696f 6e0d   ## Description.
-0002b830: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
-0002b840: 2f72 6573 6561 7263 682e 7374 6c6f 7569  /research.stloui
-0002b850: 7366 6564 2e6f 7267 2f64 6f63 732f 6170  sfed.org/docs/ap
-0002b860: 692f 6672 6173 6572 2f67 6574 5265 636f  i/fraser/getReco
-0002b870: 7264 2e68 746d 6c0d 0a0d 0a20 2020 2020  rd.html....     
-0002b880: 2020 2054 6869 7320 7265 7175 6573 7420     This request 
-0002b890: 7265 7475 726e 7320 6120 7369 6e67 6c65  returns a single
-0002b8a0: 2072 6563 6f72 6420 6672 6f6d 2074 6865   record from the
-0002b8b0: 2046 5241 5345 5220 7265 706f 7369 746f   FRASER reposito
-0002b8c0: 7279 2e0d 0a0d 0a20 2020 2020 2020 2023  ry.....        #
-0002b8d0: 2320 4150 4920 5265 7175 6573 7420 2848  # API Request (H
-0002b8e0: 5454 5053 2047 4554 290d 0a20 2020 2020  TTPS GET)..     
-0002b8f0: 2020 2068 7474 7073 3a2f 2f66 7261 7365     https://frase
-0002b900: 722e 7374 6c6f 7569 7366 6564 2e6f 7267  r.stlouisfed.org
-0002b910: 2f6f 6169 2f3f 7665 7262 3d47 6574 5265  /oai/?verb=GetRe
-0002b920: 636f 7264 2669 6465 6e74 6966 6965 723d  cord&identifier=
-0002b930: 6f61 693a 6672 6173 6572 2e73 746c 6f75  oai:fraser.stlou
-0002b940: 6973 6665 642e 6f72 673a 7469 746c 653a  isfed.org:title:
-0002b950: 3137 360d 0a0d 0a20 2020 2020 2020 2023  176....        #
-0002b960: 2320 5265 7475 726e 730d 0a20 2020 2020  # Returns..     
-0002b970: 2020 2060 7369 636b 6c65 2e6d 6f64 656c     `sickle.model
-0002b980: 732e 5265 636f 7264 600d 0a0d 0a20 2020  s.Record`....   
-0002b990: 2020 2020 2023 2320 4578 616d 706c 6520       ## Example 
-0002b9a0: 2860 7061 6e64 6173 2e44 6174 6146 7261  (`pandas.DataFra
-0002b9b0: 6d65 6029 0d0a 2020 2020 2020 2020 6060  me`)..        ``
-0002b9c0: 6070 7974 686f 6e0d 0a20 2020 2020 2020  `python..       
-0002b9d0: 2020 2020 2066 726f 6d20 7079 7374 6c6f       from pystlo
-0002b9e0: 7569 7366 6564 2069 6d70 6f72 7420 4652  uisfed import FR
-0002b9f0: 4153 4552 0d0a 0d0a 2020 2020 2020 2020  ASER....        
-0002ba00: 2020 2020 4652 4153 4552 2829 2e67 6574      FRASER().get
-0002ba10: 5f72 6563 6f72 6428 6964 656e 7469 6669  _record(identifi
-0002ba20: 6572 3d27 6f61 693a 6672 6173 6572 2e73  er='oai:fraser.s
-0002ba30: 746c 6f75 6973 6665 642e 6f72 673a 7469  tlouisfed.org:ti
-0002ba40: 746c 653a 3137 3627 290d 0a20 2020 2020  tle:176')..     
-0002ba50: 2020 2060 6060 0d0a 2020 2020 2020 2020     ```..        
-0002ba60: 2222 220d 0a0d 0a20 2020 2020 2020 2072  """....        r
-0002ba70: 6574 7572 6e20 7365 6c66 2e5f 7369 636b  eturn self._sick
-0002ba80: 6c65 2e47 6574 5265 636f 7264 2869 6465  le.GetRecord(ide
-0002ba90: 6e74 6966 6965 723d 6964 656e 7469 6669  ntifier=identifi
-0002baa0: 6572 2c20 6d65 7461 6461 7461 5072 6566  er, metadataPref
-0002bab0: 6978 3d27 6d6f 6473 2729 0d0a            ix='mods')..
+00025f60: 2020 2020 2020 2020 7469 746c 6520 6f62          title ob
+00025f70: 7365 7276 6174 696f 6e5f 7374 6172 7420  servation_start 
+00025f80: 6f62 7365 7276 6174 696f 6e5f 656e 6420  observation_end 
+00025f90: 2066 7265 7175 656e 6379 2066 7265 7175   frequency frequ
+00025fa0: 656e 6379 5f73 686f 7274 2020 2020 2020  ency_short      
+00025fb0: 2020 2020 2075 6e69 7473 2020 2020 2075       units     u
+00025fc0: 6e69 7473 5f73 686f 7274 2020 2020 2020  nits_short      
+00025fd0: 7365 6173 6f6e 616c 5f61 646a 7573 746d  seasonal_adjustm
+00025fe0: 656e 7420 7365 6173 6f6e 616c 5f61 646a  ent seasonal_adj
+00025ff0: 7573 746d 656e 745f 7368 6f72 7420 2020  ustment_short   
+00026000: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+00026010: 7570 6461 7465 6420 2070 6f70 756c 6172  updated  popular
+00026020: 6974 7920 2067 726f 7570 5f70 6f70 756c  ity  group_popul
+00026030: 6172 6974 7920 2020 2020 2020 2020 2020  arity           
+00026040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026060: 2020 206e 6f74 6573 0d0a 2020 2020 2020     notes..      
+00026070: 2020 2020 2020 6964 0d0a 2020 2020 2020        id..      
+00026080: 2020 2020 2020 4155 5343 5049 434f 5241        AUSCPICORA
+00026090: 494e 4d45 4920 2020 2020 3230 3232 2d30  INMEI     2022-0
+000260a0: 322d 3035 2020 2032 3032 322d 3032 2d30  2-05   2022-02-0
+000260b0: 3520 2043 6f6e 7375 6d65 7220 5072 6963  5  Consumer Pric
+000260c0: 6520 496e 6465 783a 2041 6c6c 2049 7465  e Index: All Ite
+000260d0: 6d73 2045 7863 6c75 6469 6e67 2046 6f6f  ms Excluding Foo
+000260e0: 642e 2e2e 2020 2020 2020 2020 3139 3732  d...        1972
+000260f0: 2d30 312d 3031 2020 2020 2020 3230 3230  -01-01      2020
+00026100: 2d30 312d 3031 2020 2020 2041 6e6e 7561  -01-01     Annua
+00026110: 6c20 2020 2020 2020 2020 2020 2020 2020  l               
+00026120: 4120 2049 6e64 6578 2032 3031 353d 3130  A  Index 2015=10
+00026130: 3020 2049 6e64 6578 2032 3031 353d 3130  0  Index 2015=10
+00026140: 3020 204e 6f74 2053 6561 736f 6e61 6c6c  0  Not Seasonall
+00026150: 7920 4164 6a75 7374 6564 2020 2020 2020  y Adjusted      
+00026160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026170: 204e 5341 2032 3032 312d 3032 2d31 3720   NSA 2021-02-17 
+00026180: 3138 3a32 373a 3339 2b30 303a 3030 2020  18:27:39+00:00  
+00026190: 2020 2020 2020 2020 2031 2020 2020 2020           1      
+000261a0: 2020 2020 2020 2020 2020 3132 2020 436f            12  Co
+000261b0: 7079 7269 6768 742c 2032 3031 362c 204f  pyright, 2016, O
+000261c0: 4543 442e 2052 6570 7269 6e74 6564 2077  ECD. Reprinted w
+000261d0: 6974 6820 7065 726d 6973 7369 2e2e 2e0d  ith permissi....
+000261e0: 0a20 2020 2020 2020 2020 2020 2041 5553  .            AUS
+000261f0: 4350 4943 4f52 5149 4e4d 4549 2020 2020  CPICORQINMEI    
+00026200: 2032 3032 322d 3032 2d30 3520 2020 3230   2022-02-05   20
+00026210: 3232 2d30 322d 3035 2020 436f 6e73 756d  22-02-05  Consum
+00026220: 6572 2050 7269 6365 2049 6e64 6578 3a20  er Price Index: 
+00026230: 416c 6c20 4974 656d 7320 4578 636c 7564  All Items Exclud
+00026240: 696e 6720 466f 6f64 2e2e 2e20 2020 2020  ing Food...     
+00026250: 2020 2031 3937 312d 3034 2d30 3120 2020     1971-04-01   
+00026260: 2020 2032 3032 312d 3037 2d30 3120 2051     2021-07-01  Q
+00026270: 7561 7274 6572 6c79 2020 2020 2020 2020  uarterly        
+00026280: 2020 2020 2020 2051 2020 496e 6465 7820         Q  Index 
+00026290: 3230 3135 3d31 3030 2020 496e 6465 7820  2015=100  Index 
+000262a0: 3230 3135 3d31 3030 2020 4e6f 7420 5365  2015=100  Not Se
+000262b0: 6173 6f6e 616c 6c79 2041 646a 7573 7465  asonally Adjuste
+000262c0: 6420 2020 2020 2020 2020 2020 2020 2020  d               
+000262d0: 2020 2020 2020 2020 4e53 4120 3230 3231          NSA 2021
+000262e0: 2d31 322d 3134 2032 313a 3537 3a30 342b  -12-14 21:57:04+
+000262f0: 3030 3a30 3020 2020 2020 2020 2020 2031  00:00          1
+00026300: 3220 2020 2020 2020 2020 2020 2020 2020  2               
+00026310: 2031 3220 2043 6f70 7972 6967 6874 2c20   12  Copyright, 
+00026320: 3230 3136 2c20 4f45 4344 2e20 5265 7072  2016, OECD. Repr
+00026330: 696e 7465 6420 7769 7468 2070 6572 6d69  inted with permi
+00026340: 7373 692e 2e2e 0d0a 2020 2020 2020 2020  ssi.....        
+00026350: 2020 2020 4155 5343 5049 464f 4441 494e      AUSCPIFODAIN
+00026360: 4d45 4920 2020 2020 3230 3232 2d30 322d  MEI     2022-02-
+00026370: 3035 2020 2032 3032 322d 3032 2d30 3520  05   2022-02-05 
+00026380: 2020 2020 2020 2020 2020 436f 6e73 756d            Consum
+00026390: 6572 2050 7269 6365 2049 6e64 6578 3a20  er Price Index: 
+000263a0: 466f 6f64 2066 6f72 2041 7573 7472 616c  Food for Austral
+000263b0: 6961 2020 2020 2020 2020 3139 3737 2d30  ia        1977-0
+000263c0: 312d 3031 2020 2020 2020 3230 3137 2d30  1-01      2017-0
+000263d0: 312d 3031 2020 2020 2041 6e6e 7561 6c20  1-01     Annual 
+000263e0: 2020 2020 2020 2020 2020 2020 2020 4120                A 
+000263f0: 2049 6e64 6578 2032 3031 303d 3130 3020   Index 2010=100 
+00026400: 2049 6e64 6578 2032 3031 303d 3130 3020   Index 2010=100 
+00026410: 204e 6f74 2053 6561 736f 6e61 6c6c 7920   Not Seasonally 
+00026420: 4164 6a75 7374 6564 2020 2020 2020 2020  Adjusted        
+00026430: 2020 2020 2020 2020 2020 2020 2020 204e                 N
+00026440: 5341 2032 3031 382d 3033 2d30 3920 3231  SA 2018-03-09 21
+00026450: 3a31 323a 3039 2b30 303a 3030 2020 2020  :12:09+00:00    
+00026460: 2020 2020 2020 2031 2020 2020 2020 2020         1        
+00026470: 2020 2020 2020 2020 2032 2020 436f 7079           2  Copy
+00026480: 7269 6768 742c 2032 3031 362c 204f 4543  right, 2016, OEC
+00026490: 442e 2052 6570 7269 6e74 6564 2077 6974  D. Reprinted wit
+000264a0: 6820 7065 726d 6973 7369 2e2e 2e0d 0a20  h permissi..... 
+000264b0: 2020 2020 2020 2020 2020 2041 5553 4350             AUSCP
+000264c0: 4946 4f44 5149 4e4d 4549 2020 2020 2032  IFODQINMEI     2
+000264d0: 3032 322d 3032 2d30 3520 2020 3230 3232  022-02-05   2022
+000264e0: 2d30 322d 3035 2020 2020 2020 2020 2020  -02-05          
+000264f0: 2043 6f6e 7375 6d65 7220 5072 6963 6520   Consumer Price 
+00026500: 496e 6465 783a 2046 6f6f 6420 666f 7220  Index: Food for 
+00026510: 4175 7374 7261 6c69 6120 2020 2020 2020  Australia       
+00026520: 2031 3937 362d 3037 2d30 3120 2020 2020   1976-07-01     
+00026530: 2032 3031 382d 3031 2d30 3120 2051 7561   2018-01-01  Qua
+00026540: 7274 6572 6c79 2020 2020 2020 2020 2020  rterly          
+00026550: 2020 2020 2051 2020 496e 6465 7820 3230       Q  Index 20
+00026560: 3130 3d31 3030 2020 496e 6465 7820 3230  10=100  Index 20
+00026570: 3130 3d31 3030 2020 4e6f 7420 5365 6173  10=100  Not Seas
+00026580: 6f6e 616c 6c79 2041 646a 7573 7465 6420  onally Adjusted 
+00026590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000265a0: 2020 2020 2020 4e53 4120 3230 3138 2d30        NSA 2018-0
+000265b0: 342d 3234 2031 393a 3531 3a30 342b 3030  4-24 19:51:04+00
+000265c0: 3a30 3020 2020 2020 2020 2020 2020 3220  :00           2 
+000265d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000265e0: 3220 2043 6f70 7972 6967 6874 2c20 3230  2  Copyright, 20
+000265f0: 3136 2c20 4f45 4344 2e20 5265 7072 696e  16, OECD. Reprin
+00026600: 7465 6420 7769 7468 2070 6572 6d69 7373  ted with permiss
+00026610: 692e 2e2e 0d0a 2020 2020 2020 2020 2020  i.....          
+00026620: 2020 4155 5443 5049 434f 5241 494e 4d45    AUTCPICORAINME
+00026630: 4920 2020 2020 3230 3232 2d30 322d 3035  I     2022-02-05
+00026640: 2020 2032 3032 322d 3032 2d30 3520 2043     2022-02-05  C
+00026650: 6f6e 7375 6d65 7220 5072 6963 6520 496e  onsumer Price In
+00026660: 6465 783a 2041 6c6c 2049 7465 6d73 2045  dex: All Items E
+00026670: 7863 6c75 6469 6e67 2046 6f6f 642e 2e2e  xcluding Food...
+00026680: 2020 2020 2020 2020 3139 3636 2d30 312d          1966-01-
+00026690: 3031 2020 2020 2020 3230 3230 2d30 312d  01      2020-01-
+000266a0: 3031 2020 2020 2041 6e6e 7561 6c20 2020  01     Annual   
+000266b0: 2020 2020 2020 2020 2020 2020 4120 2049              A  I
+000266c0: 6e64 6578 2032 3031 353d 3130 3020 2049  ndex 2015=100  I
+000266d0: 6e64 6578 2032 3031 353d 3130 3020 204e  ndex 2015=100  N
+000266e0: 6f74 2053 6561 736f 6e61 6c6c 7920 4164  ot Seasonally Ad
+000266f0: 6a75 7374 6564 2020 2020 2020 2020 2020  justed          
+00026700: 2020 2020 2020 2020 2020 2020 204e 5341               NSA
+00026710: 2032 3032 312d 3033 2d31 3620 3232 3a33   2021-03-16 22:3
+00026720: 373a 3537 2b30 303a 3030 2020 2020 2020  7:57+00:00      
+00026730: 2020 2020 2030 2020 2020 2020 2020 2020       0          
+00026740: 2020 2020 2020 2031 2020 436f 7079 7269         1  Copyri
+00026750: 6768 742c 2032 3031 362c 204f 4543 442e  ght, 2016, OECD.
+00026760: 2052 6570 7269 6e74 6564 2077 6974 6820   Reprinted with 
+00026770: 7065 726d 6973 7369 2e2e 2e0d 0a20 2020  permissi.....   
+00026780: 2020 2020 2060 6060 0d0a 2020 2020 2020       ```..      
+00026790: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+000267a0: 2061 6c6c 6f77 6564 5f6f 7264 6572 7320   allowed_orders 
+000267b0: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
+000267c0: 2065 6e75 6d73 2e4f 7264 6572 4279 2e73   enums.OrderBy.s
+000267d0: 6572 6965 735f 6964 2c0d 0a20 2020 2020  eries_id,..     
+000267e0: 2020 2020 2020 2065 6e75 6d73 2e4f 7264         enums.Ord
+000267f0: 6572 4279 2e74 6974 6c65 2c0d 0a20 2020  erBy.title,..   
+00026800: 2020 2020 2020 2020 2065 6e75 6d73 2e4f           enums.O
+00026810: 7264 6572 4279 2e75 6e69 7473 2c0d 0a20  rderBy.units,.. 
+00026820: 2020 2020 2020 2020 2020 2065 6e75 6d73             enums
+00026830: 2e4f 7264 6572 4279 2e66 7265 7175 656e  .OrderBy.frequen
+00026840: 6379 2c0d 0a20 2020 2020 2020 2020 2020  cy,..           
+00026850: 2065 6e75 6d73 2e4f 7264 6572 4279 2e73   enums.OrderBy.s
+00026860: 6561 736f 6e61 6c5f 6164 6a75 7374 6d65  easonal_adjustme
+00026870: 6e74 2c0d 0a20 2020 2020 2020 2020 2020  nt,..           
+00026880: 2065 6e75 6d73 2e4f 7264 6572 4279 2e72   enums.OrderBy.r
+00026890: 6561 6c74 696d 655f 7374 6172 742c 0d0a  ealtime_start,..
+000268a0: 2020 2020 2020 2020 2020 2020 656e 756d              enum
+000268b0: 732e 4f72 6465 7242 792e 7265 616c 7469  s.OrderBy.realti
+000268c0: 6d65 5f65 6e64 2c0d 0a20 2020 2020 2020  me_end,..       
+000268d0: 2020 2020 2065 6e75 6d73 2e4f 7264 6572       enums.Order
+000268e0: 4279 2e6c 6173 745f 7570 6461 7465 642c  By.last_updated,
+000268f0: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+00026900: 756d 732e 4f72 6465 7242 792e 6f62 7365  ums.OrderBy.obse
+00026910: 7276 6174 696f 6e5f 7374 6172 742c 0d0a  rvation_start,..
+00026920: 2020 2020 2020 2020 2020 2020 656e 756d              enum
+00026930: 732e 4f72 6465 7242 792e 6f62 7365 7276  s.OrderBy.observ
+00026940: 6174 696f 6e5f 656e 642c 0d0a 2020 2020  ation_end,..    
+00026950: 2020 2020 2020 2020 656e 756d 732e 4f72          enums.Or
+00026960: 6465 7242 792e 706f 7075 6c61 7269 7479  derBy.popularity
+00026970: 2c0d 0a20 2020 2020 2020 2020 2020 2065  ,..            e
+00026980: 6e75 6d73 2e4f 7264 6572 4279 2e67 726f  nums.OrderBy.gro
+00026990: 7570 5f70 6f70 756c 6172 6974 792c 0d0a  up_popularity,..
+000269a0: 2020 2020 2020 2020 5d0d 0a0d 0a20 2020          ]....   
+000269b0: 2020 2020 2069 6620 6f72 6465 725f 6279       if order_by
+000269c0: 206e 6f74 2069 6e20 616c 6c6f 7765 645f   not in allowed_
+000269d0: 6f72 6465 7273 3a0d 0a20 2020 2020 2020  orders:..       
+000269e0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000269f0: 4572 726f 7228 2756 6172 6961 626c 6520  Error('Variable 
+00026a00: 6f72 6465 725f 6279 2028 7b7d 2920 6973  order_by ({}) is
+00026a10: 206e 6f74 206f 6e65 206f 6620 7468 6520   not one of the 
+00026a20: 7661 6c75 6573 3a20 7b7d 272e 666f 726d  values: {}'.form
+00026a30: 6174 286f 7264 6572 5f62 792c 2027 2c20  at(order_by, ', 
+00026a40: 272e 6a6f 696e 286d 6170 2873 7472 2c20  '.join(map(str, 
+00026a50: 616c 6c6f 7765 645f 6f72 6465 7273 2929  allowed_orders))
+00026a60: 2929 0d0a 0d0a 2020 2020 2020 2020 6966  ))....        if
+00026a70: 2072 6561 6c74 696d 655f 7374 6172 7420   realtime_start 
+00026a80: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00026a90: 7265 616c 7469 6d65 5f73 7461 7274 203c  realtime_start <
+00026aa0: 2064 6174 6528 3137 3736 2c20 372c 2034   date(1776, 7, 4
+00026ab0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00026ac0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00026ad0: 2827 5661 7269 6162 6c65 2072 6561 6c74  ('Variable realt
+00026ae0: 696d 655f 7374 6172 7420 2822 7b7d 2229  ime_start ("{}")
+00026af0: 2069 7320 6265 666f 7265 206d 696e 2064   is before min d
+00026b00: 6174 6520 3137 3736 2d30 372d 3034 2e27  ate 1776-07-04.'
+00026b10: 2e66 6f72 6d61 7428 7265 616c 7469 6d65  .format(realtime
+00026b20: 5f73 7461 7274 2929 0d0a 0d0a 2020 2020  _start))....    
+00026b30: 2020 2020 6966 2072 6561 6c74 696d 655f      if realtime_
+00026b40: 7374 6172 7420 6973 206e 6f74 204e 6f6e  start is not Non
+00026b50: 6520 616e 6420 7265 616c 7469 6d65 5f65  e and realtime_e
+00026b60: 6e64 2069 7320 6e6f 7420 4e6f 6e65 2061  nd is not None a
+00026b70: 6e64 2072 6561 6c74 696d 655f 7374 6172  nd realtime_star
+00026b80: 7420 3e20 7265 616c 7469 6d65 5f65 6e64  t > realtime_end
+00026b90: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00026ba0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00026bb0: 2754 6865 2064 6174 6520 7365 7420 6279  'The date set by
+00026bc0: 2076 6172 6961 626c 6520 7265 616c 7469   variable realti
+00026bd0: 6d65 5f73 7461 7274 2028 227b 7d22 2920  me_start ("{}") 
+00026be0: 6361 6e20 6e6f 7420 6265 2061 6674 6572  can not be after
+00026bf0: 2074 6865 2064 6174 6520 7365 7420 6279   the date set by
+00026c00: 2076 6172 6961 626c 6520 7265 616c 7469   variable realti
+00026c10: 6d65 5f65 6e64 2028 227b 7d22 292e 272e  me_end ("{}").'.
+00026c20: 666f 726d 6174 2872 6561 6c74 696d 655f  format(realtime_
+00026c30: 7374 6172 742c 2072 6561 6c74 696d 655f  start, realtime_
+00026c40: 656e 6429 290d 0a0d 0a20 2020 2020 2020  end))....       
+00026c50: 2064 6620 3d20 7064 2e44 6174 6146 7261   df = pd.DataFra
+00026c60: 6d65 280d 0a20 2020 2020 2020 2020 2020  me(..           
+00026c70: 2073 656c 662e 5f63 6c69 656e 742e 6765   self._client.ge
+00026c80: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00026c90: 2020 2020 272f 6672 6564 2f74 6167 732f      '/fred/tags/
+00026ca0: 7365 7269 6573 272c 0d0a 2020 2020 2020  series',..      
+00026cb0: 2020 2020 2020 2020 2020 2773 6572 6965            'serie
+00026cc0: 7373 272c 0d0a 2020 2020 2020 2020 2020  ss',..          
+00026cd0: 2020 2020 2020 6c69 6d69 743d 3130 3030        limit=1000
+00026ce0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00026cf0: 2020 2074 6167 5f6e 616d 6573 3d74 6167     tag_names=tag
+00026d00: 5f6e 616d 6573 2c0d 0a20 2020 2020 2020  _names,..       
+00026d10: 2020 2020 2020 2020 2065 7863 6c75 6465           exclude
+00026d20: 5f74 6167 5f6e 616d 6573 3d65 7863 6c75  _tag_names=exclu
+00026d30: 6465 5f74 6167 5f6e 616d 6573 2c0d 0a20  de_tag_names,.. 
+00026d40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00026d50: 6561 6c74 696d 655f 7374 6172 743d 7265  ealtime_start=re
+00026d60: 616c 7469 6d65 5f73 7461 7274 2c0d 0a20  altime_start,.. 
+00026d70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00026d80: 6561 6c74 696d 655f 656e 643d 7265 616c  ealtime_end=real
+00026d90: 7469 6d65 5f65 6e64 2c0d 0a20 2020 2020  time_end,..     
+00026da0: 2020 2020 2020 2020 2020 206f 7264 6572             order
+00026db0: 5f62 793d 6f72 6465 725f 6279 2c0d 0a20  _by=order_by,.. 
+00026dc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00026dd0: 6f72 745f 6f72 6465 723d 736f 7274 5f6f  ort_order=sort_o
+00026de0: 7264 6572 0d0a 2020 2020 2020 2020 2020  rder..          
+00026df0: 2020 290d 0a20 2020 2020 2020 2029 0d0a    )..        )..
+00026e00: 0d0a 2020 2020 2020 2020 6461 7465 5f63  ..        date_c
+00026e10: 6f6c 756d 6e73 203d 205b 0d0a 2020 2020  olumns = [..    
+00026e20: 2020 2020 2020 2020 2772 6561 6c74 696d          'realtim
+00026e30: 655f 7374 6172 7427 2c20 2772 6561 6c74  e_start', 'realt
+00026e40: 696d 655f 656e 6427 2c0d 0a20 2020 2020  ime_end',..     
+00026e50: 2020 2020 2020 2027 6f62 7365 7276 6174         'observat
+00026e60: 696f 6e5f 7374 6172 7427 2c20 276f 6273  ion_start', 'obs
+00026e70: 6572 7661 7469 6f6e 5f65 6e64 272c 0d0a  ervation_end',..
+00026e80: 2020 2020 2020 2020 5d0d 0a0d 0a20 2020          ]....   
+00026e90: 2020 2020 2069 6620 6e6f 7420 6466 2e65       if not df.e
+00026ea0: 6d70 7479 3a0d 0a20 2020 2020 2020 2020  mpty:..         
+00026eb0: 2020 2064 665b 6461 7465 5f63 6f6c 756d     df[date_colum
+00026ec0: 6e73 5d20 3d20 6466 5b64 6174 655f 636f  ns] = df[date_co
+00026ed0: 6c75 6d6e 735d 2e61 7070 6c79 2870 642e  lumns].apply(pd.
+00026ee0: 746f 5f64 6174 6574 696d 652c 2066 6f72  to_datetime, for
+00026ef0: 6d61 743d 2725 592d 256d 2d25 6427 290d  mat='%Y-%m-%d').
+00026f00: 0a20 2020 2020 2020 2020 2020 2064 662e  .            df.
+00026f10: 6c61 7374 5f75 7064 6174 6564 203d 2070  last_updated = p
+00026f20: 642e 746f 5f64 6174 6574 696d 6528 6466  d.to_datetime(df
+00026f30: 2e6c 6173 745f 7570 6461 7465 6420 2b20  .last_updated + 
+00026f40: 2730 3027 2c20 7574 633d 5472 7565 2c20  '00', utc=True, 
+00026f50: 666f 726d 6174 3d27 2559 2d25 6d2d 2564  format='%Y-%m-%d
+00026f60: 2025 483a 254d 3a25 5325 7a27 290d 0a0d   %H:%M:%S%z')...
+00026f70: 0a20 2020 2020 2020 2020 2020 2064 6620  .            df 
+00026f80: 3d20 6466 2e61 7374 7970 6528 6474 7970  = df.astype(dtyp
+00026f90: 653d 7b0d 0a20 2020 2020 2020 2020 2020  e={..           
+00026fa0: 2020 2020 2027 6964 273a 2027 7374 7269       'id': 'stri
+00026fb0: 6e67 272c 0d0a 2020 2020 2020 2020 2020  ng',..          
+00026fc0: 2020 2020 2020 276e 6f74 6573 273a 2027        'notes': '
+00026fd0: 7374 7269 6e67 272c 0d0a 2020 2020 2020  string',..      
+00026fe0: 2020 2020 2020 2020 2020 2774 6974 6c65            'title
+00026ff0: 273a 2027 7374 7269 6e67 272c 0d0a 2020  ': 'string',..  
+00027000: 2020 2020 2020 2020 2020 2020 2020 2766                'f
+00027010: 7265 7175 656e 6379 273a 2027 6361 7465  requency': 'cate
+00027020: 676f 7279 272c 0d0a 2020 2020 2020 2020  gory',..        
+00027030: 2020 2020 2020 2020 2766 7265 7175 656e          'frequen
+00027040: 6379 5f73 686f 7274 273a 2027 6361 7465  cy_short': 'cate
+00027050: 676f 7279 272c 0d0a 2020 2020 2020 2020  gory',..        
+00027060: 2020 2020 2020 2020 2775 6e69 7473 5f73          'units_s
+00027070: 686f 7274 273a 2027 6361 7465 676f 7279  hort': 'category
+00027080: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00027090: 2020 2020 2775 6e69 7473 273a 2027 6361      'units': 'ca
+000270a0: 7465 676f 7279 272c 0d0a 2020 2020 2020  tegory',..      
+000270b0: 2020 2020 2020 2020 2020 2773 6561 736f            'seaso
+000270c0: 6e61 6c5f 6164 6a75 7374 6d65 6e74 273a  nal_adjustment':
+000270d0: 2027 6361 7465 676f 7279 272c 0d0a 2020   'category',..  
+000270e0: 2020 2020 2020 2020 2020 2020 2020 2773                's
+000270f0: 6561 736f 6e61 6c5f 6164 6a75 7374 6d65  easonal_adjustme
+00027100: 6e74 5f73 686f 7274 273a 2027 6361 7465  nt_short': 'cate
+00027110: 676f 7279 270d 0a20 2020 2020 2020 2020  gory'..         
+00027120: 2020 207d 292e 7365 745f 696e 6465 7828     }).set_index(
+00027130: 2769 6427 290d 0a0d 0a20 2020 2020 2020  'id')....       
+00027140: 2072 6574 7572 6e20 6466 0d0a 0d0a 0d0a   return df......
+00027150: 636c 6173 7320 414c 4652 4544 2846 5245  class ALFRED(FRE
+00027160: 4429 3a0d 0a20 2020 2022 2222 0d0a 2020  D):..    """..  
+00027170: 2020 414c 4652 4544 2073 7461 6e64 7320    ALFRED stands 
+00027180: 666f 7220 4172 6368 6976 616c 2046 6564  for Archival Fed
+00027190: 6572 616c 2052 6573 6572 7665 2045 636f  eral Reserve Eco
+000271a0: 6e6f 6d69 6320 4461 7461 2e0d 0a20 2020  nomic Data...   
+000271b0: 2041 4c46 5245 4420 6172 6368 6976 6573   ALFRED archives
+000271c0: 2046 5245 4420 6461 7461 2062 7920 6164   FRED data by ad
+000271d0: 6469 6e67 2074 6865 2072 6561 6c2d 7469  ding the real-ti
+000271e0: 6d65 2070 6572 696f 6420 7768 656e 2076  me period when v
+000271f0: 616c 7565 7320 7765 7265 206f 7269 6769  alues were origi
+00027200: 6e61 6c6c 7920 7265 6c65 6173 6564 2061  nally released a
+00027210: 6e64 206c 6174 6572 2072 6576 6973 6564  nd later revised
+00027220: 2e20 466f 7220 696e 7374 616e 6365 206f  . For instance o
+00027230: 6e20 4665 6272 7561 7279 2032 2c20 3139  n February 2, 19
+00027240: 3930 2c20 7468 6520 5553 2042 7572 6561  90, the US Burea
+00027250: 7520 6f66 204c 6162 6f72 2053 7461 7469  u of Labor Stati
+00027260: 7374 6963 7320 7265 706f 7274 6564 2074  stics reported t
+00027270: 6865 2055 5320 756e 656d 706c 6f79 6d65  he US unemployme
+00027280: 6e74 2072 6174 6520 666f 7220 7468 6520  nt rate for the 
+00027290: 6d6f 6e74 6820 6f66 204a 616e 7561 7279  month of January
+000272a0: 2c20 3139 3930 2061 7320 352e 3320 7065  , 1990 as 5.3 pe
+000272b0: 7263 656e 742e 0d0a 2020 2020 4f76 6572  rcent...    Over
+000272c0: 2036 2079 6561 7273 206c 6174 6572 206f   6 years later o
+000272d0: 6e20 4d61 7263 6820 382c 2031 3939 362c  n March 8, 1996,
+000272e0: 2074 6865 2055 5320 756e 656d 706c 6f79   the US unemploy
+000272f0: 6d65 6e74 2072 6174 6520 666f 7220 7468  ment rate for th
+00027300: 6520 7361 6d65 206d 6f6e 7468 204a 616e  e same month Jan
+00027310: 7561 7279 2c20 3139 3930 2077 6173 2072  uary, 1990 was r
+00027320: 6576 6973 6564 2074 6f20 352e 3420 7065  evised to 5.4 pe
+00027330: 7263 656e 742e 0d0a 0d0a 2020 2020 6874  rcent.....    ht
+00027340: 7470 733a 2f2f 616c 6672 6564 2e73 746c  tps://alfred.stl
+00027350: 6f75 6973 6665 642e 6f72 672f 0d0a 0d0a  ouisfed.org/....
+00027360: 2020 2020 6874 7470 733a 2f2f 6672 6564      https://fred
+00027370: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
+00027380: 646f 6373 2f61 7069 2f66 7265 642f 616c  docs/api/fred/al
+00027390: 6672 6564 2e68 746d 6c0d 0a20 2020 2022  fred.html..    "
+000273a0: 2222 0d0a 0d0a 0d0a 636c 6173 7320 4765  ""......class Ge
+000273b0: 6f46 5245 443a 0d0a 2020 2020 2222 220d  oFRED:..    """.
+000273c0: 0a20 2020 2054 6865 2047 656f 4652 4544  .    The GeoFRED
+000273d0: 2041 5049 2069 7320 6120 7765 6220 7365   API is a web se
+000273e0: 7276 6963 6520 7468 6174 2061 6c6c 6f77  rvice that allow
+000273f0: 7320 6465 7665 6c6f 7065 7273 2074 6f20  s developers to 
+00027400: 7772 6974 6520 7072 6f67 7261 6d73 2061  write programs a
+00027410: 6e64 2062 7569 6c64 2061 7070 6c69 6361  nd build applica
+00027420: 7469 6f6e 7320 746f 2068 6172 7665 7374  tions to harvest
+00027430: 2064 6174 6120 616e 6420 7368 6170 6520   data and shape 
+00027440: 6669 6c65 7320 666f 756e 6420 696e 2047  files found in G
+00027450: 656f 4652 4544 2077 6562 7369 7465 2068  eoFRED website h
+00027460: 6f73 7465 6420 6279 2074 6865 2045 636f  osted by the Eco
+00027470: 6e6f 6d69 6320 5265 7365 6172 6368 2044  nomic Research D
+00027480: 6976 6973 696f 6e20 6f66 2074 6865 2046  ivision of the F
+00027490: 6564 6572 616c 2052 6573 6572 7665 2042  ederal Reserve B
+000274a0: 616e 6b20 6f66 2053 742e 204c 6f75 6973  ank of St. Louis
+000274b0: 2e0d 0a0d 0a20 2020 2068 7474 7073 3a2f  .....    https:/
+000274c0: 2f67 656f 6672 6564 2e73 746c 6f75 6973  /geofred.stlouis
+000274d0: 6665 642e 6f72 672f 0d0a 0d0a 2020 2020  fed.org/....    
+000274e0: 6874 7470 733a 2f2f 6765 6f66 7265 642e  https://geofred.
+000274f0: 7374 6c6f 7569 7366 6564 2e6f 7267 2f64  stlouisfed.org/d
+00027500: 6f63 732f 6170 692f 6765 6f66 7265 642f  ocs/api/geofred/
+00027510: 0d0a 2020 2020 2222 220d 0a20 2020 2045  ..    """..    E
+00027520: 4d50 5459 5f56 414c 5545 203d 2027 2e27  MPTY_VALUE = '.'
+00027530: 0d0a 0d0a 2020 2020 2222 220d 0a20 2020  ....    """..   
+00027540: 2068 7474 7073 3a2f 2f67 656f 6672 6564   https://geofred
+00027550: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
+00027560: 0d0a 2020 2020 6874 7470 733a 2f2f 6765  ..    https://ge
+00027570: 6f66 7265 642e 7374 6c6f 7569 7366 6564  ofred.stlouisfed
+00027580: 2e6f 7267 2f64 6f63 732f 6170 692f 6765  .org/docs/api/ge
+00027590: 6f66 7265 642f 0d0a 2020 2020 2222 220d  ofred/..    """.
+000275a0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+000275b0: 745f 5f28 7365 6c66 2c20 6170 695f 6b65  t__(self, api_ke
+000275c0: 793a 2073 7472 2c20 7261 7465 6c69 6d69  y: str, ratelimi
+000275d0: 7465 725f 656e 6162 6c65 643a 2062 6f6f  ter_enabled: boo
+000275e0: 6c20 3d20 4661 6c73 652c 2072 6174 656c  l = False, ratel
+000275f0: 696d 6974 6572 5f6d 6178 5f63 616c 6c73  imiter_max_calls
+00027600: 3a20 696e 7420 3d20 322c 2072 6174 656c  : int = 2, ratel
+00027610: 696d 6974 6572 5f70 6572 696f 643a 2069  imiter_period: i
+00027620: 6e74 203d 2031 2c20 7265 7175 6573 745f  nt = 1, request_
+00027630: 7061 7261 6d73 3a20 6469 6374 203d 204e  params: dict = N
+00027640: 6f6e 6529 3a0d 0a20 2020 2020 2020 2022  one):..        "
+00027650: 2222 0d0a 2020 2020 2020 2020 5061 7261  ""..        Para
+00027660: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
+00027670: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+00027680: 2020 2020 6170 695f 6b65 793a 2073 7472      api_key: str
+00027690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000276a0: 2020 3332 2063 6861 7261 6374 6572 2061    32 character a
+000276b0: 6c70 6861 2d6e 756d 6572 6963 206c 6f77  lpha-numeric low
+000276c0: 6572 6361 7365 2073 7472 696e 670d 0a20  ercase string.. 
+000276d0: 2020 2020 2020 2072 6174 656c 696d 6974         ratelimit
+000276e0: 6572 5f65 6e61 626c 6564 3a20 626f 6f6c  er_enabled: bool
+000276f0: 0d0a 2020 2020 2020 2020 7261 7465 6c69  ..        rateli
+00027700: 6d69 7465 725f 6d61 785f 6361 6c6c 733a  miter_max_calls:
+00027710: 2069 6e74 0d0a 2020 2020 2020 2020 7261   int..        ra
+00027720: 7465 6c69 6d69 7465 725f 7065 7269 6f64  telimiter_period
+00027730: 3a20 696e 740d 0a20 2020 2020 2020 2072  : int..        r
+00027740: 6571 7565 7374 5f70 6172 616d 733a 2064  equest_params: d
+00027750: 6963 740d 0a20 2020 2020 2020 2020 2020  ict..           
+00027760: 2020 2020 2048 5454 5020 4745 5420 6d65       HTTP GET me
+00027770: 7468 6f64 2070 6172 616d 6574 6572 732c  thod parameters,
+00027780: 2073 6565 2068 7474 7073 3a2f 2f64 6f63   see https://doc
+00027790: 732e 7079 7468 6f6e 2d72 6571 7565 7374  s.python-request
+000277a0: 732e 6f72 672f 656e 2f6c 6174 6573 742f  s.org/en/latest/
+000277b0: 6170 692f 2372 6571 7565 7374 732e 7265  api/#requests.re
+000277c0: 7175 6573 740d 0a20 2020 2020 2020 2022  quest..        "
+000277d0: 2222 0d0a 0d0a 2020 2020 2020 2020 6966  ""....        if
+000277e0: 2061 7069 5f6b 6579 2069 7320 4e6f 6e65   api_key is None
+000277f0: 206f 7220 6c65 6e28 6170 695f 6b65 7929   or len(api_key)
+00027800: 2021 3d20 3332 3a0d 0a20 2020 2020 2020   != 32:..       
+00027810: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00027820: 7469 6f6e 2827 5661 7269 6162 6c65 2061  tion('Variable a
+00027830: 7069 5f6b 6579 206d 7573 7420 6265 2033  pi_key must be 3
+00027840: 3220 6368 6172 6163 7465 7220 6c65 6e67  2 character leng
+00027850: 7468 2061 6c70 6861 6e75 6d65 7269 6320  th alphanumeric 
+00027860: 7374 7269 6e67 2e27 290d 0a0d 0a20 2020  string.')....   
+00027870: 2020 2020 2073 656c 662e 5f63 6c69 656e       self._clien
+00027880: 7420 3d20 436c 6965 6e74 280d 0a20 2020  t = Client(..   
+00027890: 2020 2020 2020 2020 206b 6579 3d61 7069           key=api
+000278a0: 5f6b 6579 2e6c 6f77 6572 2829 2c0d 0a20  _key.lower(),.. 
+000278b0: 2020 2020 2020 2020 2020 2072 6174 656c             ratel
+000278c0: 696d 6974 6572 5f65 6e61 626c 6564 3d72  imiter_enabled=r
+000278d0: 6174 656c 696d 6974 6572 5f65 6e61 626c  atelimiter_enabl
+000278e0: 6564 2c0d 0a20 2020 2020 2020 2020 2020  ed,..           
+000278f0: 2072 6174 656c 696d 6974 6572 5f6d 6178   ratelimiter_max
+00027900: 5f63 616c 6c73 3d72 6174 656c 696d 6974  _calls=ratelimit
+00027910: 6572 5f6d 6178 5f63 616c 6c73 2c0d 0a20  er_max_calls,.. 
+00027920: 2020 2020 2020 2020 2020 2072 6174 656c             ratel
+00027930: 696d 6974 6572 5f70 6572 696f 643d 7261  imiter_period=ra
+00027940: 7465 6c69 6d69 7465 725f 7065 7269 6f64  telimiter_period
+00027950: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00027960: 6571 7565 7374 5f70 6172 616d 733d 7265  equest_params=re
+00027970: 7175 6573 745f 7061 7261 6d73 0d0a 2020  quest_params..  
+00027980: 2020 2020 2020 290d 0a0d 0a20 2020 2040        )....    @
+00027990: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+000279a0: 6620 7261 7465 5f6c 696d 6974 2873 656c  f rate_limit(sel
+000279b0: 6629 202d 3e20 696e 743a 0d0a 2020 2020  f) -> int:..    
+000279c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000279d0: 5f63 6c69 656e 742e 7261 7465 5f6c 696d  _client.rate_lim
+000279e0: 6974 0d0a 0d0a 2020 2020 4070 726f 7065  it....    @prope
+000279f0: 7274 790d 0a20 2020 2064 6566 2072 6174  rty..    def rat
+00027a00: 655f 6c69 6d69 745f 7265 6d61 696e 696e  e_limit_remainin
+00027a10: 6728 7365 6c66 2920 2d3e 2069 6e74 3a0d  g(self) -> int:.
+00027a20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00027a30: 7365 6c66 2e5f 636c 6965 6e74 2e72 6174  self._client.rat
+00027a40: 655f 6c69 6d69 745f 7265 6d61 696e 696e  e_limit_remainin
+00027a50: 670d 0a0d 0a20 2020 2064 6566 2073 6861  g....    def sha
+00027a60: 7065 7328 7365 6c66 2c20 7368 6170 653a  pes(self, shape:
+00027a70: 2065 6e75 6d73 2e53 6861 7065 5479 7065   enums.ShapeType
+00027a80: 2920 2d3e 204c 6973 745b 6d6f 6465 6c73  ) -> List[models
+00027a90: 2e53 6861 7065 5d3a 0d0a 2020 2020 2020  .Shape]:..      
+00027aa0: 2020 2222 220d 0a20 2020 2020 2020 2068    """..        h
+00027ab0: 7474 7073 3a2f 2f67 656f 6672 6564 2e73  ttps://geofred.s
+00027ac0: 746c 6f75 6973 6665 642e 6f72 672f 646f  tlouisfed.org/do
+00027ad0: 6373 2f61 7069 2f67 656f 6672 6564 2f73  cs/api/geofred/s
+00027ae0: 6861 7065 732e 6874 6d6c 0d0a 0d0a 2020  hapes.html....  
+00027af0: 2020 2020 2020 2323 2044 6573 6372 6970        ## Descrip
+00027b00: 7469 6f6e 0d0a 2020 2020 2020 2020 5468  tion..        Th
+00027b10: 6973 2072 6571 7565 7374 2072 6574 7572  is request retur
+00027b20: 6e73 2073 6861 7065 2066 696c 6573 2066  ns shape files f
+00027b30: 726f 6d20 4765 6f46 5245 4420 696e 2057  rom GeoFRED in W
+00027b40: 656c 6c2d 6b6e 6f77 6e20 7465 7874 2028  ell-known text (
+00027b50: 574b 5429 2066 6f72 6d61 742e 0d0a 0d0a  WKT) format.....
+00027b60: 2020 2020 2020 2020 2323 2041 5049 2052          ## API R
+00027b70: 6571 7565 7374 2028 4854 5450 5320 4745  equest (HTTPS GE
+00027b80: 5429 0d0a 2020 2020 2020 2020 6874 7470  T)..        http
+00027b90: 733a 2f2f 6170 692e 7374 6c6f 7569 7366  s://api.stlouisf
+00027ba0: 6564 2e6f 7267 2f67 656f 6672 6564 2f73  ed.org/geofred/s
+00027bb0: 6861 7065 732f 6669 6c65 3f73 6861 7065  hapes/file?shape
+00027bc0: 3d62 6561 2661 7069 5f6b 6579 3d61 6263  =bea&api_key=abc
+00027bd0: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
+00027be0: 7475 7677 7879 7a31 3233 3435 360d 0a0d  tuvwxyz123456...
+00027bf0: 0a20 2020 2020 2020 2023 2320 4150 4920  .        ## API 
+00027c00: 5265 7370 6f6e 7365 0d0a 2020 2020 2020  Response..      
+00027c10: 2020 6060 606a 736f 6e0d 0a20 2020 2020    ```json..     
+00027c20: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00027c30: 2262 6561 223a 205b 0d0a 2020 2020 2020  "bea": [..      
+00027c40: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00027c50: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00027c60: 4661 7220 5765 7374 222c 0d0a 2020 2020  Far West",..    
+00027c70: 2020 2020 2020 2020 2020 2263 6f64 6522            "code"
+00027c80: 3a20 2238 222c 0d0a 2020 2020 2020 2020  : "8",..        
+00027c90: 2020 2020 2020 2263 656e 7472 6f69 6422        "centroid"
+00027ca0: 3a20 2250 4f49 4e54 282d 3134 322e 3336  : "POINT(-142.36
+00027cb0: 3239 3438 3337 3834 3332 2035 372e 3134  2948378432 57.14
+00027cc0: 3738 3733 3438 3239 3038 3529 222c 0d0a  78734829085)",..
+00027cd0: 2020 2020 2020 2020 2020 2020 2020 2267                "g
+00027ce0: 656f 6d65 7472 7922 3a20 224d 554c 5449  eometry": "MULTI
+00027cf0: 504f 4c59 474f 4e28 2828 2d31 3535 2e37  POLYGON(((-155.7
+00027d00: 3738 3233 3420 3230 2e32 3435 3734 332c  78234 20.245743,
+00027d10: 2d31 3535 2e37 3732 3733 3420 2e2e 2e29  -155.772734 ...)
+00027d20: 2929 222c 0d0a 2020 2020 2020 2020 2020  ))",..          
+00027d30: 2020 2020 2272 6570 6f72 7420 6e61 6d65      "report name
+00027d40: 223a 2022 4e6f 7274 6820 4164 616d 732c  ": "North Adams,
+00027d50: 204d 412d 5654 220d 0a20 2020 2020 2020   MA-VT"..       
+00027d60: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+00027d70: 2020 2020 2e2e 2e0d 0a20 2020 2020 2020      .....       
+00027d80: 2020 205d 0d0a 2020 2020 2020 2020 7d0d     ]..        }.
+00027d90: 0a20 2020 2020 2020 2060 6060 0d0a 0d0a  .        ```....
+00027da0: 2020 2020 2020 2020 2323 2052 6574 7572          ## Retur
+00027db0: 6e73 0d0a 2020 2020 2020 2020 604c 6973  ns..        `Lis
+00027dc0: 745b 7079 7374 6c6f 7569 7366 6564 2e6d  t[pystlouisfed.m
+00027dd0: 6f64 656c 732e 5368 6170 655d 600d 0a0d  odels.Shape]`...
+00027de0: 0a20 2020 2020 2020 2023 2320 4578 616d  .        ## Exam
+00027df0: 706c 650d 0a20 2020 2020 2020 2060 6060  ple..        ```
+00027e00: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
+00027e10: 2020 2020 696d 706f 7274 206d 6174 706c      import matpl
+00027e20: 6f74 6c69 622e 7079 706c 6f74 2061 7320  otlib.pyplot as 
+00027e30: 706c 740d 0a20 2020 2020 2020 2020 2020  plt..           
+00027e40: 2066 726f 6d20 6465 7363 6172 7465 7320   from descartes 
+00027e50: 696d 706f 7274 2050 6f6c 7967 6f6e 5061  import PolygonPa
+00027e60: 7463 680d 0a20 2020 2020 2020 2020 2020  tch..           
+00027e70: 2066 726f 6d20 7079 7374 6c6f 7569 7366   from pystlouisf
+00027e80: 6564 2e63 6c69 656e 7420 696d 706f 7274  ed.client import
+00027e90: 2047 656f 4652 4544 2c20 5368 6170 6554   GeoFRED, ShapeT
+00027ea0: 7970 650d 0a0d 0a20 2020 2020 2020 2020  ype....         
+00027eb0: 2020 2070 6c74 2e66 6967 7572 6528 290d     plt.figure().
+00027ec0: 0a20 2020 2020 2020 2020 2020 2061 7820  .            ax 
+00027ed0: 3d20 706c 742e 6178 6573 2829 0d0a 2020  = plt.axes()..  
+00027ee0: 2020 2020 2020 2020 2020 6765 6f5f 6672            geo_fr
+00027ef0: 6564 203d 2047 656f 4652 4544 2861 7069  ed = GeoFRED(api
+00027f00: 5f6b 6579 3d27 6162 6364 6566 6768 696a  _key='abcdefghij
+00027f10: 6b6c 6d6e 6f70 7172 7374 7576 7778 797a  klmnopqrstuvwxyz
+00027f20: 3132 3334 3536 2729 0d0a 0d0a 2020 2020  123456')....    
+00027f30: 2020 2020 2020 2020 666f 7220 636f 756e          for coun
+00027f40: 7472 795f 7368 6170 6520 696e 2067 656f  try_shape in geo
+00027f50: 5f66 7265 642e 7368 6170 6573 2873 6861  _fred.shapes(sha
+00027f60: 7065 3d53 6861 7065 5479 7065 2e63 6f75  pe=ShapeType.cou
+00027f70: 6e74 7279 293a 0d0a 2020 2020 2020 2020  ntry):..        
+00027f80: 2020 2020 2020 2020 6178 2e61 6464 5f70          ax.add_p
+00027f90: 6174 6368 2850 6f6c 7967 6f6e 5061 7463  atch(PolygonPatc
+00027fa0: 6828 636f 756e 7472 795f 7368 6170 652e  h(country_shape.
+00027fb0: 6765 6f6d 6574 7279 2c20 6563 3d27 2339  geometry, ec='#9
+00027fc0: 3939 3939 3927 2c20 6663 3d27 2336 3639  99999', fc='#669
+00027fd0: 3963 6327 2c20 616c 7068 613d 302e 352c  9cc', alpha=0.5,
+00027fe0: 207a 6f72 6465 723d 3229 290d 0a20 2020   zorder=2))..   
+00027ff0: 2020 2020 2020 2020 2061 782e 6178 6973           ax.axis
+00028000: 2827 7363 616c 6564 2729 0d0a 2020 2020  ('scaled')..    
+00028010: 2020 2020 2020 2020 706c 742e 7368 6f77          plt.show
+00028020: 2829 0d0a 2020 2020 2020 2020 6060 600d  ()..        ```.
+00028030: 0a20 2020 2020 2020 202e 2e20 696d 6167  .        .. imag
+00028040: 653a 3a20 6765 6f66 7265 645f 7368 6170  e:: geofred_shap
+00028050: 655f 6d61 702e 706e 670d 0a20 2020 2020  e_map.png..     
+00028060: 2020 2022 2222 0d0a 0d0a 2020 2020 2020     """....      
+00028070: 2020 776b 745f 6c69 7374 203d 2073 656c    wkt_list = sel
+00028080: 662e 5f63 6c69 656e 742e 6765 7428 0d0a  f._client.get(..
+00028090: 2020 2020 2020 2020 2020 2020 272f 6765              '/ge
+000280a0: 6f66 7265 642f 7368 6170 6573 2f66 696c  ofred/shapes/fil
+000280b0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+000280c0: 2073 6861 7065 2e76 616c 7565 2c0d 0a20   shape.value,.. 
+000280d0: 2020 2020 2020 2020 2020 2073 6861 7065             shape
+000280e0: 3d73 6861 7065 0d0a 2020 2020 2020 2020  =shape..        
+000280f0: 290d 0a0d 0a20 2020 2020 2020 2023 2072  )....        # r
+00028100: 6570 6c61 6365 2077 6869 7465 7370 6163  eplace whitespac
+00028110: 6573 2069 6e20 6469 6374 206b 6579 730d  es in dict keys.
+00028120: 0a20 2020 2020 2020 2066 6f72 2077 6b74  .        for wkt
+00028130: 2069 6e20 776b 745f 6c69 7374 3a0d 0a20   in wkt_list:.. 
+00028140: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00028150: 6579 2069 6e20 6c69 7374 2877 6b74 2e6b  ey in list(wkt.k
+00028160: 6579 7328 2929 3a0d 0a20 2020 2020 2020  eys()):..       
+00028170: 2020 2020 2020 2020 2077 6b74 5b6b 6579           wkt[key
+00028180: 2e72 6570 6c61 6365 2827 2027 2c20 275f  .replace(' ', '_
+00028190: 2729 5d20 3d20 776b 742e 706f 7028 6b65  ')] = wkt.pop(ke
+000281a0: 7929 0d0a 0d0a 2020 2020 2020 2020 7265  y)....        re
+000281b0: 7475 726e 206c 6973 7428 6d61 7028 6c61  turn list(map(la
+000281c0: 6d62 6461 2077 6b74 3a20 6d6f 6465 6c73  mbda wkt: models
+000281d0: 2e53 6861 7065 282a 2a77 6b74 292c 2077  .Shape(**wkt), w
+000281e0: 6b74 5f6c 6973 7429 290d 0a0d 0a20 2020  kt_list))....   
+000281f0: 2064 6566 2073 6572 6965 735f 6772 6f75   def series_grou
+00028200: 7028 7365 6c66 2c20 7365 7269 6573 5f69  p(self, series_i
+00028210: 643a 2073 7472 2920 2d3e 206d 6f64 656c  d: str) -> model
+00028220: 732e 5365 7269 6573 4772 6f75 703a 0d0a  s.SeriesGroup:..
+00028230: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00028240: 2020 2020 2068 7474 7073 3a2f 2f67 656f       https://geo
+00028250: 6672 6564 2e73 746c 6f75 6973 6665 642e  fred.stlouisfed.
+00028260: 6f72 672f 646f 6373 2f61 7069 2f67 656f  org/docs/api/geo
+00028270: 6672 6564 2f73 6572 6965 735f 6772 6f75  fred/series_grou
+00028280: 702e 6874 6d6c 0d0a 0d0a 2020 2020 2020  p.html....      
+00028290: 2020 2323 2044 6573 6372 6970 7469 6f6e    ## Description
+000282a0: 0d0a 2020 2020 2020 2020 5468 6973 2072  ..        This r
+000282b0: 6571 7565 7374 2072 6574 7572 6e73 2074  equest returns t
+000282c0: 6865 206d 6574 6120 696e 666f 726d 6174  he meta informat
+000282d0: 696f 6e20 6e65 6564 6564 2074 6f20 6d61  ion needed to ma
+000282e0: 6b65 2072 6571 7565 7374 7320 666f 7220  ke requests for 
+000282f0: 4765 6f46 5245 4420 6461 7461 2e0d 0a20  GeoFRED data... 
+00028300: 2020 2020 2020 204d 696e 696d 756d 2061         Minimum a
+00028310: 6e64 206d 6178 696d 756d 2064 6174 6520  nd maximum date 
+00028320: 6172 6520 616c 736f 2073 7570 706c 6965  are also supplie
+00028330: 6420 666f 7220 7468 6520 6461 7461 2072  d for the data r
+00028340: 616e 6765 2061 7661 696c 6162 6c65 2e0d  ange available..
+00028350: 0a0d 0a20 2020 2020 2020 2023 2320 4150  ...        ## AP
+00028360: 4920 5265 7175 6573 7420 2848 5454 5053  I Request (HTTPS
+00028370: 2047 4554 290d 0a20 2020 2020 2020 2068   GET)..        h
+00028380: 7474 7073 3a2f 2f61 7069 2e73 746c 6f75  ttps://api.stlou
+00028390: 6973 6665 642e 6f72 672f 6765 6f66 7265  isfed.org/geofre
+000283a0: 642f 7365 7269 6573 2f67 726f 7570 3f73  d/series/group?s
+000283b0: 6572 6965 735f 6964 3d53 4d55 3536 3030  eries_id=SMU5600
+000283c0: 3030 3030 3530 3030 3030 3030 3161 2661  0000500000001a&a
+000283d0: 7069 5f6b 6579 3d61 6263 6465 6667 6869  pi_key=abcdefghi
+000283e0: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
+000283f0: 7a31 3233 3435 360d 0a0d 0a20 2020 2020  z123456....     
+00028400: 2020 2023 2320 4150 4920 5265 7370 6f6e     ## API Respon
+00028410: 7365 0d0a 2020 2020 2020 2020 6060 606a  se..        ```j
+00028420: 736f 6e0d 0a20 2020 2020 2020 207b 0d0a  son..        {..
+00028430: 2020 2020 2020 2020 2020 2273 6572 6965            "serie
+00028440: 735f 6772 6f75 7022 3a20 5b0d 0a20 2020  s_group": [..   
+00028450: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
+00028460: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
+00028470: 223a 2022 416c 6c20 456d 706c 6f79 6565  ": "All Employee
+00028480: 733a 2054 6f74 616c 2050 7269 7661 7465  s: Total Private
+00028490: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000284a0: 2020 2267 656f 6d5f 7479 7065 223a 2022    "geom_type": "
+000284b0: 7374 6174 6522 2c0d 0a20 2020 2020 2020  state",..       
+000284c0: 2020 2020 2020 2022 6772 6f75 705f 6964         "group_id
+000284d0: 223a 2022 3139 3222 2c0d 0a20 2020 2020  ": "192",..     
+000284e0: 2020 2020 2020 2020 2022 7365 6173 6f6e           "season
+000284f0: 223a 2022 4e53 4122 2c0d 0a20 2020 2020  ": "NSA",..     
+00028500: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+00028510: 3a20 2254 686f 7573 616e 6473 206f 6620  : "Thousands of 
+00028520: 5065 7273 6f6e 7322 2c0d 0a20 2020 2020  Persons",..     
+00028530: 2020 2020 2020 2020 2022 6672 6571 7565           "freque
+00028540: 6e63 7922 3a20 226d 222c 0d0a 2020 2020  ncy": "m",..    
+00028550: 2020 2020 2020 2020 2020 226d 696e 5f73            "min_s
+00028560: 7461 7274 5f64 6174 6522 3a20 2231 3939  tart_date": "199
+00028570: 302d 3031 2d30 3122 2c0d 0a20 2020 2020  0-01-01",..     
+00028580: 2020 2020 2020 2020 2022 6d61 785f 7374           "max_st
+00028590: 6172 745f 6461 7465 223a 2022 3230 3135  art_date": "2015
+000285a0: 2d30 362d 3031 220d 0a20 2020 2020 2020  -06-01"..       
+000285b0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+000285c0: 2020 5d0d 0a20 2020 2020 2020 207d 0d0a    ]..        }..
+000285d0: 2020 2020 2020 2020 6060 600d 0a0d 0a20          ```.... 
+000285e0: 2020 2020 2020 2023 2320 5265 7475 726e         ## Return
+000285f0: 730d 0a20 2020 2020 2020 2060 6d6f 6465  s..        `mode
+00028600: 6c73 2e53 6572 6965 7347 726f 7570 600d  ls.SeriesGroup`.
+00028610: 0a0d 0a20 2020 2020 2020 2023 2320 4578  ...        ## Ex
+00028620: 616d 706c 650d 0a20 2020 2020 2020 2060  ample..        `
+00028630: 6060 7079 7468 6f6e 0d0a 2020 2020 2020  ``python..      
+00028640: 2020 2020 2020 3e3e 3e20 6765 6f5f 6672        >>> geo_fr
+00028650: 6564 203d 2047 656f 4652 4544 2861 7069  ed = GeoFRED(api
+00028660: 5f6b 6579 3d27 6162 6364 6566 6768 696a  _key='abcdefghij
+00028670: 6b6c 6d6e 6f70 7172 7374 7576 7778 797a  klmnopqrstuvwxyz
+00028680: 3132 3334 3536 2729 0d0a 2020 2020 2020  123456')..      
+00028690: 2020 2020 2020 3e3e 3e20 7072 696e 7428        >>> print(
+000286a0: 6765 6f5f 6672 6564 2e73 6572 6965 735f  geo_fred.series_
+000286b0: 6772 6f75 7028 7365 7269 6573 5f69 643d  group(series_id=
+000286c0: 2753 4d55 3536 3030 3030 3030 3530 3030  'SMU560000005000
+000286d0: 3030 3030 3161 2729 290d 0a20 2020 2020  00001a'))..     
+000286e0: 2020 2020 2020 2053 6572 6965 7347 726f         SeriesGro
+000286f0: 7570 2874 6974 6c65 3d27 416c 6c20 456d  up(title='All Em
+00028700: 706c 6f79 6565 733a 2054 6f74 616c 2050  ployees: Total P
+00028710: 7269 7661 7465 272c 2072 6567 696f 6e5f  rivate', region_
+00028720: 7479 7065 3d27 7374 6174 6527 2c20 7365  type='state', se
+00028730: 7269 6573 5f67 726f 7570 3d27 3132 3233  ries_group='1223
+00028740: 272c 2073 6561 736f 6e3d 274e 5341 272c  ', season='NSA',
+00028750: 2075 6e69 7473 3d27 5468 6f75 7361 6e64   units='Thousand
+00028760: 7320 6f66 2050 6572 736f 6e73 272c 2066  s of Persons', f
+00028770: 7265 7175 656e 6379 3d27 6127 2c20 6d69  requency='a', mi
+00028780: 6e5f 6461 7465 3d64 6174 6574 696d 652e  n_date=datetime.
+00028790: 6461 7465 2831 3939 302c 2031 2c20 3129  date(1990, 1, 1)
+000287a0: 2c20 6d61 785f 6461 7465 3d64 6174 6574  , max_date=datet
+000287b0: 696d 652e 6461 7465 2832 3032 302c 2031  ime.date(2020, 1
+000287c0: 2c20 3129 290d 0a20 2020 2020 2020 2060  , 1))..        `
+000287d0: 6060 0d0a 2020 2020 2020 2020 2222 220d  ``..        """.
+000287e0: 0a0d 0a20 2020 2020 2020 2064 6174 6120  ...        data 
+000287f0: 3d20 7365 6c66 2e5f 636c 6965 6e74 2e67  = self._client.g
+00028800: 6574 280d 0a20 2020 2020 2020 2020 2020  et(..           
+00028810: 2027 2f67 656f 6672 6564 2f73 6572 6965   '/geofred/serie
+00028820: 732f 6772 6f75 7027 2c0d 0a20 2020 2020  s/group',..     
+00028830: 2020 2020 2020 2027 7365 7269 6573 5f67         'series_g
+00028840: 726f 7570 272c 0d0a 2020 2020 2020 2020  roup',..        
+00028850: 2020 2020 7365 7269 6573 5f69 643d 7365      series_id=se
+00028860: 7269 6573 5f69 640d 0a20 2020 2020 2020  ries_id..       
+00028870: 2029 0d0a 0d0a 2020 2020 2020 2020 7265   )....        re
+00028880: 7475 726e 206d 6f64 656c 732e 5365 7269  turn models.Seri
+00028890: 6573 4772 6f75 7028 2a2a 6461 7461 5b30  esGroup(**data[0
+000288a0: 5d29 0d0a 0d0a 2020 2020 6465 6620 7365  ])....    def se
+000288b0: 7269 6573 5f64 6174 6128 7365 6c66 2c20  ries_data(self, 
+000288c0: 7365 7269 6573 5f69 643a 2073 7472 2c20  series_id: str, 
+000288d0: 6461 7465 3a20 6461 7465 203d 204e 6f6e  date: date = Non
+000288e0: 652c 2073 7461 7274 5f64 6174 653a 2064  e, start_date: d
+000288f0: 6174 6520 3d20 4e6f 6e65 2920 2d3e 2070  ate = None) -> p
+00028900: 642e 4461 7461 4672 616d 653a 0d0a 2020  d.DataFrame:..  
+00028910: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00028920: 2020 2023 2320 5061 7261 6d65 7465 7273     ## Parameters
+00028930: 0d0a 0d0a 2020 2020 2020 2020 6073 6572  ....        `ser
+00028940: 6965 735f 6964 600d 0a20 2020 2020 2020  ies_id`..       
+00028950: 2054 6865 2046 5245 4420 7365 7269 6573   The FRED series
+00028960: 5f69 6420 796f 7520 7761 6e74 2074 6f20  _id you want to 
+00028970: 7265 7175 6573 7420 4765 6f46 5245 4420  request GeoFRED 
+00028980: 6461 7461 2066 6f72 2e20 4e6f 7420 616c  data for. Not al
+00028990: 6c20 7365 7269 6573 2074 6861 7420 6172  l series that ar
+000289a0: 6520 696e 2046 5245 4420 6861 7665 2067  e in FRED have g
+000289b0: 656f 6772 6170 6869 6361 6c20 6461 7461  eographical data
+000289c0: 2e0d 0a0d 0a20 2020 2020 2020 2060 6461  .....        `da
+000289d0: 7465 600d 0a20 2020 2020 2020 2054 6865  te`..        The
+000289e0: 2064 6174 6520 796f 7520 7761 6e74 2074   date you want t
+000289f0: 6f20 7265 7175 6573 7420 7365 7269 6573  o request series
+00028a00: 2067 726f 7570 2064 6174 6120 6672 6f6d   group data from
+00028a10: 2e0d 0a0d 0a20 2020 2020 2020 2060 7374  .....        `st
+00028a20: 6172 745f 6461 7465 600d 0a20 2020 2020  art_date`..     
+00028a30: 2020 2054 6865 2073 7461 7274 2064 6174     The start dat
+00028a40: 6520 796f 7520 7761 6e74 2074 6f20 7265  e you want to re
+00028a50: 7175 6573 7420 7365 7269 6573 2067 726f  quest series gro
+00028a60: 7570 2064 6174 6120 6672 6f6d 2e20 5468  up data from. Th
+00028a70: 6973 2061 6c6c 6f77 7320 796f 7520 746f  is allows you to
+00028a80: 2070 756c 6c20 6120 7261 6e67 6520 6f66   pull a range of
+00028a90: 2064 6174 610d 0a0d 0a20 2020 2020 2020   data....       
+00028aa0: 2023 2320 4465 7363 7269 7074 696f 6e0d   ## Description.
+00028ab0: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
+00028ac0: 2f67 656f 6672 6564 2e73 746c 6f75 6973  /geofred.stlouis
+00028ad0: 6665 642e 6f72 672f 646f 6373 2f61 7069  fed.org/docs/api
+00028ae0: 2f67 656f 6672 6564 2f73 6572 6965 735f  /geofred/series_
+00028af0: 6461 7461 2e68 746d 6c0d 0a0d 0a20 2020  data.html....   
+00028b00: 2020 2020 2054 6869 7320 7265 7175 6573       This reques
+00028b10: 7420 7265 7475 726e 7320 6120 6372 6f73  t returns a cros
+00028b20: 7320 7365 6374 696f 6e20 6f66 2072 6567  s section of reg
+00028b30: 696f 6e61 6c20 6461 7461 2066 6f72 2061  ional data for a
+00028b40: 2073 7065 6369 6669 6564 2072 656c 6561   specified relea
+00028b50: 7365 2064 6174 652e 0d0a 2020 2020 2020  se date...      
+00028b60: 2020 4966 206e 6f20 6461 7465 2069 7320    If no date is 
+00028b70: 7370 6563 6966 6965 642c 2074 6865 206d  specified, the m
+00028b80: 6f73 7420 7265 6365 6e74 2064 6174 6120  ost recent data 
+00028b90: 6176 6169 6c61 626c 6520 6172 6520 7265  available are re
+00028ba0: 7475 726e 6564 2e0d 0a0d 0a20 2020 2020  turned.....     
+00028bb0: 2020 2023 2320 4150 4920 5265 7175 6573     ## API Reques
+00028bc0: 7420 2848 5454 5053 2047 4554 290d 0a20  t (HTTPS GET).. 
+00028bd0: 2020 2020 2020 2068 7474 7073 3a2f 2f61         https://a
+00028be0: 7069 2e73 746c 6f75 6973 6665 642e 6f72  pi.stlouisfed.or
+00028bf0: 672f 6765 6f66 7265 642f 7365 7269 6573  g/geofred/series
+00028c00: 2f64 6174 613f 7365 7269 6573 5f69 643d  /data?series_id=
+00028c10: 5749 5043 5049 2661 7069 5f6b 6579 3d61  WIPCPI&api_key=a
+00028c20: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
+00028c30: 7273 7475 7677 7879 7a31 3233 3435 3626  rstuvwxyz123456&
+00028c40: 6461 7465 3d32 3031 322d 3031 2d30 310d  date=2012-01-01.
+00028c50: 0a0d 0a20 2020 2020 2020 2023 2320 4150  ...        ## AP
+00028c60: 4920 5265 7370 6f6e 7365 0d0a 2020 2020  I Response..    
+00028c70: 2020 2020 6060 606a 736f 6e0d 0a20 2020      ```json..   
+00028c80: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00028c90: 2020 226d 6574 6122 3a20 7b0d 0a20 2020    "meta": {..   
+00028ca0: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
+00028cb0: 3a20 2250 6572 2043 6170 6974 6120 5065  : "Per Capita Pe
+00028cc0: 7273 6f6e 616c 2049 6e63 6f6d 6520 6279  rsonal Income by
+00028cd0: 2053 7461 7465 2028 446f 6c6c 6172 7329   State (Dollars)
+00028ce0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00028cf0: 2272 6567 696f 6e22 3a20 2273 7461 7465  "region": "state
+00028d00: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00028d10: 2273 6561 736f 6e61 6c69 7479 223a 2022  "seasonality": "
+00028d20: 4e6f 7420 5365 6173 6f6e 616c 6c79 2041  Not Seasonally A
+00028d30: 646a 7573 7465 6422 2c0d 0a20 2020 2020  djusted",..     
+00028d40: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00028d50: 2244 6f6c 6c61 7273 222c 0d0a 2020 2020  "Dollars",..    
+00028d60: 2020 2020 2020 2020 2266 7265 7175 656e          "frequen
+00028d70: 6379 223a 2022 416e 6e75 616c 222c 0d0a  cy": "Annual",..
+00028d80: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
+00028d90: 6522 3a20 2232 3031 322d 3031 2d30 3122  e": "2012-01-01"
+00028da0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00028db0: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
+00028dc0: 2020 2020 2020 2020 2232 3032 3022 3a20          "2020": 
+00028dd0: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00028de0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00028df0: 2020 2020 2020 2020 2272 6567 696f 6e22          "region"
+00028e00: 3a20 2241 6c61 6261 6d61 222c 0d0a 2020  : "Alabama",..  
+00028e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028e20: 2263 6f64 6522 3a20 2230 3122 2c0d 0a20  "code": "01",.. 
+00028e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028e40: 2022 7661 6c75 6522 3a20 2234 3634 3739   "value": "46479
+00028e50: 2e30 222c 0d0a 2020 2020 2020 2020 2020  .0",..          
+00028e60: 2020 2020 2020 2020 2273 6572 6965 735f          "series_
+00028e70: 6964 223a 2022 414c 5043 5049 220d 0a20  id": "ALPCPI".. 
+00028e80: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00028e90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00028ea0: 202e 2e2e 0d0a 2020 2020 2020 2020 2020   .....          
+00028eb0: 2020 5d0d 0a20 2020 2020 2020 2020 207d    ]..          }
+00028ec0: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
+00028ed0: 2020 2020 2060 6060 0d0a 0d0a 2020 2020       ```....    
+00028ee0: 2020 2020 2323 2052 6574 7572 6e73 0d0a      ## Returns..
+00028ef0: 2020 2020 2020 2020 6070 616e 6461 732e          `pandas.
+00028f00: 4461 7461 4672 616d 6560 0d0a 0d0a 2020  DataFrame`....  
+00028f10: 2020 2020 2020 2323 2045 7861 6d70 6c65        ## Example
+00028f20: 2028 6070 616e 6461 732e 4461 7461 4672   (`pandas.DataFr
+00028f30: 616d 6560 290d 0a20 2020 2020 2020 2060  ame`)..        `
+00028f40: 6060 7079 7468 6f6e 0d0a 2020 2020 2020  ``python..      
+00028f50: 2020 3e3e 3e20 6765 6f5f 6672 6564 203d    >>> geo_fred =
+00028f60: 2047 656f 4652 4544 2861 7069 5f6b 6579   GeoFRED(api_key
+00028f70: 3d27 6162 6364 6566 6768 696a 6b6c 6d6e  ='abcdefghijklmn
+00028f80: 6f70 7172 7374 7576 7778 797a 3132 3334  opqrstuvwxyz1234
+00028f90: 3536 2729 0d0a 2020 2020 2020 2020 3e3e  56')..        >>
+00028fa0: 3e20 6765 6f5f 6672 6564 2e73 6572 6965  > geo_fred.serie
+00028fb0: 735f 6461 7461 2873 6572 6965 735f 6964  s_data(series_id
+00028fc0: 3d27 5749 5043 5049 2729 0d0a 2020 2020  ='WIPCPI')..    
+00028fd0: 2020 2020 2020 2020 2020 2072 6567 696f             regio
+00028fe0: 6e20 636f 6465 2020 2020 7661 6c75 6520  n code    value 
+00028ff0: 7365 7269 6573 5f69 6420 2079 6561 720d  series_id  year.
+00029000: 0a20 2020 2020 2020 2030 2020 2020 2041  .        0     A
+00029010: 6c61 6261 6d61 2020 2030 3120 2034 3634  labama   01  464
+00029020: 3739 2e30 2020 2020 414c 5043 5049 2020  79.0    ALPCPI  
+00029030: 3230 3230 0d0a 2020 2020 2020 2020 3120  2020..        1 
+00029040: 2020 2020 2041 6c61 736b 6120 2020 3032       Alaska   02
+00029050: 2020 3633 3530 322e 3020 2020 2041 4b50    63502.0    AKP
+00029060: 4350 4920 2032 3032 300d 0a20 2020 2020  CPI  2020..     
+00029070: 2020 2032 2020 2020 2041 7269 7a6f 6e61     2     Arizona
+00029080: 2020 2030 3420 2034 3936 3438 2e30 2020     04  49648.0  
+00029090: 2020 415a 5043 5049 2020 3230 3230 0d0a    AZPCPI  2020..
+000290a0: 2020 2020 2020 2020 3320 2020 2041 726b          3    Ark
+000290b0: 616e 7361 7320 2020 3035 2020 3437 3233  ansas   05  4723
+000290c0: 352e 3020 2020 2041 5250 4350 4920 2032  5.0    ARPCPI  2
+000290d0: 3032 300d 0a20 2020 2020 2020 2034 2020  020..        4  
+000290e0: 4361 6c69 666f 726e 6961 2020 2030 3620  California   06 
+000290f0: 2037 3031 3932 2e30 2020 2020 4341 5043   70192.0    CAPC
+00029100: 5049 2020 3230 3230 0d0a 2020 2020 2020  PI  2020..      
+00029110: 2020 6060 600d 0a20 2020 2020 2020 2022    ```..        "
+00029120: 2222 0d0a 0d0a 2020 2020 2020 2020 7965  ""....        ye
+00029130: 6172 7320 3d20 7365 6c66 2e5f 636c 6965  ars = self._clie
+00029140: 6e74 2e67 6574 280d 0a20 2020 2020 2020  nt.get(..       
+00029150: 2020 2020 2027 2f67 656f 6672 6564 2f73       '/geofred/s
+00029160: 6572 6965 732f 6461 7461 272c 0d0a 2020  eries/data',..  
+00029170: 2020 2020 2020 2020 2020 276d 6574 612e            'meta.
+00029180: 6461 7461 272c 0d0a 2020 2020 2020 2020  data',..        
+00029190: 2020 2020 7365 7269 6573 5f69 643d 7365      series_id=se
+000291a0: 7269 6573 5f69 642c 0d0a 2020 2020 2020  ries_id,..      
+000291b0: 2020 2020 2020 6461 7465 3d64 6174 652c        date=date,
+000291c0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+000291d0: 6172 745f 6461 7465 3d73 7461 7274 5f64  art_date=start_d
+000291e0: 6174 650d 0a20 2020 2020 2020 2029 0d0a  ate..        )..
+000291f0: 0d0a 2020 2020 2020 2020 6466 203d 2070  ..        df = p
+00029200: 642e 4461 7461 4672 616d 6528 0d0a 2020  d.DataFrame(..  
+00029210: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00029220: 6164 645f 7965 6172 7328 7965 6172 735b  add_years(years[
+00029230: 305d 290d 0a20 2020 2020 2020 2029 0d0a  0])..        )..
+00029240: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00029250: 2064 662e 656d 7074 793a 0d0a 2020 2020   df.empty:..    
+00029260: 2020 2020 2020 2020 6466 2e76 616c 7565          df.value
+00029270: 203d 2064 662e 7661 6c75 652e 7265 706c   = df.value.repl
+00029280: 6163 6528 7365 6c66 2e45 4d50 5459 5f56  ace(self.EMPTY_V
+00029290: 414c 5545 2c20 6e70 2e6e 616e 290d 0a0d  ALUE, np.nan)...
+000292a0: 0a20 2020 2020 2020 2020 2020 2064 6620  .            df 
+000292b0: 3d20 6466 2e61 7374 7970 6528 6474 7970  = df.astype(dtyp
+000292c0: 653d 7b0d 0a20 2020 2020 2020 2020 2020  e={..           
+000292d0: 2020 2020 2027 7661 6c75 6527 3a20 2766       'value': 'f
+000292e0: 6c6f 6174 3634 272c 0d0a 2020 2020 2020  loat64',..      
+000292f0: 2020 2020 2020 2020 2020 2779 6561 7227            'year'
+00029300: 3a20 2769 6e74 3634 270d 0a20 2020 2020  : 'int64'..     
+00029310: 2020 2020 2020 207d 290d 0a0d 0a20 2020         })....   
+00029320: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
+00029330: 0d0a 2020 2020 6465 6620 7265 6769 6f6e  ..    def region
+00029340: 616c 5f64 6174 6128 0d0a 2020 2020 2020  al_data(..      
+00029350: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+00029360: 2020 2020 2020 2020 2073 6572 6965 735f           series_
+00029370: 6772 6f75 703a 2073 7472 2c0d 0a20 2020  group: str,..   
+00029380: 2020 2020 2020 2020 2072 6567 696f 6e5f           region_
+00029390: 7479 7065 3a20 656e 756d 732e 5265 6769  type: enums.Regi
+000293a0: 6f6e 5479 7065 2c0d 0a20 2020 2020 2020  onType,..       
+000293b0: 2020 2020 2064 6174 653a 2064 6174 652c       date: date,
+000293c0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000293d0: 6173 6f6e 3a20 656e 756d 732e 5365 6173  ason: enums.Seas
+000293e0: 6f6e 616c 6974 792c 0d0a 2020 2020 2020  onality,..      
+000293f0: 2020 2020 2020 756e 6974 733a 2073 7472        units: str
+00029400: 203d 2027 446f 6c6c 6172 7327 2c20 2023   = 'Dollars',  #
+00029410: 2044 6f63 756d 656e 7461 7469 6f6e 2069   Documentation i
+00029420: 7320 6d69 7373 696e 670d 0a20 2020 2020  s missing..     
+00029430: 2020 2020 2020 2073 7461 7274 5f64 6174         start_dat
+00029440: 653a 2064 6174 6520 3d20 4e6f 6e65 2c0d  e: date = None,.
+00029450: 0a20 2020 2020 2020 2020 2020 2066 7265  .            fre
+00029460: 7175 656e 6379 3a20 656e 756d 732e 4672  quency: enums.Fr
+00029470: 6571 7565 6e63 7920 3d20 4e6f 6e65 2c0d  equency = None,.
+00029480: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+00029490: 6e73 666f 726d 6174 696f 6e3a 2065 6e75  nsformation: enu
+000294a0: 6d73 2e55 6e69 7420 3d20 656e 756d 732e  ms.Unit = enums.
+000294b0: 556e 6974 2e6c 696e 2c0d 0a20 2020 2020  Unit.lin,..     
+000294c0: 2020 2020 2020 2061 6767 7265 6761 7469         aggregati
+000294d0: 6f6e 5f6d 6574 686f 643a 2065 6e75 6d73  on_method: enums
+000294e0: 2e41 6767 7265 6761 7469 6f6e 4d65 7468  .AggregationMeth
+000294f0: 6f64 203d 2065 6e75 6d73 2e41 6767 7265  od = enums.Aggre
+00029500: 6761 7469 6f6e 4d65 7468 6f64 2e61 7665  gationMethod.ave
+00029510: 7261 6765 0d0a 2020 2020 2920 2d3e 2070  rage..    ) -> p
+00029520: 642e 4461 7461 4672 616d 653a 0d0a 2020  d.DataFrame:..  
+00029530: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00029540: 2020 2023 2320 5061 7261 6d65 7465 7273     ## Parameters
+00029550: 0d0a 0d0a 2020 2020 2020 2020 6073 6572  ....        `ser
+00029560: 6965 735f 6772 6f75 7060 0d0a 2020 2020  ies_group`..    
+00029570: 2020 2020 5468 6520 4944 2066 6f72 2061      The ID for a
+00029580: 2067 726f 7570 206f 6620 7365 7269 6573   group of series
+00029590: 7320 666f 756e 6420 696e 2047 656f 4652  s found in GeoFR
+000295a0: 4544 2e0d 0a0d 0a20 2020 2020 2020 2060  ED.....        `
+000295b0: 7265 6769 6f6e 5f74 7970 6560 0d0a 2020  region_type`..  
+000295c0: 2020 2020 2020 5468 6520 7265 6769 6f6e        The region
+000295d0: 2079 6f75 2077 616e 7420 7761 6e74 2074   you want want t
+000295e0: 6f20 7075 6c6c 2064 6174 6120 666f 722e  o pull data for.
+000295f0: 0d0a 0d0a 2020 2020 2020 2020 6064 6174  ....        `dat
+00029600: 650d 0a20 2020 2020 2020 2054 6865 2064  e..        The d
+00029610: 6174 6520 796f 7520 7761 6e74 2074 6f20  ate you want to 
+00029620: 7075 6c6c 2061 2073 6572 6965 7320 6772  pull a series gr
+00029630: 6f75 7020 6461 7461 2066 726f 6d2e 0d0a  oup data from...
+00029640: 0d0a 2020 2020 2020 2020 6073 7461 7274  ..        `start
+00029650: 5f64 6174 6560 0d0a 2020 2020 2020 2020  _date`..        
+00029660: 5468 6520 7374 6172 7420 6461 7465 2079  The start date y
+00029670: 6f75 2077 616e 7420 746f 2072 6571 7565  ou want to reque
+00029680: 7374 2073 6572 6965 7320 6772 6f75 7020  st series group 
+00029690: 6461 7461 2066 726f 6d2e 0d0a 2020 2020  data from...    
+000296a0: 2020 2020 5468 6973 2061 6c6c 6f77 7320      This allows 
+000296b0: 796f 7520 746f 2070 756c 6c20 6120 7261  you to pull a ra
+000296c0: 6e67 6520 6f66 2064 6174 610d 0a0d 0a20  nge of data.... 
+000296d0: 2020 2020 2020 2060 756e 6974 7360 0d0a         `units`..
+000296e0: 2020 2020 2020 2020 5468 6520 756e 6974          The unit
+000296f0: 7320 6f66 2074 6865 2073 6572 6965 7320  s of the series 
+00029700: 796f 7520 7761 6e74 2074 6f20 7075 6c6c  you want to pull
+00029710: 2e0d 0a0d 0a20 2020 2020 2020 2060 7365  .....        `se
+00029720: 6173 6f6e 600d 0a20 2020 2020 2020 2054  ason`..        T
+00029730: 6865 2073 6561 736f 6e61 6c69 7479 206f  he seasonality o
+00029740: 6620 7468 6520 7365 7269 6573 2067 726f  f the series gro
+00029750: 7570 2e0d 0a0d 0a20 2020 2020 2020 2060  up.....        `
+00029760: 6672 6571 7565 6e63 7960 0d0a 2020 2020  frequency`..    
+00029770: 2020 2020 416e 206f 7074 696f 6e61 6c20      An optional 
+00029780: 7061 7261 6d65 7465 7220 7468 6174 2069  parameter that i
+00029790: 6e64 6963 6174 6573 2061 206c 6f77 6572  ndicates a lower
+000297a0: 2066 7265 7175 656e 6379 2074 6f20 6167   frequency to ag
+000297b0: 6772 6567 6174 6520 7661 6c75 6573 2074  gregate values t
+000297c0: 6f2e 0d0a 2020 2020 2020 2020 5468 6520  o...        The 
+000297d0: 4765 6f46 5245 4420 6672 6571 7565 6e63  GeoFRED frequenc
+000297e0: 7920 6167 6772 6567 6174 696f 6e20 6665  y aggregation fe
+000297f0: 6174 7572 6520 636f 6e76 6572 7473 2068  ature converts h
+00029800: 6967 6865 7220 6672 6571 7565 6e63 7920  igher frequency 
+00029810: 6461 7461 2073 6572 6965 7320 696e 746f  data series into
+00029820: 206c 6f77 6572 2066 7265 7175 656e 6379   lower frequency
+00029830: 2064 6174 6120 7365 7269 6573 2028 652e   data series (e.
+00029840: 672e 2063 6f6e 7665 7274 7320 6120 6d6f  g. converts a mo
+00029850: 6e74 686c 7920 6461 7461 2073 6572 6965  nthly data serie
+00029860: 7320 696e 746f 2061 6e20 616e 6e75 616c  s into an annual
+00029870: 2064 6174 6120 7365 7269 6573 292e 0d0a   data series)...
+00029880: 2020 2020 2020 2020 496e 2047 656f 4652          In GeoFR
+00029890: 4544 2c20 7468 6520 6869 6768 6573 7420  ED, the highest 
+000298a0: 6672 6571 7565 6e63 7920 6461 7461 2069  frequency data i
+000298b0: 7320 6461 696c 792c 2061 6e64 2074 6865  s daily, and the
+000298c0: 206c 6f77 6573 7420 6672 6571 7565 6e63   lowest frequenc
+000298d0: 7920 6461 7461 2069 7320 616e 6e75 616c  y data is annual
+000298e0: 2e0d 0a20 2020 2020 2020 2054 6865 7265  ...        There
+000298f0: 2061 7265 2033 2061 6767 7265 6761 7469   are 3 aggregati
+00029900: 6f6e 206d 6574 686f 6473 2061 7661 696c  on methods avail
+00029910: 6162 6c65 2d20 6176 6572 6167 652c 2073  able- average, s
+00029920: 756d 2c20 616e 6420 656e 6420 6f66 2070  um, and end of p
+00029930: 6572 696f 642e 0d0a 2020 2020 2020 2020  eriod...        
+00029940: 5365 6520 7468 6520 6167 6772 6567 6174  See the aggregat
+00029950: 696f 6e5f 6d65 7468 6f64 2070 6172 616d  ion_method param
+00029960: 6574 6572 2e0d 0a0d 0a20 2020 2020 2020  eter.....       
+00029970: 2060 7472 616e 7366 6f72 6d61 7469 6f6e   `transformation
+00029980: 600d 0a20 2020 2020 2020 2041 206b 6579  `..        A key
+00029990: 2074 6861 7420 696e 6469 6361 7465 7320   that indicates 
+000299a0: 6120 6461 7461 2076 616c 7565 2074 7261  a data value tra
+000299b0: 6e73 666f 726d 6174 696f 6e2e 0d0a 0d0a  nsformation.....
+000299c0: 2020 2020 2020 2020 2323 2044 6573 6372          ## Descr
+000299d0: 6970 7469 6f6e 0d0a 2020 2020 2020 2020  iption..        
+000299e0: 6874 7470 733a 2f2f 6765 6f66 7265 642e  https://geofred.
+000299f0: 7374 6c6f 7569 7366 6564 2e6f 7267 2f64  stlouisfed.org/d
+00029a00: 6f63 732f 6170 692f 6765 6f66 7265 642f  ocs/api/geofred/
+00029a10: 7265 6769 6f6e 616c 5f64 6174 612e 6874  regional_data.ht
+00029a20: 6d6c 0d0a 0d0a 2020 2020 2020 2020 5468  ml....        Th
+00029a30: 6973 2072 6571 7565 7374 2072 6574 7572  is request retur
+00029a40: 6e73 2061 2063 726f 7373 2073 6563 7469  ns a cross secti
+00029a50: 6f6e 206f 6620 7265 6769 6f6e 616c 2064  on of regional d
+00029a60: 6174 610d 0a0d 0a20 2020 2020 2020 2023  ata....        #
+00029a70: 2320 4150 4920 5265 7175 6573 7420 2848  # API Request (H
+00029a80: 5454 5053 2047 4554 290d 0a20 2020 2020  TTPS GET)..     
+00029a90: 2020 2068 7474 7073 3a2f 2f61 7069 2e73     https://api.s
+00029aa0: 746c 6f75 6973 6665 642e 6f72 672f 6765  tlouisfed.org/ge
+00029ab0: 6f66 7265 642f 7265 6769 6f6e 616c 2f64  ofred/regional/d
+00029ac0: 6174 613f 6170 695f 6b65 793d 6162 6364  ata?api_key=abcd
+00029ad0: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
+00029ae0: 7576 7778 797a 3132 3334 3536 2673 6572  uvwxyz123456&ser
+00029af0: 6965 735f 6772 6f75 703d 3838 3226 6461  ies_group=882&da
+00029b00: 7465 3d32 3031 332d 3031 2d30 3126 7265  te=2013-01-01&re
+00029b10: 6769 6f6e 5f74 7970 653d 7374 6174 6526  gion_type=state&
+00029b20: 756e 6974 733d 446f 6c6c 6172 7326 6672  units=Dollars&fr
+00029b30: 6571 7565 6e63 793d 6126 7365 6173 6f6e  equency=a&season
+00029b40: 3d4e 5341 0d0a 2020 2020 2020 2020 2323  =NSA..        ##
+00029b50: 2041 5049 2052 6573 706f 6e73 650d 0a20   API Response.. 
+00029b60: 2020 2020 2020 2060 6060 6a73 6f6e 0d0a         ```json..
+00029b70: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00029b80: 2020 2020 2022 6d65 7461 223a 207b 0d0a       "meta": {..
+00029b90: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
+00029ba0: 6c65 223a 2022 5065 7220 4361 7069 7461  le": "Per Capita
+00029bb0: 2050 6572 736f 6e61 6c20 496e 636f 6d65   Personal Income
+00029bc0: 2062 7920 5374 6174 6520 2844 6f6c 6c61   by State (Dolla
+00029bd0: 7273 2922 2c0d 0a20 2020 2020 2020 2020  rs)",..         
+00029be0: 2020 2022 7265 6769 6f6e 223a 2022 7374     "region": "st
+00029bf0: 6174 6522 2c0d 0a20 2020 2020 2020 2020  ate",..         
+00029c00: 2020 2022 7365 6173 6f6e 616c 6974 7922     "seasonality"
+00029c10: 3a20 224e 6f74 2053 6561 736f 6e61 6c6c  : "Not Seasonall
+00029c20: 7920 4164 6a75 7374 6564 222c 0d0a 2020  y Adjusted",..  
+00029c30: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+00029c40: 223a 2022 446f 6c6c 6172 7322 2c0d 0a20  ": "Dollars",.. 
+00029c50: 2020 2020 2020 2020 2020 2022 6672 6571             "freq
+00029c60: 7565 6e63 7922 3a20 2241 6e6e 7561 6c22  uency": "Annual"
+00029c70: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00029c80: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
+00029c90: 2020 2020 2020 2020 2232 3031 3322 3a20          "2013": 
+00029ca0: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00029cb0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00029cc0: 2020 2020 2020 2020 2272 6567 696f 6e22          "region"
+00029cd0: 3a20 2241 6c61 6261 6d61 222c 0d0a 2020  : "Alabama",..  
+00029ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029cf0: 2263 6f64 6522 3a20 2230 3122 2c0d 0a20  "code": "01",.. 
+00029d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d10: 2022 7661 6c75 6522 3a20 2233 3632 3538   "value": "36258
+00029d20: 2e30 222c 0d0a 2020 2020 2020 2020 2020  .0",..          
+00029d30: 2020 2020 2020 2020 2273 6572 6965 735f          "series_
+00029d40: 6964 223a 2022 414c 5043 5049 220d 0a20  id": "ALPCPI".. 
+00029d50: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00029d60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00029d70: 2020 202e 2e2e 0d0a 2020 2020 2020 2020     .....        
+00029d80: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
+00029d90: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00029da0: 2020 2020 7d0d 0a20 2020 2020 2020 207d      }..        }
+00029db0: 0d0a 2020 2020 2020 2020 6060 600d 0a0d  ..        ```...
+00029dc0: 0a20 2020 2020 2020 2023 2320 5265 7475  .        ## Retu
+00029dd0: 726e 730d 0a20 2020 2020 2020 2060 7061  rns..        `pa
+00029de0: 6e64 6173 2e44 6174 6146 7261 6d65 600d  ndas.DataFrame`.
+00029df0: 0a0d 0a20 2020 2020 2020 2023 2320 4578  ...        ## Ex
+00029e00: 616d 706c 6520 2860 7061 6e64 6173 2e44  ample (`pandas.D
+00029e10: 6174 6146 7261 6d65 6029 0d0a 2020 2020  ataFrame`)..    
+00029e20: 2020 2020 6060 6070 7974 686f 6e0d 0a20      ```python.. 
+00029e30: 2020 2020 2020 203e 3e3e 2067 656f 5f66         >>> geo_f
+00029e40: 7265 6420 3d20 4765 6f46 5245 4428 6170  red = GeoFRED(ap
+00029e50: 695f 6b65 793d 2761 6263 6465 6667 6869  i_key='abcdefghi
+00029e60: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
+00029e70: 7a31 3233 3435 3627 290d 0a20 2020 2020  z123456')..     
+00029e80: 2020 203e 3e3e 2067 656f 5f66 7265 642e     >>> geo_fred.
+00029e90: 7265 6769 6f6e 616c 5f64 6174 6128 7365  regional_data(se
+00029ea0: 7269 6573 5f67 726f 7570 3d27 3838 3227  ries_group='882'
+00029eb0: 2c20 6461 7465 3d64 6174 6528 3230 3133  , date=date(2013
+00029ec0: 2c20 312c 2031 292c 2072 6567 696f 6e5f  , 1, 1), region_
+00029ed0: 7479 7065 3d52 6567 696f 6e54 7970 652e  type=RegionType.
+00029ee0: 7374 6174 652c 2066 7265 7175 656e 6379  state, frequency
+00029ef0: 3d46 7265 7175 656e 6379 2e61 6e75 616c  =Frequency.anual
+00029f00: 2c20 7365 6173 6f6e 3d53 6561 736f 6e61  , season=Seasona
+00029f10: 6c69 7479 2e6e 6f74 5f73 6561 736f 6e61  lity.not_seasona
+00029f20: 6c6c 795f 6164 6a75 7374 6564 290d 0a20  lly_adjusted).. 
+00029f30: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00029f40: 6769 6f6e 2063 6f64 6520 2020 2076 616c  gion code    val
+00029f50: 7565 2073 6572 6965 735f 6964 2020 7965  ue series_id  ye
+00029f60: 6172 0d0a 2020 2020 2020 2020 3020 2020  ar..        0   
+00029f70: 2020 416c 6162 616d 6120 2020 3031 2020    Alabama   01  
+00029f80: 3336 3235 382e 3020 2020 2041 4c50 4350  36258.0    ALPCP
+00029f90: 4920 2032 3031 330d 0a20 2020 2020 2020  I  2013..       
+00029fa0: 2031 2020 2020 2020 416c 6173 6b61 2020   1      Alaska  
+00029fb0: 2030 3220 2035 3238 3433 2e30 2020 2020   02  52843.0    
+00029fc0: 414b 5043 5049 2020 3230 3133 0d0a 2020  AKPCPI  2013..  
+00029fd0: 2020 2020 2020 3220 2020 2020 4172 697a        2     Ariz
+00029fe0: 6f6e 6120 2020 3034 2020 3336 3733 392e  ona   04  36739.
+00029ff0: 3020 2020 2041 5a50 4350 4920 2032 3031  0    AZPCPI  201
+0002a000: 330d 0a20 2020 2020 2020 2033 2020 2020  3..        3    
+0002a010: 4172 6b61 6e73 6173 2020 2030 3520 2033  Arkansas   05  3
+0002a020: 3636 3035 2e30 2020 2020 4152 5043 5049  6605.0    ARPCPI
+0002a030: 2020 3230 3133 0d0a 2020 2020 2020 2020    2013..        
+0002a040: 3420 2043 616c 6966 6f72 6e69 6120 2020  4  California   
+0002a050: 3036 2020 3438 3534 392e 3020 2020 2043  06  48549.0    C
+0002a060: 4150 4350 4920 2032 3031 330d 0a20 2020  APCPI  2013..   
+0002a070: 2020 2020 2060 6060 0d0a 2020 2020 2020       ```..      
+0002a080: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+0002a090: 2069 6620 6672 6571 7565 6e63 7920 6973   if frequency is
+0002a0a0: 206e 6f74 204e 6f6e 6520 616e 6420 6672   not None and fr
+0002a0b0: 6571 7565 6e63 7920 6e6f 7420 696e 2065  equency not in e
+0002a0c0: 6e75 6d73 2e46 7265 7175 656e 6379 3a0d  nums.Frequency:.
+0002a0d0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0002a0e0: 7365 2056 616c 7565 4572 726f 7228 2756  se ValueError('V
+0002a0f0: 6172 6961 626c 6520 6672 6571 7565 6e63  ariable frequenc
+0002a100: 7920 6973 206e 6f74 206f 6e65 206f 6620  y is not one of 
+0002a110: 7468 6520 7661 6c75 6573 3a20 7b7d 272e  the values: {}'.
+0002a120: 666f 726d 6174 2827 2c20 272e 6a6f 696e  format(', '.join
+0002a130: 286d 6170 2873 7472 2c20 656e 756d 732e  (map(str, enums.
+0002a140: 4672 6571 7565 6e63 7929 2929 290d 0a0d  Frequency))))...
+0002a150: 0a20 2020 2020 2020 2069 6620 6167 6772  .        if aggr
+0002a160: 6567 6174 696f 6e5f 6d65 7468 6f64 206e  egation_method n
+0002a170: 6f74 2069 6e20 656e 756d 732e 4167 6772  ot in enums.Aggr
+0002a180: 6567 6174 696f 6e4d 6574 686f 643a 0d0a  egationMethod:..
+0002a190: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0002a1a0: 6520 5661 6c75 6545 7272 6f72 2827 5661  e ValueError('Va
+0002a1b0: 7269 6162 6c65 2061 6767 7265 6761 7469  riable aggregati
+0002a1c0: 6f6e 5f6d 6574 686f 6420 6973 206e 6f74  on_method is not
+0002a1d0: 206f 6e65 206f 6620 7468 6520 7661 6c75   one of the valu
+0002a1e0: 6573 3a20 7b7d 272e 666f 726d 6174 2827  es: {}'.format('
+0002a1f0: 2c20 272e 6a6f 696e 286d 6170 2873 7472  , '.join(map(str
+0002a200: 2c20 656e 756d 732e 4167 6772 6567 6174  , enums.Aggregat
+0002a210: 696f 6e4d 6574 686f 6429 2929 290d 0a0d  ionMethod))))...
+0002a220: 0a20 2020 2020 2020 2069 6620 7472 616e  .        if tran
+0002a230: 7366 6f72 6d61 7469 6f6e 206e 6f74 2069  sformation not i
+0002a240: 6e20 656e 756d 732e 556e 6974 3a0d 0a20  n enums.Unit:.. 
+0002a250: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0002a260: 2056 616c 7565 4572 726f 7228 2756 6172   ValueError('Var
+0002a270: 6961 626c 6520 7472 616e 7366 6f72 6d61  iable transforma
+0002a280: 7469 6f6e 2069 7320 6e6f 7420 6f6e 6520  tion is not one 
+0002a290: 6f66 2074 6865 2076 616c 7565 733a 207b  of the values: {
+0002a2a0: 7d27 2e66 6f72 6d61 7428 272c 2027 2e6a  }'.format(', '.j
+0002a2b0: 6f69 6e28 6d61 7028 7374 722c 2065 6e75  oin(map(str, enu
+0002a2c0: 6d73 2e55 6e69 7429 2929 290d 0a0d 0a20  ms.Unit)))).... 
+0002a2d0: 2020 2020 2020 2079 6561 7273 203d 2073         years = s
+0002a2e0: 656c 662e 5f63 6c69 656e 742e 6765 7428  elf._client.get(
+0002a2f0: 0d0a 2020 2020 2020 2020 2020 2020 272f  ..            '/
+0002a300: 6765 6f66 7265 642f 7265 6769 6f6e 616c  geofred/regional
+0002a310: 2f64 6174 6127 2c0d 0a20 2020 2020 2020  /data',..       
+0002a320: 2020 2020 2027 6d65 7461 2e64 6174 6127       'meta.data'
+0002a330: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+0002a340: 6572 6965 735f 6772 6f75 703d 7365 7269  eries_group=seri
+0002a350: 6573 5f67 726f 7570 2c0d 0a20 2020 2020  es_group,..     
+0002a360: 2020 2020 2020 2072 6567 696f 6e5f 7479         region_ty
+0002a370: 7065 3d72 6567 696f 6e5f 7479 7065 2c0d  pe=region_type,.
+0002a380: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0002a390: 653d 6461 7465 2c0d 0a20 2020 2020 2020  e=date,..       
+0002a3a0: 2020 2020 2075 6e69 7473 3d75 6e69 7473       units=units
+0002a3b0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+0002a3c0: 6561 736f 6e3d 7365 6173 6f6e 2c0d 0a20  eason=season,.. 
+0002a3d0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+0002a3e0: 5f64 6174 653d 7374 6172 745f 6461 7465  _date=start_date
+0002a3f0: 2c0d 0a20 2020 2020 2020 2020 2020 2066  ,..            f
+0002a400: 7265 7175 656e 6379 3d66 7265 7175 656e  requency=frequen
+0002a410: 6379 2c0d 0a20 2020 2020 2020 2020 2020  cy,..           
+0002a420: 2074 7261 6e73 666f 726d 6174 696f 6e3d   transformation=
+0002a430: 7472 616e 7366 6f72 6d61 7469 6f6e 2c0d  transformation,.
+0002a440: 0a20 2020 2020 2020 2020 2020 2061 6767  .            agg
+0002a450: 7265 6761 7469 6f6e 5f6d 6574 686f 643d  regation_method=
+0002a460: 6167 6772 6567 6174 696f 6e5f 6d65 7468  aggregation_meth
+0002a470: 6f64 0d0a 2020 2020 2020 2020 290d 0a0d  od..        )...
+0002a480: 0a20 2020 2020 2020 2064 6620 3d20 7064  .        df = pd
+0002a490: 2e44 6174 6146 7261 6d65 280d 0a20 2020  .DataFrame(..   
+0002a4a0: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+0002a4b0: 6464 5f79 6561 7273 2879 6561 7273 5b30  dd_years(years[0
+0002a4c0: 5d29 0d0a 2020 2020 2020 2020 290d 0a0d  ])..        )...
+0002a4d0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0002a4e0: 6466 2e65 6d70 7479 3a0d 0a20 2020 2020  df.empty:..     
+0002a4f0: 2020 2020 2020 2064 662e 7661 6c75 6520         df.value 
+0002a500: 3d20 6466 2e76 616c 7565 2e72 6570 6c61  = df.value.repla
+0002a510: 6365 2873 656c 662e 454d 5054 595f 5641  ce(self.EMPTY_VA
+0002a520: 4c55 452c 206e 702e 6e61 6e29 0d0a 0d0a  LUE, np.nan)....
+0002a530: 2020 2020 2020 2020 2020 2020 6466 203d              df =
+0002a540: 2064 662e 6173 7479 7065 2864 7479 7065   df.astype(dtype
+0002a550: 3d7b 0d0a 2020 2020 2020 2020 2020 2020  ={..            
+0002a560: 2020 2020 2776 616c 7565 273a 2027 666c      'value': 'fl
+0002a570: 6f61 7436 3427 2c0d 0a20 2020 2020 2020  oat64',..       
+0002a580: 2020 2020 2020 2020 2027 7965 6172 273a           'year':
+0002a590: 2027 696e 7436 3427 0d0a 2020 2020 2020   'int64'..      
+0002a5a0: 2020 2020 2020 7d29 0d0a 0d0a 2020 2020        })....    
+0002a5b0: 2020 2020 7265 7475 726e 2064 660d 0a0d      return df...
+0002a5c0: 0a20 2020 2064 6566 205f 6164 645f 7965  .    def _add_ye
+0002a5d0: 6172 7328 7365 6c66 2c20 6461 7461 3a20  ars(self, data: 
+0002a5e0: 6469 6374 2920 2d3e 2047 656e 6572 6174  dict) -> Generat
+0002a5f0: 6f72 5b64 6963 742c 204e 6f6e 652c 204e  or[dict, None, N
+0002a600: 6f6e 655d 3a0d 0a20 2020 2020 2020 2022  one]:..        "
+0002a610: 2222 0d0a 2020 2020 2020 2020 7472 616e  ""..        tran
+0002a620: 7366 6f72 6d20 6469 6374 2069 6e64 6578  sform dict index
+0002a630: 6564 2062 7920 7965 6172 2066 726f 6d3a  ed by year from:
+0002a640: 0d0a 2020 2020 2020 2020 6060 606a 736f  ..        ```jso
+0002a650: 6e0d 0a20 2020 2020 2020 207b 0d0a 2020  n..        {..  
+0002a660: 2020 2020 2020 2020 2232 3032 3022 3a20          "2020": 
+0002a670: 5b0d 0a20 2020 2020 2020 2020 2020 207b  [..            {
+0002a680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0002a690: 2272 6567 696f 6e22 3a20 2241 6c61 6261  "region": "Alaba
+0002a6a0: 6d61 222c 0d0a 2020 2020 2020 2020 2020  ma",..          
+0002a6b0: 2020 2020 2263 6f64 6522 3a20 2230 3122      "code": "01"
+0002a6c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0002a6d0: 2022 7661 6c75 6522 3a20 2234 3634 3739   "value": "46479
+0002a6e0: 2e30 222c 0d0a 2020 2020 2020 2020 2020  .0",..          
+0002a6f0: 2020 2020 2273 6572 6965 735f 6964 223a      "series_id":
+0002a700: 2022 414c 5043 5049 220d 0a20 2020 2020   "ALPCPI"..     
+0002a710: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
+0002a720: 2020 2020 2020 202e 2e2e 0d0a 2020 2020         .....    
+0002a730: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
+0002a740: 207d 0d0a 2020 2020 2020 2020 6060 600d   }..        ```.
+0002a750: 0a20 2020 2020 2020 2074 6f0d 0a20 2020  .        to..   
+0002a760: 2020 2020 2060 6060 6a73 6f6e 0d0a 2020       ```json..  
+0002a770: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
+0002a780: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+0002a790: 2020 2272 6567 696f 6e22 3a20 2241 6c61    "region": "Ala
+0002a7a0: 6261 6d61 222c 0d0a 2020 2020 2020 2020  bama",..        
+0002a7b0: 2020 2020 2263 6f64 6522 3a20 2230 3122      "code": "01"
+0002a7c0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+0002a7d0: 7661 6c75 6522 3a20 2234 3634 3739 2e30  value": "46479.0
+0002a7e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0002a7f0: 2273 6572 6965 735f 6964 223a 2022 414c  "series_id": "AL
+0002a800: 5043 5049 222c 0d0a 2020 2020 2020 2020  PCPI",..        
+0002a810: 2020 2020 2279 6561 7222 3a20 2232 3032      "year": "202
+0002a820: 3022 0d0a 2020 2020 2020 2020 2020 7d2c  0"..          },
+0002a830: 0d0a 2020 2020 2020 2020 2020 2e2e 2e0d  ..          ....
+0002a840: 0a20 2020 2020 2020 205d 0d0a 2020 2020  .        ]..    
+0002a850: 2020 2020 6060 600d 0a20 2020 2020 2020      ```..       
+0002a860: 2022 2222 0d0a 2020 2020 2020 2020 666f   """..        fo
+0002a870: 7220 7965 6172 2c20 726f 7773 2069 6e20  r year, rows in 
+0002a880: 6461 7461 2e69 7465 6d73 2829 3a0d 0a20  data.items():.. 
+0002a890: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
+0002a8a0: 6f77 2069 6e20 726f 7773 3a0d 0a20 2020  ow in rows:..   
+0002a8b0: 2020 2020 2020 2020 2020 2020 2072 6f77               row
+0002a8c0: 5b27 7965 6172 275d 203d 2079 6561 720d  ['year'] = year.
+0002a8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a8e0: 2079 6965 6c64 2072 6f77 0d0a 0d0a 0d0a   yield row......
+0002a8f0: 636c 6173 7320 4652 4153 4552 3a0d 0a20  class FRASER:.. 
+0002a900: 2020 2022 2222 0d0a 2020 2020 4652 4153     """..    FRAS
+0002a910: 4552 2069 7320 6120 6469 6769 7461 6c20  ER is a digital 
+0002a920: 6c69 6272 6172 7920 6f66 2055 2e53 2e20  library of U.S. 
+0002a930: 6563 6f6e 6f6d 6963 2c20 6669 6e61 6e63  economic, financ
+0002a940: 6961 6c2c 2061 6e64 2062 616e 6b69 6e67  ial, and banking
+0002a950: 2068 6973 746f 7279 e280 9470 6172 7469   history...parti
+0002a960: 6375 6c61 726c 7920 7468 6520 6869 7374  cularly the hist
+0002a970: 6f72 7920 6f66 2074 6865 2046 6564 6572  ory of the Feder
+0002a980: 616c 2052 6573 6572 7665 2053 7973 7465  al Reserve Syste
+0002a990: 6d2e 0d0a 0d0a 2020 2020 5072 6f76 6964  m.....    Provid
+0002a9a0: 696e 6720 6563 6f6e 6f6d 6963 2069 6e66  ing economic inf
+0002a9b0: 6f72 6d61 7469 6f6e 2061 6e64 2064 6174  ormation and dat
+0002a9c0: 6120 746f 2074 6865 2070 7562 6c69 6320  a to the public 
+0002a9d0: 6973 2061 6e20 696d 706f 7274 616e 7420  is an important 
+0002a9e0: 6d69 7373 696f 6e20 666f 7220 7468 6520  mission for the 
+0002a9f0: 5374 2e20 4c6f 7569 7320 4665 6420 7374  St. Louis Fed st
+0002aa00: 6172 7465 6420 6279 2066 6f72 6d65 7220  arted by former 
+0002aa10: 5374 2e20 4c6f 7569 7320 4665 6420 5265  St. Louis Fed Re
+0002aa20: 7365 6172 6368 2044 6972 6563 746f 7220  search Director 
+0002aa30: 486f 6d65 7220 4a6f 6e65 7320 696e 2031  Homer Jones in 1
+0002aa40: 3935 382e 0d0a 2020 2020 4652 4153 4552  958...    FRASER
+0002aa50: 2062 6567 616e 2061 7320 6120 6461 7461   began as a data
+0002aa60: 2070 7265 7365 7276 6174 696f 6e20 616e   preservation an
+0002aa70: 6420 6163 6365 7373 6962 696c 6974 7920  d accessibility 
+0002aa80: 7072 6f6a 6563 7420 6f66 2074 6865 2046  project of the F
+0002aa90: 6564 6572 616c 2052 6573 6572 7665 2042  ederal Reserve B
+0002aaa0: 616e 6b20 6f66 2053 742e 204c 6f75 6973  ank of St. Louis
+0002aab0: 2069 6e20 3230 3034 2061 6e64 206e 6f77   in 2004 and now
+0002aac0: 2070 726f 7669 6465 7320 6163 6365 7373   provides access
+0002aad0: 2074 6f20 6461 7461 2061 6e64 2070 6f6c   to data and pol
+0002aae0: 6963 7920 646f 6375 6d65 6e74 7320 6672  icy documents fr
+0002aaf0: 6f6d 2074 6865 2046 6564 6572 616c 2052  om the Federal R
+0002ab00: 6573 6572 7665 2053 7973 7465 6d20 616e  eserve System an
+0002ab10: 6420 6d61 6e79 206f 7468 6572 2069 6e73  d many other ins
+0002ab20: 7469 7475 7469 6f6e 732e 0d0a 0d0a 2020  titutions.....  
+0002ab30: 2020 6874 7470 733a 2f2f 6672 6173 6572    https://fraser
+0002ab40: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
+0002ab50: 0d0a 2020 2020 6874 7470 733a 2f2f 7265  ..    https://re
+0002ab60: 7365 6172 6368 2e73 746c 6f75 6973 6665  search.stlouisfe
+0002ab70: 642e 6f72 672f 646f 6373 2f61 7069 2f66  d.org/docs/api/f
+0002ab80: 7261 7365 722f 0d0a 2020 2020 2222 220d  raser/..    """.
+0002ab90: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+0002aba0: 745f 5f28 7365 6c66 293a 0d0a 2020 2020  t__(self):..    
+0002abb0: 2020 2020 7365 6c66 2e5f 7369 636b 6c65      self._sickle
+0002abc0: 203d 2073 6963 6b6c 652e 5369 636b 6c65   = sickle.Sickle
+0002abd0: 2827 6874 7470 733a 2f2f 6672 6173 6572  ('https://fraser
+0002abe0: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
+0002abf0: 6f61 6927 290d 0a0d 0a20 2020 2064 6566  oai')....    def
+0002ac00: 206c 6973 745f 7265 636f 7264 7328 7365   list_records(se
+0002ac10: 6c66 2c20 6967 6e6f 7265 5f64 656c 6574  lf, ignore_delet
+0002ac20: 6564 3a20 626f 6f6c 203d 2046 616c 7365  ed: bool = False
+0002ac30: 2c20 7365 743a 2073 7472 203d 204e 6f6e  , set: str = Non
+0002ac40: 6529 202d 3e20 7369 636b 6c65 2e69 7465  e) -> sickle.ite
+0002ac50: 7261 746f 722e 4261 7365 4f41 4949 7465  rator.BaseOAIIte
+0002ac60: 7261 746f 723a 0d0a 2020 2020 2020 2020  rator:..        
+0002ac70: 2222 220d 0a20 2020 2020 2020 2023 2320  """..        ## 
+0002ac80: 5061 7261 6d65 7465 7273 0d0a 0d0a 2020  Parameters....  
+0002ac90: 2020 2020 2020 6073 6574 600d 0a20 2020        `set`..   
+0002aca0: 2020 2020 2054 6869 7320 7061 7261 6d65       This parame
+0002acb0: 7465 7220 7370 6563 6966 6965 7320 7468  ter specifies th
+0002acc0: 6520 7365 7453 7065 6320 7661 6c75 6520  e setSpec value 
+0002acd0: 616e 6420 6c69 6d69 7473 2074 6865 2072  and limits the r
+0002ace0: 6563 6f72 6473 2074 6861 7420 6172 6520  ecords that are 
+0002acf0: 7265 7472 6965 7665 6420 746f 206f 6e6c  retrieved to onl
+0002ad00: 7920 7468 6f73 6520 696e 2074 6865 2073  y those in the s
+0002ad10: 7065 6369 6669 6564 2073 6574 2e0d 0a20  pecified set... 
+0002ad20: 2020 2020 2020 2049 676e 6f72 6520 7468         Ignore th
+0002ad30: 6973 2070 6172 616d 6574 6572 2074 6f20  is parameter to 
+0002ad40: 7265 7475 726e 2061 6c6c 2072 6563 6f72  return all recor
+0002ad50: 6473 2e0d 0a0d 0a20 2020 2020 2020 2023  ds.....        #
+0002ad60: 2320 4465 7363 7269 7074 696f 6e0d 0a20  # Description.. 
+0002ad70: 2020 2020 2020 2068 7474 7073 3a2f 2f72         https://r
+0002ad80: 6573 6561 7263 682e 7374 6c6f 7569 7366  esearch.stlouisf
+0002ad90: 6564 2e6f 7267 2f64 6f63 732f 6170 692f  ed.org/docs/api/
+0002ada0: 6672 6173 6572 2f6c 6973 7452 6563 6f72  fraser/listRecor
+0002adb0: 6473 2e68 746d 6c0d 0a0d 0a20 2020 2020  ds.html....     
+0002adc0: 2020 2054 6869 7320 7265 7175 6573 7420     This request 
+0002add0: 7265 7475 726e 7320 7469 746c 6520 7265  returns title re
+0002ade0: 636f 7264 7320 6672 6f6d 2074 6865 2046  cords from the F
+0002adf0: 5241 5345 5220 7265 706f 7369 746f 7279  RASER repository
+0002ae00: 2e0d 0a20 2020 2020 2020 2041 2072 6573  ...        A res
+0002ae10: 756d 7074 696f 6e54 6f6b 656e 2063 616e  umptionToken can
+0002ae20: 2062 6520 7573 6564 2074 6f20 7265 7472   be used to retr
+0002ae30: 6965 7665 2061 6c6c 2072 6563 6f72 6473  ieve all records
+0002ae40: 2075 7369 6e67 206d 756c 7469 706c 6520   using multiple 
+0002ae50: 7265 7175 6573 7473 2e0d 0a0d 0a20 2020  requests.....   
+0002ae60: 2020 2020 2041 6464 6974 696f 6e61 6c20       Additional 
+0002ae70: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+0002ae80: 7420 616e 2069 6e64 6976 6964 7561 6c20  t an individual 
+0002ae90: 7469 746c 652c 2069 6e63 6c75 6469 6e67  title, including
+0002aea0: 2074 6865 2074 6974 6c65 2773 2063 6869   the title's chi
+0002aeb0: 6c64 2072 6563 6f72 6473 2c20 6361 6e20  ld records, can 
+0002aec0: 6265 2072 6574 7269 6576 6564 2075 7369  be retrieved usi
+0002aed0: 6e67 2074 6865 2047 6574 5265 636f 7264  ng the GetRecord
+0002aee0: 2072 6571 7565 7374 2e0d 0a0d 0a20 2020   request.....   
+0002aef0: 2020 2020 2023 2320 4150 4920 5265 7175       ## API Requ
+0002af00: 6573 7420 2848 5454 5053 2047 4554 290d  est (HTTPS GET).
+0002af10: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
+0002af20: 2f66 7261 7365 722e 7374 6c6f 7569 7366  /fraser.stlouisf
+0002af30: 6564 2e6f 7267 2f6f 6169 2f3f 7665 7262  ed.org/oai/?verb
+0002af40: 3d4c 6973 7452 6563 6f72 6473 266d 6574  =ListRecords&met
+0002af50: 6164 6174 6150 7265 6669 783d 6d6f 6473  adataPrefix=mods
+0002af60: 2672 6573 756d 7074 696f 6e54 6f6b 656e  &resumptionToken
+0002af70: 3d31 3436 3932 3939 3539 383a 300d 0a0d  =1469299598:0...
+0002af80: 0a20 2020 2020 2020 2023 2320 5265 7475  .        ## Retu
+0002af90: 726e 730d 0a20 2020 2020 2020 2060 7369  rns..        `si
+0002afa0: 636b 6c65 2e69 7465 7261 746f 722e 4261  ckle.iterator.Ba
+0002afb0: 7365 4f41 4949 7465 7261 746f 7260 0d0a  seOAIIterator`..
+0002afc0: 0d0a 2020 2020 2020 2020 2323 2045 7861  ..        ## Exa
+0002afd0: 6d70 6c65 2028 6070 616e 6461 732e 4461  mple (`pandas.Da
+0002afe0: 7461 4672 616d 6560 290d 0a20 2020 2020  taFrame`)..     
+0002aff0: 2020 2060 6060 7079 7468 6f6e 0d0a 2020     ```python..  
+0002b000: 2020 2020 2020 2020 2020 6672 6f6d 2070            from p
+0002b010: 7973 746c 6f75 6973 6665 6420 696d 706f  ystlouisfed impo
+0002b020: 7274 2046 5241 5345 520d 0a0d 0a20 2020  rt FRASER....   
+0002b030: 2020 2020 2020 2020 2066 6f72 2072 6563           for rec
+0002b040: 6f72 6420 696e 2046 5241 5345 5228 292e  ord in FRASER().
+0002b050: 6c69 7374 5f72 6563 6f72 6473 2829 3a0d  list_records():.
+0002b060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b070: 2070 7269 6e74 2872 6563 6f72 642e 6765   print(record.ge
+0002b080: 745f 6d65 7461 6461 7461 2829 290d 0a20  t_metadata()).. 
+0002b090: 2020 2020 2020 2060 6060 0d0a 2020 2020         ```..    
+0002b0a0: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
+0002b0b0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0002b0c0: 7369 636b 6c65 2e4c 6973 7452 6563 6f72  sickle.ListRecor
+0002b0d0: 6473 286d 6574 6164 6174 6150 7265 6669  ds(metadataPrefi
+0002b0e0: 783d 276d 6f64 7327 2c20 6967 6e6f 7265  x='mods', ignore
+0002b0f0: 5f64 656c 6574 6564 3d69 676e 6f72 655f  _deleted=ignore_
+0002b100: 6465 6c65 7465 642c 2073 6574 3d73 6574  deleted, set=set
+0002b110: 290d 0a0d 0a20 2020 2064 6566 206c 6973  )....    def lis
+0002b120: 745f 7365 7473 2873 656c 6629 202d 3e20  t_sets(self) -> 
+0002b130: 7369 636b 6c65 2e69 7465 7261 746f 722e  sickle.iterator.
+0002b140: 4261 7365 4f41 4949 7465 7261 746f 723a  BaseOAIIterator:
+0002b150: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0002b160: 2020 2020 2020 2023 2320 4465 7363 7269         ## Descri
+0002b170: 7074 696f 6e0d 0a20 2020 2020 2020 2068  ption..        h
+0002b180: 7474 7073 3a2f 2f72 6573 6561 7263 682e  ttps://research.
+0002b190: 7374 6c6f 7569 7366 6564 2e6f 7267 2f64  stlouisfed.org/d
+0002b1a0: 6f63 732f 6170 692f 6672 6173 6572 2f6c  ocs/api/fraser/l
+0002b1b0: 6973 7453 6574 732e 6874 6d6c 0d0a 0d0a  istSets.html....
+0002b1c0: 2020 2020 2020 2020 5468 6973 2072 6571          This req
+0002b1d0: 7565 7374 2072 6574 7572 6e73 2074 6865  uest returns the
+0002b1e0: 2073 6574 2073 7472 7563 7475 7265 2066   set structure f
+0002b1f0: 6f72 2072 6563 6f72 6473 2069 6e20 7468  or records in th
+0002b200: 6520 4652 4153 4552 2072 6570 6f73 6974  e FRASER reposit
+0002b210: 6f72 792e 0d0a 2020 2020 2020 2020 4120  ory...        A 
+0002b220: 7265 7375 6d70 7469 6f6e 546f 6b65 6e20  resumptionToken 
+0002b230: 6361 6e20 6265 2075 7365 6420 746f 2072  can be used to r
+0002b240: 6574 7269 6576 6520 7468 6520 636f 6d70  etrieve the comp
+0002b250: 6c65 7465 2073 6574 2073 7472 7563 7475  lete set structu
+0002b260: 7265 2075 7369 6e67 206d 756c 7469 706c  re using multipl
+0002b270: 6520 7265 7175 6573 7473 2e0d 0a0d 0a20  e requests..... 
+0002b280: 2020 2020 2020 2023 2320 4150 4920 5265         ## API Re
+0002b290: 7175 6573 7420 2848 5454 5053 2047 4554  quest (HTTPS GET
+0002b2a0: 290d 0a20 2020 2020 2020 2068 7474 7073  )..        https
+0002b2b0: 3a2f 2f66 7261 7365 722e 7374 6c6f 7569  ://fraser.stloui
+0002b2c0: 7366 6564 2e6f 7267 2f6f 6169 2f3f 7665  sfed.org/oai/?ve
+0002b2d0: 7262 3d4c 6973 7453 6574 7326 7265 7375  rb=ListSets&resu
+0002b2e0: 6d70 7469 6f6e 546f 6b65 6e3d 3134 3738  mptionToken=1478
+0002b2f0: 3730 3736 3338 3a30 0d0a 0d0a 2020 2020  707638:0....    
+0002b300: 2020 2020 2323 2052 6574 7572 6e73 0d0a      ## Returns..
+0002b310: 2020 2020 2020 2020 6073 6963 6b6c 652e          `sickle.
+0002b320: 6974 6572 6174 6f72 2e42 6173 654f 4149  iterator.BaseOAI
+0002b330: 4974 6572 6174 6f72 600d 0a0d 0a20 2020  Iterator`....   
+0002b340: 2020 2020 2023 2320 4578 616d 706c 6520       ## Example 
+0002b350: 2860 7061 6e64 6173 2e44 6174 6146 7261  (`pandas.DataFra
+0002b360: 6d65 6029 0d0a 2020 2020 2020 2020 6060  me`)..        ``
+0002b370: 6070 7974 686f 6e0d 0a20 2020 2020 2020  `python..       
+0002b380: 2020 2020 2066 726f 6d20 7079 7374 6c6f       from pystlo
+0002b390: 7569 7366 6564 2069 6d70 6f72 7420 4652  uisfed import FR
+0002b3a0: 4153 4552 0d0a 0d0a 2020 2020 2020 2020  ASER....        
+0002b3b0: 2020 2020 666f 7220 7365 7420 696e 2046      for set in F
+0002b3c0: 5241 5345 5228 292e 6c69 7374 5f73 6574  RASER().list_set
+0002b3d0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+0002b3e0: 2020 2020 2020 7072 696e 7428 7365 7429        print(set)
+0002b3f0: 0d0a 2020 2020 2020 2020 6060 600d 0a20  ..        ```.. 
+0002b400: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
+0002b410: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0002b420: 662e 5f73 6963 6b6c 652e 4c69 7374 5365  f._sickle.ListSe
+0002b430: 7473 2829 0d0a 0d0a 2020 2020 6465 6620  ts()....    def 
+0002b440: 6c69 7374 5f69 6465 6e74 6966 6965 7273  list_identifiers
+0002b450: 2873 656c 662c 2069 676e 6f72 655f 6465  (self, ignore_de
+0002b460: 6c65 7465 643a 2062 6f6f 6c20 3d20 4661  leted: bool = Fa
+0002b470: 6c73 652c 2073 6574 3a20 7374 7220 3d20  lse, set: str = 
+0002b480: 4e6f 6e65 2920 2d3e 2073 6963 6b6c 652e  None) -> sickle.
+0002b490: 6974 6572 6174 6f72 2e42 6173 654f 4149  iterator.BaseOAI
+0002b4a0: 4974 6572 6174 6f72 3a0d 0a20 2020 2020  Iterator:..     
+0002b4b0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0002b4c0: 2323 2050 6172 616d 6574 6572 730d 0a0d  ## Parameters...
+0002b4d0: 0a20 2020 2020 2020 2060 7365 7460 0d0a  .        `set`..
+0002b4e0: 2020 2020 2020 2020 5468 6973 2070 6172          This par
+0002b4f0: 616d 6574 6572 2073 7065 6369 6669 6573  ameter specifies
+0002b500: 2074 6865 2073 6574 5370 6563 2076 616c   the setSpec val
+0002b510: 7565 2061 6e64 206c 696d 6974 7320 7468  ue and limits th
+0002b520: 6520 7265 636f 7264 7320 7468 6174 2061  e records that a
+0002b530: 7265 2072 6574 7269 6576 6564 2074 6f20  re retrieved to 
+0002b540: 6f6e 6c79 2074 686f 7365 2069 6e20 7468  only those in th
+0002b550: 6520 7370 6563 6966 6965 6420 7365 7420  e specified set 
+0002b560: 4967 6e6f 7265 2074 6869 7320 7061 7261  Ignore this para
+0002b570: 6d65 7465 7220 746f 2072 6574 7572 6e20  meter to return 
+0002b580: 616c 6c20 7265 636f 7264 732e 0d0a 0d0a  all records.....
+0002b590: 2020 2020 2020 2020 2323 2044 6573 6372          ## Descr
+0002b5a0: 6970 7469 6f6e 0d0a 2020 2020 2020 2020  iption..        
+0002b5b0: 6874 7470 733a 2f2f 7265 7365 6172 6368  https://research
+0002b5c0: 2e73 746c 6f75 6973 6665 642e 6f72 672f  .stlouisfed.org/
+0002b5d0: 646f 6373 2f61 7069 2f66 7261 7365 722f  docs/api/fraser/
+0002b5e0: 6c69 7374 4964 656e 7469 6669 6572 732e  listIdentifiers.
+0002b5f0: 6874 6d6c 0d0a 0d0a 2020 2020 2020 2020  html....        
+0002b600: 5468 6973 2072 6571 7565 7374 2072 6574  This request ret
+0002b610: 7572 6e73 2068 6561 6465 7273 2066 6f72  urns headers for
+0002b620: 2072 6563 6f72 6473 2069 6e20 7468 6520   records in the 
+0002b630: 4652 4153 4552 2072 6570 6f73 6974 6f72  FRASER repositor
+0002b640: 792e 0d0a 2020 2020 2020 2020 4120 7265  y...        A re
+0002b650: 7375 6d70 7469 6f6e 546f 6b65 6e20 6361  sumptionToken ca
+0002b660: 6e20 6265 2075 7365 6420 746f 2072 6574  n be used to ret
+0002b670: 7269 6576 6520 616c 6c20 7265 636f 7264  rieve all record
+0002b680: 7320 7573 696e 6720 6d75 6c74 6970 6c65  s using multiple
+0002b690: 2072 6571 7565 7374 732e 0d0a 0d0a 2020   requests.....  
+0002b6a0: 2020 2020 2020 2323 2041 5049 2052 6571        ## API Req
+0002b6b0: 7565 7374 2028 4854 5450 5320 4745 5429  uest (HTTPS GET)
+0002b6c0: 0d0a 2020 2020 2020 2020 6874 7470 733a  ..        https:
+0002b6d0: 2f2f 6672 6173 6572 2e73 746c 6f75 6973  //fraser.stlouis
+0002b6e0: 6665 642e 6f72 672f 6f61 692f 3f76 6572  fed.org/oai/?ver
+0002b6f0: 623d 4c69 7374 4964 656e 7469 6669 6572  b=ListIdentifier
+0002b700: 7326 7265 7375 6d70 7469 6f6e 546f 6b65  s&resumptionToke
+0002b710: 6e3d 3134 3639 3330 3034 3531 3a30 0d0a  n=1469300451:0..
+0002b720: 0d0a 2020 2020 2020 2020 2323 2052 6574  ..        ## Ret
+0002b730: 7572 6e73 0d0a 2020 2020 2020 2020 6073  urns..        `s
+0002b740: 6963 6b6c 652e 6974 6572 6174 6f72 2e42  ickle.iterator.B
+0002b750: 6173 654f 4149 4974 6572 6174 6f72 600d  aseOAIIterator`.
+0002b760: 0a0d 0a20 2020 2020 2020 2023 2320 4578  ...        ## Ex
+0002b770: 616d 706c 6520 2860 7061 6e64 6173 2e44  ample (`pandas.D
+0002b780: 6174 6146 7261 6d65 6029 0d0a 2020 2020  ataFrame`)..    
+0002b790: 2020 2020 6060 6070 7974 686f 6e0d 0a20      ```python.. 
+0002b7a0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
+0002b7b0: 7079 7374 6c6f 7569 7366 6564 2069 6d70  pystlouisfed imp
+0002b7c0: 6f72 7420 4652 4153 4552 0d0a 0d0a 2020  ort FRASER....  
+0002b7d0: 2020 2020 2020 2020 2020 666f 7220 6865            for he
+0002b7e0: 6164 6572 2069 6e20 4652 4153 4552 2829  ader in FRASER()
+0002b7f0: 2e6c 6973 745f 6964 656e 7469 6669 6572  .list_identifier
+0002b800: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+0002b810: 2020 2020 2020 7072 696e 7428 6865 6164        print(head
+0002b820: 6572 2e69 6465 6e74 6966 6965 7229 0d0a  er.identifier)..
+0002b830: 2020 2020 2020 2020 6060 600d 0a20 2020          ```..   
+0002b840: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
+0002b850: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0002b860: 5f73 6963 6b6c 652e 4c69 7374 4964 656e  _sickle.ListIden
+0002b870: 7469 6669 6572 7328 6d65 7461 6461 7461  tifiers(metadata
+0002b880: 5072 6566 6978 3d27 6d6f 6473 272c 2069  Prefix='mods', i
+0002b890: 676e 6f72 655f 6465 6c65 7465 643d 6967  gnore_deleted=ig
+0002b8a0: 6e6f 7265 5f64 656c 6574 6564 2c20 7365  nore_deleted, se
+0002b8b0: 743d 7365 7429 0d0a 0d0a 2020 2020 6465  t=set)....    de
+0002b8c0: 6620 6765 745f 7265 636f 7264 2873 656c  f get_record(sel
+0002b8d0: 662c 2069 6465 6e74 6966 6965 723a 2073  f, identifier: s
+0002b8e0: 7472 2920 2d3e 2073 6963 6b6c 652e 6d6f  tr) -> sickle.mo
+0002b8f0: 6465 6c73 2e52 6563 6f72 643a 0d0a 2020  dels.Record:..  
+0002b900: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0002b910: 2020 2023 2320 4465 7363 7269 7074 696f     ## Descriptio
+0002b920: 6e0d 0a20 2020 2020 2020 2068 7474 7073  n..        https
+0002b930: 3a2f 2f72 6573 6561 7263 682e 7374 6c6f  ://research.stlo
+0002b940: 7569 7366 6564 2e6f 7267 2f64 6f63 732f  uisfed.org/docs/
+0002b950: 6170 692f 6672 6173 6572 2f67 6574 5265  api/fraser/getRe
+0002b960: 636f 7264 2e68 746d 6c0d 0a0d 0a20 2020  cord.html....   
+0002b970: 2020 2020 2054 6869 7320 7265 7175 6573       This reques
+0002b980: 7420 7265 7475 726e 7320 6120 7369 6e67  t returns a sing
+0002b990: 6c65 2072 6563 6f72 6420 6672 6f6d 2074  le record from t
+0002b9a0: 6865 2046 5241 5345 5220 7265 706f 7369  he FRASER reposi
+0002b9b0: 746f 7279 2e0d 0a0d 0a20 2020 2020 2020  tory.....       
+0002b9c0: 2023 2320 4150 4920 5265 7175 6573 7420   ## API Request 
+0002b9d0: 2848 5454 5053 2047 4554 290d 0a20 2020  (HTTPS GET)..   
+0002b9e0: 2020 2020 2068 7474 7073 3a2f 2f66 7261       https://fra
+0002b9f0: 7365 722e 7374 6c6f 7569 7366 6564 2e6f  ser.stlouisfed.o
+0002ba00: 7267 2f6f 6169 2f3f 7665 7262 3d47 6574  rg/oai/?verb=Get
+0002ba10: 5265 636f 7264 2669 6465 6e74 6966 6965  Record&identifie
+0002ba20: 723d 6f61 693a 6672 6173 6572 2e73 746c  r=oai:fraser.stl
+0002ba30: 6f75 6973 6665 642e 6f72 673a 7469 746c  ouisfed.org:titl
+0002ba40: 653a 3137 360d 0a0d 0a20 2020 2020 2020  e:176....       
+0002ba50: 2023 2320 5265 7475 726e 730d 0a20 2020   ## Returns..   
+0002ba60: 2020 2020 2060 7369 636b 6c65 2e6d 6f64       `sickle.mod
+0002ba70: 656c 732e 5265 636f 7264 600d 0a0d 0a20  els.Record`.... 
+0002ba80: 2020 2020 2020 2023 2320 4578 616d 706c         ## Exampl
+0002ba90: 6520 2860 7061 6e64 6173 2e44 6174 6146  e (`pandas.DataF
+0002baa0: 7261 6d65 6029 0d0a 2020 2020 2020 2020  rame`)..        
+0002bab0: 6060 6070 7974 686f 6e0d 0a20 2020 2020  ```python..     
+0002bac0: 2020 2020 2020 2066 726f 6d20 7079 7374         from pyst
+0002bad0: 6c6f 7569 7366 6564 2069 6d70 6f72 7420  louisfed import 
+0002bae0: 4652 4153 4552 0d0a 0d0a 2020 2020 2020  FRASER....      
+0002baf0: 2020 2020 2020 4652 4153 4552 2829 2e67        FRASER().g
+0002bb00: 6574 5f72 6563 6f72 6428 6964 656e 7469  et_record(identi
+0002bb10: 6669 6572 3d27 6f61 693a 6672 6173 6572  fier='oai:fraser
+0002bb20: 2e73 746c 6f75 6973 6665 642e 6f72 673a  .stlouisfed.org:
+0002bb30: 7469 746c 653a 3137 3627 290d 0a20 2020  title:176')..   
+0002bb40: 2020 2020 2060 6060 0d0a 2020 2020 2020       ```..      
+0002bb50: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+0002bb60: 2072 6574 7572 6e20 7365 6c66 2e5f 7369   return self._si
+0002bb70: 636b 6c65 2e47 6574 5265 636f 7264 2869  ckle.GetRecord(i
+0002bb80: 6465 6e74 6966 6965 723d 6964 656e 7469  dentifier=identi
+0002bb90: 6669 6572 2c20 6d65 7461 6461 7461 5072  fier, metadataPr
+0002bba0: 6566 6978 3d27 6d6f 6473 2729 0d0a       efix='mods')..
```

### Comparing `pystlouisfed-2.1.0/pystlouisfed/enums.py` & `pystlouisfed-2.1.1/pystlouisfed/enums.py`

 * *Files identical despite different names*

### Comparing `pystlouisfed-2.1.0/pystlouisfed/models.py` & `pystlouisfed-2.1.1/pystlouisfed/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from dataclasses import dataclass
 from datetime import date, datetime
 
 from shapely import geos
 from shapely.geometry import Point, MultiPolygon
 
+from typing import Optional
+
 
 @dataclass
 class Category:
     id: int
     name: str
     parent_id: int
 
@@ -25,15 +27,15 @@
     units: str
     units_short: str
     seasonal_adjustment: str
     seasonal_adjustment_short: str
     last_updated: datetime
     popularity: int
     # group_popularity: int
-    notes: str
+    notes: Optional[str] = None
 
     def __post_init__(self):
         self.realtime_start = datetime.strptime(self.realtime_start, "%Y-%m-%d").date()
         self.realtime_end = datetime.strptime(self.realtime_end, "%Y-%m-%d").date()
         self.observation_start = datetime.strptime(self.observation_start, "%Y-%m-%d").date()
         self.observation_end = datetime.strptime(self.observation_end, "%Y-%m-%d").date()
         self.last_updated = datetime.strptime(self.last_updated + '00', '%Y-%m-%d %H:%M:%S%z')
```

### Comparing `pystlouisfed-2.1.0/pystlouisfed.egg-info/PKG-INFO` & `pystlouisfed-2.1.1/pystlouisfed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystlouisfed
-Version: 2.1.0
+Version: 2.1.1
 Summary: Federal Reserve Bank of St. Louis - FRED, ALFRED, GeoFRED and FRASER
 Home-page: https://github.com/TomasKoutek/pystlouisfed
 Download-URL: https://github.com/TomasKoutek/pystlouisfed.git
 Author: Tomas Koutek
 Author-email: 66636b6f6666@gmail.com
 Maintainer: Tomas Koutek
 License: MIT
@@ -115,15 +115,15 @@
 other methods return `pandas.DataFrame`
 For example method `FRED.category_series` (all series for a specific category)
 
 ```python
 from pystlouisfed import FRED
 
 fred = FRED(api_key='abcdefghijklmnopqrstuvwxyz123456')
-df = fred.category_series(category_id=125).head()
+df = fred.category_series(category_id=125)
 
 print(df.head())
 ```
 
 ```
         realtime_start realtime_end                                              title observation_start observation_end  frequency frequency_short                units units_short      seasonal_adjustment seasonal_adjustment_short              last_updated  popularity  group_popularity                                              notes
 id                                                                                                                                                                                                                                                                                                                                                
@@ -213,28 +213,28 @@
 
 FRED (ALFRED) has many different parameters, which are not the same for each method. So there is no need to remember everything or keep looking at the documentation.
 `pystlouisfed` uses the [Enums](https://tomaskoutek.github.io/pystlouisfed/enums.html) constants. For example, the API endpoint FRED:series_observations (and
 method `FRED.series_observations`) has the optional parameters
 "units", "frequency", "aggregation_method" or "output_type":
 
 ```
-    def series_observations(
-            self,
-            series_id: str,
-            realtime_start: date = date.today(),
-            realtime_end: date = date.today(),
-            sort_order: enums.SortOrder = enums.SortOrder.asc,
-            observation_start: date = date(1776, 7, 4),
-            observation_end: date = date(9999, 12, 31),
-            units: enums.Unit = enums.Unit.lin,
-            frequency: enums.Frequency = None,
-            aggregation_method: enums.AggregationMethod = enums.AggregationMethod.average,
-            output_type: enums.OutputType = enums.OutputType.realtime_period,
-            vintage_dates: List[str] = None
-    ) -> pd.DataFram:
+def series_observations(
+        self,
+        series_id: str,
+        realtime_start: date = None,
+        realtime_end: date = None,
+        sort_order: enums.SortOrder = enums.SortOrder.asc,
+        observation_start: date = date(1776, 7, 4),
+        observation_end: date = date(9999, 12, 31),
+        units: enums.Unit = enums.Unit.lin,
+        frequency: enums.Frequency = None,
+        aggregation_method: enums.AggregationMethod = enums.AggregationMethod.average,
+        output_type: enums.OutputType = enums.OutputType.realtime_period,
+        vintage_dates: List[str] = None
+) -> pd.DataFrame:
 ```
 
 But what should be the value? For example, for the parameter "aggregation_method" it is possible to use `pystlouisfed.AggregationMethod`:
 
 ```python
 from enum import Enum
 
@@ -477,9 +477,7 @@
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 
 
-
-
```

### Comparing `pystlouisfed-2.1.0/setup.py` & `pystlouisfed-2.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from setuptools import setup
 
 setup(
     name='pystlouisfed',
-    version='2.1.0',
+    version='2.1.1',
     packages=['pystlouisfed'],
     url='https://github.com/TomasKoutek/pystlouisfed',
     license='MIT',
     author='Tomas Koutek',
     author_email='66636b6f6666@gmail.com',
     maintainer="Tomas Koutek",
     # maintainer_email="",
```

