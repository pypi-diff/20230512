# Comparing `tmp/boto_addins-0.8.1.tar.gz` & `tmp/boto_addins-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/boto_addins-0.8.1.tar", last modified: Fri Jul  5 14:21:24 2019, max compression
+gzip compressed data, was "dist/boto_addins-0.9.9.tar", last modified: Wed Nov  6 23:22:01 2019, max compression
```

## Comparing `boto_addins-0.8.1.tar` & `boto_addins-0.9.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 Master     (501) staff       (20)        0 2019-07-05 14:21:24.000000 boto_addins-0.8.1/
--rw-r--r--   0 Master     (501) staff       (20)      349 2019-07-05 14:21:24.000000 boto_addins-0.8.1/PKG-INFO
-drwxr-xr-x   0 Master     (501) staff       (20)        0 2019-07-05 14:21:24.000000 boto_addins-0.8.1/boto_addins.egg-info/
--rw-r--r--   0 Master     (501) staff       (20)      349 2019-07-05 14:21:24.000000 boto_addins-0.8.1/boto_addins.egg-info/PKG-INFO
--rw-r--r--   0 Master     (501) staff       (20)      266 2019-07-05 14:21:24.000000 boto_addins-0.8.1/boto_addins.egg-info/SOURCES.txt
--rw-r--r--   0 Master     (501) staff       (20)       53 2019-07-05 14:21:24.000000 boto_addins-0.8.1/boto_addins.egg-info/requires.txt
--rw-r--r--   0 Master     (501) staff       (20)       12 2019-07-05 14:21:24.000000 boto_addins-0.8.1/boto_addins.egg-info/top_level.txt
--rw-r--r--   0 Master     (501) staff       (20)        1 2019-07-05 14:21:24.000000 boto_addins-0.8.1/boto_addins.egg-info/dependency_links.txt
-drwxr-xr-x   0 Master     (501) staff       (20)        0 2019-07-05 14:21:24.000000 boto_addins-0.8.1/boto_addins/
--rw-r--r--   0 Master     (501) staff       (20)     1494 2019-04-30 10:09:28.000000 boto_addins-0.8.1/boto_addins/sqs.py
--rw-r--r--   0 Master     (501) staff       (20)     4255 2019-04-30 10:09:28.000000 boto_addins-0.8.1/boto_addins/lambda_.py
--rw-r--r--   0 Master     (501) staff       (20)        0 2019-04-19 10:55:44.000000 boto_addins-0.8.1/boto_addins/__init__.py
--rw-r--r--   0 Master     (501) staff       (20)     9305 2019-07-05 14:18:12.000000 boto_addins-0.8.1/boto_addins/s3.py
--rwxr-xr-x   0 Master     (501) staff       (20)      558 2019-07-05 14:20:05.000000 boto_addins-0.8.1/setup.py
--rw-r--r--   0 Master     (501) staff       (20)       59 2019-07-05 14:21:24.000000 boto_addins-0.8.1/setup.cfg
+drwxr-xr-x   0 Master     (501) staff       (20)        0 2019-11-06 23:22:01.000000 boto_addins-0.9.9/
+-rw-r--r--   0 Master     (501) staff       (20)      336 2019-11-06 23:22:01.000000 boto_addins-0.9.9/PKG-INFO
+drwxr-xr-x   0 Master     (501) staff       (20)        0 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/
+-rw-r--r--   0 Master     (501) staff       (20)      336 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/PKG-INFO
+-rw-r--r--   0 Master     (501) staff       (20)      247 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/SOURCES.txt
+-rw-r--r--   0 Master     (501) staff       (20)       49 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/requires.txt
+-rw-r--r--   0 Master     (501) staff       (20)       12 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/top_level.txt
+-rw-r--r--   0 Master     (501) staff       (20)        1 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/dependency_links.txt
+drwxr-xr-x   0 Master     (501) staff       (20)        0 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins/
+-rw-r--r--   0 Master     (501) staff       (20)     4079 2019-11-06 21:39:24.000000 boto_addins-0.9.9/boto_addins/lambda_.py
+-rw-r--r--   0 Master     (501) staff       (20)        0 2019-04-19 10:55:44.000000 boto_addins-0.9.9/boto_addins/__init__.py
+-rw-r--r--   0 Master     (501) staff       (20)     9145 2019-11-06 22:48:14.000000 boto_addins-0.9.9/boto_addins/s3.py
+-rwxr-xr-x   0 Master     (501) staff       (20)      529 2019-11-06 23:20:58.000000 boto_addins-0.9.9/setup.py
+-rw-r--r--   0 Master     (501) staff       (20)       59 2019-11-06 23:22:01.000000 boto_addins-0.9.9/setup.cfg
```

### Comparing `boto_addins-0.8.1/boto_addins/lambda_.py` & `boto_addins-0.9.9/boto_addins/lambda_.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import unicode_literals
 
 import json
