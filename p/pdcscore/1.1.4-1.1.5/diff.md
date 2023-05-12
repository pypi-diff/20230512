# Comparing `tmp/pdcscore-1.1.4.tar.gz` & `tmp/pdcscore-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdcscore-1.1.4.tar", last modified: Tue May  9 02:46:58 2023, max compression
+gzip compressed data, was "pdcscore-1.1.5.tar", last modified: Fri May 12 03:14:41 2023, max compression
```

## Comparing `pdcscore-1.1.4.tar` & `pdcscore-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 02:46:58.076979 pdcscore-1.1.4/
--rw-rw-rw-   0        0        0     1099 2023-05-09 02:44:59.000000 pdcscore-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     5621 2023-05-09 02:46:58.076979 pdcscore-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4419 2023-05-09 02:44:59.000000 pdcscore-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 02:46:58.054356 pdcscore-1.1.4/pdcscore/
--rw-rw-rw-   0        0        0       81 2023-05-09 02:44:59.000000 pdcscore-1.1.4/pdcscore/__init__.py
--rw-rw-rw-   0        0        0     4336 2023-05-09 02:44:59.000000 pdcscore-1.1.4/pdcscore/pdcscore.py
-drwxrwxrwx   0        0        0        0 2023-05-09 02:46:58.075980 pdcscore-1.1.4/pdcscore.egg-info/
--rw-rw-rw-   0        0        0     5621 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 02:46:58.077978 pdcscore-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1646 2023-05-09 02:44:59.000000 pdcscore-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:14:40.998701 pdcscore-1.1.5/
+-rw-rw-rw-   0        0        0     1099 2023-05-12 03:08:46.000000 pdcscore-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     5580 2023-05-12 03:14:40.998701 pdcscore-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4378 2023-05-12 03:08:46.000000 pdcscore-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 03:14:40.981695 pdcscore-1.1.5/pdcscore/
+-rw-rw-rw-   0        0        0       81 2023-05-12 03:08:46.000000 pdcscore-1.1.5/pdcscore/__init__.py
+-rw-rw-rw-   0        0        0     3869 2023-05-12 03:08:46.000000 pdcscore-1.1.5/pdcscore/pdcscore.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:14:40.996699 pdcscore-1.1.5/pdcscore.egg-info/
+-rw-rw-rw-   0        0        0     5580 2023-05-12 03:14:40.000000 pdcscore-1.1.5/pdcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-12 03:14:40.000000 pdcscore-1.1.5/pdcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 03:14:40.000000 pdcscore-1.1.5/pdcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-12 03:14:40.000000 pdcscore-1.1.5/pdcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 03:14:40.000000 pdcscore-1.1.5/pdcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 03:14:40.998701 pdcscore-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2023-05-12 03:14:04.000000 pdcscore-1.1.5/setup.py
```

### Comparing `pdcscore-1.1.4/LICENSE` & `pdcscore-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pdcscore-1.1.4/PKG-INFO` & `pdcscore-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.1.4
+Version: 1.1.5
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: https://github.com/famutimine/pdcscore
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
@@ -29,15 +29,15 @@
 The objective of this package is to offer a Python-based solution for computing the Proportion of Days Covered (PDC), a widely used metric in the healthcare industry to evaluate medication adherence. As the healthcare analytics sector shifts away from SAS, there is a growing need to recreate key metrics in alternative platforms. This package aims to simplify the process and reduce the workload for business analysts in the healthcare ecosystem by providing a readily available PDC calculation tool, thereby eliminating the need to build it from scratch.
 
 I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 
-Current update accounts for 6 months washout period and is optimized for multiprocessing large datasets.
+Current update is optimized for multiprocessing large datasets.
 
 Please use as described below:
 
 **INPUT PARAMETERS:**
 
 **dataframe** - *A pandas dataframe containing the required columns described below.*
```

### Comparing `pdcscore-1.1.4/README.md` & `pdcscore-1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 The objective of this package is to offer a Python-based solution for computing the Proportion of Days Covered (PDC), a widely used metric in the healthcare industry to evaluate medication adherence. As the healthcare analytics sector shifts away from SAS, there is a growing need to recreate key metrics in alternative platforms. This package aims to simplify the process and reduce the workload for business analysts in the healthcare ecosystem by providing a readily available PDC calculation tool, thereby eliminating the need to build it from scratch.
 
 I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 
-Current update accounts for 6 months washout period and is optimized for multiprocessing large datasets.
+Current update is optimized for multiprocessing large datasets.
 
 Please use as described below:
 
 **INPUT PARAMETERS:**
 
 **dataframe** - *A pandas dataframe containing the required columns described below.*
