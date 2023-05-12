# Comparing `tmp/sosin-1.1.1.tar.gz` & `tmp/sosin-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.1.1.tar", last modified: Thu May 11 05:23:12 2023, max compression
+gzip compressed data, was "sosin-1.1.2.tar", last modified: Fri May 12 11:31:14 2023, max compression
```

## Comparing `sosin-1.1.1.tar` & `sosin-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.531532 sosin-1.1.1/
--rwx------   0 sosin      (501) staff       (20)     1083 2023-04-17 11:46:46.000000 sosin-1.1.1/LICENSE
--rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-05-11 05:23:12.531263 sosin-1.1.1/PKG-INFO
--rwx------   0 sosin      (501) staff       (20)      863 2023-04-17 11:46:46.000000 sosin-1.1.1/README.md
--rw-r--r--   0 sosin      (501) staff       (20)       38 2023-05-11 05:23:12.531632 sosin-1.1.1/setup.cfg
--rwx------   0 sosin      (501) staff       (20)      994 2023-05-11 05:22:59.000000 sosin-1.1.1/setup.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.527333 sosin-1.1.1/sosin/
--rwx------   0 sosin      (501) staff       (20)        0 2023-04-17 12:05:52.000000 sosin-1.1.1/sosin/__init__.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.528392 sosin-1.1.1/sosin/databases/
--rwx------   0 sosin      (501) staff       (20)     4934 2023-04-24 10:38:48.000000 sosin-1.1.1/sosin/databases/fs.py
--rwx------   0 sosin      (501) staff       (20)     9667 2023-05-10 06:56:55.000000 sosin-1.1.1/sosin/databases/rdb.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.528710 sosin-1.1.1/sosin/rpa/
--rwx------   0 sosin      (501) staff       (20)    10828 2023-04-22 13:06:11.000000 sosin-1.1.1/sosin/rpa/email_mgr.py
--rwx------   0 sosin      (501) staff       (20)     3698 2023-05-10 06:56:55.000000 sosin-1.1.1/sosin/rpa/sms_mgr.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.529657 sosin-1.1.1/sosin/utils/
--rwx------   0 sosin      (501) staff       (20)     1687 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/utils/currency.py
--rwx------   0 sosin      (501) staff       (20)      304 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/utils/log.py
--rwx------   0 sosin      (501) staff       (20)      527 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/utils/progress.py
--rwx------   0 sosin      (501) staff       (20)      385 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/utils/secret.py
--rwx------   0 sosin      (501) staff       (20)      885 2023-05-10 06:56:55.000000 sosin-1.1.1/sosin/utils/zip.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.530614 sosin-1.1.1/sosin/web/
--rwx------   0 sosin      (501) staff       (20)     1055 2023-04-18 14:49:45.000000 sosin-1.1.1/sosin/web/content.py
--rwx------   0 sosin      (501) staff       (20)     5506 2023-05-10 10:02:28.000000 sosin-1.1.1/sosin/web/session.py
--rwx------   0 sosin      (501) staff       (20)     1018 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/web/translate.py
--rwx------   0 sosin      (501) staff       (20)     4796 2023-04-24 07:25:27.000000 sosin-1.1.1/sosin/web/virtual.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.528072 sosin-1.1.1/sosin.egg-info/
--rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/PKG-INFO
--rw-r--r--   0 sosin      (501) staff       (20)      471 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/SOURCES.txt
--rw-r--r--   0 sosin      (501) staff       (20)        1 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/dependency_links.txt
--rw-r--r--   0 sosin      (501) staff       (20)       32 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/requires.txt
--rw-r--r--   0 sosin      (501) staff       (20)        6 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:14.838907 sosin-1.1.2/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-05-12 11:31:14.838399 sosin-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 11:31:14.838907 sosin-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      966 2023-05-12 11:29:54.000000 sosin-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:14.798325 sosin-1.1.2/sosin/
+-rw-rw-rw-   0        0        0       23 2023-05-12 11:29:34.000000 sosin-1.1.2/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:14.824183 sosin-1.1.2/sosin/databases/
+-rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.1.2/sosin/databases/fs.py
+-rw-rw-rw-   0        0        0     9763 2023-05-12 11:29:34.000000 sosin-1.1.2/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:14.826691 sosin-1.1.2/sosin/rpa/
+-rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.1.2/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3698 2023-05-10 06:56:55.000000 sosin-1.1.2/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:14.832253 sosin-1.1.2/sosin/utils/
+-rw-rw-rw-   0        0        0     1797 2023-05-12 11:29:34.000000 sosin-1.1.2/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.1.2/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.1.2/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.1.2/sosin/utils/secret.py
+-rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.1.2/sosin/utils/zip.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:14.837391 sosin-1.1.2/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.1.2/sosin/web/content.py
+-rw-rw-rw-   0        0        0     5505 2023-05-12 11:29:29.000000 sosin-1.1.2/sosin/web/session.py
+-rw-rw-rw-   0        0        0     1051 2023-05-12 11:29:34.000000 sosin-1.1.2/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4414 2023-05-12 11:29:34.000000 sosin-1.1.2/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:14.821726 sosin-1.1.2/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-05-12 11:31:14.000000 sosin-1.1.2/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-05-12 11:31:14.000000 sosin-1.1.2/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 11:31:14.000000 sosin-1.1.2/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-12 11:31:14.000000 sosin-1.1.2/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-12 11:31:14.000000 sosin-1.1.2/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.1.1/LICENSE` & `sosin-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.1.1/README.md` & `sosin-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.1.1/sosin/databases/fs.py` & `sosin-1.1.2/sosin/databases/fs.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.1/sosin/databases/rdb.py` & `sosin-1.1.2/sosin/databases/rdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import pymysql
+try:
+    import pymysql
+except:
+    print('you need to install pymysql\n$ : python -m pip install pymysql')
 import traceback
 
 from typing import Iterable, Union
 
 class MariaDB:
     """
     MariaDB
```

### Comparing `sosin-1.1.1/sosin/rpa/email_mgr.py` & `sosin-1.1.2/sosin/rpa/email_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.1/sosin/rpa/sms_mgr.py` & `sosin-1.1.2/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.1/sosin/utils/currency.py` & `sosin-1.1.2/sosin/utils/currency.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import requests
-from bs4 import BeautifulSoup
+try:
+    from bs4 import BeautifulSoup
+except:
+    print('you need to install BeautifulSoup4\n$ : python -m pip install BeautifulSoup4')
 
 country_list = [
     '미국', '유럽연합', '일본', '중국', '홍콩', '대만', '영국', '오만', '캐나다', 
     '스위스', '스웨덴', '호주', '뉴질랜드', '체코', '칠레', '터키', '몽골', '이스라엘', 
     '덴마크', '노르웨이', '사우디아라비아', '쿠웨이트', '바레인', '아랍에미리트', '요르단', 
     '이집트', '태국', '싱가포르', '말레이시아', '인도네시아', '카타르', '카자흐스탄', '브루나이', 
     '인도', '파키스탄', '방글라데시', '필리핀', '멕시코', '브라질', '베트남', '남아프리카',
```

### Comparing `sosin-1.1.1/sosin/utils/progress.py` & `sosin-1.1.2/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.1/sosin/utils/zip.py` & `sosin-1.1.2/sosin/utils/zip.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.1/sosin/web/content.py` & `sosin-1.1.2/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.1/sosin/web/session.py` & `sosin-1.1.2/sosin/web/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
     Session Manager
     """
 
     history:list[requests.Response] = []
 
     def __init__(self, cookie_path:str='./cookie', history_mode:bool=False) -> None:
         self._headers = { 'User-Agent': 'Mozilla/5.0' }
