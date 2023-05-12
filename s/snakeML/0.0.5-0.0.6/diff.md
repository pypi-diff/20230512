# Comparing `tmp/snakeML-0.0.5-py3-none-any.whl.zip` & `tmp/snakeML-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 6523 bytes, number of entries: 15
+Zip file size: 8155 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      167 b- defN 23-Mar-20 22:19 snakeML/__init__.py
--rw-r--r--  2.0 unx     2162 b- defN 23-May-11 17:49 snakeML/density_estimation.py
--rw-r--r--  2.0 unx     1591 b- defN 23-May-11 17:49 snakeML/dimensionality_reduction.py
+-rw-r--r--  2.0 unx     2162 b- defN 23-May-12 17:28 snakeML/density_estimation.py
+-rw-r--r--  2.0 unx     1670 b- defN 23-May-12 16:21 snakeML/dimensionality_reduction.py
 -rw-r--r--  2.0 unx       93 b- defN 23-Mar-17 14:36 snakeML/dist.py
--rw-r--r--  2.0 unx       93 b- defN 23-May-11 17:47 snakeML/distance.py
--rw-r--r--  2.0 unx     1646 b- defN 23-May-11 17:49 snakeML/loads.py
--rw-r--r--  2.0 unx      756 b- defN 23-May-11 17:47 snakeML/numpy_transformations.py
--rw-r--r--  2.0 unx      410 b- defN 23-May-11 17:47 snakeML/preprocessing.py
+-rw-r--r--  2.0 unx      181 b- defN 23-May-11 20:35 snakeML/distance.py
+-rw-r--r--  2.0 unx     5328 b- defN 23-May-12 17:35 snakeML/gaussian.py
+-rw-r--r--  2.0 unx     2351 b- defN 23-May-12 17:29 snakeML/loads.py
+-rw-r--r--  2.0 unx      756 b- defN 23-May-11 20:35 snakeML/numpy_transformations.py
+-rw-r--r--  2.0 unx      410 b- defN 23-May-11 20:35 snakeML/preprocessing.py
 -rw-r--r--  2.0 unx      571 b- defN 23-Mar-17 14:29 snakeML/test.py
--rw-r--r--  2.0 unx      547 b- defN 23-May-11 17:47 snakeML/validation.py
--rw-r--r--  2.0 unx     2450 b- defN 23-May-11 17:49 snakeML/visualization.py
--rw-r--r--  2.0 unx      581 b- defN 23-May-11 17:50 snakeML-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 17:50 snakeML-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-11 17:50 snakeML-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1163 b- defN 23-May-11 17:50 snakeML-0.0.5.dist-info/RECORD
-15 files, 12330 bytes uncompressed, 4607 bytes compressed:  62.6%
+-rw-r--r--  2.0 unx      547 b- defN 23-May-11 20:35 snakeML/validation.py
+-rw-r--r--  2.0 unx     3286 b- defN 23-May-11 21:30 snakeML/visualization.py
+-rw-r--r--  2.0 unx      581 b- defN 23-May-12 17:39 snakeML-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 17:39 snakeML-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-12 17:39 snakeML-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1240 b- defN 23-May-12 17:39 snakeML-0.0.6.dist-info/RECORD
+16 files, 19443 bytes uncompressed, 6125 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: snakeML/dist.py
 Comment: 
 
 Filename: snakeML/distance.py
 Comment: 
 
+Filename: snakeML/gaussian.py
+Comment: 
+
 Filename: snakeML/loads.py
 Comment: 
 
 Filename: snakeML/numpy_transformations.py
 Comment: 
 
 Filename: snakeML/preprocessing.py
@@ -27,20 +30,20 @@
 
 Filename: snakeML/validation.py
 Comment: 
 
 Filename: snakeML/visualization.py
 Comment: 
 
-Filename: snakeML-0.0.5.dist-info/METADATA
+Filename: snakeML-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: snakeML-0.0.5.dist-info/WHEEL
+Filename: snakeML-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: snakeML-0.0.5.dist-info/top_level.txt
+Filename: snakeML-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: snakeML-0.0.5.dist-info/RECORD
+Filename: snakeML-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## snakeML/density_estimation.py

