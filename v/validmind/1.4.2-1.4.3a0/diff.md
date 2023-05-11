# Comparing `tmp/validmind-1.4.2-py3-none-any.whl.zip` & `tmp/validmind-1.4.3a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,30 @@
-Zip file size: 73623 bytes, number of entries: 39
+Zip file size: 75749 bytes, number of entries: 42
 -rw-r--r--  2.0 unx     1380 b- defN 80-Jan-01 00:00 validmind/__init__.py
 -rw-r--r--  2.0 unx    11353 b- defN 80-Jan-01 00:00 validmind/api_client.py
 -rw-r--r--  2.0 unx     8788 b- defN 80-Jan-01 00:00 validmind/client.py
 -rw-r--r--  2.0 unx      590 b- defN 80-Jan-01 00:00 validmind/data_validation/__init__.py
--rw-r--r--  2.0 unx    34464 b- defN 80-Jan-01 00:00 validmind/data_validation/metrics.py
--rw-r--r--  2.0 unx    23675 b- defN 80-Jan-01 00:00 validmind/data_validation/threshold_tests.py
+-rw-r--r--  2.0 unx    34444 b- defN 80-Jan-01 00:00 validmind/data_validation/metrics.py
+-rw-r--r--  2.0 unx    23919 b- defN 80-Jan-01 00:00 validmind/data_validation/threshold_tests.py
+-rw-r--r--  2.0 unx     1290 b- defN 80-Jan-01 00:00 validmind/datasets/regression/__init__.py
+-rw-r--r--  2.0 unx      187 b- defN 80-Jan-01 00:00 validmind/datasets/regression/fred.py
+-rw-r--r--  2.0 unx      195 b- defN 80-Jan-01 00:00 validmind/datasets/regression/lending_club.py
 -rw-r--r--  2.0 unx    10529 b- defN 80-Jan-01 00:00 validmind/model_utils.py
 -rw-r--r--  2.0 unx     1290 b- defN 80-Jan-01 00:00 validmind/model_validation/__init__.py
 -rw-r--r--  2.0 unx     4927 b- defN 80-Jan-01 00:00 validmind/model_validation/model_metadata.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 validmind/model_validation/sklearn/__init__.py
 -rw-r--r--  2.0 unx    12925 b- defN 80-Jan-01 00:00 validmind/model_validation/sklearn/metrics.py
 -rw-r--r--  2.0 unx    30637 b- defN 80-Jan-01 00:00 validmind/model_validation/sklearn/threshold_tests.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 validmind/model_validation/statsmodels/__init__.py
--rw-r--r--  2.0 unx    22475 b- defN 80-Jan-01 00:00 validmind/model_validation/statsmodels/metrics.py
+-rw-r--r--  2.0 unx    25419 b- defN 80-Jan-01 00:00 validmind/model_validation/statsmodels/metrics.py
 -rw-r--r--  2.0 unx     1317 b- defN 80-Jan-01 00:00 validmind/model_validation/statsmodels/threshold_tests.py
 -rw-r--r--  2.0 unx     1657 b- defN 80-Jan-01 00:00 validmind/model_validation/utils.py
--rw-r--r--  2.0 unx     5292 b- defN 80-Jan-01 00:00 validmind/test_plans/__init__.py
+-rw-r--r--  2.0 unx     5388 b- defN 80-Jan-01 00:00 validmind/test_plans/__init__.py
 -rw-r--r--  2.0 unx     2431 b- defN 80-Jan-01 00:00 validmind/test_plans/sklearn_classifier.py
--rw-r--r--  2.0 unx     2464 b- defN 80-Jan-01 00:00 validmind/test_plans/statsmodels_timeseries.py
+-rw-r--r--  2.0 unx     2751 b- defN 80-Jan-01 00:00 validmind/test_plans/statsmodels_timeseries.py
 -rw-r--r--  2.0 unx     2068 b- defN 80-Jan-01 00:00 validmind/test_plans/tabular_datasets.py
 -rw-r--r--  2.0 unx     6814 b- defN 80-Jan-01 00:00 validmind/test_plans/time_series.py
 -rw-r--r--  2.0 unx     6647 b- defN 80-Jan-01 00:00 validmind/utils.py
 -rw-r--r--  2.0 unx     1065 b- defN 80-Jan-01 00:00 validmind/vm_models/__init__.py
 -rw-r--r--  2.0 unx    10156 b- defN 80-Jan-01 00:00 validmind/vm_models/dataset.py
 -rw-r--r--  2.0 unx     8287 b- defN 80-Jan-01 00:00 validmind/vm_models/dataset_utils.py
 -rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 validmind/vm_models/figure.py