-        self._cookies = {}
         self._cookie_path = cookie_path
         self._mode = history_mode
         
         try:
             open(cookie_path, 'r')
             self._load_cookies()
-        except: pass
+        except:
+            self._cookies = {}
 
     def __del__(self):
         self._save_cookies()
     
     # ------------------------------------------------------------------------
     # Request Management
     def get(self, url:str, headers:dict={}, cookies:dict={}, **kwargs) -> requests.Response:
```

### Comparing `sosin-1.1.1/sosin/web/translate.py` & `sosin-1.1.2/sosin/web/translate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import time
-
-from sosin.web.virtual import VirtualDriver, By, WebDriverWait, EC
+try:
+    from sosin.web.virtual import VirtualDriver, By, WebDriverWait, EC
+except:
+    pass
 
 def papago(txts:list[str]) -> list[str]:
+    
     """
     파파고 번역기
     """
     webdriver = VirtualDriver()
     webdriver.set_argument()
     driver = webdriver.get_driver()
     driver.execute_script("window.open('https://papago.naver.com/')")
```

### Comparing `sosin-1.1.1/sosin/web/virtual.py` & `sosin-1.1.2/sosin/web/virtual.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# python -m pip install selenium
-# python -m pip install webdriver-manager
-
 # ---------------------------------------------------------------------------------------------
 # Selnium Setting
 try:
     from selenium import webdriver
     from selenium.webdriver.chrome.service import Service
     from webdriver_manager.chrome import ChromeDriverManager
 except:
-    raise ImportError('you need to install selenium, webdriver-manager\n$ : python -m pip install selenium\n$ : python -m pip install webdriver-manager')
+    print('you need to install selenium, webdriver-manager\n$ : python -m pip install selenium webdriver-manager')
 
 class VirtualDriver:
     """
     Selenium VirtualDriver
     """
     def __init__(self, engine='chrome') -> None:
+
         self.engine = engine.lower().strip()
         if self.engine  == 'chrome':
             self.options = webdriver.ChromeOptions()
         
     def set_argument(self, headless=True, linux=True, maximize=True, 
                         user_agent=False, lang_kr=False, secret_mode=False, download_path=None):
         """
@@ -80,58 +78,45 @@
             driver.maximize_window()
             driver.implicitly_wait(5)
             return driver
 
 
 # ---------------------------------------------------------------------------------------------
 # Selenium Utils
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.common.alert import Alert
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
+try:
+    from selenium.webdriver.common.by import By
+    from selenium.webdriver.common.keys import Keys
+    from selenium.webdriver.common.alert import Alert
+    from selenium.webdriver.support.ui import WebDriverWait
+    from selenium.webdriver.support import expected_conditions as EC
+except: pass
 
 import time
 
 MAX_RETRY_COUNT = 5
 def click_alert(d):
     """
-    알림창 처리
+    alert
     """
-    retry = 0
-    while True:
+    for _ in range(MAX_RETRY_COUNT):
         try:
             Alert(d).accept()
             break
-        except:
-            time.sleep(1)
-            retry+=1
-
-        if retry == MAX_RETRY_COUNT:
-            # 에러 발생
-            assert False, '알림창 클릭 실패 !!'
+        except: time.sleep(1)
+    else: assert False, 'fail, alert not found'
 
-# WebDriver 클래스로 webdriver 객체를 생성했다고 가정
 if __name__ == '__main__':
-    # 1. 예외처리문 활용
+    # 1. try-except
     try:
-        driver = webdriver.get_driver()
-
-        """
-        Code Blocks
-        """
+        driver = VirtualDriver().get_driver()
     except Exception as e:
         print(e)
     finally:
         driver.quit()
 
-    # 2. 클래스의 생성자, 소멸자 활용
+    # 2. class
     class MyWeb:
         def __init__(self):
-            self.driver = webdriver.get_driver()
+            self.driver = VirtualDriver().get_driver()
             
         def __del__(self):
             self.driver.quit()
-
-    """
-    Code Blocks
-    """
```

