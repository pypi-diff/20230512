# Comparing `tmp/smartis_sdk-0.2.0.tar.gz` & `tmp/smartis_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartis_sdk-0.2.0.tar", max compression
+gzip compressed data, was "smartis_sdk-0.3.0.tar", max compression
```

## Comparing `smartis_sdk-0.2.0.tar` & `smartis_sdk-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-05-11 10:40:57.750065 smartis_sdk-0.2.0/LICENSE
--rw-r--r--   0        0        0       27 2023-05-11 10:42:26.070440 smartis_sdk-0.2.0/README.md
--rw-r--r--   0        0        0     1199 2023-05-12 02:25:16.269680 smartis_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      385 2023-05-12 02:24:39.116163 smartis_sdk-0.2.0/src/smartis_sdk/__init__.py
--rw-r--r--   0        0        0     5899 2023-05-11 15:55:02.746357 smartis_sdk-0.2.0/src/smartis_sdk/client.py
--rw-r--r--   0        0        0     1303 2023-05-11 11:59:04.485496 smartis_sdk-0.2.0/src/smartis_sdk/common.py
--rw-r--r--   0        0        0     3135 2023-05-12 02:22:17.878788 smartis_sdk-0.2.0/src/smartis_sdk/entity.py
--rw-r--r--   0        0        0      169 2023-05-11 08:47:15.864966 smartis_sdk-0.2.0/src/smartis_sdk/utils.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 smartis_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-11 10:40:57.750065 smartis_sdk-0.3.0/LICENSE
+-rw-r--r--   0        0        0       27 2023-05-11 10:42:26.070440 smartis_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0     1199 2023-05-12 10:53:50.294013 smartis_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      385 2023-05-12 02:24:39.116163 smartis_sdk-0.3.0/src/smartis_sdk/__init__.py
+-rw-r--r--   0        0        0     6123 2023-05-12 10:50:38.623181 smartis_sdk-0.3.0/src/smartis_sdk/client.py
+-rw-r--r--   0        0        0     1303 2023-05-11 11:59:04.485496 smartis_sdk-0.3.0/src/smartis_sdk/common.py
+-rw-r--r--   0        0        0     3135 2023-05-12 02:22:17.878788 smartis_sdk-0.3.0/src/smartis_sdk/entity.py
+-rw-r--r--   0        0        0      279 2023-05-12 08:01:58.268061 smartis_sdk-0.3.0/src/smartis_sdk/errors.py
+-rw-r--r--   0        0        0      169 2023-05-11 08:47:15.864966 smartis_sdk-0.3.0/src/smartis_sdk/utils.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 smartis_sdk-0.3.0/PKG-INFO
```

### Comparing `smartis_sdk-0.2.0/LICENSE` & `smartis_sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.2.0/pyproject.toml` & `smartis_sdk-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartis_sdk"
-version = "0.2.0"
+version = "0.3.0"
 description = "SDK для Smartis API"
 license = "MIT"
 authors = ["viktor <vi.dave@yandex.ru>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `smartis_sdk-0.2.0/src/smartis_sdk/client.py` & `smartis_sdk-0.3.0/src/smartis_sdk/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pydantic import ValidationError, BaseModel
 
 from .entity import Ads, Ad, Payload
 from .entity import Campaigns, Campaign
 from .entity import Channels, Placements
 from .entity import Keywords, Keyword
 from .common import Method
+from .errors import ApiLimitError
 import logging
 
 
 class ContentType(Enum):
     application = "application/json"
 
 
@@ -86,52 +87,59 @@
         all_keywords: list[Keyword] = []
         items: Keywords = self._get_entity(keywords_ids, Method.get_keywords, Keywords)
         all_keywords.extend(items.keywords)
         return all_keywords
 
     def status_code_handler(self, response: requests.Response, retry: int) -> None:
         """Обработка статус кодов"""
-        if response.status_code == 429:
-            if int(response.headers['X-Ratelimit-Remaining']) == 0:
+
+        match response.status_code:
+            case 200:
+                return
+            case 400 | 403:
+                resp_body: dict = response.json()
+                message = resp_body.get("error")
+                raise ConnectionError(f"{response.status_code}:{response.text}. details: {message}")
+            case 429:
+                if int(response.headers['X-Ratelimit-Remaining']) == 0:
+                    logging.warning(f"Status code: {response.status_code}. "
+                                    f"Причина: {response.reason}. "
+                                    f"Пауза: {response.headers['Retry-After']} с.")
+                    raise ApiLimitError(int(response.headers['Retry-After']), response.text)
+            case 500 | 502:
                 logging.warning(f"Status code: {response.status_code}. "
                                 f"Причина: {response.reason}. "
-                                f"Пауза: {response.headers['Retry-After']} с.")
-                time.sleep(int(response.headers['Retry-After']))
-                logging.info(f"Повтор запроса: {(self.TRY_REQUEST - retry + 1)}"
-                             f"/{self.TRY_REQUEST}")
-        elif response.status_code in {500, 502}:
-            logging.warning(f"Status code: {response.status_code}. "
-                            f"Причина: {response.reason}. "
-                            f"Пауза: 60 с.")
-            time.sleep(60)
-        elif response.status_code != 200:
-            logging.critical(f" Необработанное исключение. "
-                             f"Status code: {response.status_code}. "
-                             f"Причина: {response.reason}. ")
-            logging.info(response.headers)
-            time.sleep(60)
+                                f"Пауза: 60 с.")
+                time.sleep(60)
+            case _:
+                logging.warning(f" Необработанное исключение. "
+                                f"Status code: {response.status_code}. "
+                                f"Причина: {response.reason}. ")
+                logging.info(response.headers)
+                time.sleep(60)
 
     def get_report(self, payload: Payload, retry: int = TRY_REQUEST) -> requests.Response:
         """Выполнение запросов с обработкой ошибок"""
         payload_json = payload.to_json()
         try:
             time.sleep(self.REQUEST_PAUSE)
             answer = requests.post(f"{self.host}reports/getReport", headers=self.header, data=payload_json)
             self.status_code_handler(answer, self.TRY_REQUEST)