-
-from six.moves.urllib_parse import quote
+from urllib.parse import quote
 
 from botocore.auth import SigV4Auth
 from botocore.awsrequest import AWSRequest
-from tornado import gen
 from tornado.curl_httpclient import CurlAsyncHTTPClient
 from tornado.httpclient import HTTPRequest
 from yurl import URL
 
 
 class LambdaCallError(Exception):
     """AWS Lambda remote call exception.
@@ -43,27 +41,22 @@
          asynchronously.
 
          See http://docs.aws.amazon.com/lambda/latest/dg/API_Invoke.html
          for details.
 
         Usage example:
 
-          _ioloop = ioloop.IOLoop.instance()
-
-          @gen.coroutine
-          def async_request():
+          async def request():
             credentials = Credentials(access_key=<access_key>,
                                       secret_key=<secret_key>)
             payload = {'input_bucket': 'bucket', ...}
             service = Lambda('some-service', credentials, <region>)
-            result = yield service(payload)
-            _ioloop.stop()
+            result = await service(payload)
 
-          _ioloop.add_callback(async_request)
-          _ioloop.start()
+          ioloop.IOLoop.instance().run_sync(request)
 
         :param name: Name of the AWS Lambda function.
         :param credentials: AWS credentials.
         :param region: AWS Lambda function region.
         :param qualifier: Lambda function alias or version.
 
         """
@@ -87,16 +80,15 @@
         """Sign request to AWS with SigV4Auth."""
         aws_request = AWSRequest(method=request.method, url=request.url,
                                  data=request.body)
         signer = SigV4Auth(self._credentials, 'lambda', self.region)
         signer.add_auth(aws_request)
         request.headers.update(dict(aws_request.headers.items()))
 