@@ -31,11 +34,11 @@
 -rw-r--r--  2.0 unx     3739 b- defN 80-Jan-01 00:00 validmind/vm_models/plot_utils.py
 -rw-r--r--  2.0 unx     1518 b- defN 80-Jan-01 00:00 validmind/vm_models/result_summary.py
 -rw-r--r--  2.0 unx     3195 b- defN 80-Jan-01 00:00 validmind/vm_models/test_context.py
 -rw-r--r--  2.0 unx    10124 b- defN 80-Jan-01 00:00 validmind/vm_models/test_plan.py
 -rw-r--r--  2.0 unx    19083 b- defN 80-Jan-01 00:00 validmind/vm_models/test_plan_result.py
 -rw-r--r--  2.0 unx     1698 b- defN 80-Jan-01 00:00 validmind/vm_models/test_result.py
 -rw-r--r--  2.0 unx     3621 b- defN 80-Jan-01 00:00 validmind/vm_models/threshold_test.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 validmind-1.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx     1369 b- defN 80-Jan-01 00:00 validmind-1.4.2.dist-info/METADATA
-?rw-r--r--  2.0 unx     3566 b- defN 16-Jan-01 00:00 validmind-1.4.2.dist-info/RECORD
-39 files, 267659 bytes uncompressed, 67843 bytes compressed:  74.7%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 validmind-1.4.3a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1371 b- defN 80-Jan-01 00:00 validmind-1.4.3a0.dist-info/METADATA
+?rw-r--r--  2.0 unx     3864 b- defN 16-Jan-01 00:00 validmind-1.4.3a0.dist-info/RECORD
+42 files, 273182 bytes uncompressed, 69483 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -12,14 +12,23 @@
 
 Filename: validmind/data_validation/metrics.py
 Comment: 
 
 Filename: validmind/data_validation/threshold_tests.py
 Comment: 
 
+Filename: validmind/datasets/regression/__init__.py
+Comment: 
+
+Filename: validmind/datasets/regression/fred.py
+Comment: 
+
+Filename: validmind/datasets/regression/lending_club.py
+Comment: 
+
 Filename: validmind/model_utils.py
 Comment: 
 
 Filename: validmind/model_validation/__init__.py
 Comment: 
 
 Filename: validmind/model_validation/model_metadata.py
@@ -102,17 +111,17 @@
 
 Filename: validmind/vm_models/test_result.py
 Comment: 
 
 Filename: validmind/vm_models/threshold_test.py
 Comment: 
 
-Filename: validmind-1.4.2.dist-info/WHEEL
+Filename: validmind-1.4.3a0.dist-info/WHEEL
 Comment: 
 
-Filename: validmind-1.4.2.dist-info/METADATA
+Filename: validmind-1.4.3a0.dist-info/METADATA
 Comment: 
 
-Filename: validmind-1.4.2.dist-info/RECORD
+Filename: validmind-1.4.3a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## validmind/data_validation/metrics.py

```diff
@@ -612,26 +612,26 @@
         results = {
             "observed": sd.observed,
             "trend": sd.trend,
             "seasonal": sd.seasonal,
             "resid": sd.resid,
         }
 
-        # Convert pandas Series to DataFrames, reset their indices, and format the dates as strings
+        # Convert pandas Series to DataFrames, reset their indices, and convert the dates to strings
         dfs = [
             pd.DataFrame(series)
             .pipe(
                 lambda x: x.reset_index()
                 if not isinstance(x.index, pd.DatetimeIndex)
                 else x.reset_index().rename(columns={x.index.name: "Date"})
             )
             .assign(
-                Date=lambda x: x["Date"].dt.strftime("%Y-%m-%d")
+                Date=lambda x: x["Date"].astype(str)
                 if "Date" in x.columns
-                else x.index.strftime("%Y-%m-%d")
+                else x.index.astype(str)
             )
             for series in results.values()
         ]
 
         # Merge DataFrames on the 'Date' column
         merged_df = dfs[0]
         for df in dfs[1:]:
```