```

### Comparing `pdcscore-1.1.4/pdcscore/pdcscore.py` & `pdcscore-1.1.5/pdcscore/pdcscore.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,33 +14,27 @@
         self.msr_end_dt_col = msr_end_dt_col
 
     def calculate_pdc(self, n_workers=cpu_count()):
         pool = Pool(processes=n_workers)
         df = self.dataframe.copy()
 
         # Calculate the date difference
-        df['date_diff'] = df[self.msr_start_dt_col] - df[self.filldate_col] + pd.Timedelta(days=1)
-
-        # Filter rows where date difference is less than or equal to 180 days
-        df = df[df['date_diff'] < pd.Timedelta(days=180)]
-
-        # Remove the date_diff column
-        df = df.drop('date_diff', axis=1)
+        df=df[df[self.filldate_col]>=df[self.msr_start_dt_col]]
 
         # Get the fill_enddate
         df['fill_enddate'] = df[self.filldate_col] + pd.to_timedelta(df[self.supply_days_col], unit='D') - pd.Timedelta(days=1)
 
         # Group the dataframe and select the first value of each column within each group
         df_sorted=df.sort_values(by=[self.patient_id_col, self.drugname_col,self.filldate_col])
         first_fill_dates=df_sorted.groupby([self.patient_id_col, self.drugname_col])[self.filldate_col].first().reset_index().rename(columns={self.filldate_col:'first_filldate'})
         
         # derive the effective measurement start date
         base_data = first_fill_dates.merge(df[[self.patient_id_col, self.drugname_col,self.msr_start_dt_col,self.msr_end_dt_col]],on=[self.patient_id_col, self.drugname_col], how='left').drop_duplicates()
         base_data['effective_msr_start_dt'] = base_data.apply(lambda row: row['first_filldate']
-                                                        if row['first_filldate'] >= row[self.msr_start_dt_col]
+                                                        if row['first_filldate'] > row[self.msr_start_dt_col]
                                                         else row[self.msr_start_dt_col], axis=1)
 
           
         # Calculate the totaldays: denominator for each patient-drugname pair
         base_data['totaldays']=(base_data[self.msr_end_dt_col] + pd.Timedelta(days=1) - base_data['effective_msr_start_dt']).dt.days
         base_data=base_data.drop_duplicates()
 
@@ -51,18 +45,15 @@
 
 
         # Create a date array for each row that represents all valid rows based on logic below:
         # if the filldate_col is less than effective_msr_start_dt (effective start date of the measurement period) then use effective_msr_start_dt
         # else use filldate_col as the start of the range, the end date of the range is the fill_enddate less of msr_end_dt_col
 
         def generate_date_array(row):
-            date_range = pd.date_range(start=row['effective_msr_start_dt']
-                                       if row[self.filldate_col] < row['effective_msr_start_dt']
-                                       else row[self.filldate_col],
-                                       end=row['fill_enddate'])
+            date_range = pd.date_range(start=row['effective_msr_start_dt'],end=row['fill_enddate'])
             return [str(date.date()) for date in date_range if date <= row[self.msr_end_dt_col]]
 
         dc['date_array'] = [generate_date_array(row) for _, row in dc.iterrows()]
         
         # Group by 'patient_id_col', 'drugname_col', 'totaldays' and aggregate by a concatenated list of unique dates (to avoid overlapping dates)
         # the array length represents the dayscovered
         pdc = dc.groupby([self.patient_id_col, self.drugname_col, 'totaldays'])['date_array'].apply(lambda x: len(np.unique(np.concatenate(x.tolist())))).reset_index(name='dayscovered')
```

### Comparing `pdcscore-1.1.4/pdcscore.egg-info/PKG-INFO` & `pdcscore-1.1.5/pdcscore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.1.4
+Version: 1.1.5
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: https://github.com/famutimine/pdcscore
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
@@ -29,15 +29,15 @@
 The objective of this package is to offer a Python-based solution for computing the Proportion of Days Covered (PDC), a widely used metric in the healthcare industry to evaluate medication adherence. As the healthcare analytics sector shifts away from SAS, there is a growing need to recreate key metrics in alternative platforms. This package aims to simplify the process and reduce the workload for business analysts in the healthcare ecosystem by providing a readily available PDC calculation tool, thereby eliminating the need to build it from scratch.
 
 I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 
-Current update accounts for 6 months washout period and is optimized for multiprocessing large datasets.
+Current update is optimized for multiprocessing large datasets.
 
 Please use as described below:
 
 **INPUT PARAMETERS:**
 
 **dataframe** - *A pandas dataframe containing the required columns described below.*
```

### Comparing `pdcscore-1.1.4/setup.py` & `pdcscore-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdcscore',
-    version='1.1.4',
+    version='1.1.5',
     description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/famutimine/pdcscore',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