-    @gen.coroutine
-    def __call__(self, payload):
+    async def __call__(self, payload):
         """Make async call to synchronously invoke AWS Lambda function with
         `payload` data.
 
         :param dict payload: Data payload for function call.
 
         :return function result in JSON.
 
@@ -107,17 +99,17 @@
         request = HTTPRequest(
             method='POST', url=self.url, headers=headers,
             # Maximum execution duration per request is 300 seconds
             request_timeout=10 * 60,
             body=json.dumps(payload)
         )
         self.__sign_request(request)
-        response = yield self.client.fetch(request)
+        response = await self.client.fetch(request)
         error = response.headers.get('X-Amz-Function-Error', None)
         body = json.loads(response.body)
         if error:
             if 'errorType' in body:
                 error = '{0} {1}'.format(error, body['errorType'])
             raise LambdaCallError(error_type=error,
                                   message=body.get('errorMessage'),
                                   trace=body.get('stackTrace'))
-        raise gen.Return(body)
+        return body
```

### Comparing `boto_addins-0.8.1/boto_addins/s3.py` & `boto_addins-0.9.9/boto_addins/s3.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import os
 import weakref
 import logging
 import xml.sax
 import socket
 from uuid import uuid4
-from six.moves.urllib_parse import quote
+import asyncio
+from urllib.parse import quote
 
 from boto.handler import XmlHandler
 from boto.s3.acl import Policy
 from boto.s3.connection import S3Connection, Bucket, Key
 from boto.utils import merge_meta
 from tornado import gen, httpclient, simple_httpclient, curl_httpclient
 
@@ -57,59 +58,57 @@
 
         async_request = httpclient.HTTPRequest(
             "{0.protocol}://{0.host}{0.path}".format(req),
             req.method, req.headers, **kwargs
         )
         return fetch_request(async_request, attempts=attempts)
 
-    def async_set_contents_from_file(self, bucket, key_name, fp, headers=None,
+    async def set_contents_from_file(self, bucket, key_name, fp, headers=None,
                                      policy=None, encrypt_key=False,
                                      metadata=None, attempts=3,
                                      request_timeout=10 * 60):
         headers = headers or {}
         if policy:
             headers[self.provider.acl_header] = policy
         if encrypt_key:
             headers[self.provider.server_side_encryption_header] = 'AES256'
         if metadata is not None:
             headers = merge_meta(headers, metadata, self.provider)
 
-        return self.generate_async_request(
+        return await self.generate_async_request(
             'PUT', bucket, key_name, headers=headers, body=fp.read(),
             request_timeout=request_timeout, attempts=attempts,
         )
 
-    @gen.coroutine
-    def async_copy_key(self, src_key, dst_key, temp_dir, metadata=None,
+    async def copy_key(self, src_key, dst_key, temp_dir, metadata=None,
                        policy=None, encrypt_key=False, headers=None,
                        request_timeout=10 * 60):
         headers = headers or {}
         if policy:
             headers[self.provider.acl_header] = policy
         if encrypt_key:
             headers[self.provider.server_side_encryption_header] = 'AES256'
         if metadata is not None:
             headers = merge_meta(headers, metadata, self.provider)
 
         url = src_key.generate_url(S3_TEMP_URL_TTL)
         destination = os.path.join(temp_dir, '_' + str(uuid4()))
-        yield async_http_download(url, destination,
-                                  request_timeout=request_timeout)
+        await http_download(url, destination,
+                            request_timeout=request_timeout)
 
-        @gen.coroutine
-        def producer(write):
+        async def producer(write):
             with open(destination, 'r') as f:
                 while True:
                     data = f.read(DATA_SIZE)
                     if not data:
                         break
-                    yield write(data)
+                    await write(data)
 
         try:
-            yield self.generate_async_request(
+            await self.generate_async_request(
                 'PUT', dst_key.bucket.name, dst_key.name,
                 headers=headers, body_producer=producer,
                 content_length=src_key.size,
                 # Timeout for whole request, not tcp.
                 request_timeout=request_timeout,
             )
         finally:
@@ -118,88 +117,84 @@
 
 
 class AsyncBucket(Bucket):
     def __init__(self, connection=None, name=None):
         self._downloading_files = weakref.WeakValueDictionary()
         super(AsyncBucket, self).__init__(connection, name, key_class=AsyncKey)
 
-    def async_get_key_contents(self, key_name, attempts=3, **kwargs):
-        return self.connection.generate_async_request(
+    async def get_key_contents(self, key_name, attempts=3, **kwargs):
+        return await self.connection.generate_async_request(
             'GET', self.name, key_name, attempts=attempts, **kwargs
         )
 
-    @gen.coroutine
-    def async_get_key(self, key_name, headers=None, version_id=None,
+    async def get_key(self, key_name, headers=None, version_id=None,
                       response_headers=None, attempts=3):
         query_args_l = []
         if version_id:
             query_args_l.append('versionId=%s' % version_id)
         if response_headers:
             for rk, rv in response_headers.items():
                 query_args_l.append('%s=%s' % (rk, quote(rv)))
 
         query_args = '&'.join(query_args_l) or None
         try:
-            response = yield self.connection.generate_async_request(
+            response = await self.connection.generate_async_request(
                 'HEAD', self.name, key_name,
                 headers=headers, query_args=query_args, attempts=attempts,
             )
         except httpclient.HTTPError as e:
             if e.code == 404:
-                raise gen.Return(False)
+                return False
             raise
         key = self.key_class(self)
         key.name = key_name
         clen = response.headers['content-length']
         key.size = int(clen) if clen else 0
-        raise gen.Return(key)
+        return key
 
-    @gen.coroutine
-    def async_get_acl(self, key_name='', headers=None, version_id=None,
+    async def get_acl(self, key_name='', headers=None, version_id=None,
                       attempts=3):
         query_args = 'acl'
         if version_id:
             query_args += '&versionId=%s' % version_id
 
-        resp = yield self.connection.generate_async_request(
+        resp = await self.connection.generate_async_request(
             'GET', self.name, key_name, query_args=query_args, headers=headers,
             attempts=attempts,
         )
 
         policy = Policy(self)
         h = XmlHandler(policy, self)
         xml.sax.parseString(resp.body, h)
-        raise gen.Return(policy)
+        return policy
 
-    @gen.coroutine
-    def async_download_key(self, key, path,
+    async def download_key(self, key, path,
                            request_timeout=10 * 60, attempts=3):
         # Get shared downloading.
         future = self._downloading_files.get(key.name)
 
         if future is None:
             url = key.generate_url(S3_TEMP_URL_TTL)
-            future = async_http_download(
+            future = asyncio.ensure_future(http_download(
                 url, path, request_timeout=request_timeout, attempts=attempts,
-            )
+            ))
 
             # Share downloading.
             self._downloading_files[key.name] = future
 
         # Run task.
-        yield future
+        await future
 
 
 class AsyncKey(Key):
-    def async_exist(self):
-        return self.bucket.async_get_key(self.name)
+    async def exist(self):
+        return await self.bucket.get_key(self.name)
 
 
-@gen.coroutine
-def fetch_request(request, client=None, retry_callback=None, attempts=1):
+async def fetch_request(request, client=None, retry_callback=None, attempts=1):
     if client is None:
         client = simple_httpclient.SimpleAsyncHTTPClient()
 
     if attempts <= 0:
         raise ValueError('attempts should be > 0')
 
     # Fail faster on connection if we can retry
@@ -207,55 +202,53 @@
 
     # Save exceptions history for further analysis
     except_history = []
 
     while attempts:
         wait_before_retry = 0
         try:
-            resp = yield client.fetch(request)
+            resp = await client.fetch(request)
         except httpclient.HTTPError as e:
             # retry on s3 errors
             if e.code == 500:
                 wait_before_retry = 0.2
             elif e.code in (503, 599):
                 wait_before_retry = 1
             else:
                 raise
             except_history.append(e)
         except socket.error as e:
             # retry
             except_history.append(e)
 
         else:
-            raise gen.Return(resp)
+            return resp
 
         attempts -= 1
         if not attempts:
             raise except_history[-1]
 
         if wait_before_retry:
-            yield gen.sleep(wait_before_retry)
+            await gen.sleep(wait_before_retry)
         if retry_callback:
-            yield retry_callback(request, attempts)
+            await retry_callback(request, attempts)
 
 
-@gen.coroutine
-def async_http_download(source, destination,
+async def http_download(source, destination,
                         request_timeout=10 * 60, attempts=3):
     tmp_name = '{}.{}'.format(destination, str(uuid4())[:8])
 
     try:
         with open(tmp_name, 'wb') as iobuffer:
 
-            @gen.coroutine
-            def reset_iobuffer(*args):
+            async def reset_iobuffer(*args):
                 iobuffer.seek(0)
                 iobuffer.truncate()
 
-            yield fetch_request(
+            await fetch_request(
                 httpclient.HTTPRequest(
                     source,
                     # Direct write to file.
                     streaming_callback=iobuffer.write,
                     # Timeout for whole request, not tcp.
                     request_timeout=request_timeout,
                 ),
```

