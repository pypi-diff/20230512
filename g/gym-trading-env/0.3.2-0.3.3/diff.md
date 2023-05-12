# Comparing `tmp/gym-trading-env-0.3.2.tar.gz` & `tmp/gym-trading-env-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.3.2.tar", last modified: Tue May  9 07:51:33 2023, max compression
+gzip compressed data, was "gym-trading-env-0.3.3.tar", last modified: Fri May 12 16:42:55 2023, max compression
```

## Comparing `gym-trading-env-0.3.2.tar` & `gym-trading-env-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 07:51:33.589528 gym-trading-env-0.3.2/
--rw-rw-rw-   0        0        0     1088 2023-03-29 17:01:42.000000 gym-trading-env-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0       44 2023-05-06 13:10:40.000000 gym-trading-env-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4428 2023-05-09 07:51:33.587548 gym-trading-env-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2566 2023-05-06 13:10:40.000000 gym-trading-env-0.3.2/README.md
--rw-rw-rw-   0        0        0      853 2023-05-09 07:49:59.000000 gym-trading-env-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 07:51:33.590529 gym-trading-env-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 07:51:33.461530 gym-trading-env-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 07:51:33.499529 gym-trading-env-0.3.2/src/gym_trading_env/
--rw-rw-rw-   0        0        0      333 2023-04-13 13:15:17.000000 gym-trading-env-0.3.2/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     4164 2023-04-13 12:39:12.000000 gym-trading-env-0.3.2/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0    16685 2023-05-09 07:48:52.000000 gym-trading-env-0.3.2/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2504 2023-05-06 13:10:40.000000 gym-trading-env-0.3.2/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:51:33.574526 gym-trading-env-0.3.2/src/gym_trading_env/templates/
--rw-rw-rw-   0        0        0     3878 2023-05-06 13:10:40.000000 gym-trading-env-0.3.2/src/gym_trading_env/templates/index.html
-drwxrwxrwx   0        0        0        0 2023-05-09 07:51:33.584530 gym-trading-env-0.3.2/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:13:00.000000 gym-trading-env-0.3.2/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-10 08:13:00.000000 gym-trading-env-0.3.2/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-13 09:31:51.000000 gym-trading-env-0.3.2/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-10 08:13:00.000000 gym-trading-env-0.3.2/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:51:33.540532 gym-trading-env-0.3.2/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0     4428 2023-05-09 07:51:33.000000 gym-trading-env-0.3.2/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-05-09 07:51:33.000000 gym-trading-env-0.3.2/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 07:51:33.000000 gym-trading-env-0.3.2/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-09 07:51:33.000000 gym-trading-env-0.3.2/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 07:51:33.000000 gym-trading-env-0.3.2/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 16:42:55.833612 gym-trading-env-0.3.3/
+-rw-rw-rw-   0        0        0     1088 2023-03-29 17:01:42.000000 gym-trading-env-0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       44 2023-05-06 13:10:40.000000 gym-trading-env-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4428 2023-05-12 16:42:55.832610 gym-trading-env-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2566 2023-05-06 13:10:40.000000 gym-trading-env-0.3.3/README.md
+-rw-rw-rw-   0        0        0      853 2023-05-12 16:42:30.000000 gym-trading-env-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 16:42:55.834611 gym-trading-env-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 16:42:55.739967 gym-trading-env-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 16:42:55.771114 gym-trading-env-0.3.3/src/gym_trading_env/
+-rw-rw-rw-   0        0        0      333 2023-04-13 13:15:17.000000 gym-trading-env-0.3.3/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-04-13 12:39:12.000000 gym-trading-env-0.3.3/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0    17466 2023-05-12 16:26:50.000000 gym-trading-env-0.3.3/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2504 2023-05-06 13:10:40.000000 gym-trading-env-0.3.3/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:42:55.815820 gym-trading-env-0.3.3/src/gym_trading_env/templates/
+-rw-rw-rw-   0        0        0     3878 2023-05-06 13:10:40.000000 gym-trading-env-0.3.3/src/gym_trading_env/templates/index.html
+drwxrwxrwx   0        0        0        0 2023-05-12 16:42:55.829613 gym-trading-env-0.3.3/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:13:00.000000 gym-trading-env-0.3.3/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-10 08:13:00.000000 gym-trading-env-0.3.3/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3369 2023-05-12 16:07:55.000000 gym-trading-env-0.3.3/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3158 2023-05-12 16:07:55.000000 gym-trading-env-0.3.3/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:42:55.811818 gym-trading-env-0.3.3/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0     4428 2023-05-12 16:42:55.000000 gym-trading-env-0.3.3/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-05-12 16:42:55.000000 gym-trading-env-0.3.3/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 16:42:55.000000 gym-trading-env-0.3.3/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-12 16:42:55.000000 gym-trading-env-0.3.3/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-12 16:42:55.000000 gym-trading-env-0.3.3/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.3.2/LICENSE.txt` & `gym-trading-env-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.2/PKG-INFO` & `gym-trading-env-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.2 Summary: A simple,
+Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.3 Summary: A simple,
 easy, customizable Open IA Gym environments for trading. Author-email: Clement
 Perroud
 perroud.pro@gmail.com> License: MIT License Copyright (c) [year] [fullname]
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `gym-trading-env-0.3.2/README.md` & `gym-trading-env-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.2/pyproject.toml` & `gym-trading-env-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.3.2"
+version = "0.3.3"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gym-trading-env-0.3.2/src/gym_trading_env/downloader.py` & `gym-trading-env-0.3.3/src/gym_trading_env/downloader.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.2/src/gym_trading_env/environments.py` & `gym-trading-env-0.3.3/src/gym_trading_env/environments.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,24 @@
 from collections import Counter
 from .utils.history import History
 from .utils.portfolio import Portfolio, TargetPortfolio
 
 import tempfile, os
 import warnings
 warnings.filterwarnings("error")
+
 def basic_reward_function(history : History):
     return np.log(history["portfolio_valuation", -1] / history["portfolio_valuation", -2])
 
+def dynamic_feature_last_position_taken(history):
+    return history['position', -1]
+
+def dynamic_feature_real_position(history):
+    return history['real_position', -1]
+
 class TradingEnv(gym.Env):
     """
     An easy trading environment for OpenAI gym. It is recommended to use it this way :
 
     .. code-block:: python
 
         import gymnasium as gym
@@ -29,14 +36,21 @@
 
     :param df: The market DataFrame. It must contain 'open', 'high', 'low', 'close'. Index must be DatetimeIndex. Your desired inputs need to contain 'feature' in their column name : this way, they will be returned as observation at each step.
     :type df: pandas.DataFrame
 
     :param positions: List of the positions allowed by the environment.
     :type positions: optional - list[int or float]
 
+    :param dynamic_feature_functions: The list of the dynamic features functions. By default, two dynamic features are added :
+    
+        * the last position taken by the agent.
+        * the real position of the portfolio (that varies according to the price fluctuations)
+
+    :type dynamic_feature_functions: optional - list   
+
     :param reward_function: Take the History object of the environment and must return a float.
     :type reward_function: optional - function<History->float>
 
     :param windows: Default is None. If it is set to an int: N, every step observation will return the past N observations. It is recommended for Recurrent Neural Network based Agents.
     :type windows: optional - None or int
 
     :param trading_fees: Transaction trading fees (buy and sell operations). eg: 0.01 corresponds to 1% fees
@@ -47,16 +61,16 @@
 
     :param portfolio_initial_value: Initial valuation of the portfolio.
     :type portfolio_initial_value: float or int
 
     :param initial_position: You can specify the initial position of the environment or set it to 'random'. It must contained in the list parameter 'positions'.
     :type initial_position: optional - float or int
 
-    :param include_position_in_features: Whether or not you want the current position to be added to the step observations. If windows is set an int, it will add the last N-step positions.
-    :type include_position_in_features: optional - bool
+    :param max_episode_duration: If a integer value is used, each episode will be truncated after reaching the desired max duration in steps (by returning `truncated` as `True`). When using a max duration, each episode will start at a random starting point.
+    :type max_episode_duration: optional - int or 'max'
 
     :param max_episode_duration: If a integer value is used, each episode will be truncated after reaching the desired max duration in steps (by returning `truncated` as `True`). When using a max duration, each episode will start at a random starting point.
     :type max_episode_duration: optional - int or 'max'
 
     :param verbose: If 0, no log is outputted. If 1, the env send episode result logs.
     :type verbose: optional - int
     
@@ -64,40 +78,41 @@
     :type name: optional - str
     
     """
     metadata = {'render_modes': ['logs']}
     def __init__(self,
                 df : pd.DataFrame,
                 positions : list = [0, 1],
+                dynamic_feature_functions = [dynamic_feature_last_position_taken, dynamic_feature_real_position],
                 reward_function = basic_reward_function,
                 windows = None,
                 trading_fees = 0,
                 borrow_interest_rate = 0,
                 portfolio_initial_value = 1000,
                 initial_position ='random',
-                include_position_in_features = True,
                 max_episode_duration = 'max',
                 verbose = 1,
                 name = "Stock",
                 render_mode= "logs"
                 ):
         self.max_episode_duration = max_episode_duration
         self.name = name
         self.verbose = verbose
 
         self.positions = positions
+        self.dynamic_feature_functions = dynamic_feature_functions
         self.reward_function = reward_function
         self.windows = windows
         self.trading_fees = trading_fees
         self.borrow_interest_rate = borrow_interest_rate
         self.portfolio_initial_value = float(portfolio_initial_value)
         self.initial_position = initial_position
         assert self.initial_position in self.positions or self.initial_position == 'random', "The 'initial_position' parameter must be 'random' or a position mentionned in the 'position' (default is [0, 1]) parameter."
-        self.include_position_in_features = include_position_in_features
         assert render_mode is None or render_mode in self.metadata["render_modes"]
+        self.max_episode_duration = max_episode_duration
         self.render_mode = render_mode
         self._set_df(df)
         
         self.action_space = spaces.Discrete(len(positions))
         self.observation_space = spaces.Box(
             -np.inf,
             np.inf,
@@ -114,67 +129,75 @@
 
 
     def _set_df(self, df):
         df = df.copy()
         self._features_columns = [col for col in df.columns if "feature" in col]
         self._info_columns = list(set(list(df.columns) + ["close"]) - set(self._features_columns))
         self._nb_features = len(self._features_columns)
-    
+        self._nb_static_features = self._nb_features
 
-        if self.include_position_in_features:
-            df["feature_position"] = 0
-            self._features_columns.append("feature_position")
+        for i  in range(len(self.dynamic_feature_functions)):
+            df[f"dynamic_feature__{i}"] = 0
+            self._features_columns.append(f"dynamic_feature__{i}")
             self._nb_features += 1
+
         self.df = df
         self._obs_array = np.array(self.df[self._features_columns], dtype= np.float32)
         self._info_array = np.array(self.df[self._info_columns])
         self._price_array = np.array(self.df["close"])
 
 
     
     def _get_ticker(self, delta = 0):
-        return self.df.iloc[self._step + self._starting_idx + delta]
+        return self.df.iloc[self._idx + delta]
     def _get_price(self, delta = 0):
-        return self._price_array[self._step + self._starting_idx + delta]
+        return self._price_array[self._idx + delta]
     
     def _get_obs(self):
-        if self.include_position_in_features: self._obs_array[self._step + self._starting_idx, -1] = self._position
+        for i, dynamic_feature_function in enumerate(self.dynamic_feature_functions):
+            self._obs_array[self._idx, self._nb_static_features + i] = dynamic_feature_function(self.historical_info)
+
         if self.windows is None:
-            _step_index = self._step + self._starting_idx
+            _step_index = self._idx
         else: 
-            _step_index = np.arange(self._step + self._starting_idx + 1 - self.windows , self._step + self._starting_idx + 1)
+            _step_index = np.arange(self._idx + 1 - self.windows , self._idx + 1)
         return self._obs_array[_step_index]
 
     
     def reset(self, seed = None, options=None):
         super().reset(seed = seed)
+        
         self._step = 0
         self._position = np.random.choice(self.positions) if self.initial_position == 'random' else self.initial_position
         self._limit_orders = {}
         
-        self._starting_idx = 0
-
-        if self.max_episode_duration != 'max' and len(self.df) - self.max_episode_duration > 0:
-            windows_adjustement = 0 if self.windows is None else self.windows - 1
-            self._starting_idx = np.random.choice(len(self.df)- self.max_episode_duration - windows_adjustement)
-        if self.windows is not None: self._starting_idx += self.windows - 1
 
+        self._idx = 0
+        if self.windows is not None: self._idx = self.windows - 1
+        if self.max_episode_duration != 'max':
+            self._idx = np.random.randint(
+                low = self._idx, 
+                high = len(self.df) - self.max_episode_duration - self._idx
+            )
+        
         self._portfolio  = TargetPortfolio(
             position = self._position,
             value = self.portfolio_initial_value,
             price = self._get_price()
         )
         
         self.historical_info = History(max_size= len(self.df))
         self.historical_info.set(
+            idx = self._idx,
             step = self._step,
-            date = self.df.index.values[self._step + self._starting_idx],
+            date = self.df.index.values[self._idx],
             position_index =self.positions.index(self._position),
             position = self._position,
-            data =  dict(zip(self._info_columns, self._info_array[self._step + self._starting_idx])),
+            real_position = self._position,
+            data =  dict(zip(self._info_columns, self._info_array[self._idx])),
             portfolio_valuation = self.portfolio_initial_value,
             portfolio_distribution = self._portfolio.get_portfolio_distribution(),
             reward = 0,
         )
 
         return self._get_obs(), self.historical_info[0]
 
@@ -208,48 +231,53 @@
         self._limit_orders[position] = {
             'limit' : limit,
             'persistent': persistent
         }
     
     def step(self, position_index = None):
         if position_index is not None: self._take_action(self.positions[position_index])
+        self._idx += 1
         self._step += 1
 
         self._take_action_order_limit()
         price = self._get_price()
         self._portfolio.update_interest(borrow_interest_rate= self.borrow_interest_rate)
         portfolio_value = self._portfolio.valorisation(price)
         portfolio_distribution = self._portfolio.get_portfolio_distribution()
 
         done, truncated = False, False
-        if portfolio_value <= 0: done = True
-        if self._step + self._starting_idx >= len(self.df) - 1:
+
+        if portfolio_value <= 0:
+            done = True
+        if self._idx >= len(self.df) - 1:
             truncated = True
         if isinstance(self.max_episode_duration,int) and self._step >= self.max_episode_duration - 1:
             truncated = True
 
         self.historical_info.add(
+            idx = self._idx,
             step = self._step,
-            date = self.df.index.values[self._step + self._starting_idx],
+            date = self.df.index.values[self._idx],
             position_index =position_index,
             position = self._position,
-            data =  dict(zip(self._info_columns, self._info_array[self._step + self._starting_idx])),
+            real_position = self._portfolio.real_position(price),
+            data =  dict(zip(self._info_columns, self._info_array[self._idx])),
             portfolio_valuation = portfolio_value,
             portfolio_distribution = portfolio_distribution, 
             reward = 0
         )
         if not done:
             reward = self.reward_function(self.historical_info)
             self.historical_info["reward", -1] = reward
 
         if done or truncated:
             self.calculate_metrics()
             self.log()
-
         return self._get_obs(),  self.historical_info["reward", -1], done, truncated, self.historical_info[-1]
+
     def add_metric(self, name, function):
         self.log_metrics.append({
             'name': name,
             'function': function
         })
     def calculate_metrics(self):
         self.results_metrics = {
@@ -263,14 +291,15 @@
         return self.results_metrics
     def log(self):
         if self.verbose > 0:
             text = ""
             for key, value in self.results_metrics.items():
                 text += f"{key} : {value}   |   "
             print(text)
+
     def save_for_render(self, dir = "render_logs"):
         assert "open" in self.df and "high" in self.df and "low" in self.df and "close" in self.df, "Your DataFrame needs to contain columns : open, high, low, close to render !"
         columns = list(set(self.historical_info.columns) - set([f"date_{col}" for col in self._info_columns]))
         history_df = pd.DataFrame(
             self.historical_info[columns], columns= columns
         )
         history_df.set_index("date", inplace= True)
@@ -331,27 +360,25 @@
                     preprocess= preprocess,
                 )
     
     :type preprocess: function<pandas.DataFrame->pandas.DataFrame>
 
     :param episodes_between_dataset_switch: Number of times a dataset is used to create an episode, before moving on to another dataset. It can be useful for performances when `max_episode_duration` is low.
     :type episodes_between_dataset_switch: optional - int
-
     """
     def __init__(self,
                 dataset_dir, 
                 *args, 
 
                 preprocess = lambda df : df,
                 episodes_between_dataset_switch = 1,
                 **kwargs):
         self.dataset_dir = dataset_dir
         self.preprocess = preprocess
         self.episodes_between_dataset_switch = episodes_between_dataset_switch
-
         self.dataset_pathes = glob.glob(self.dataset_dir)
         self.dataset_nb_uses = np.zeros(shape=(len(self.dataset_pathes), ))
         super().__init__(self.next_dataset(), *args, **kwargs)
 
     def next_dataset(self):
         self._episodes_on_this_dataset = 0
         # Find the indexes of the less explored dataset
```

