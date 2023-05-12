# Comparing `tmp/cnki_html2json-0.1.8.tar.gz` & `tmp/cnki_html2json-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.1.8.tar", last modified: Mon May  8 08:03:51 2023, max compression
+gzip compressed data, was "cnki_html2json-0.1.9.tar", last modified: Fri May 12 13:46:46 2023, max compression
```

## Comparing `cnki_html2json-0.1.8.tar` & `cnki_html2json-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 08:03:51.000000 cnki_html2json-0.1.8/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:03:51.173741 cnki_html2json-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/tests/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 08:03:26.000000 cnki_html2json-0.1.8/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 13:46:34.000000 cnki_html2json-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-12 13:46:34.000000 cnki_html2json-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 13:46:34.000000 cnki_html2json-0.1.9/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 13:46:46.000000 cnki_html2json-0.1.9/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:46:46.014777 cnki_html2json-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/tests/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 13:46:35.000000 cnki_html2json-0.1.9/tests/test_metadata.py
```

### Comparing `cnki_html2json-0.1.8/LICENSE` & `cnki_html2json-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.8/PKG-INFO` & `cnki_html2json-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki_html2json
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -65,17 +65,17 @@
 print(ExtractContent(raw_html).extract(mode='raw',export_path=None))
 ```
 `extract` 函数参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `raw` |
-| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为json文件 |
+| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为 `json` 文件 |
 
-> 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
+> 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据。
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
 $ cnki-crawler
 ```
 ```console
@@ -96,15 +96,15 @@
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
 | -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
 | -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下;  
+> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下；  
 > 由于提取的是文献正文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
 start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
 ```
```

### Comparing `cnki_html2json-0.1.8/README.md` & `cnki_html2json-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 print(ExtractContent(raw_html).extract(mode='raw',export_path=None))
 ```
 `extract` 函数参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `raw` |
-| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为json文件 |
+| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为 `json` 文件 |
 
-> 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
+> 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据。
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
 $ cnki-crawler
 ```
 ```console
@@ -73,15 +73,15 @@
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
 | -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
 | -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下;  
+> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下；  
 > 由于提取的是文献正文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
 start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
 ```
```

### Comparing `cnki_html2json-0.1.8/cnki_html2json/cli.py` & `cnki_html2json-0.1.9/cnki_html2json/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import argparse
 from cnki_html2json.crawl import start_crawl
 
 def main():
     parser = argparse.ArgumentParser(description='CNKI crawler. Convert the html format of papers to json format.')
     parser.add_argument('-s','--start_paper_index',type=int,default=1,help='start index, default is 1')
     parser.add_argument('-e','--end_paper_index',type=int,default=None,help='end index, default is None, which means download to the end')
