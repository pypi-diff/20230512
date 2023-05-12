# Comparing `tmp/wombatoo-0.0.6.tar.gz` & `tmp/wombatoo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Prashant\Desktop\wombatoo\dist\.tmp-7yohr9n5\wombatoo-0.0.6.tar", last modified: Sun May  7 17:10:56 2023, max compression
+gzip compressed data, was "C:\Users\Prashant\Desktop\wombatoo\dist\.tmp-oh1nm8ja\wombatoo-0.0.7.tar", last modified: Fri May 12 09:55:37 2023, max compression
```

## Comparing `wombatoo-0.0.6.tar` & `wombatoo-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:56.000000 wombatoo-0.0.6/
--rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-0.0.6/LICENSE.md
--rw-rw-rw-   0        0        0      409 2023-05-07 17:10:56.000000 wombatoo-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombatoo-0.0.6/README.md
--rw-rw-rw-   0        0        0      723 2023-05-07 17:10:13.000000 wombatoo-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 17:10:56.000000 wombatoo-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:56.000000 wombatoo-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:56.000000 wombatoo-0.0.6/src/wombatoo/
--rw-rw-rw-   0        0        0      189 2023-04-11 16:01:38.000000 wombatoo-0.0.6/src/wombatoo/DataCard.txt
--rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombatoo-0.0.6/src/wombatoo/__init__.py
--rw-rw-rw-   0        0        0     9595 2023-05-07 14:44:30.000000 wombatoo-0.0.6/src/wombatoo/wombatoo.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:56.000000 wombatoo-0.0.6/src/wombatoo.egg-info/
--rw-rw-rw-   0        0        0      409 2023-05-07 17:10:56.000000 wombatoo-0.0.6/src/wombatoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-05-07 17:10:56.000000 wombatoo-0.0.6/src/wombatoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 17:10:56.000000 wombatoo-0.0.6/src/wombatoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-07 17:10:56.000000 wombatoo-0.0.6/src/wombatoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 17:10:56.000000 wombatoo-0.0.6/src/wombatoo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 09:55:37.000000 wombatoo-0.0.7/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-0.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0      409 2023-05-12 09:55:37.000000 wombatoo-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombatoo-0.0.7/README.md
+-rw-rw-rw-   0        0        0      723 2023-05-12 09:53:14.000000 wombatoo-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 09:55:37.000000 wombatoo-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 09:55:37.000000 wombatoo-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:55:37.000000 wombatoo-0.0.7/src/wombatoo/
+-rw-rw-rw-   0        0        0      189 2023-04-11 16:01:38.000000 wombatoo-0.0.7/src/wombatoo/DataCard.txt
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombatoo-0.0.7/src/wombatoo/__init__.py
+-rw-rw-rw-   0        0        0     8673 2023-05-12 09:54:19.000000 wombatoo-0.0.7/src/wombatoo/wombatoo.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:55:37.000000 wombatoo-0.0.7/src/wombatoo.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-05-12 09:55:37.000000 wombatoo-0.0.7/src/wombatoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-05-12 09:55:37.000000 wombatoo-0.0.7/src/wombatoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 09:55:37.000000 wombatoo-0.0.7/src/wombatoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-12 09:55:37.000000 wombatoo-0.0.7/src/wombatoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 09:55:37.000000 wombatoo-0.0.7/src/wombatoo.egg-info/top_level.txt
```

### Comparing `wombatoo-0.0.6/LICENSE.md` & `wombatoo-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wombatoo-0.0.6/pyproject.toml` & `wombatoo-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
                     
 [project]
 name = "wombatoo"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Prashant Singh", email="prashdash112@gmail.com" },
 ]
 description = "A Data-Ops tool for devs"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = ["numpy==1.23.5",
```

### Comparing `wombatoo-0.0.6/src/wombatoo/wombatoo.py` & `wombatoo-0.0.7/src/wombatoo/wombatoo.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,236 +6,234 @@
 import os
 import random
 import string
 import hashlib
 import os
 from pyhtml2pdf import converter
 
-class wombatoo:
-    def __init__(self) -> None:
-        pass
+def metric_summary(df, path_to_save=None, columns=None):
+    '''
+    Summarizes metrics of a dataframe:
 
-    def metric_summary(df, path_to_save=None, columns=None):
-        '''
-        Summarizes metrics of a dataframe:
-    
-        >>> from datetime import date
-        >>> df = pd.DataFrame(
-        ...     {
-        ...         "a": [1.0, 2.8, 3.0],
-        ...         "b": [4, 5, None],
-        ...         "c": [True, False, True],
-        ...         "d": [None, "b", "c"],
-        ...         "e": ["usd", "eur", None],
-        ...         "f": [date(2020, 1, 1), date(2021, 1, 1), date(2022, 1, 1)],
-        ...     }
-        ... )
-    
-        >>> metric_summary(df)
-        shape: (7, 7)
-        ┌────────────┬──────────┬──────────┬──────────┬──────┬──────┬────────────┐
-        │ describe   ┆ a        ┆ b        ┆ c        ┆ d    ┆ e    ┆ f          │
-        │ ---        ┆ ---      ┆ ---      ┆ ---      ┆ ---  ┆ ---  ┆ ---        │
-        │ str        ┆ f64      ┆ f64      ┆ f64      ┆ str  ┆ str  ┆ str        │
-        ╞════════════╪══════════╪══════════╪══════════╪══════╪══════╪════════════╡
-        │ count      ┆ 3.0      ┆ 3.0      ┆ 3.0      ┆ 3    ┆ 3    ┆ 3          │
-        │ null_count ┆ 0.0      ┆ 1.0      ┆ 0.0      ┆ 1    ┆ 1    ┆ 0          │
-        │ mean       ┆ 2.266667 ┆ 4.5      ┆ 0.666667 ┆ null ┆ null ┆ null       │
-        │ std        ┆ 1.101514 ┆ 0.707107 ┆ 0.57735  ┆ null ┆ null ┆ null       │
-        │ min        ┆ 1.0      ┆ 4.0      ┆ 0.0      ┆ b    ┆ eur  ┆ 2020-01-01 │
-        │ max        ┆ 3.0      ┆ 5.0      ┆ 1.0      ┆ c    ┆ usd  ┆ 2022-01-01 │
-        │ median     ┆ 2.8      ┆ 4.5      ┆ 1.0      ┆ null ┆ null ┆ null       │
-        └────────────┴──────────┴──────────┴──────────┴──────┴──────┴────────────┘
-    
-        df: Dataframe to describe
-
-        path_to_save: path to save the metric summary results in csv format;
-
-        columns: Columns of dataframe to select
-
-        e.g: metric_summary(df,columns=['b','c','e'],path_to_save='./metric_summary.csv')
-
-    '''
-        if type(columns) == list:
-            describe = df.describe()
-            describe = describe[columns].T
-        else:
-            describe = df.describe().T
+    >>> from datetime import date
+    >>> df = pd.DataFrame(
+    ...     {
+    ...         "a": [1.0, 2.8, 3.0],
+    ...         "b": [4, 5, None],
+    ...         "c": [True, False, True],
+    ...         "d": [None, "b", "c"],
+    ...         "e": ["usd", "eur", None],
+    ...         "f": [date(2020, 1, 1), date(2021, 1, 1), date(2022, 1, 1)],
+    ...     }
+    ... )
+
+    >>> metric_summary(df)
+    shape: (7, 7)
+    ┌────────────┬──────────┬──────────┬──────────┬──────┬──────┬────────────┐
+    │ describe   ┆ a        ┆ b        ┆ c        ┆ d    ┆ e    ┆ f          │
+    │ ---        ┆ ---      ┆ ---      ┆ ---      ┆ ---  ┆ ---  ┆ ---        │
+    │ str        ┆ f64      ┆ f64      ┆ f64      ┆ str  ┆ str  ┆ str        │
+    ╞════════════╪══════════╪══════════╪══════════╪══════╪══════╪════════════╡
+    │ count      ┆ 3.0      ┆ 3.0      ┆ 3.0      ┆ 3    ┆ 3    ┆ 3          │
+    │ null_count ┆ 0.0      ┆ 1.0      ┆ 0.0      ┆ 1    ┆ 1    ┆ 0          │
+    │ mean       ┆ 2.266667 ┆ 4.5      ┆ 0.666667 ┆ null ┆ null ┆ null       │
+    │ std        ┆ 1.101514 ┆ 0.707107 ┆ 0.57735  ┆ null ┆ null ┆ null       │
+    │ min        ┆ 1.0      ┆ 4.0      ┆ 0.0      ┆ b    ┆ eur  ┆ 2020-01-01 │
+    │ max        ┆ 3.0      ┆ 5.0      ┆ 1.0      ┆ c    ┆ usd  ┆ 2022-01-01 │
+    │ median     ┆ 2.8      ┆ 4.5      ┆ 1.0      ┆ null ┆ null ┆ null       │
+    └────────────┴──────────┴──────────┴──────────┴──────┴──────┴────────────┘
+
+    df: Dataframe to describe
+
+    path_to_save: path to save the metric summary results in csv format;
+
+    columns: Columns of dataframe to select
+
+    e.g: metric_summary(df,columns=['b','c','e'],path_to_save='./metric_summary.csv')
+
+'''
+    if type(columns) == list:
+        describe = df.describe()
+        describe = describe[columns].T
+    else:
+        describe = df.describe().T
+
+    describe.to_csv(path_to_save) if path_to_save!= None else 0
+
+    return describe
+
+def schema(df, path_to_save=None, show=True):
+    '''
+    Function to print and save data schema in CSV or txt format.
+
+    df: Dataframe
+
+    path_to_save: path to save the schema results in csv format;
+
+    show: To show the schema on stdout.
+
+    e.g: schema(df,path_to_save='schema.csv', show=0)
+    '''
+
+    textStream = StringIO()
+    df.info(show_counts=False, memory_usage=False, buf=textStream)
+    lst =textStream.getvalue()
+    #removing unnecessary info
+    trim_list = lst.split()[19:]
+    dump = []
+    for i in range(0,len(trim_list)-3, 3):
+        dump.append(trim_list[i] + ',' + trim_list[i+1] + ',' +  trim_list[i+2])
+    if path_to_save != None:
+        np.savetxt(path_to_save, dump, delimiter=",",fmt='%s')
+    else:
+        pass
+    if show==True:
+        df.info()
+    else:
+        pass
     
-        describe.to_csv(path_to_save) if path_to_save!= None else 0
+def datacard(df, path_to_save='Datacard_user.txt'):
+    '''
+    Function to create datacard of a dataset
     
-        return describe
+    df: pandas dataframe for which user wants to generate a data card
     
-    def schema(df, path_to_save=None, show=True):
-        '''
-        Function to print and save data schema in CSV or txt format.
+    path_to_save: user-specific location of data card txt file. 
+                Defaulted to current working directory.
+    
+    e.g: datacard(df, './DataCard.txt')
+    '''
+    with open("DataCard.txt", "r+") as f:
+        old = f.read()
+    file_list = old.strip().split('\n')
+    dt = datetime.now()
+    file_list[2] = file_list[2] + str(dt)
+    file_list[4] = file_list[4] + os.getlogin()
+    arr = []
+    for i in df.columns:
+        x = df.shape[0]
+        l = df[i].drop_duplicates().shape[0]
+        if x == l:
+            arr.append(i)
+        else:
+            2
+    if len(arr) == 0:
+        p_key = "No primary key found"
+    else:
+        p_key = "Primary keys found: {arr}".format(arr=arr)
+    letters = string.ascii_lowercase
+    name = 'WOM' + ''.join(random.choice(letters) for i in range(5))
+    file_list[10] = file_list[10] + "Dataset: {name} Shape: {shape} Size of dataset: {size}. {p_key}".format(
+        name=name,
+        shape=str(df.shape),
+        size=str(df.size),
+        p_key = p_key
+    )
+    
+    file_list[14] = file_list[14] + '\n'+ str(df.describe().T)
+    with open(path_to_save, 'w') as f:
+        for line in file_list:
+            f.write(f"{line}\n")
+    return 'Datacard created at location: {loc}'.format(loc=path_to_save)
 
-        df: Dataframe
+def version(df, file_name, folder_path=None, unique_identifier=None):
+    '''
+    Version function to version small to medium datasets locally. 
+    
+    df: Pandas dataframe to version locally
+    
+    file_name: Name of the data file
+    
+    folder_path: Path of the local repository
+    
+    User can version the dataset(df) with a filename(file_name) under a initialized repo(folder_path).
+    Version function generates hash for dataset.describe method and uses it to distinguish between different datasets.
+    
+    file_name is used to distinguish between different types of datasets instead of different versions.
+    
+    Function generates an empty hash txt file along with the copy of dataset named 
+    'WOM'+last_8_hash_keys+_latest(identifier of the latest file in sequence)  
+    
+    e.g: version(df.head(10), file_name='dataset_name', folder_path = '../local_repo_user')
+    
+    Returns:
+    
+    DIR_NAME: ../local_repo_user/local_repo/dataset_name/WOMe65329e0.csv
+    HASH_KEY: d6c6d0409cdbf3bed8a255fde92fc8f1e65329e0'
+    
+    Current_status:
+    Versions dataframe in CSV format only.
+    
+    '''
+    
+    df_describe_str = str(df.describe)
+    hash_ = hashlib.sha1(df_describe_str.encode('utf-8'))
+    
+    if folder_path == None:
+        dr = os.getcwd() + '/' + 'local_repo' + '/' + file_name 
+    else:
+        dr = folder_path + '/' + 'local_repo' + '/' + file_name
+    
+    if not os.path.exists(dr):
+        os.makedirs(dr)
+    
+    if unique_identifier !=None:
+        unique_identifier = unique_identifier
+    else:
+        unique_identifier = ''
+    
+    letters = string.ascii_lowercase
+    name = 'WOM'+ hash_.hexdigest()[32:41] +'_'+ unique_identifier + '_latest' + '.csv'
+    name_txt_path = dr + '/'+ hash_.hexdigest() + '.txt'
+    
+    files = os.listdir(path=dr)
+    if len(files) != 0:
+        for i in files:
+            if i[-3:] == 'csv' and '_latest' in i:
+                new_name=i.replace('_latest','')
+                if new_name in files:
+                    os.replace(src=dr+'/'+i, dst=dr+'/'+new_name)
+                else:
+                    os.rename(src=dr+'/'+i, dst=dr+'/'+new_name)
+            else:
+                pass
+    else:
+        pass
+    
+    with open(name_txt_path, 'w') as fp:
+        pass
+    
+    df.to_csv(path_or_buf=dr+'/'+name)
+    print('DIR_NAME: ' + dr+'/'+name)
+    
+    return 'HASH_KEY: '+ hash_.hexdigest()
 
-        path_to_save: path to save the schema results in csv format;
+def generate_report(df, path_to_save='Data_Profile_Report.html', pdf=False):
+    '''
+    generate_report function generates the report of an dataframe using ydata profiling capabilities 
+    and stores it at path_to_save location.
+    
+    
+    df: Pandas dataframe
+    
+    path_to_save: user specific location of the report 
+    
+    pdf: Generates PDF of the report.
+    Type: Boolean True or False
+    
+    e.g: generate_report(df=df.head(10), path_to_save='../Data_Profile_Report.html', pdf=True)
+    
+    Note: Report can be saved in HTML,JSON and PDF format only.
+    '''
+    
+    profile = ProfileReport(df=df, minimal=True)
+    profile.to_file(path_to_save)
+    
+    if pdf==True:
+        path = os.path.abspath(path_to_save)
+        converter.convert(source=path, target=path_to_save[:-4]+'pdf', power=4 )
+    else:
+        pass
+    
+    return 'Report is saved at location:-' + path_to_save
 
-        show: To show the schema on stdout.
 
-        e.g: schema(df,path_to_save='schema.csv', show=0)
-        '''
-    
-        textStream = StringIO()
-        df.info(show_counts=False, memory_usage=False, buf=textStream)
-        lst =textStream.getvalue()
-        #removing unnecessary info
-        trim_list = lst.split()[19:]
-        dump = []
-        for i in range(0,len(trim_list)-3, 3):
-            dump.append(trim_list[i] + ',' + trim_list[i+1] + ',' +  trim_list[i+2])
-        if path_to_save != None:
-            np.savetxt(path_to_save, dump, delimiter=",",fmt='%s')
-        else:
-            pass
-        if show==True:
-            df.info()
-        else:
-            pass
-        
-    def datacard(df, path_to_save='Datacard_user.txt'):
-        '''
-        Function to create datacard of a dataset
-        
-        df: pandas dataframe for which user wants to generate a data card
-        
-        path_to_save: user-specific location of data card txt file. 
-                    Defaulted to current working directory.
-        
-        e.g: datacard(df, './DataCard.txt')
-        '''
-        with open("DataCard.txt", "r+") as f:
-            old = f.read()
-        file_list = old.strip().split('\n')
-        dt = datetime.now()
-        file_list[2] = file_list[2] + str(dt)
-        file_list[4] = file_list[4] + os.getlogin()
-        arr = []
-        for i in df.columns:
-            x = df.shape[0]
-            l = df[i].drop_duplicates().shape[0]
-            if x == l:
-                arr.append(i)
-            else:
-                2
-        if len(arr) == 0:
-            p_key = "No primary key found"
-        else:
-            p_key = "Primary keys found: {arr}".format(arr=arr)
-        letters = string.ascii_lowercase
-        name = 'WOM' + ''.join(random.choice(letters) for i in range(5))
-        file_list[10] = file_list[10] + "Dataset: {name} Shape: {shape} Size of dataset: {size}. {p_key}".format(
-            name=name,
-            shape=str(df.shape),
-            size=str(df.size),
-            p_key = p_key
-        )
-        
-        file_list[14] = file_list[14] + '\n'+ str(df.describe().T)
-        with open(path_to_save, 'w') as f:
-            for line in file_list:
-                f.write(f"{line}\n")
-        return 'Datacard created at location: {loc}'.format(loc=path_to_save)
-
-    def version(df, file_name, folder_path=None, unique_identifier=None):
-        '''
-        Version function to version small to medium datasets locally. 
-        
-        df: Pandas dataframe to version locally
-        
-        file_name: Name of the data file
-        
-        folder_path: Path of the local repository
-        
-        User can version the dataset(df) with a filename(file_name) under a initialized repo(folder_path).
-        Version function generates hash for dataset.describe method and uses it to distinguish between different datasets.
-        
-        file_name is used to distinguish between different types of datasets instead of different versions.
-        
-        Function generates an empty hash txt file along with the copy of dataset named 
-        'WOM'+last_8_hash_keys+_latest(identifier of the latest file in sequence)  
-        
-        e.g: version(df.head(10), file_name='dataset_name', folder_path = '../local_repo_user')
-        
-        Returns:
-        
-        DIR_NAME: ../local_repo_user/local_repo/dataset_name/WOMe65329e0.csv
-        HASH_KEY: d6c6d0409cdbf3bed8a255fde92fc8f1e65329e0'
-        
-        Current_status:
-        Versions dataframe in CSV format only.
-        
-        '''
-        
-        df_describe_str = str(df.describe)
-        hash_ = hashlib.sha1(df_describe_str.encode('utf-8'))
-        
-        if folder_path == None:
-            dr = os.getcwd() + '/' + 'local_repo' + '/' + file_name 
-        else:
-            dr = folder_path + '/' + 'local_repo' + '/' + file_name
-        
-        if not os.path.exists(dr):
-            os.makedirs(dr)
-        
-        if unique_identifier !=None:
-            unique_identifier = unique_identifier
-        else:
-            unique_identifier = ''
-        
-        letters = string.ascii_lowercase
-        name = 'WOM'+ hash_.hexdigest()[32:41] +'_'+ unique_identifier + '_latest' + '.csv'
-        name_txt_path = dr + '/'+ hash_.hexdigest() + '.txt'
-        
-        files = os.listdir(path=dr)
-        if len(files) != 0:
-            for i in files:
-                if i[-3:] == 'csv' and '_latest' in i:
-                    new_name=i.replace('_latest','')
-                    if new_name in files:
-                        os.replace(src=dr+'/'+i, dst=dr+'/'+new_name)
-                    else:
-                        os.rename(src=dr+'/'+i, dst=dr+'/'+new_name)
-                else:
-                    pass
-        else:
-            pass
-        
-        with open(name_txt_path, 'w') as fp:
-            pass
-        
-        df.to_csv(path_or_buf=dr+'/'+name)
-        print('DIR_NAME: ' + dr+'/'+name)
-        
-        return 'HASH_KEY: '+ hash_.hexdigest()
-
-    def generate_report(df, path_to_save='Data_Profile_Report.html', pdf=False):
-        '''
-        generate_report function generates the report of an dataframe using ydata profiling capabilities 
-        and stores it at path_to_save location.
-        
-        
-        df: Pandas dataframe
-        
-        path_to_save: user specific location of the report 
-        
-        pdf: Generates PDF of the report.
-        Type: Boolean True or False
-        
-        e.g: generate_report(df=df.head(10), path_to_save='../Data_Profile_Report.html', pdf=True)
-        
-        Note: Report can be saved in HTML,JSON and PDF format only.
-        '''
-        
-        profile = ProfileReport(df=df, minimal=True)
-        profile.to_file(path_to_save)
-        
-        if pdf==True:
-            path = os.path.abspath(path_to_save)
-            converter.convert(source=path, target=path_to_save[:-4]+'pdf', power=4 )
-        else:
-            pass
-        
-        return 'Report is saved at location:-' + path_to_save
```