```diff
@@ -1,11 +1,11 @@
 import numpy
 import matplotlib.pyplot as plt
 import math
-from snakeML.numpy_transformations import mcol, mrow, mean_cov
+from testlib.numpy_transformations import mcol, mrow, mean_cov
 
 def logpdf_GAU_ND_unoptimized(x, mu, C):
     C_inv=numpy.linalg.inv(C)
     det = numpy.linalg.slogdet(C)[1]
     M=x.shape[0]
     log_pi=math.log(2*math.pi)
     ab=(-M*log_pi-det)/2
```

## snakeML/dimensionality_reduction.py

```diff
@@ -1,24 +1,35 @@
-from snakeML.loads import loadData
-from snakeML.numpy_transformations import mcol
-from snakeML.visualization import scatter_attributeVSattribute
-from snakeML.preprocessing import oneHotEncoding
+from testlib.loads import loadData
+from testlib.numpy_transformations import mcol
+from testlib.visualization import scatter_attributeVSattribute
 import numpy
 import scipy
 
-def PCA(data, m):
-    mu=data.mean(1)
-    DC=data-mcol(mu)
-    C=numpy.dot(DC,DC.T)/data.shape[1]
+def PCA(D, m, flipped=False):
+    mu=D.mean(1)
+    DC=D-mcol(mu)
+    C=numpy.dot(DC,DC.T)/D.shape[1]
     s, U = numpy.linalg.eigh(C)
-    P = U[:, ::-1][:, 0:m]
-    DP=numpy.dot(P.T,data)
+    if flipped:
+        P = -U[:, ::-1][:, 0:m]
+    else:
+        P = U[:, ::-1][:, 0:m]
+    DP=numpy.dot(P.T,D)
     return DP
 
-def LDA(m, D, L,L_names):
+def scatter_PCA(D,L,L_names,m,flipped=False):
+    #D,L=loadData(filename, row_attributes=True, labels=True, numpyDataType=numpy.float32)
+    #L, L_names=oneHotEncoding(L, return_dictionary=True)
+    DP=PCA(D,m, flipped)
+    features=[]
+    for i in range(m):
+        features.append("Axis "+str(i))
+    scatter_attributeVSattribute(DP,L,features,L_names,row_attributes=True,is_label_dict=True)
+
+def LDA(D, L,L_names, m,flipped=False):
     mu=D.mean(1)
     SW=numpy.zeros(D.shape[0])
     SB=numpy.zeros(D.shape[0])
     for i in L_names:
         #SW
         data=D[:, L==L_names[i]]
         muC=data.mean(1)
@@ -34,22 +45,14 @@
     s, U = scipy.linalg.eigh(SB, SW)
     W = U[:, ::-1][:, 0:m]
     UW, _, _ = numpy.linalg.svd(W)
     U = UW[:, 0:m]
     DP=numpy.dot(W.T,D)
     return DP
 
-def scatter_LDA(m, D, L, L_names):
-    DP=LDA(m,D,L, L_names)
+def scatter_LDA(D, L, L_names, m,flipped=False):
+    DP=LDA(m,D,L, L_names, flipped)
     features=[]
     for i in range(m):
         features.append("Axis "+str(i))
     scatter_attributeVSattribute(DP,L,features,L_names,row_attributes=True,is_label_dict=True)
 
-def scatter_PCA(filename, m):
-    D,L=loadData(filename, row_attributes=True, labels=True, numpyDataType=numpy.float32)
-    L, L_names=oneHotEncoding(L, return_dictionary=True)
-    DP=PCA(D,m)
-    features=[]
-    for i in range(m):
-        features.append("Axis "+str(i))
-    scatter_attributeVSattribute(DP,L,features,L_names,row_attributes=True,is_label_dict=True)
```

## snakeML/distance.py

```diff
@@ -1,2 +1,5 @@
-def euclidean_distance(obj1, obj2):
-    return ((obj1.x-obj2.x)**2 + (obj1.y-obj2.y)**2)**0.5
+def euclidean_distance_objects(obj1, obj2):
+    return ((obj1.x-obj2.x)**2 + (obj1.y-obj2.y)**2)**0.5
+
+def euclidean_distance(x1,x2,y1,y2):
+    return ((x1-x2)**2 + (y1-y2)**2)**0.5
```

## snakeML/loads.py