-    parser.add_argument('-m','--mode',type=str,default='raw',help='mode: raw(default)|structure|plain')
-    parser.add_argument('-b','--browser_type',type=str,default='Chrome',help='browser type: Chrome(default)|Firefox|Edge')
+    parser.add_argument('-m','--mode',type=str,default='raw',choices=['raw','structure','plain'])
+    parser.add_argument('-b','--browser_type',type=str,default='Chrome',choices=['Chrome','Edge','Firefox'])
     parser.add_argument('-save','--save_path',type=str,default='dataset',help='save path, default is <dataset> folder in the current directory')
     parser.add_argument('-wait','--wait_time',type=int,default=120,help='waiting time for search, default is 120 seconds')
     parser.add_argument('-l','--log',action='store_true',help="whether to save log, specify this parameter to save log, no need to pass value")
     args = parser.parse_args()
     start_crawl(start_paper_index = args.start_paper_index,
                 end_paper_index = args.end_paper_index,
                 mode = args.mode,
```

### Comparing `cnki_html2json-0.1.8/cnki_html2json/crawl.py` & `cnki_html2json-0.1.9/cnki_html2json/crawl.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,63 +47,45 @@
     
     # 点击进入html页面
     try:
         driver.find_element(By.XPATH,f'//tbody/tr[{url_index}]/td[@class="operat"]/a[@class="icon-html"]').click()
     except:
         logger.error('论文未提供html页面')
         return concat_content(metadata,{'body_text':None,'citation':None})
-
-    # driver.execute_script("window.open('about:blank', '_blank');")
-    # 获取所有窗口的句柄
-        # handles = driver.window_handles
-        # driver.switch_to.window(handles[-1])
-    # driver.get(paper_url)
-    # time.sleep(3)
-
-    # metadata_html = driver.page_source
-    # metadata = parse_metadata.Parse(metadata_html).extract_metadata()
-    
-    # 点击进入html页面
-    # try:
-    #     driver.find_element(By.XPATH,'//*[@id="DownLoadParts"]/div[2]/ul/li[2]/a').click()
-    # except:
-    #     logger.error('论文未提供html页面')
-    #     return concat_content(metadata,{'body_text':None,'citation':None})
-    
     else:
         handles = driver.window_handles
         driver.switch_to.window(handles[-1])
         # time.sleep(10)
         # 将固定等待10s改为动态等待，直到页面加载完成
         wait = WebDriverWait(driver, 15, 1)
         wait.until(lambda driver: driver.execute_script('return document.readyState') == 'complete')
-        time.sleep(random.randint(1,5))
+        time.sleep(random.randint(3,5))
 
         # 调用判断验证码函数
         recogize_count = process_slider(driver)
         
         if recogize_count > 0:
             logger.info(f'验证码识别{recogize_count}次后通过')
 
         paper_raw_html = driver.page_source
         paper_dict = html2json.ExtractContent(paper_raw_html).extract(mode)
         driver.close() # 关闭当前窗口
         driver.switch_to.window(handles[0]) # 切换回原窗口
         
         if not paper_dict:
-            logger.error('无法解析html页面')
+            logger.error('html页面解析错误')
         return concat_content(metadata,paper_dict) # type: ignore
 
 def concat_content(metadata,paper_dict:dict)->dict:
     """将论文的元数据和正文内容合并"""
     return {**metadata,**paper_dict}
 
 def jump_page(current_page:int,start_page:int,driver):
     """
-    current_page:当前页面
+    current_page:当前页面\n
     start_page:开始下载页面
     """
     while current_page < start_page:
         if current_page == 1:
             visible_page_index = list(range(1,10))
         else:
             visible_page_elements = driver.find_elements(By.XPATH,'//div[@class="pages"]/a[position() >= 3 and position() <= last()-1]')
@@ -119,21 +101,21 @@
         else:
             driver.execute_script('window.scrollTo(0,0)')
             driver.find_element(By.XPATH,f'//a[@id="page{visible_page_index[-1]}"]').click()
             time.sleep(3)
             current_page = visible_page_index[-1]
      
 def start_crawl(start_paper_index=1,end_paper_index=None,mode='raw',browser_type='Chrome',log=True,save_path='dataset',wait_time=120):
-    """爬取cnki网站的论文
-    start_paper_index: 开始爬取的论文索引，默认为1
-    end_paper_index: 结束爬取的论文索引，默认为None，即爬取到最后
-    mode: 模式，structure|plain|raw，默认为raw
-    save_path: 下载文件的保存路径，默认为当前目录的<dataset>文件夹
-    log: 是否保存日志，默认为True
-    wait_time: 为检索预留的等待时间，单位为秒
+    """爬取cnki网站的论文\n
+    start_paper_index: 开始爬取的论文索引，默认为1\n
+    end_paper_index: 结束爬取的论文索引，默认为None，即爬取到最后\n
+    mode: 模式，structure|plain|raw，默认为raw\n
+    save_path: 下载文件的保存路径，默认为当前目录的<dataset>文件夹\n
+    log: 是否保存日志，默认为True\n
+    wait_time: 为检索预留的等待时间，单位为秒\n
     browser_type: Chrome(默认)|Firefox|Edge
     """
 
     if not os.path.exists(save_path):
         os.makedirs(save_path)
         logger.info(f'已创建{save_path}文件夹')
     else:
@@ -160,15 +142,15 @@
     if browser_type=='Chrome':
         driver = webdriver.Chrome()
     elif browser_type=='Firefox':
         driver = webdriver.Firefox()
     elif browser_type=='Edge':
         driver = webdriver.Edge()
     else:
-        raise ValueError('请选用合适的浏览器，程序已退出')
+        raise ValueError('请选用合适的浏览器类型')
 
     logger.info(f'已启动 {browser_type} 浏览器')
     driver.get('https://kns.cnki.net/kns8/AdvSearch')
     
     # 完成检索的等待时间
     time.sleep(wait_time)
     logger.info(f'请在弹出的浏览器窗口中完成检索，{wait_time}秒后将自动开始下载')
@@ -251,22 +233,13 @@
                 driver.quit()
                 sys.exit()
                 
         logger.info(f'第 {current_page} 页下载完成')
         
         # 点击下一页
         driver.find_element(By.ID,'PageNext').click()
-
-        # time.sleep(5)
-        # 关闭第一页之外的其他窗口
-        # handles = driver.window_handles
-        # for i in range(1,len(handles)):
-        #     driver.switch_to.window(handles[i])
-        #     time.sleep(1)
-        #     driver.close()
-        # driver.switch_to.window(handles[0])
         wait_seconds = random.randint(60,120)
         logger.info(f'等待 {wait_seconds} 秒')
         time.sleep(wait_seconds)
         current_page += 1
         # if current_page%100 == 0:
         #     time.sleep(300)
```

### Comparing `cnki_html2json-0.1.8/cnki_html2json/html2json.py` & `cnki_html2json-0.1.9/cnki_html2json/html2json.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,16 +165,17 @@
         folder_path = os.path.dirname(json_path)
         if not os.path.exists(folder_path):
             os.makedirs(folder_path)
         with open(json_path,'w',encoding='utf-8') as f:
             json.dump(text,f,ensure_ascii=False,indent=4)
 
     def extract(self,mode:str='raw',export_path=None):
-        """将论文的html字符串转换为字典
-        mode: 模式，structure|plain|raw，默认为raw
+        """
+        将论文的html字符串转换为字典\n
+        mode: 模式，structure|plain|raw，默认为raw\n
         export_path: 导出json文件的路径，默认为None，如果导出json文件，该参数必须指定
         """
         
         self._process_html()
         if self.error:
             return {'body_text':None,'other':None}
         self._extract_node()
```

### Comparing `cnki_html2json-0.1.8/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.1.9/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.8/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.1.9/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.8/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.1.9/cnki_html2json.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki-html2json
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -65,17 +65,17 @@
 print(ExtractContent(raw_html).extract(mode='raw',export_path=None))
 ```
 `extract` 函数参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `raw` |
-| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为json文件 |
+| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为 `json` 文件 |
 
-> 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
+> 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据。
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
 $ cnki-crawler
 ```
 ```console
@@ -96,15 +96,15 @@
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
 | -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
 | -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下;  
+> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下；  
 > 由于提取的是文献正文，1分钟大概能下载4篇文献，可以放到夜间运行 (自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
 start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
 ```
```

### Comparing `cnki_html2json-0.1.8/setup.py` & `cnki_html2json-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.8",
+    version="0.1.9",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=["cnki_html2json"],
```

### Comparing `cnki_html2json-0.1.8/tests/test_html2json.py` & `cnki_html2json-0.1.9/tests/test_html2json.py`

 * *Files identical despite different names*