### Comparing `gym-trading-env-0.3.2/src/gym_trading_env/renderer.py` & `gym-trading-env-0.3.3/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.2/src/gym_trading_env/templates/index.html` & `gym-trading-env-0.3.3/src/gym_trading_env/templates/index.html`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.2/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.3.3/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.3.2/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.3.3/src/gym_trading_env/utils/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
                 values.append(value)
 
         if columns == self.columns:
             self.history_storage[self.size, :] = values
             self.size = min(self.size+1, self.height)
         else:
             raise ValueError(f"Make sur that your inputs match the initial ones... Initial ones : {self.columns}. New ones {columns}")
+    def __len__(self):
+        return self.size
     def __getitem__(self, arg):
         if isinstance(arg, tuple):
             column, t = arg
             try:
                 column_index = self.columns.index(column)
             except ValueError as e:
                 raise ValueError(f"Feature {column} does not exist ... Check the available features : {self.columns}")
@@ -67,11 +69,8 @@
 
     def __setitem__(self, arg, value):
         column, t = arg
         try:
             column_index = self.columns.index(column)
         except ValueError as e:
             raise ValueError(f"Feature {column} does not exist ... Check the available features : {self.columns}")
-        self.history_storage[:self.size][t, column_index] = value
-
-
-        
+        self.history_storage[:self.size][t, column_index] = value
```

### Comparing `gym-trading-env-0.3.2/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.3.3/src/gym_trading_env/utils/portfolio.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     def valorisation(self, price):
         return sum([
             self.asset * price,
             self.fiat,
             - self.interest_asset * price,
             - self.interest_fiat
         ])
+    def real_position(self, price):
+        return (self.asset - self.interest_asset)* price / self.valorisation(price)
     def position(self, price):
         return self.asset * price / self.valorisation(price)
     def trade_to_position(self, position, price, trading_fees):
         # Repay interest
         current_position = self.position(price)
         interest_reduction_ratio = 1
         if (position <= 0 and current_position < 0):
```

### Comparing `gym-trading-env-0.3.2/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.3.3/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.2 Summary: A simple,
+Metadata-Version: 2.1 Name: gym-trading-env Version: 0.3.3 Summary: A simple,
 easy, customizable Open IA Gym environments for trading. Author-email: Clement
 Perroud
 perroud.pro@gmail.com> License: MIT License Copyright (c) [year] [fullname]
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `gym-trading-env-0.3.2/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.3.3/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