## validmind/data_validation/threshold_tests.py

```diff
@@ -382,20 +382,26 @@
 
         temp_df = self.df.copy(deep=True)
         temp_df = temp_df.dropna()
         typeset = ProfilingTypeSet(Settings())
         dataset_types = typeset.infer_type(temp_df)
         test_results = []
         test_figures = []
-        num_features_columns = [k for k, v in dataset_types.items() if str(v) == "Numeric"]
+        num_features_columns = [
+            k for k, v in dataset_types.items() if str(v) == "Numeric"
+        ]
 
-        outliers_table = self._identify_outliers(temp_df[num_features_columns], zscore_threshold)
+        outliers_table = self._identify_outliers(
+            temp_df[num_features_columns], zscore_threshold
+        )
         fig = self._plot_outliers(temp_df, outliers_table)
         passed = outliers_table.empty
-        outliers_table["Date"] = outliers_table["Date"].astype(str)
+
+        if not outliers_table.empty:
+            outliers_table["Date"] = outliers_table["Date"].astype(str)
 
         test_results.append(
             TestResult(
                 test_name="outliers",
                 passed=passed,
                 values=outliers_table.to_dict(orient="list"),
             )
@@ -422,53 +428,64 @@
         """
         z_scores = pd.DataFrame(stats.zscore(df), index=df.index, columns=df.columns)
         outliers = z_scores[(z_scores > threshold).any(axis=1)]
         outlier_table = []
         for idx, row in outliers.iterrows():
             for col in df.columns:
                 if abs(row[col]) > threshold:
-                    outlier_table.append({"Variable": col, "z-score": row[col], "Threshold": threshold, "Date": idx})
+                    outlier_table.append(
+                        {
+                            "Variable": col,
+                            "z-score": row[col],
+                            "Threshold": threshold,
+                            "Date": idx,
+                        }
+                    )
         return pd.DataFrame(outlier_table)
 
     def _plot_outliers(self, df, outliers_table):
         """
         Plots time series with identified outliers.
 
         Args:
             df (pandas.DataFrame): Input data with time series.
             outliers_table (pandas.DataFrame): DataFrame with identified outliers.
 
         Returns:
             matplotlib.figure.Figure: A matplotlib figure object with subplots for each variable.
         """
+        print(outliers_table)
         sns.set(style="darkgrid")
         n_variables = len(df.columns)
         fig, axes = plt.subplots(n_variables, 1, sharex=True)
 
         for i, col in enumerate(df.columns):
             sns.lineplot(data=df, x=df.index, y=col, ax=axes[i], label=col)
 
-            variable_outliers = outliers_table[outliers_table["Variable"] == col]
-            for idx, row in variable_outliers.iterrows():
-                date = row["Date"]
-                outlier_value = df.loc[date, col]
-                axes[i].scatter(date, outlier_value, marker="o", s=100, c="red",
-                                label="Outlier" if idx == 0 else "")
+            if not outliers_table.empty:
+                variable_outliers = outliers_table[outliers_table["Variable"] == col]
+                for idx, row in variable_outliers.iterrows():
+                    date = row["Date"]
+                    outlier_value = df.loc[date, col]
+                    axes[i].scatter(
+                        date,
+                        outlier_value,
+                        marker="o",
+                        s=100,
+                        c="red",
+                        label="Outlier" if idx == 0 else "",
+                    )
 
             axes[i].legend()
-            axes[i].set_ylabel(
-                col, weight="bold", fontsize=16
-            )
+            axes[i].set_ylabel(col, weight="bold", fontsize=16)
             axes[i].set_title(
                 f"Time Series with Outliers for {col}", weight="bold", fontsize=16
             )
 
-        plt.xlabel(
-            "Date", weight="bold", fontsize=16
-        )
+        plt.xlabel("Date", weight="bold", fontsize=16)
         plt.tight_layout()
 
         # Do this if you want to prevent the figure from being displayed
         plt.close("all")
         return fig
 
 
@@ -505,67 +522,59 @@
         ]
 
         fig_barplot = self._barplot(self.df, rotation=45, font_size=16)
         fig_heatmap = self._heatmap(self.df)
         test_figures = []
         if fig_barplot is not None:
             test_figures.append(
-                Figure(
-                    key=f"{self.name}:barplot",
-                    figure=fig_barplot,
-                    metadata={}
-                )
+                Figure(key=f"{self.name}:barplot", figure=fig_barplot, metadata={})
             )
             test_figures.append(
-                Figure(
-                    key=f"{self.name}:heatmap",
-                    figure=fig_heatmap,
-                    metadata={}
-                )
+                Figure(key=f"{self.name}:heatmap", figure=fig_heatmap, metadata={})
             )
 
-        return self.cache_results(test_results, passed=all([r.passed for r in test_results]), figures=test_figures)
+        return self.cache_results(
+            test_results,
+            passed=all([r.passed for r in test_results]),
+            figures=test_figures,
+        )
 
-    def _barplot(self, df: pd.DataFrame, rotation: int = 45,
-                 font_size: int = 18) -> plt.Figure:
+    def _barplot(
+        self, df: pd.DataFrame, rotation: int = 45, font_size: int = 18
+    ) -> plt.Figure:
         """
         Generate a bar plot of missing values in a pandas DataFrame.
 
         Args:
         df (pandas.DataFrame): The input DataFrame to plot the missing values of.
         rotation (int): The rotation angle for x-axis labels. Default is 45.
         font_size (int): The font size for x-axis and y-axis labels. Default is 18.
 
         Returns:
         matplotlib.figure.Figure: A matplotlib figure object containing the bar plot.
         """
         # Create a bar plot using seaborn library
         missing_values = df.isnull().sum()
         if sum(missing_values.values) != 0:
-
-            with plt.style.context('seaborn'):
+            with plt.style.context("seaborn"):
                 fig, ax = plt.subplots()
                 sns.barplot(
                     data=missing_values,
                     x=missing_values.index,
                     y=missing_values.values,
                     ax=ax,
                 )
                 ax.set_xticklabels(
                     labels=missing_values.index, rotation=rotation, fontsize=font_size
                 )
-                plt.yticks(
-                    rotation=45, fontsize=font_size
-                )
+                plt.yticks(rotation=45, fontsize=font_size)
                 ax.set_ylabel(
                     "Number of Missing Values", weight="bold", fontsize=font_size
                 )
-                ax.set_xlabel(
-                    "Variables (Columns)", weight="bold", fontsize=font_size
-                )
+                ax.set_xlabel("Variables (Columns)", weight="bold", fontsize=font_size)
                 ax.set_title(
                     "Total Number of Missing Values per Variable",
                     weight="bold",
                     fontsize=font_size + 2,
                 )
         else:
             fig = None
@@ -588,32 +597,28 @@
         # Create a boolean mask for missing values
         missing_mask = df.isnull()
         # Set seaborn plot style
         sns.set(style="darkgrid")
         fig, ax = plt.subplots()
 
         # Plot the heatmap
-        sns.heatmap(missing_mask.T, cmap='viridis', cbar=False, xticklabels=False, ax=ax)
+        sns.heatmap(
+            missing_mask.T, cmap="viridis", cbar=False, xticklabels=False, ax=ax
+        )
 
         # Add actual years on the x-axis
         years = df.index.year.unique()
-        xticks = [df.index.get_loc(df.index[df.index.year == year][0]) for year in years]
-        plt.xticks(
-            xticks, years, rotation=45, fontsize=18
-        )
-        plt.yticks(
-            rotation=45, fontsize=18
-        )
+        xticks = [
+            df.index.get_loc(df.index[df.index.year == year][0]) for year in years
+        ]
+        plt.xticks(xticks, years, rotation=45, fontsize=18)
+        plt.yticks(rotation=45, fontsize=18)
         plt.gca().xaxis.set_major_locator(plt.MultipleLocator(5))
-        ax.set_xlabel(
-            "Rows (Years)", weight="bold", fontsize=18
-        )
-        ax.set_ylabel(
-            "Variables (Columns)", weight="bold", fontsize=18
-        )
+        ax.set_xlabel("Rows (Years)", weight="bold", fontsize=18)
+        ax.set_ylabel("Variables (Columns)", weight="bold", fontsize=18)
         ax.set_title(
             "Missing Values Heatmap with Actual Years in Rows",
             weight="bold",
             fontsize=20,
         )
         # Do this if you want to prevent the figure from being displayed
         plt.close("all")
@@ -643,43 +648,54 @@
                 passed=n_frequencies == 1,
                 values=freq_df.to_dict(orient="list"),
             )
         ]
         fig_frequency = self._frequncy_plot(self.df)
         test_figures = []
         test_figures.append(
-            Figure(
-                key=f"{self.name}:frequecyplot",
-                figure=fig_frequency,
-                metadata={}
-            )
+            Figure(key=f"{self.name}:frequecyplot", figure=fig_frequency, metadata={})
+        )
+        return self.cache_results(
+            test_results,
+            passed=all([r.passed for r in test_results]),
+            figures=test_figures,
         )
-        return self.cache_results(test_results, passed=all([r.passed for r in test_results]), figures=test_figures)
 
     def _identify_frequencies(self, df):
         """
         Identify the frequency of each series in the DataFrame.
 
         :param df: Time-series DataFrame
         :return: DataFrame with two columns: 'Variable' and 'Frequency'
         """
         frequencies = []
-        freq_dict = {'S': 'Second', 'T': 'Minute', 'min': 'Minute', 'H': 'Hourly', 'D': 'Daily',
-                     'B': 'Business day', 'W': 'Weekly', 'MS': 'Monthly', 'M': 'Monthly', 'Q': 'Quarterly',
-                     'A': 'Yearly', 'Y': 'Yearly'}
+        freq_dict = {
+            "S": "Second",
+            "T": "Minute",
+            "min": "Minute",
+            "H": "Hourly",
+            "D": "Daily",
+            "B": "Business day",
+            "W": "Weekly",
+            "MS": "Monthly",
+            "M": "Monthly",
+            "Q": "Quarterly",
+            "A": "Yearly",
+            "Y": "Yearly",
+        }
 
         for column in df.columns:
             series = df[column].dropna()
             if not series.empty:
                 freq = pd.infer_freq(series.index)
                 label = freq_dict[freq] if freq in freq_dict.keys() else freq
             else:
                 label = None
 
-            frequencies.append({'Variable': column, 'Frequency': label})
+            frequencies.append({"Variable": column, "Frequency": label})
 
         freq_df = pd.DataFrame(frequencies)
 
         return freq_df
 
     def _frequncy_plot(self, df):
         """
@@ -695,30 +711,24 @@
         # Calculate the time differences between consecutive entries
         time_diff = df.index.to_series().diff().dropna()
 
         # Convert the time differences to a suitable unit (e.g., days)
         time_diff_days = time_diff.dt.total_seconds() / (60 * 60 * 24)
 
         # Create a DataFrame with the time differences
-        time_diff_df = pd.DataFrame({'Time Differences (Days)': time_diff_days})
+        time_diff_df = pd.DataFrame({"Time Differences (Days)": time_diff_days})
         fig, ax = plt.subplots()
         # Plot the frequency distribution of the time differences
         sns.histplot(
-            data=time_diff_df, x='Time Differences (Days)', bins=50, kde=False, ax=ax
+            data=time_diff_df, x="Time Differences (Days)", bins=50, kde=False, ax=ax
         )
 
-        plt.yticks(
-            rotation=45, fontsize=18
-        )
-        ax.set_ylabel(
-            "Frequency", weight="bold", fontsize=18
-        )
-        ax.set_xlabel(
-            "Time Differences (Days)", weight="bold", fontsize=18
-        )
+        plt.yticks(rotation=45, fontsize=18)
+        ax.set_ylabel("Frequency", weight="bold", fontsize=18)
+        ax.set_xlabel("Time Differences (Days)", weight="bold", fontsize=18)
         ax.set_title(
             "Frequency",
             weight="bold",
             fontsize=20,
         )
 
         # Do this if you want to prevent the figure from being displayed
```