```diff
@@ -1,7 +1,8 @@
+import sklearn.datasets
 from snakeML.numpy_transformations import mcol, mrow
 import numpy
 from snakeML.preprocessing import oneHotEncoding
 
 def loadData(filename, row_attributes= False, labels= False, separator=',', numpyDataType=None):
     data=[]
     with open(filename) as f:
@@ -33,11 +34,32 @@
                         attrs = numpy.array(attrs,dtype=numpyDataType)
                     data.append(attrs)
                 except:
                     pass
             return numpy.array(data)
         
 
-def loadEncodedData(filename):
-    D,L=loadData(filename, row_attributes=True, labels=True, numpyDataType=numpy.float32)
+def loadEncodedData(filename, row_attributes=True, numpyDataType=numpy.float32):
+    D,L=loadData(filename, row_attributes=row_attributes, labels=True, numpyDataType=numpyDataType)
     L, L_names=oneHotEncoding(L, return_dictionary=True)
-    return D,L,L_names
+    return D,L,L_names
+
+def read_txt(filename):
+    with open(filename) as f:
+        lines = f.readlines()
+        return map(lambda x:x.strip(),lines)
+    
+def load_iris():
+    D, L = sklearn.datasets.load_iris()['data'].T, sklearn.datasets.load_iris() ['target']
+    return D, L
+
+def db_train_test_split(D, L, seed=0):
+    nTrain = int(D.shape[1]*2.0/3.0)
+    numpy.random.seed(seed)
+    idx = numpy.random.permutation(D.shape[1])
+    idxTrain = idx[0:nTrain]
+    idxTest = idx[nTrain:]
+    x_train = D[:, idxTrain]
+    x_test = D[:, idxTest]
+    y_train = L[idxTrain]
+    y_test = L[idxTest]
+    return (x_train, y_train), (x_test, y_test)
```

## snakeML/visualization.py

```diff
@@ -1,50 +1,82 @@
+import math
 import matplotlib.pyplot as plt
+from snakeML.numpy_transformations import mcol, mrow
 
-def histogram_attributeVSfrequency(data, labels, features, label_names, is_label_dict=False,row_attributes=False, dense=False, save = False):
+def find_dimensions(total):
+    rows=1
+    cols=1
+    alternate=True
+    while rows*cols<total:
+        if alternate:
+            rows+=1
+            alternate=False
+        else:
+            cols+=1
+            alternate=True
+    return rows, cols
+
+
+def histogram_attributeVSfrequency(data, labels, features, label_names, is_label_dict=False,row_attributes=False, dense=False, save = False, center_data=True):
+    plt.figure()
+    rows, cols=find_dimensions(len(features))
+    if center_data:
+        if row_attributes:
+            data=data-mcol(data.mean(axis=1))
+        else:
+            data=data-mrow(data.mean(axis=0))
     if is_label_dict:
         lab=list(label_names.keys())
     else:
         lab=label_names
     for i in range(len(features)):
-        plt.figure()
+        plt.subplot(rows,cols,i+1)
         plt.xlabel(features[i])
         for j in range(len(lab)):
             if row_attributes:
                 plt.hist(data[:, labels==j][i, :], density = dense, label = lab[j])        
             else:
                 plt.hist(data[labels==j, :][:, i], density = dense, label = lab[j])        
         plt.legend()
         plt.tight_layout() # Use with non-default font size to keep axis label inside the figure
-        if save:
-            plt.savefig('hist_%d.png' % i)
-        plt.show()
+    if save:
+        plt.savefig('hist_%d.png' % i)
+    plt.show()
 
-def scatter_attributeVSattribute(data, labels, features, label_names, is_label_dict=False,row_attributes=False, dense=False, save = False):
+def scatter_attributeVSattribute(data, labels, features, label_names, is_label_dict=False,row_attributes=False, dense=False, save = False, center_data=False):
+    plt.figure()
+    rows, cols=find_dimensions(math.factorial(len(features)-1))
+    if center_data:
+        if row_attributes:
+            data=data-mcol(data.mean(axis=1))
+        else:
+            data=data-mrow(data.mean(axis=0))
     if is_label_dict:
         lab=list(label_names.keys())
     else:
         lab=label_names
+    counter=1
     for i in range(len(features)):
         for k in range(len(features)):
             if i >= k:
                 continue
-            plt.figure()
+            plt.subplot(rows,cols,counter)
+            counter+=1
             plt.xlabel(features[i])
             plt.ylabel(features[k])
             for j in range(len(lab)):
                 if row_attributes:
                     plt.scatter(data[:, labels==j][i, :],data[:, labels==j][k, :], label = lab[j])        
                 else:
                     plt.scatter(data[labels==j, :][:, i],data[labels==j, :][:, k], label = lab[j])        
             plt.legend()
             plt.tight_layout() # Use with non-default font size to keep axis label inside the figure
-            if save:
-                plt.savefig('scatter_%d_%d.png' % i, k)
-            plt.show()
+    if save:
+        plt.savefig('scatter_%d_%d.png' % i, k)
+    plt.show()
 
 def scatter_categories(data, labels, label_names, is_label_dict=False,row_attributes=False,  save = False):
     if is_label_dict:
         lab=list(label_names.keys())
     else:
         lab=label_names
     plt.figure()
```

