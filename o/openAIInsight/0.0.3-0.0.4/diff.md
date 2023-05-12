# Comparing `tmp/openAIInsight-0.0.3-py3-none-any.whl.zip` & `tmp/openAIInsight-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5222 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     9399 b- defN 23-May-12 04:50 openAIInsight/OpenAI_PineConeVector.py
+Zip file size: 5288 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     9644 b- defN 23-May-12 06:15 openAIInsight/OpenAI_PineConeVector.py
 -rw-rw-r--  2.0 unx     2200 b- defN 23-May-10 11:41 openAIInsight/__init__.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      609 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      596 b- defN 23-May-12 06:00 openAIInsight-0.0.3.dist-info/RECORD
-7 files, 13983 bytes uncompressed, 4156 bytes compressed:  70.3%
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      609 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      596 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/RECORD
+7 files, 14228 bytes uncompressed, 4222 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: openAIInsight/OpenAI_PineConeVector.py
 Comment: 
 
 Filename: openAIInsight/__init__.py
 Comment: 
 
-Filename: openAIInsight-0.0.3.dist-info/LICENCE.txt
+Filename: openAIInsight-0.0.4.dist-info/LICENCE.txt
 Comment: 
 
-Filename: openAIInsight-0.0.3.dist-info/METADATA
+Filename: openAIInsight-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: openAIInsight-0.0.3.dist-info/WHEEL
+Filename: openAIInsight-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: openAIInsight-0.0.3.dist-info/top_level.txt
+Filename: openAIInsight-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: openAIInsight-0.0.3.dist-info/RECORD
+Filename: openAIInsight-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openAIInsight/OpenAI_PineConeVector.py

```diff
@@ -1,17 +1,19 @@
 import json
 import openai
 import pinecone
+import datetime
 import traceback
 import pandas as pd
 from flask import request
 import loggerutility as logger
 import commonutility as common
 from openai.embeddings_utils import get_embedding, get_embeddings, cosine_similarity
 
+
 class OpenAI_PineConeVector:
     
     index_name      =   "" 
     openAI_apiKey   =   "" 
     pineCone_apiKey =   "" 
     queryList       =   "" 
     dfJson          =   ""
@@ -136,17 +138,19 @@
             pinecone.init(api_key=self.pineCone_apiKey, environment='us-west4-gcp')
             
             pinecone_IndexList = pinecone.list_indexes()
             
             if self.index_name in pinecone_IndexList:
                 self.my_index = pinecone.Index(index_name=self.index_name)
                 logger.log(f"self.my_index::: {self.my_index}","0")
+                logger.log(f"Pinecone execution START Time::: {datetime.datetime.now().strftime('%H:%M:%S')}","0")
                 for i in self.queryList:
                     if i != "" and i != None:
                         result.append(self.my_index.query(vector=get_embedding(i, engine=self.engineName),top_k=1, include_metadata=True))
+                logger.log(f"Pinecone execution END Time::: {datetime.datetime.now().strftime('%H:%M:%S')}","0")
                 logger.log(f"OpenAI_PineConeVector class getLookUP() Response::: \n{result}\tlen::: {len(result)}\t{type(result)}", "0")
 
                 id_list = [element["matches"][0]["id"] for element in result]
                 IdDescription_dict = dict(zip(self.queryList, id_list))
                 logger.log(f"\n\nOpenAI_PineConeVector class getLookUP() IdDescription_dict::: \n{IdDescription_dict}\tlen::: {len(IdDescription_dict)}\t{type(IdDescription_dict)}", "0")
 
                 return str(IdDescription_dict)
```

## Comparing `openAIInsight-0.0.3.dist-info/LICENCE.txt` & `openAIInsight-0.0.4.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `openAIInsight-0.0.3.dist-info/METADATA` & `openAIInsight-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openAIInsight
-Version: 0.0.3
+Version: 0.0.4
 Summary: Proteus openAI File
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