## validmind/model_validation/statsmodels/metrics.py

```diff
@@ -739,7 +739,83 @@
             "Independent Variables": X_columns,
             "R-Squared": r2,
             "Adjusted R-Squared": adj_r2,
             "MSE": mse,
             "RMSE": rmse,
         }
         return self.cache_results(results)
+
+
+@dataclass
+class RegressionModelInsampleComparison(Metric):
+    """
+    Test that output the comparison of stats library regression models.
+    """
+
+    category = "model_performance"
+    scope = "test"
+    name = "regression_insample_performance"
+
+    def description(self):
+        return """
+        This section shows In-sample comparison of regression models involves comparing
+        the performance of different regression models on the same dataset that was used
+        to train the models. This is typically done by calculating a goodness-of-fit statistic
+        such as the R-squared or mean squared error (MSE) for each model, and then comparing
+        these statistics to determine which model has the best fit to the data.
+        """
+
+    def run(self):
+        # Check models list is not empty
+        if not self.models:
+            raise ValueError("List of models must be provided in the models parameter")
+        all_models = []
+        for model in self.models:
+            if model.model.__class__.__name__ != "RegressionResultsWrapper":
+                raise ValueError("Only RegressionResultsWrapper models of statsmodels library supported")
+            all_models.append(model.model)
+
+        results = self._in_sample_performance_ols(all_models)
+        return self.cache_results(results)
+
+    def _in_sample_performance_ols(self, models):
+        """
+        Computes the in-sample performance evaluation metrics for a list of OLS models.
+
+        Args:
+        models (list): A list of statsmodels OLS models.
+
+        Returns:
+        list: A list of dictionaries containing the evaluation results for each model.
+        Each dictionary contains the following keys:
+        - 'Model': A string identifying the model.
+        - 'Independent Variables': A list of strings identifying the independent variables used in the model.
+        - 'R-Squared': The R-squared value of the model.
+        - 'Adjusted R-Squared': The adjusted R-squared value of the model.
+        - 'MSE': The mean squared error of the model.
+        - 'RMSE': The root mean squared error of the model.
+        """
+        evaluation_results = []
+
+        for i, model in enumerate(models):
+            # print(model.model)
+            X_columns = model.model.exog_names
+
+            # Extract R-squared and Adjusted R-squared
+            r2 = model.rsquared
+            adj_r2 = model.rsquared_adj
+
+            # Calculate the Mean Squared Error (MSE) and Root Mean Squared Error (RMSE)
+            mse = model.mse_resid
+            rmse = mse ** 0.5
+
+            # Append the results to the evaluation_results list
+            evaluation_results.append({
+                'Model': f'Model_{i + 1}',
+                'Independent Variables': X_columns,
+                'R-Squared': r2,
+                'Adjusted R-Squared': adj_r2,
+                'MSE': mse,
+                'RMSE': rmse
+            })
+
+        return evaluation_results
```