## Comparing `snakeML-0.0.5.dist-info/METADATA` & `snakeML-0.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakeML
-Version: 0.0.5
+Version: 0.0.6
 Summary: Machine Learning Library
 Author: Manuel Escobar
 Author-email: manuelescobar.dev@gmail.com
 License: MIT
 Keywords: python,ML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

## Comparing `snakeML-0.0.5.dist-info/RECORD` & `snakeML-0.0.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 snakeML/__init__.py,sha256=b5WWDnKBauFF-ASORtGYzwbyfZWtyRF6ppIJ0mUm5Qo,167
-snakeML/density_estimation.py,sha256=hGCk_9x9emo1rOi157uU9ziqsJ-gBUgxr4NzTk4Su8c,2162
-snakeML/dimensionality_reduction.py,sha256=tSLc4CRCNrRibyEFN1FahSN3DhD6dCDGBKUbKRFuoNk,1591
+snakeML/density_estimation.py,sha256=yf0TyKtpyQZgilrloP_PsKl14NOPqYKaeN6UH-BZcvA,2162
+snakeML/dimensionality_reduction.py,sha256=OiF75HkBRGAvDhKsnhPgPykPb-liVsBBfSuDizy6VfU,1670
 snakeML/dist.py,sha256=jEfRCPnls4bxExxy0fOpww-x38z-yRdg7TfRYqMt4Zk,93
-snakeML/distance.py,sha256=jEfRCPnls4bxExxy0fOpww-x38z-yRdg7TfRYqMt4Zk,93
-snakeML/loads.py,sha256=pVUr1HUw0PVkpzJdaaF3Tu7Gvr-48KjVn_NogVRckg4,1646
+snakeML/distance.py,sha256=AxQmEaXwvxLlIswY2ynRoGBitkgOsOxGuAo_BxM_W3A,181
+snakeML/gaussian.py,sha256=tHrtPx06XonPZjll4RWC2ea3eAyCK_v7lnilYAnlzFQ,5328
+snakeML/loads.py,sha256=M-sso5ZCWW1z91f_XTXWiz2X08zF7frPDTA6Micm5aI,2351
 snakeML/numpy_transformations.py,sha256=kYl19OPMt1Zsw7ylyvQ-w4HATGbey-s-ZWitgEIiMQs,756
 snakeML/preprocessing.py,sha256=FxxNt6amAOi8vPBl2-qAjfBMNAnCn1j4HHPQ6dX1GMg,410
 snakeML/test.py,sha256=oFYUiQkDZiO1mRkBMUbq3QBWKUEwPItA9fKtTKDVNkQ,571
 snakeML/validation.py,sha256=rFBBtgQ8IU31mHeTIAiIipGyoLdZFgLWdyC_e244AO0,547
-snakeML/visualization.py,sha256=c4-G8CtiSOF_oTEAyIvpW57YfXY4ua0YJ1F0lgyuoRM,2450
-snakeML-0.0.5.dist-info/METADATA,sha256=nvTUb0kOoFTb4ZVA95WgIKIUwumwOYuSlFEZH34UPMI,581
-snakeML-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-snakeML-0.0.5.dist-info/top_level.txt,sha256=7VKNcGzWlpoujvutf-2KcaIVne9pbUmfoqLdoQst_0E,8
-snakeML-0.0.5.dist-info/RECORD,,
+snakeML/visualization.py,sha256=x7SHGpt2QVSRb07avKaXhIhrOc_r4ao90iWOPn02mfk,3286
+snakeML-0.0.6.dist-info/METADATA,sha256=we-wPyZCeDWG0h_52TtWrSzZs9CT1RY5et2CcZw2Jo4,581
+snakeML-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+snakeML-0.0.6.dist-info/top_level.txt,sha256=7VKNcGzWlpoujvutf-2KcaIVne9pbUmfoqLdoQst_0E,8
+snakeML-0.0.6.dist-info/RECORD,,
```