+        except ApiLimitError as apiErr:
+            if retry == 0:
+                return self.retry_get_report(payload)
+            logging.warning(f"error: {apiErr.message}")
+            logging.info(f"Повтор запроса: {self.TRY_REQUEST - retry + 1}/{self.TRY_REQUEST}")
+            return self.get_report(payload, retry=retry - 1)
         except Exception as er:
-            if retry != 0:
-                logging.warning(f"Необработанное исключение. error: {er}")
-                logging.info(f"Повтор запроса: {self.TRY_REQUEST - retry + 1}/{self.TRY_REQUEST}")
-                return self.get_report(payload, retry=retry - 1)
-            else:
-                logging.info("Количество ошибок больше заданного! Пауза 10 мин")
-                time.sleep(self.FORCE_PAUSE)
-                return self.get_report(payload)
+            if retry == 0:
+                return self.retry_get_report(payload)
+            logging.warning(f"Необработанное исключение. error: {er}")
+            logging.info(f"Повтор запроса: {self.TRY_REQUEST - retry + 1}/{self.TRY_REQUEST}")
+            return self.get_report(payload, retry=retry - 1)
         else:
-            if answer.status_code == 200:
-                return answer
-            if retry:
-                return self.get_report(payload, retry=(retry - 1))
-            logging.warning(f"Количество ошибок подряд достигло {self.TRY_REQUEST}, "
-                            f"пауза {self.FORCE_PAUSE / 60} минут")
-            time.sleep(self.FORCE_PAUSE)
-            self.get_report(payload)
+            return answer
+
+    def retry_get_report(self, payload: Payload) -> requests.Response:
+        logging.info("Количество ошибок больше заданного! Пауза 10 мин")
+        time.sleep(self.FORCE_PAUSE)
+        return self.get_report(payload)
```

### Comparing `smartis_sdk-0.2.0/src/smartis_sdk/common.py` & `smartis_sdk-0.3.0/src/smartis_sdk/common.py`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.2.0/src/smartis_sdk/entity.py` & `smartis_sdk-0.3.0/src/smartis_sdk/entity.py`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.2.0/PKG-INFO` & `smartis_sdk-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartis-sdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: SDK для Smartis API
 License: MIT
 Author: viktor
 Author-email: vi.dave@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