## validmind/test_plans/__init__.py

```diff
@@ -23,14 +23,15 @@
     NormalityTestPlan,
     AutocorrelationTestPlan,
     SesonalityTestPlan,
     UnitRoot,
     StationarityTestPlan,
     TimeSeries,
     RegressionModelPerformance,
+    RegressionModelsComparison,
 )
 from .time_series import (
     TimeSeriesUnivariate,
     TimeSeriesMultivariate,
     TimeSeriesForecast,
 )
 
@@ -50,14 +51,15 @@
     "timeseries": TimeSeries,
     "time_series_data_quality": TimeSeriesDataQuality,
     "time_series_dataset": TimeSeriesDataset,
     "time_series_univariate": TimeSeriesUnivariate,
     "time_series_multivariate": TimeSeriesMultivariate,
     "time_series_forecast": TimeSeriesForecast,
     "regression_model_performance": RegressionModelPerformance,
+    "regression_models_comparison": RegressionModelsComparison,
 }
 
 # These test plans can be added by the user
 custom_test_plans = {}
 
 
 def _get_all_test_plans():
```

## validmind/test_plans/statsmodels_timeseries.py

```diff
@@ -14,14 +14,15 @@
     ADF,
     KPSS,
     PhillipsPerronArch,
     ZivotAndrewsArch,
     DFGLSArch,
     ResidualsVisualInspection,
     RegressionModelSummary,
+    RegressionModelInsampleComparison,
 )
 
 
 class AutocorrelationTestPlan(TestPlan):
     """
     Test plan to perform autocorrelation tests.
     """
@@ -96,14 +97,23 @@
         SesonalityTestPlan,
         StationarityTestPlan,
     ]
 
 
 class RegressionModelPerformance(TestPlan):
     """
-    Test plan for statsmodels regressor models that includes
-    both metrics and validation tests
+    Test plan for performance metric of regression model of statsmodels library
     """
 
     name = "regression_model_performance"
     required_context = ["model"]
     tests = [RegressionModelSummary]
+
+
+class RegressionModelsComparison(TestPlan):
+    """
+    Test plan for metrics comparison of regression model of statsmodels library
+    """
+
+    name = "regression_models_comparison"
+    required_context = ["models"]
+    tests = [RegressionModelInsampleComparison]
```

