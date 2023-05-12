# Comparing `tmp/openAIInsight-0.0.2-py3-none-any.whl.zip` & `tmp/openAIInsight-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 3247 bytes, number of entries: 6
--rw-rw-r--  2.0 unx     3838 b- defN 23-Apr-04 16:18 openAIInsight/__init__.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-04 17:04 openAIInsight-0.0.2.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      549 b- defN 23-Apr-04 17:04 openAIInsight-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 17:04 openAIInsight-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Apr-04 17:04 openAIInsight-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      501 b- defN 23-Apr-04 17:04 openAIInsight-0.0.2.dist-info/RECORD
-6 files, 6067 bytes uncompressed, 2333 bytes compressed:  61.5%
+Zip file size: 5222 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     9399 b- defN 23-May-12 04:50 openAIInsight/OpenAI_PineConeVector.py
+-rw-rw-r--  2.0 unx     2200 b- defN 23-May-10 11:41 openAIInsight/__init__.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      609 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      596 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/RECORD
+7 files, 13983 bytes uncompressed, 4156 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
+Filename: openAIInsight/OpenAI_PineConeVector.py
+Comment: 
+
 Filename: openAIInsight/__init__.py
 Comment: 
 
-Filename: openAIInsight-0.0.2.dist-info/LICENCE.txt
+Filename: openAIInsight-0.0.3.dist-info/LICENCE.txt
 Comment: 
 
-Filename: openAIInsight-0.0.2.dist-info/METADATA
+Filename: openAIInsight-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: openAIInsight-0.0.2.dist-info/WHEEL
+Filename: openAIInsight-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: openAIInsight-0.0.2.dist-info/top_level.txt
+Filename: openAIInsight-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: openAIInsight-0.0.2.dist-info/RECORD
+Filename: openAIInsight-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openAIInsight/__init__.py

```diff
@@ -3,57 +3,34 @@
 import loggerutility as logger
 
 class openAI:
     def getCompletionEndpoint(self):
         try:
             jsonData = request.get_data('jsonData', None)
             jsonData = json.loads(jsonData[9:])
-            logger.log(f"\njsonData openAI class::: {jsonData}","0")
+            logger.log(f"jsonData openAI class::: {jsonData}","0")
 
             licenseKey   = jsonData['license_key']
             insightInput = jsonData['insight_input']
             openai.api_key = licenseKey
             openAI_trainingData = open("openAI_trainingData.txt","r").read()
             
-            # response = openai.Completion.create(
-            # model="code-davinci-001",
-            # prompt= openAI_trainingData + insightInput,
-            # temperature=0.25,
-            # max_tokens=198,
-            # top_p=0.5,
-            # frequency_penalty=0,
-            # presence_penalty=0,
-            # stop=["\n"]
-            # )
-
-            # logger.log(f"Response openAI completion endpoint::::: {response}","0")
-            # finalResult=str(response["choices"][0]["text"])
-            # logger.log(f"OpenAI completion endpoint finalResult ::::: {finalResult}","0")
-            # return finalResult
-        
-            logger.log(f"\n\nopenAI_trainingData before conversion :::::: {type(openAI_trainingData)} \n{openAI_trainingData}","0")
-            openAI_trainingData = openAI_trainingData.replace("<insight_input>", insightInput)
-            logger.log(f"\n\nopenAI_trainingData after replacing <insight_input> :::::: \n{openAI_trainingData} \n{type(openAI_trainingData)}","0")
-            messageList = json.loads(openAI_trainingData)
-            logger.log(f"\n\nmessageList after conversion :::::: {messageList} \n{type(messageList)}","0")
-            
-            logger.log(f"\n\nfinal messageList :::::: {messageList}","0")
-
-            response = openai.ChatCompletion.create(
-                                                        model="gpt-3.5-turbo",
-                                                        messages= messageList,
-                                                        temperature=0.25,
-                                                        max_tokens=350,
-                                                        top_p=0.5,
-                                                        frequency_penalty=0,
-                                                        presence_penalty=0,
-                                                        )
-            logger.log(f"\n\nResponse openAI ChatCompletion endpoint::::: {response} \n{type(response)}","0")
-            finalResult=str(response["choices"][0]["message"]["content"])
-            logger.log(f"\n\nOpenAI ChatCompletion endpoint finalResult ::::: {finalResult} \n{type(finalResult)}","0")
+            response = openai.Completion.create(
+            model="code-davinci-001",
+            prompt= openAI_trainingData + insightInput,
+            temperature=0.25,
+            max_tokens=198,
+            top_p=0.5,
+            frequency_penalty=0,
+            presence_penalty=0,
+            stop=["\n"]
+            )
+            logger.log(f"Response openAI completion endpoint::::: {response}","0")
+            finalResult=str(response["choices"][0]["text"])
+            logger.log(f"OpenAI completion endpoint finalResult ::::: {finalResult}","0")
             return finalResult
         
         except Exception as e:
             logger.log(f'\n In getCompletionEndpoint exception stacktrace : ', "1")
             trace = traceback.format_exc()
             descr = str(e)
             returnErr = self.getErrorXml(descr, trace)
```

## Comparing `openAIInsight-0.0.2.dist-info/LICENCE.txt` & `openAIInsight-0.0.3.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `openAIInsight-0.0.2.dist-info/METADATA` & `openAIInsight-0.0.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: openAIInsight
-Version: 0.0.2
+Version: 0.0.3
 Summary: Proteus openAI File
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENCE.txt
 Requires-Dist: openai
+Requires-Dist: commonutility
+Requires-Dist: pinecone-client
 
 Proteus openAI File
```