## Comparing `validmind-1.4.2.dist-info/METADATA` & `validmind-1.4.3a0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validmind
-Version: 1.4.2
+Version: 1.4.3a0
 Summary: ValidMind SDK
 Author: Andres Rodriguez
 Author-email: andres@validmind.ai
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `validmind-1.4.2.dist-info/RECORD` & `validmind-1.4.3a0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 validmind/__init__.py,sha256=_-1gzCQo2v2TEjQPyRD2SLJ7UCOiaPVFWnTkxMf7gfY,1380
 validmind/api_client.py,sha256=fqEWQii5H5uS4gbjm2X05mKKfPGeQiV6VkuMf_fC2Gw,11353
 validmind/client.py,sha256=EdMYEoCi0ujBflAXDhTEJdvIxxksBC1a-Ysxszhl3i4,8788
 validmind/data_validation/__init__.py,sha256=xytRpsfQ86fDnIZRoAO7GMVVU_TwWVMXxSCwm0mb45I,590
-validmind/data_validation/metrics.py,sha256=gtg-iDBdYoMyyvkhlH6silAZz6kv3HgwxxdXP5PZ_fg,34464
-validmind/data_validation/threshold_tests.py,sha256=UdZebkWgU-5tNt3Rr3wSelrITj2SqNk-9hG_ZfBcPIY,23675
+validmind/data_validation/metrics.py,sha256=6-IvmaSmsZWE88rp_f2kCtIZTWKxB-jzLatybBBUrIE,34444
+validmind/data_validation/threshold_tests.py,sha256=L7PRkFxtVVZZXMco1pX4tjwBle7JFty1ZTsh6L6baw8,23919
+validmind/datasets/regression/__init__.py,sha256=uFK8Qxq6dSapwz6WrRz7uxi3n-msUxw6bOlZn3gKAUM,1290
+validmind/datasets/regression/fred.py,sha256=_czEU3LzmC_a-kjpGf93-XCc7y0bS0acNxK5qolov7c,187
+validmind/datasets/regression/lending_club.py,sha256=vZ1kvXzM7xuc43G2exGszeFh4cOV7acn_sA_8TyFKhs,195
 validmind/model_utils.py,sha256=DuPN2tF582ho167mfodODseJ6LIVuQOF9Xx0zv6b4Yk,10529
 validmind/model_validation/__init__.py,sha256=uFK8Qxq6dSapwz6WrRz7uxi3n-msUxw6bOlZn3gKAUM,1290
 validmind/model_validation/model_metadata.py,sha256=7zWQjRgMCpxWvHWTe7oG10872WaXGW18qMVu22DG3UA,4927
 validmind/model_validation/sklearn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 validmind/model_validation/sklearn/metrics.py,sha256=b92o5W5djP_Oyb_0qXY2VA6BvJhpqKApSVkX3e_mbGM,12925
 validmind/model_validation/sklearn/threshold_tests.py,sha256=DNdBWvb2AdOcLIVDFQoC49b2aa_EAUsGrcS_UbsGpPQ,30637
 validmind/model_validation/statsmodels/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-validmind/model_validation/statsmodels/metrics.py,sha256=9157bMX7Vu8iLixCndtsue-Mq-Xl0_ENc36ixW1krqI,22475
+validmind/model_validation/statsmodels/metrics.py,sha256=v36pYQggBTGKf6yNCcOmjTxUEARVBZEznuwWdRhsqnU,25419
 validmind/model_validation/statsmodels/threshold_tests.py,sha256=SyEv7oaNIgiQ1ML3dQrGN54pSP88j9htOy4V2l4Ipwk,1317
 validmind/model_validation/utils.py,sha256=lOq-C_mucS5JZ-7V43PnSqYkGc5ybdGDbzhclWp4V3A,1657
-validmind/test_plans/__init__.py,sha256=3STA6iXcfJ_c-v6a4TWXzv6W0qK0VFOgAZ3eNCgx6uw,5292
+validmind/test_plans/__init__.py,sha256=KwWG62GTWuQpGnY6f14Sqc23AJCJxuw0nVoxRidQR0Y,5388
 validmind/test_plans/sklearn_classifier.py,sha256=hSnhsOYHmjBoXysQA9WYG0PLCfrraItWLblvNtDpSy4,2431
-validmind/test_plans/statsmodels_timeseries.py,sha256=Zo-UhpDX5CzfQmM0xgzuZ4PAUiRR0r0FobXiiCsn4lU,2464
+validmind/test_plans/statsmodels_timeseries.py,sha256=yXb0A6eaVewf0V3e39xDYtPcm80uGvmMqrrUYvHuxws,2751
 validmind/test_plans/tabular_datasets.py,sha256=5uyGOGnt5ngTsSJ-0DdonAlbErhprq9dZdZ2c0EXKik,2068
 validmind/test_plans/time_series.py,sha256=6cQTS6qWMZZD7ntgvGhhDeQDcM6SyQXj1uN_gAK01es,6814
 validmind/utils.py,sha256=X3RMB7OlJU9jhKOkQFYbTifzpROn8pqIjxJXe6NilWY,6647
 validmind/vm_models/__init__.py,sha256=9KA42gT5a9ocSfum5b3UaXHxuaI_NWiKAXalOWg9G3E,1065
 validmind/vm_models/dataset.py,sha256=7cAJdmKQCFfST4-Dot5Hq-vqTO9sRVNJHl3fHBhTt80,10156
 validmind/vm_models/dataset_utils.py,sha256=xWq6dbxe9fCUdpKCiEFvbxhy9t7cOKh0boS-zw6ynZo,8287
 validmind/vm_models/figure.py,sha256=EarfMm49J2BWf6UhsMFGr3VSdGu8v2ZewzArKKp_LfU,592
@@ -30,10 +33,10 @@
 validmind/vm_models/plot_utils.py,sha256=OwydtuOvdpdi80creg5srNr87LbqGBYow4dS0Lzg4cw,3739
 validmind/vm_models/result_summary.py,sha256=1YGlWqcO4PY2NtDm7fbuOSLXPIu6KM1USp_pgh6rmJM,1518
 validmind/vm_models/test_context.py,sha256=q1PGyA76R1ncWVtkK4U9W_8_dpjPuHnEA5EvXA8uu2s,3195
 validmind/vm_models/test_plan.py,sha256=1zl3_Nc4bWol6b2KSBCqfYjmrvxxD4hKjsX-FbuXyKs,10124
 validmind/vm_models/test_plan_result.py,sha256=UG3PdlkdFED-LGmqYtFHWqkmexBIHPPg6SNcfWlq4h4,19083
 validmind/vm_models/test_result.py,sha256=jiX8yb1NptBXZQ_pOyHloc8I6yS6zamYm0j9OWUqrHs,1698
 validmind/vm_models/threshold_test.py,sha256=uqTqHDf443_Xm2J4G5KBnMH0GLRVVIpv6V-A3f-tSvE,3621
-validmind-1.4.2.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-validmind-1.4.2.dist-info/METADATA,sha256=xT5GWWtxidgkmZe4zTkM7zQ8yaP7QNe0u4gGB_QykpA,1369
-validmind-1.4.2.dist-info/RECORD,,
+validmind-1.4.3a0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+validmind-1.4.3a0.dist-info/METADATA,sha256=hNE6FdSv5u9WypdxZO7CH4JRsxKaixm-jl9i2_EoqEs,1371
+validmind-1.4.3a0.dist-info/RECORD,,
```

