# Comparing `tmp/DTCO-0.1.2.tar.gz` & `tmp/DTCO-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DTCO-0.1.2.tar", last modified: Fri May  5 10:48:04 2023, max compression
+gzip compressed data, was "DTCO-0.1.3.tar", last modified: Fri May 12 11:31:00 2023, max compression
```

## Comparing `DTCO-0.1.2.tar` & `DTCO-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.144781 DTCO-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.129214 DTCO-0.1.2/DTCO.egg-info/
--rw-rw-rw-   0        0        0     3478 2023-05-05 10:48:03.000000 DTCO-0.1.2/DTCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-05 10:48:04.000000 DTCO-0.1.2/DTCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 10:48:03.000000 DTCO-0.1.2/DTCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-05 10:48:03.000000 DTCO-0.1.2/DTCO.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.129214 DTCO-0.1.2/GRO/
--rw-rw-rw-   0        0        0       51 2023-05-05 05:23:41.000000 DTCO-0.1.2/GRO/__init__.py
--rw-rw-rw-   0        0        0    37339 2023-05-05 05:23:41.000000 DTCO-0.1.2/GRO/classGRO.py
--rw-rw-rw-   0        0        0     2068 2023-05-05 05:23:41.000000 DTCO-0.1.2/GRO/gro.py
--rw-rw-rw-   0        0        0     1113 2023-05-05 05:23:41.000000 DTCO-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3478 2023-05-05 10:48:04.144781 DTCO-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3051 2023-05-05 09:10:11.000000 DTCO-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.129214 DTCO-0.1.2/copernic/
--rw-rw-rw-   0        0        0       63 2023-05-05 07:07:04.000000 DTCO-0.1.2/copernic/__init__.py
--rw-rw-rw-   0        0        0    29038 2023-05-05 07:45:01.000000 DTCO-0.1.2/copernic/classCPAnalysis.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:48:04.129214 DTCO-0.1.2/libMetric/
--rw-rw-rw-   0        0        0       63 2023-05-05 05:23:41.000000 DTCO-0.1.2/libMetric/__init__.py
--rw-rw-rw-   0        0        0    48880 2023-05-05 05:23:41.000000 DTCO-0.1.2/libMetric/classLiberty.py
--rw-rw-rw-   0        0        0       86 2023-05-05 10:48:04.144781 DTCO-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-05-05 10:46:14.000000 DTCO-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:00.127138 DTCO-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:00.122132 DTCO-0.1.3/DTCO.egg-info/
+-rw-rw-rw-   0        0        0     3478 2023-05-12 11:30:59.000000 DTCO-0.1.3/DTCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-12 11:31:00.000000 DTCO-0.1.3/DTCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 11:30:59.000000 DTCO-0.1.3/DTCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-12 11:30:59.000000 DTCO-0.1.3/DTCO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:00.124128 DTCO-0.1.3/GRO/
+-rw-rw-rw-   0        0        0       51 2023-05-05 05:23:41.000000 DTCO-0.1.3/GRO/__init__.py
+-rw-rw-rw-   0        0        0    37339 2023-05-05 05:23:41.000000 DTCO-0.1.3/GRO/classGRO.py
+-rw-rw-rw-   0        0        0     2068 2023-05-05 05:23:41.000000 DTCO-0.1.3/GRO/gro.py
+-rw-rw-rw-   0        0        0     1113 2023-05-05 05:23:41.000000 DTCO-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3478 2023-05-12 11:31:00.127138 DTCO-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3051 2023-05-05 09:10:11.000000 DTCO-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:00.126124 DTCO-0.1.3/copernic/
+-rw-rw-rw-   0        0        0       57 2023-05-12 10:45:11.000000 DTCO-0.1.3/copernic/__init__.py
+-rw-rw-rw-   0        0        0    31521 2023-05-12 09:55:03.000000 DTCO-0.1.3/copernic/classDTCO.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:31:00.127138 DTCO-0.1.3/libMetric/
+-rw-rw-rw-   0        0        0       63 2023-05-05 05:23:41.000000 DTCO-0.1.3/libMetric/__init__.py
+-rw-rw-rw-   0        0        0    48880 2023-05-05 05:23:41.000000 DTCO-0.1.3/libMetric/classLiberty.py
+-rw-rw-rw-   0        0        0       86 2023-05-12 11:31:00.129134 DTCO-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-05-12 11:16:26.000000 DTCO-0.1.3/setup.py
```

### Comparing `DTCO-0.1.2/DTCO.egg-info/PKG-INFO` & `DTCO-0.1.3/DTCO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DTCO
-Version: 0.1.2
+Version: 0.1.3
 Summary: DTCO Utility
 Home-page: https://github.com/dipsci/DTCO
 Author: hockchen
 Author-email: hock.chen@dipsci.com
 Keywords: DTCO,process monitor,liberty,metric,timing,EDA,physical design,WAT,CP,Binning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DTCO-0.1.2/GRO/classGRO.py` & `DTCO-0.1.3/GRO/classGRO.py`

 * *Files identical despite different names*

### Comparing `DTCO-0.1.2/GRO/gro.py` & `DTCO-0.1.3/GRO/gro.py`

 * *Files identical despite different names*

### Comparing `DTCO-0.1.2/LICENSE` & `DTCO-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DTCO-0.1.2/PKG-INFO` & `DTCO-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DTCO
-Version: 0.1.2
+Version: 0.1.3
 Summary: DTCO Utility
 Home-page: https://github.com/dipsci/DTCO
 Author: hockchen
 Author-email: hock.chen@dipsci.com
 Keywords: DTCO,process monitor,liberty,metric,timing,EDA,physical design,WAT,CP,Binning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DTCO-0.1.2/README.md` & `DTCO-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `DTCO-0.1.2/copernic/classCPAnalysis.py` & `DTCO-0.1.3/copernic/classDTCO.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,138 +1,209 @@
 '''
-CP Analysis Utility
+Design Technology Co-optimization Platform
 
 Copyright (C) 2022, by DipSci Technology Corpopation, LTD.
 This software tool is independently developed and owned by DipSci Technology Co., Ltd.
 It is freely licensed to industry and academia to use, share, reproduce, or improve, provided 
 this copyright notice is retained or the initial creater is listed on the contributors list.
 Derivatives developed for profit based on this software tool must still include this copyright 
 notice or credit the initial creater on the contributors list.
 
 Revision History:
 2021/10/26 hockchen init
 2021/11/09 hockchen update pass core profile 3D 
+2022/02/01 hockchen generated model for wafer-level CP & WAT data
 '''
-
 import pandas as pd
 import numpy as np
-import scipy.stats
+import pickle, io
+import torch # os.environ['KMP_DUPLICATE_LIB_OK']='True' for libiomp5md.dll issue
 import matplotlib.pyplot as plt
+import matplotlib.gridspec as gridspec
 import plotly.offline as ply
 import plotly.graph_objs as go
-from mpl_toolkits.mplot3d import Axes3D
-from scipy import interpolate
+from scipy import interpolate, stats, linalg
+from mpl_toolkits.axes_grid1 import make_axes_locatable
+#from scipy.interpolate import griddata
 
 #pd.set_option('expand_frame_repr', False)
 #pd.set_option('precision',8)
 #plt.rcParams.update({'font.family': 'monospace'})
 
-class CPAnalysis:
+#np.set_printoptions(linewidth=200)
+#cList=list(plt.cm.colors.cnames.keys()) # color list
+#colL = list(plt.matplotlib.colors.TABLEAU_COLORS)+['k'] # 11 colors
+
+class DTCO:
     def __init__(self,local=True):
-        #self.local = local
+        print('init class DTCO ...')
         self.mouseTriggle = False
         self.colL = list(plt.matplotlib.colors.TABLEAU_COLORS)+['k'] # 11 colors
         self.mrkL = ['o','v','^','<','>','d','s','h','H','p','*','D','+','x']
         
     def sigma_percentage(self,sigma):
         '''return left and right % boundary based on the specified sigma value'''
-        sta = scipy.stats.norm(0,1)
+        sta = stats.norm(0,1)
         p = 100-sta.cdf(-1*sigma)*2*100
         h = round((100-p)/2,1)
         h = 0 if h==0 else h
         return h,100-h
 
+    def convert2CSV(self,data,features,outCSV=None):
+        '''convert generated data in PIL style (batch,H,W,C) to Dataframe'''
+        batch_size,H,W,C = data.shape
+        gx, gy = np.meshgrid(np.arange(1,W+1),np.arange(1,H+1))
+        ix, iy = np.tile(gx.ravel(),batch_size), np.tile(gy.ravel(),batch_size)
+        wid = np.arange(1,batch_size+1).repeat(W*H).astype(int)
+        d = data.transpose(3, 0, 1, 2).reshape(C, -1).T
+        df = pd.DataFrame(np.column_stack([wid,ix,iy,d]),columns=['WID','X','Y']+features) 
+        df = df.dropna(subset=features)
+        print(f'convert generated data to dataframe: {df.shape}')
+        if outCSV!=None:
+            df.to_csv(outCSV,float_format='%g',index=False)
+            print(f'generated data was saved into {outCSV} ...')
+        return df
+
+    def df2Grid(self,df,feature,H,W):
+        '''convert dataframe to griddata (interpolation) for non-existing points'''
+        x,y,z = df[['X','Y',feature]].values.T
+        gx,gy = np.meshgrid(np.arange(1,W+1),np.arange(1,H+1))
+        gz = interpolate.griddata(np.stack([x,y],axis=1),z,(gx,gy),method='cubic',fill_value=0) # 1st
+        return gx,gy,gz
+
+    def genFakeData(self,model_pkl,num=300,outCSV=None):
+        '''load generator model (pickle) and generate wafer-level CP and WAT data'''
+        print(f'load generated model & parameter {model_pkl} ...')
+        with open(model_pkl, 'rb') as f:
+            pkg = pickle.load(f)
+            mask = pkg['mask']
+            scale = pkg['scale']
+            features = pkg['features']
+            G = torch.jit.load(io.BytesIO(pkg['model']), 'cpu')
+        
+        print(f'generate {num} wafer-level CP & WAT data ...')
+        latent_size = 100
+        noises = torch.randn(num,latent_size) # generate num wafers 
+        x = G(noises).detach().numpy().transpose(0,2,3,1) # as grid data (PIL) fasion (batch,H,W,C)
+    
+        # normalization & legalization
+        H,W,C = x.shape[1:] # PIL shape
+        dmin,dmax = scale.reshape(C,1,1,1,2).T
+        xmin = np.nanmin(x,axis=(0,1,2,)).reshape(1,1,1,-1)
+        xmax = np.nanmax(x,axis=(0,1,2,)).reshape(1,1,1,-1)
+        x = (x-xmin)/(xmax-xmin)*dmax # set dmin=0, but keep dmin(real min)
+        x = np.where((dmin<=x)&(x<=dmax), x, np.nan) # drop out of scale range
+        x = np.where(mask.reshape(1,H,W,1),x,np.nan) # apply wafer mask
+        
+        # convert grid data to dataframe
+        df = self.convert2CSV(x,features,outCSV)
+        return df
+
+    def showData(self,df,feature='SIDD',num=None,ncol=None,dtype='2d',view=(90,90),zoom=1.7):
+        num = num or (30 if df.shape[0]>30 else df.shape[0])
+        ncol = ncol or 10
+        nrow = int(np.ceil(num/ncol))
+        plt.figure(figsize=(ncol*1.8,nrow*1.8))
+        plt.suptitle(f'{feature} {dtype.upper()}',y=0.99,c='b')
+        for i in range(num):
+            x,y,z = df.loc[i+1][['X','Y',feature]].values.T
+            if dtype!='3d':
+                ax = plt.subplot(nrow,ncol,i+1,title=f'{i+1}')
+                ax.tricontourf(x,y,z,levels=20)
+            else:
+                ax = plt.subplot(nrow,ncol,i+1,title=f'{i+1}',projection='3d')
+                ax.plot_trisurf(x,y,z,antialiased=False,linewidth=0,edgecolors='none',cmap='viridis')
+                ax.view_init(*view)
+                ax.set_box_aspect(None, zoom=zoom)
+            ax.invert_yaxis() # set origin to top left
+            ax.axis('off')
+        plt.tight_layout(rect=(0,0,1,0.98))
+    
     def filterData(self,df,itemL,sigma=2.5):
+        '''filter outlier, where the specified df should be indexed with WID'''
         s1,s2 = self.sigma_percentage(sigma)
-        n1 = len(df)
+        num = df.shape[0]
         for item in itemL:
-            m = df[item].describe(percentiles=[s1/100,s2/100])
-            df = df[(m[f'{s1}%']<=df[item])&(df[item]<=m[f'{s2}%'])]
-        n2 = len(df)
-        print(f'filter out {n1-n2} of {n1} samples, {n2*100/n1:.2f}%')
+            m = df[item].quantile([s1/100,s2/100])
+            df = df[(m[s1/100]<=df[item])&(df[item]<=m[s2/100])]
+        print(f'filter out {num-df.shape[0]} out of {num} samples, {df.shape[0]*100/num:.2f}%')
+        #widL = df.index.unique().tolist()
+        #dL = []
+        #for wid in widL:
+        #    d = df.loc[wid]
+        #    for item in itemL:
+        #        m = d[item].quantile([s1/100,s2/100])
+        #        d = d[(m[s1/100]<=d[item])&(d[item]<=m[s2/100])]
+        #    if nlimit!=None and d.shape[0]<nlimit:
+        #        print(f'WARN! drop unqualified wafer: {wid}, size={d.shape[0]}<{nlimit}')
+        #    else:
+        #        dL += [d]
+        #dt = None if len(dL)==0 else pd.concat(dL)
+        #print(f'filter out {df.shape[0]-dt.shape[0]} samples, {dt.shape[0]*100/df.shape[0]:.2f}%')
         return df
 
-    def augmentPE(self,df,pcAll=600,volt='033'):
-        pcItem = [v for v in df.columns if f'PC_{volt}' in v]
-        diItem = [v for v in df.columns if f'DI_{volt}' in v] # turn-on one big-core (4 engine)
-        vsItem = [v for v in df.columns if f'VS_{volt}' in v]
-        f = np.array([v.split('_')[-1] for v in pcItem],int)
-        t = pd.DataFrame(df[pcItem].values,columns=f) # pass core only
-        v = pd.DataFrame(df[vsItem].values,columns=f) # voltage
-        i = pd.DataFrame(df[diItem].values,columns=f) # current
-        s = df[['SIDD']]
-        i = (i-s.values)/4*pcAll+s.values
-        p = i*v # P= I*V 
-        h = (t*f)*1e-6 # TH
-        e = (p/(1e-12+h)) #.dropna() # PE
-        dt = df.copy()
-        dt['eff_cp'] = e.min(axis=1).values
-        return dt,e
-
-    def featureScatter(self,df,wid=None,fx='ROu',fy='SIDD',sigma=2.5,alpha=0.5,s=5,args={'alpha':0.3}):
+    def featureScatter(self,df,wid=None,fx='ROu',fy='SIDD',sigma=None,alpha=0.5,s=5,args={'alpha':0.5}):
         dt = df if wid==None else df.loc[wid]
-        dt = self.filterData(dt,[fx,fy],sigma=sigma)
+        dt = dt if sigma==None else self.filterData(dt,itemL=[fx,fy],sigma=sigma) 
+        dm = dt[['X','Y','SIDD']].groupby(['X','Y']).mean().reset_index() # average surface
         widL = dt.index.unique().tolist()
-        f = plt.figure(figsize=(10,7))
+        f = plt.figure(figsize=(7,6))
         ax = f.gca()
-        for wid in widL:
-            d = dt.loc[wid]
-            plt.scatter(d[fx].values,d[fy].values,alpha=alpha,s=s,picker=2,label=f'{wid}:{len(d)}')
-        plt.title(f'({sigma}$\sigma$, {len(d)} samples)')
+        plt.title(f'{len(widL)} wafers: ({dt.shape[0]} samples)')
+        plt.scatter(dt[fx],dt[fy],s=s,alpha=alpha,edgecolors=None,picker=4)
         plt.xlabel(f'{fx}')
         plt.ylabel(f'{fy}')
         plt.grid(which='major',linestyle='-',zorder=0)
         plt.grid(which='minor',linestyle=':',zorder=0)
         plt.minorticks_on()
-        plt.subplots_adjust(left=0.1,bottom=0.1,right=0.7,top=0.95,wspace=0,hspace=0.1)
-        #plt.legend()
-        plt.legend(loc='center left',bbox_to_anchor=(1.0,0.5),fontsize=10)
+        plt.tight_layout(rect=(0,0,1,0.98))
+        #plt.legend(loc='center left',bbox_to_anchor=(1.0,0.5),fontsize=10)
         ann = ax.annotate('',xy=(0,0),xytext=(-50,20),textcoords="offset points",zorder=100,
             bbox=dict(boxstyle='round4', fc='linen',ec='k',lw=1),arrowprops=dict(arrowstyle='-|>'))
         ann.set_visible(False)
         def onRelease(event):
             self.mouseTriggle = False
-        def onPick(event,ax,df):
+        def onPick(event,ax,dt):
             if self.mouseTriggle:
                 return
             self.mouseTriggle = True
-            indL = event.ind
-            wid,size = map(eval,event.artist.get_label().split(':'))
-            d = df.loc[wid].set_index(['X','Y'])
-            idx = d.iloc[indL].index.values
-            print(f'====>{wid},{size}')
-            print(d.iloc[indL][[fx,fy]])
+            # visualize with the mean wafer
+            inds = event.ind
+            idx = dt.iloc[inds][['X','Y']].set_index(['X','Y']).index.unique().values
             ann.xy = (event.mouseevent.xdata,event.mouseevent.ydata)
-            ann.set_text(f'{wid}:\n{d.iloc[indL[0]][[fx,fy]]}')
+            ann.set_text(f'{len(idx):,} samples')
             ann.set_visible(True)
             ax.figure.canvas.draw_idle()
-            self.featureSurface(df,wid,feature='SIDD',xyL=idx,**args)
-        f.canvas.mpl_connect('pick_event',lambda event: onPick(event,ax,df))
+            self.featureSurface(dm,wid=None,feature='SIDD',xyL=idx,**args)
+        f.canvas.mpl_connect('pick_event',lambda event: onPick(event,ax,dt))
         f.canvas.mpl_connect('button_release_event',onRelease)
 
-    def featureSurface(self,df,wid=None,feature='SIDD',xyL=None,sigma=2.5,alpha=1,pcvolt='035',view=(70,300)):#,zlim=(None,None)):
-        '''wid := lot-wafer id as string 'LotID_WID' or tuple ('LotID',WID)'''
-        dt = df if wid==None else df.loc[wid]
-        dt = dt[dt[feature].notna()] # drop nan first
-        d = self.filterData(dt,[feature],sigma=sigma)
-        f = plt.figure(figsize=(8,7))
-        ax = Axes3D(f)
+    def featureSurface(self,df,wid=None,feature='SIDD',sigma=None,xyL=None,alpha=1,view=(70,300)):
+        '''wafer-level feature surface'''
+        dt = df.groupby(['X','Y']).mean().reset_index() if wid==None else df.loc[wid]
+        dt = dt if sigma==None else self.filterData(dt,itemL=[feature],sigma=sigma) 
+        dt = dt.dropna(subset=[feature]) # drop nan features
+        f = plt.figure(figsize=(7,6))
+        ax = plt.axes(projection='3d')
         ax.plot_trisurf(
-            d['X'].values,d['Y'].values,d[feature].values.astype('float'),
-            alpha=alpha,
+            dt['X'].values,dt['Y'].values,dt[feature].values.astype('float'),
+            alpha=alpha,zorder=0,
             antialiased=False,linewidth=0,edgecolors='none',cmap=plt.cm.viridis)
         # dies on surface
+        d = None
         if xyL is not None:
-            d = d.set_index(['X','Y']).loc[xyL].reset_index()
-            ax.scatter(d['X'].values,d['Y'].values,d[feature].values,color='r',s=20,zorder=10000,picker=5)
-        ax.set_title(f'{wid}:{feature} ({sigma}$\sigma$, {len(d)} samples)')
+            d = dt.set_index(['X','Y']).loc[xyL].reset_index()
+            ax.scatter(d['X'].values,d['Y'].values,d[feature].values,color='r',s=40,zorder=10000,picker=5)
+        ax.set_title(f'{wid or "Mean"}:{feature} ({dt.shape[0]:,} samples)')
         ax.set_xlabel('X')
         ax.set_ylabel('Y')
-        ax.set_zlabel('%s'%feature,rotation=90)
-        ax.view_init(view[0],view[1])
+        ax.set_zlabel(feature,rotation=90)
+        ax.view_init(*view)
+        ax.set_box_aspect(None, zoom=1.0)
+        plt.tight_layout(rect=(0,0,1,0.98)) 
         ann = ax.annotate('',xy=(0,0),xytext=(-50,20),textcoords="offset points",zorder=100,
             bbox=dict(boxstyle='round4', fc='linen',ec='k',lw=1),arrowprops=dict(arrowstyle='-|>'))
         ann.set_visible(False)
         def onRelease(event):
             self.mouseTriggle = False
         def onPick(event,ax,d):
             if self.mouseTriggle:
@@ -140,51 +211,269 @@
             self.mouseTriggle = True
             indL = event.ind
             idx = d.index.values[indL]
             ann.xy = (event.mouseevent.xdata,event.mouseevent.ydata)
             ann.set_text(f'{wid}: {idx[0]}')
             ann.set_visible(True)
             ax.figure.canvas.draw_idle()
-            self.passCoreProfile(d.reset_index(),xyL=idx,volt=pcvolt,sigma=sigma,args={'alpha':0.9,'lw':2,'color':'g'})
         f.canvas.mpl_connect('pick_event',lambda event: onPick(event,ax,d.set_index(['X','Y'])))
         f.canvas.mpl_connect('button_release_event',onRelease)
         plt.show()
 
-    def featurePlotly(self,df,wid=None,feature='SIDD',sigma=3,outDir='.',resolution=100j):
-        '''convert vector to mesh grid with griddata (interpolation) for non-existing points
-           wid := lot-wafer id as string 'LotID_WID' or tuple ('LotID',WID)'''
+    def featurePlotly(self,df,wid=None,feature='SIDD',sigma=3,outDir='.'):
+        '''convert vector to mesh grid with griddata (interpolation) for non-existing points'''
         dt = df if wid==None else df.loc[wid]
-        dt = dt[dt[feature].notna()] # drop nan first
-        dt = self.filterData(dt.reset_index()[['X','Y',feature]],[feature],sigma=sigma)
-        x,y,z = dt[['X','Y',feature]].values.T
-        gx,gy = np.mgrid[x.min():x.max():resolution,y.min():y.max():resolution]
-        gz = interpolate.griddata(np.array([x,y]).T,z,(gx,gy),method='linear')
-        trace = go.Surface(x=gx,y=gy,z=gz)
-        layout = go.Layout(
-            title='uniformity',
-            showlegend=False,
-            height=500,width=800,margin=dict(l=0,r=0,b=0,t=0),
-            scene={'xaxis':{'title':'X'},'yaxis':{'title':'Y'},'zaxis':{'title':'Z','range':[z.min()*0.8,z.max()*1.2]}},
-            scene_camera={'eye':{'x':-1,'y':-1,'z':1.0}}
+        dt = dt if sigma==None else self.filterData(dt.reset_index()[['X','Y',feature]],[feature],sigma=sigma)
+        dt = dt.dropna(subset=[feature]) # drop nan features
+        HW = dt[['Y','X']].max().values.T
+        gx,gy,gz = self.df2Grid(dt, feature, *HW)
+        fig = go.Figure(
+            go.Surface(x=gx, y=gy, z=gz)
         )
-        fig = go.Figure(data=[trace],layout=layout)
+        fig.update_layout(
+            width=600, height=400,
+            margin=dict(l=0, r=0, b=0, t=0),
+            scene=dict(
+                xaxis=dict(title='X',visible=True),
+                yaxis=dict(title='Y',visible=True),
+                zaxis=dict(title='Z',visible=True),
+                aspectratio=dict(x=1, y=1, z=0.5),
+                camera=dict(eye=dict(x=0, y=0, z=1.8)),
+            )
+        )
+        #fig.update_xaxes(showticklabels=False,title_text='')
+        #fig.update_yaxes(showticklabels=False,title_text='')
         ply.plot(fig,filename=f'{outDir}/uniformity_{feature}.html',auto_open=True)
-    
 
-    # adjacent die-to-die derating
-    def d2dDerating(self,df,wid=None,feature='ROu',sd=1,sigma=2.9,detail=False):
+    ### design for productivity optimization
+    def waferSort(self,df,itemL=['ROu','SIDD'],nsize=None):
+        indexL = df.index.names
+        dm = df.groupby(indexL)[itemL].mean().sort_values(itemL,ascending=False)
+        nsize = len(dm) if nsize==None else nsize
+        #widL = [str(v) for v in dm.index.tolist()]
+        f = plt.figure(figsize=(12,7))
+        ax1 = f.subplots()
+        ax2 = plt.twinx()  # instantiate a second axes that shares the same x-axis
+        ax1.plot(range(nsize),dm[itemL[1]].iloc[:nsize],marker='o',ms=5,color='r',zorder=0,alpha=0.5)
+        ax2.plot(range(nsize),dm[itemL[0]].iloc[:nsize],marker='o',ms=5,color='b',zorder=0,alpha=0.5,picker=5) # picker can only be applied on top
+        ax1.set_xlabel('WID')
+        ax1.set_xticks(np.arange(1,nsize+1,10))
+        #ax1.set_xticklabels(widL[:nsize],rotation=90)
+        ax1.set_ylabel(itemL[1],color='r')
+        ax2.set_ylabel(itemL[0],color='b')
+        ax1.tick_params(axis='x',rotation=90)
+        ax1.tick_params(axis='y',labelcolor='r')
+        ax2.tick_params(axis='y',labelcolor='b')
+        ax1.grid(color='r',alpha=0.5,zorder=0)
+        ax2.grid(color='b',ls='--',alpha=0.5,zorder=0)
+        plt.title(f'Wafer Sorting by {itemL} ({nsize} wafers)')
+        plt.tight_layout(rect=(0,0,1,0.98))
+        ann = ax2.annotate('',xy=(0,0),xytext=(-10,20),textcoords="offset points",zorder=100,
+            bbox=dict(boxstyle='round4', fc='linen',ec='k',lw=1),arrowprops=dict(arrowstyle='-|>'))
+        ann.set_visible(False)
+        def onPick(event,ax,df,dm):
+            indL = event.ind
+            wid = dm.index[indL[0]]
+            ann.xy = (event.mouseevent.xdata,event.mouseevent.ydata)
+            ann.set_text(f'{dm.loc[wid]}')
+            ann.set_visible(True)
+            ax.figure.canvas.draw_idle()
+            self.featureSurface(df,wid,feature='SIDD',sigma=2.5)
+        f.canvas.mpl_connect('pick_event',lambda event: onPick(event,ax2,df,dm))
+        return dm
+
+    def pcmDensity3D(self,df,widL=None,fx='ROu',fy='SIDD',sigma=None,view=(60,240),bins=(30,30),rangeL=None):
+        '''df should be indexed with WID'''
+        widL = widL if widL is not None else df.index.unique().tolist()
+        if sigma!=None:
+            dt = self.filterData(df.loc[widL],itemL=[fx,fy],sigma=sigma)
+        else:
+            dt = df.loc[widL][[fx,fy]].dropna()
+        x,y = dt[fx].values,dt[fy].values
+        H,binx,biny = np.histogram2d(x,y,bins=bins,range=rangeL)
+        binx,biny = (binx[:-1]+binx[1:])/2,(biny[:-1]+biny[1:])/2
+        gx,gy = np.meshgrid(binx,biny)
+        f = plt.figure(figsize=(8,7))
+        ax = plt.axes(projection='3d')
+        ax.contour(gx,gy,H.T,zdir='x',levels=30,offset=dt[fx].min()*0.9) 
+        ax.contour(gx,gy,H.T,zdir='y',levels=30,offset=dt[fy].max()*1.1) 
+        ax.contour(gx,gy,H.T,levels=30,linewidths=2)  # line contour
+        cs = ax.contourf(gx,gy,H.T,levels=30,offset=0) # surface contour, project to z=0
+        f.colorbar(cs,extend='both',shrink=0.8) #,aspect=30)
+        #ax.clabel(cs,fmt='%2.3f',colors='b',fontsize=14,inline=True) # inline notation
+        ax.plot_surface(
+            gx,gy,H.T,zorder=0,alpha=0.6,
+            antialiased=False,linewidth=0,edgecolors='none',
+            cmap=plt.cm.Blues_r) #,cmap=plt.cm.viridis)
+        ax.set_title(f'PCM Histogram {sigma}$\sigma$ ({dt.shape[0]:,} samples, {len(widL):,} wafers)')
+        ax.set_xlabel(fx)
+        ax.set_ylabel(fy)
+        ax.set_zlabel('Occurrence')
+        ax.view_init(view[0],view[1])
+        #plt.setp(cs.collections,linewidth=2)
+        plt.tight_layout(rect=(0,0,1,1))
+        return binx,biny,H.T
+
+    def pcmDensity2D(self,df,widL=None,fx='ROu',fy='SIDD',sigma=None,bins=(10,10),rangeL=None):
+        '''df should be indexed with WID'''
+        widL = widL if widL is not None else df.index.unique().tolist()
+        if sigma!=None:
+            dt = self.filterData(df.loc[widL],itemL=[fx,fy],sigma=sigma)
+        else:
+            dt = df.loc[widL][[fx,fy]].dropna()
+        # projection contour
+        x,y = dt[fx].values,dt[fy].values
+        H,binx,biny = np.histogram2d(x,y,bins=bins,range=rangeL)
+        binx,biny = (binx[:-1]+binx[1:])/2,(biny[:-1]+biny[1:])/2
+        gx,gy = np.meshgrid(binx,biny)
+        f,ax = plt.subplots()
+        f.set_size_inches((8,7))
+        #cs = ax.contour(gx,gy,H.T,levels=30,linewidths=3,alpha=0.7) # line contour
+        cs = ax.contourf(gx,gy,H.T,levels=30,alpha=0.7) # surface contour
+        f.colorbar(cs,extend='both',shrink=1)
+        ax.set_title(f'PCM Histogram {sigma}$\sigma$ ({dt.shape[0]:,} samples, {len(widL):,} wafers)')
+        ax.set_xlabel(fx)
+        ax.set_ylabel(fy)
+        dx,dy = (binx[1]-binx[0])/2,(biny[1]-biny[0])/2
+        plt.xticks(np.arange(binx[0]-dx,binx[-1]+dx*1.1,dx*2))
+        plt.yticks(np.arange(biny[0]-dy,biny[-1]+dy*1.1,dy*2))
+        plt.grid(which='major',lw=1,color='r',alpha=0.5)
+        plt.grid(which='minor',lw=1,color='gray',ls=':',alpha=0.2)
+        plt.minorticks_on()
+        plt.tight_layout(rect=(0,0,1,1))
+        return binx,biny,H.T
+
+    def pcmDensity(self,df,widL=None,fx='ROu',fy='SIDD',sigma=None,percentiles=[10,20,30],bins=(100,100),sub=1):
+        '''df should be indexed with WID'''
+        widL = widL if widL is not None else df.index.unique().tolist()
+        if sigma!=None:
+            dt = self.filterData(df.loc[widL],itemL=[fx,fy],sigma=sigma)
+        else:
+            dt = df.loc[widL][[fx,fy]].dropna()
+        x,y = dt[[fx,fy]].values[::sub].T
+        H, bx, by = np.histogram2d(x, y, bins=bins)
+        bx, by = (bx[:-1]+bx[1:])/2, (by[:-1]+by[1:])/2
+        gx, gy = np.meshgrid(bx, by)
+        S = np.sort(H.ravel()) 
+        cdf = np.cumsum(S)*100/H.sum()
+        levels = S[[np.argmax(cdf>v) for v in percentiles]] # index where cdf>percentile
+        ctags = {l:f'{p}%' for l,p in zip(levels,percentiles)} # contour tags
+        G = gridspec.GridSpec(nrows=1,ncols=2,width_ratios=[0.5,0.5])
+        fig = plt.figure(figsize=(10,6))
+        ax = fig.add_subplot(G[0,0],projection='3d',title='PCM Density')
+        ax.plot_trisurf(gx.ravel(),gy.ravel(),H.T.ravel(), cmap='viridis',
+            antialiased=False,linewidth=0,edgecolors='none')
+        ax.tricontour(gx.ravel(),gy.ravel(),H.T.ravel(), cmap='Blues', levels=20, zdir='x', offset=x.min()*0.9)
+        ax.tricontour(gx.ravel(),gy.ravel(),H.T.ravel(), cmap='Blues', levels=20, zdir='y', offset=y.max()*1.1)
+        ax.view_init(70,250)
+        ax.set_box_aspect(None, zoom=1.2)
+        ax.set_xlabel(fx)
+        ax.set_ylabel(fy)
+        ax = fig.add_subplot(G[0,1],title='PCM Contour')
+        tc = ax.contour(gx,gy,H.T, cmap='jet', levels=levels)
+        cl = ax.clabel(tc, inline=1, fontsize=12, fmt=ctags, inline_spacing=2)
+        [txt.set_bbox(dict(facecolor='white', edgecolor='none', pad=1, alpha=0.8)) for txt in cl]
+        ax.set_xlabel(fx)
+        ax.set_ylabel(fy)
+        plt.suptitle(f'PCM 3D ({len(widL):,} wafers, {dt.shape[0]:,} samples, sub:{sub})',y=0.99,color='b')
+        plt.tight_layout(rect=(0,0,1,1))
+
+    def pcmBinning(self,df,widL=None,fx='ROu',fy='SIDD',sigma=None,bins=(6,6),rangeL=None):
+        '''df should be indexed with WID'''
+        widL = widL if widL is not None else df.index.unique().tolist()
+        if sigma!=None:
+            #s1,s2 = sigma_percentage(sigma)
+            dt = self.filterData(df.loc[widL],itemL=[fx,fy],sigma=sigma)
+        else:
+            dt = df.loc[widL][[fx,fy]].dropna()
+        x,y = dt[[fx,fy]].values.T
+        H,binx,biny = np.histogram2d(x,y,bins=bins,range=rangeL)
+        bx,by = (binx[:-1]+binx[1:])/2,(biny[:-1]+biny[1:])/2
+        gx,gy = np.meshgrid(bx,by)
+        tx,ty = gx.ravel(),gy.ravel()
+        dx,dy = (bx[1]-bx[0])/2,(by[1]-by[0])/2
+        yy = H.T.flatten()*100/df.shape[0] # yield
+        d = pd.DataFrame(np.column_stack([tx-dx,ty-dy,tx+dx,ty+dy,yy]),
+            columns=['ROu_left','SIDD_left','ROu_riget','SID_right','Yield'])
+        d['BIN'] = np.arange(1,H.size+1).astype(int)
+        d = d.sort_values(['Yield'],ascending=False).set_index(['BIN'])
+        
+        # projection contour (high quality)
+        H,tbx,tby = np.histogram2d(x,y,bins=(50,50),range=rangeL)
+        tbx,tby = (tbx[:-1]+tbx[1:])/2,(tby[:-1]+tby[1:])/2
+        gx,gy = np.meshgrid(tbx,tby)
+        f,ax = plt.subplots(figsize=(8,7))
+        ax.set_title(f'Bin Yield Assessment ({df.shape[0]:,} samples, {len(widL):,} wafers)')
+        cs = ax.contourf(gx,gy,H.T,levels=30,alpha=0.7) # surface contour
+        f.colorbar(cs,extend='both',shrink=1)
+        for i,(x,y) in enumerate(zip(tx,ty),start=1):
+            e = d.loc[i]['Yield']
+            plt.text(x-dx/3,y-dy/3,f'{i:02d}\n{e:.1f}%',fontsize=12,color='b',bbox={'edgecolor':'w','facecolor':'w','alpha':0.3,'pad':0})
+        plt.xticks(binx)
+        plt.yticks(biny)
+        plt.xlabel(fx)
+        plt.ylabel(fy)
+        plt.grid()
+        plt.minorticks_on()
+        plt.tight_layout(rect=(0,0,1,1))
+        return d.round(2)
+
+    def pcmYieldAssessment(self,df,widL=None,fx='ROu',fy='SIDD',sigma=None,percentiles=[10,20,30],bins=(100,100),sub=1):
+        '''df should be indexed with WID'''
+        widL = widL if widL is not None else df.index.unique().tolist()
+        if sigma!=None:
+            #s1,s2 = sigma_percentage(sigma)
+            dt = self.filterData(df.loc[widL],itemL=[fx,fy],sigma=sigma)
+        else:
+            dt = df.loc[widL][[fx,fy]].dropna()
+            
+        x,y = dt[[fx,fy]].values[::sub].T
+        H, bx, by = np.histogram2d(x, y, bins=bins)
+        bx, by = (bx[:-1]+bx[1:])/2, (by[:-1]+by[1:])/2
+        gx, gy = np.meshgrid(bx, by)
+        
+        S = np.sort(H.ravel()) 
+        cdf = np.cumsum(S)*100/H.sum()
+        idx = [np.argmax(cdf>v) for v in percentiles] # index where cdf>percentile
+        levels = S[idx]
+        ctags = {l:f'{p}%' for l,p in zip(levels,percentiles)} # contour tags
+        
+        G = gridspec.GridSpec(nrows=2,ncols=2,height_ratios=[0.8,0.2],width_ratios=[0.8,0.2])
+        fig = plt.figure(figsize=(10,8))
+        ax = fig.add_subplot(G[0,0],title=f'PCM Yield Assessment ({len(widL):,} wafers, {dt.shape[0]:,} samples, sub:{sub})')
+        tf = ax.contourf(gx, gy, H.reshape(gx.shape).T, levels=10, alpha=0.5, cmap='Blues')
+        tc = ax.contour(gx, gy, H.T, levels=levels, colors=['r','g','b'])
+        cl = ax.clabel(tc, inline=1, fontsize=12, fmt=ctags, inline_spacing=2)
+        ax.set_xlabel(fx)
+        ax.set_ylabel(fy)
+        [txt.set_bbox(dict(facecolor='white', edgecolor='none', pad=1, alpha=0.8)) for txt in cl]
+    
+        # create an axis for the colorbar
+        divider = make_axes_locatable(ax)
+        cax = divider.append_axes('right', size='2%', pad=0.01)
+        cb = plt.colorbar(tf,cax=cax,shrink=0.8,aspect=20)
+        cb.outline.set_visible(False) # 隱藏周圍的框線
+    
+        ax2 = fig.add_subplot(G[0,1]) #title=f'{fy} Density'
+        ax2.hist(y,bins=bins[1],orientation='horizontal')
+        
+        ax3 = fig.add_subplot(G[1,0]) #title=f'{fx} Density'
+        ax3.hist(x,bins=bins[0])
+        plt.tight_layout(rect=(0,0,1,1))
+    
+    ### design recipe/margin optimization (OCV analysis)
+    def d2dDerating(self,df,wid=None,feature='ROu',sd=3,sigma=2.5,detail=False):
         '''
         sd := search distance
         return a distribution of all adjacent die-to-die derating with-in a wafer
             dr := early & late derating table using its searching distance as the hash key
             dm := sigma boundary % of the derating table (dr) grouped by its searching distance 
         '''
         dt = df if wid==None else df.loc[wid]
         d = dt[['X','Y',feature]].groupby(['X','Y']).mean() # resolve indexing problems
-        #d = filterData(dt.reset_index()[['X','Y',feature]],[feature],sigma=sigma)
         s1,s2 = self.sigma_percentage(sigma)
         m = d[feature].describe(percentiles=[s1/100,s2/100]) # !NOTE! need to waive huge gradient
         d = d[(m[f'{s1}%']<=d[feature])&(d[feature]<=m[f'{s2}%'])] # filter outliers
         xyzL = d.reset_index()[['X','Y',feature]].values
         rx,ry = np.arange(-sd,sd+1),np.arange(-sd,sd+1)
         dx,dy = map(np.ravel,np.meshgrid(rx,ry)) # delta search index
         rateL = []
@@ -215,32 +504,30 @@
                 plt.axvline(e,c='b',alpha=0.5,label=f'early={e:.2f}')
                 plt.axvline(l,c='r',alpha=0.5,label=f'late ={l:.2f}')
                 plt.title(f'Adjacent {dist}D {sigma}$\sigma$ {len(rx)}x{len(ry)} ({wid},{len(d)} samples)')
                 plt.ylabel('Density')
                 plt.xlabel('Derating')
                 plt.grid()
                 plt.legend()
-                plt.show()
         # adjacent D2D summary
         if detail>1:
             plt.figure(figsize=(8,5))
             plt.plot(dm.index.values,dm[f'{s1}%'].values,marker='o',label=f'{sigma}$\sigma$ early')
             plt.plot(dm.index.values,dm[f'{s2}%'].values,marker='o',label=f'{sigma}$\sigma$ late')
             plt.axhline(1,c='lightblue',lw=3,alpha=0.8)
             plt.title(f'Adjacent {sd*2+1}x{sd*2+1} D2D {sigma}$\sigma$ ({s1}%,{s2}%)')
             plt.xlabel('Distance')
             plt.ylabel('Derating')
             plt.xticks(np.arange(dm.index.min(),dm.index.max(),0.5))
             plt.legend()
             plt.grid()
-            plt.show()
         return dr,dm
 
     # sigma derating distribution
-    def d2dDeratingSigmaRange(self,df,wid=None,sd=1,sigmaL=[1.65,2.0]):
+    def d2dDeratingSigmaRange(self,df,wid=None,sd=5,sigmaL=[1.65,2.0]):
         dt = df if wid==None else df.loc[wid]
         plt.figure(figsize=(7,8))
         drL,dmL = [],[]
         for i,sigma in enumerate(sigmaL):
             s1,s2 = self.sigma_percentage(sigma=sigma)
             dr,dm = self.d2dDerating(dt,wid,sd=sd,sigma=sigma) # derating with +/-1 search distance 
             plt.plot(dm.index.values,dm[f'{s1}%'].values,marker='o',lw=i+1,c='b',alpha=0.6,label=f'{sigma}$\sigma$ early')
@@ -251,26 +538,26 @@
         plt.title(f'{wid} Adjacent +/-{sd}({sd*2+1}x{sd*2+1}) D2D {sigma}$\sigma$ ({s1}%,{s2}%)')
         plt.xlabel('Distance')
         plt.ylabel('Derating')
         plt.legend()
         plt.grid(which='major',linestyle='-',color='b',alpha=0.5)
         plt.grid(which='minor',linestyle=':',color='b',alpha=0.3)
         plt.minorticks_on()
-        plt.show()
+        plt.tight_layout(rect=(0,0,1,0.98))
         dr = pd.concat(drL,keys=sigmaL,names=['Sigma'])
         dm = pd.concat(dmL,keys=sigmaL,names=['Sigma'])
         return dr,dm
-
-    def polynormFitting(self,dm,order=4):
+    
+    def polynormFitting(self,dm,order=2):
         '''D0 regression based on the die-to-die variation dm (early & late derating) distribution
            dm := mean of the derating table grouped by its searching distance'''
-        x,(y1,y2) = dm.index.values,zip(*dm.values)
+        x,(y1,y2) = dm.index.values,dm.values.T
         X = np.array([np.ones(x.shape)]+[x**i for i in range(1,order+1)]).T
-        C1,_,_,_ = scipy.linalg.lstsq(X,y1) # inner product coefficient (early)
-        C2,_,_,_ = scipy.linalg.lstsq(X,y2) # inner product coefficient (late)
+        C1,_,_,_ = linalg.lstsq(X,y1) # inner product coefficient (early)
+        C2,_,_,_ = linalg.lstsq(X,y2) # inner product coefficient (late)
         t = np.arange(0,np.ceil(x.max()),0.1) # detail grid
         T = np.array([np.ones(t.shape)]+[t**i for i in range(1,order+1)]).T 
         e1 = ' '.join([f'{v:+.1g}t^{i}' for i,v in enumerate(C1)]) # equation
         e2 = ' '.join([f'{v:+.1g}t^{i}' for i,v in enumerate(C2)]) # equation
         p1 = np.dot(T,C1) # predict early
         p2 = np.dot(T,C2) # predict late
         plt.figure(figsize=(6,8))
@@ -282,280 +569,49 @@
         plt.text(0,p2[0],f'{p2[0]:.2f}',c='r') # D0 late derating
         plt.title(f'{e1}\n{e2}')
         plt.xlabel('Distance')
         plt.ylabel('Derating')
         plt.xticks(np.arange(0,dm.index.max(),0.5))
         plt.legend()
         plt.grid()
-        plt.show()
         return p1[0],p2[0] # D0 derating
-
-    # kernel = x,x^alpha,exp(belta*x), alpha=2,belta=0.02
-    def polynormFittingCustomKernel(self,dm,alpha=2,belta=0.02):
-        '''custom D0 regression based on the die-to-die variation dm (early & late derating) distribution'''
-        x,(y1,y2) = dm.index.values,zip(*dm.values)
-        #X = np.array([np.ones(x.shape)]+[x**i for i in range(1,order+1)]).T
-        X = np.array([np.ones(x.shape)]+[x,x**alpha,np.exp(belta*x)]).T # best1
-        C1,_,_,_ = scipy.linalg.lstsq(X,y1) # inner product coefficient (early)
-        C2,_,_,_ = scipy.linalg.lstsq(X,y2) # inner product coefficient (late)
-        t = np.arange(0,np.ceil(x.max()),0.1) # detail grid
-        T = np.array([np.ones(t.shape)]+[t,t**alpha,np.exp(belta*t)]).T # best1
-        e1 = ' '.join([f'{v:+.2g}t^{i}' for i,v in enumerate(C1)]) # equation
-        e2 = ' '.join([f'{v:+.2g}t^{i}' for i,v in enumerate(C2)]) # equation
-        p1 = np.dot(T,C1) # predict early
-        p2 = np.dot(T,C2) # predict late
-        plt.figure(figsize=(6,8))
-        plt.scatter(x,y1,c='b',alpha=0.6) #,label='early (original)')
-        plt.scatter(x,y2,c='r',alpha=0.6) #,label='late  (original)')
-        plt.plot(t,p1,c='b',label=f'early (D0={p1[0]:.2f})')
-        plt.plot(t,p2,c='r',label=f'late  (D0={p2[0]:.2f})')
-        plt.axhline(1,c='lightblue',lw=3,alpha=0.8)
-        plt.text(0,p1[0],f'{p1[0]:.2f}',c='b') # D0 early derating
-        plt.text(0,p2[0],f'{p2[0]:.2f}',c='r') # D0 late derating
-        plt.title(f'{e1}\n{e2}')
-        plt.xlabel('Distance')
-        plt.ylabel('Derating')
-        plt.ylim(bottom=0.8,top=1.3)
-        plt.legend()
-        plt.grid()
-        plt.show()
-        return np.array(p1[0],p2[0]).round(3) # D0 derating
-
-    def waferSort(self,df,itemL=['cumHash','SIDD'],nsize=None):
-        indexL = df.index.names
-        dm = df.groupby(indexL)[itemL].mean().sort_values(itemL,ascending=False)
-        nsize = len(dm) if nsize==None else nsize
-        widL = [str(v) for v in dm.index.tolist()]
-        f = plt.figure(figsize=(15,8))
-        ax1 = f.subplots()
-        ax2 = plt.twinx()  # instantiate a second axes that shares the same x-axis
-        ax1.plot(widL[:nsize],dm[itemL[1]][:nsize],marker='o',ms=5,color='r',zorder=0,alpha=0.5)
-        ax2.plot(widL[:nsize],dm[itemL[0]][:nsize],marker='o',ms=5,color='b',zorder=0,alpha=0.5,picker=5) # picker can only be applied on top
-        ax1.set_xticks(np.arange(0,nsize,1))
-        ax1.set_xticklabels(widL[:nsize],rotation=90)
-        ax1.set_ylabel(itemL[1],color='r')
-        ax2.set_ylabel(itemL[0],color='b')
-        ax1.tick_params(axis='x',rotation=90)
-        ax1.tick_params(axis='y',labelcolor='r')
-        ax2.tick_params(axis='y',labelcolor='b')
-        ax1.grid(color='r',alpha=0.5,zorder=0)
-        ax2.grid(color='b',ls='--',alpha=0.5,zorder=0)
-        #ax2.legend().set_zorder(100)
-        plt.title(f'Wafer Sorting by {itemL} ({nsize} wafers)')
-        plt.subplots_adjust(bottom=0.2,top=0.92,left=0.06,right=0.93)
-        plt.show()
-        ann = ax2.annotate('',xy=(0,0),xytext=(-len(widL[0])*5,20),textcoords="offset points",zorder=100,
-            bbox=dict(boxstyle='round4', fc='linen',ec='k',lw=1),arrowprops=dict(arrowstyle='-|>'))
-        ann.set_visible(False)
-        def onPick(event,ax,df,dm):
-            indL = event.ind
-            wid = dm.index[indL[0]]
-            ann.xy = (event.mouseevent.xdata,event.mouseevent.ydata)
-            ann.set_text(f'{dm.loc[wid]}')
-            ann.set_visible(True)
-            print(f'OnPick: Ind={indL},n={len(indL)}, wid={wid}')
-            print(f'{dm.iloc[indL[0]]}')
-            ax.figure.canvas.draw_idle()
-            self.featureSurface(df,wid,feature='SIDD',sigma=2.5)
-            #self.passCoreProfile(df,wid,volt='035',sigma=1.2)
-        f.canvas.mpl_connect('pick_event',lambda event: onPick(event,ax2,df,dm))
-        return dm
-
-    def passCoreProfile(self,df,wid=None,xyL=None,volt='033',step=20,sigma=2,args={'alpha':0.2,'lw':1,'color':'gray'},figsize=(8,6)):
-        itemPC = ['X','Y']+[v for v in df.columns if f'PC_{volt}' in v]
-        s1,s2 = self.sigma_percentage(sigma=sigma)
-        d = df.loc[wid][itemPC] if wid!=None else df[itemPC]
-        d = d.reset_index()[itemPC].set_index(['X','Y'])
-        d.columns = np.array([v.split('_')[2] for v in d.columns],dtype='int')
-        m = d.describe(percentiles=[s1/100,s2/100]) # sigma bound of all input patterns
-        d = d.loc[xyL] if xyL is not None else d
-        d = d.dropna() 
-        plt.figure(figsize=figsize)
-        plt.title(f'{wid}@{volt} ({len(d)} samples)')
-        for v in d.values[::step]: # sub sampling to speedup the display
-            plt.plot(d.columns.values,v,**args)
-        plt.plot(m.columns.values,m.loc['mean'].values,lw=3,alpha=0.4,color='black',label='$\mu$')
-        plt.plot(m.columns.values,m.loc[f'{s1}%'].values,lw=3,alpha=0.4,color='r',label=f'-{sigma}$\sigma$')
-        plt.plot(m.columns.values,m.loc[f'{s2}%'].values,lw=3,alpha=0.4,color='b',label=f'+{sigma}$\sigma$')
-        plt.xlabel('Frequency (MHz)')
-        plt.ylabel('Pass Core#')
-        plt.grid()
-        plt.legend()
-        plt.subplots_adjust(left=0.08,bottom=0.1,right=0.95,top=0.95,wspace=0.01,hspace=0.01)
-        plt.show()
-        return d
-
-    def passCoreProfile3D(self,df,wid=('LotID',1),volt='031',sigma=2.5,step=50,level=0.5,line=True):
-        #dt = self.filterData(df[df.index.str.contains(wid)],itemL=['SIDD'],sigma=sigma)
-        itemPC = ['X','Y','SIDD']+[v for v in df.columns if f'PC_{volt}' in v]
-        freqL = np.array([v.split('_')[-1] for v in df.columns if f'PC_{volt}' in v],int)
-        dt = df.loc[wid][itemPC] if wid!=None else df[itemPC]
-        dt = dt.reset_index()[itemPC].set_index(['X','Y'])
-        f = plt.figure(figsize=(8,7))
-        ax = Axes3D(f)
-        #level = 0.5
-        for sidd,*pc in dt.values[::step,:]:
-            order = int(sidd/level)
-            color = self.colL[order%len(self.colL)]
-            if line:
-                ax.plot(freqL,pc,sidd,alpha=0.1,marker='o',ms=2,c=color,zorder=order) # line
-            else:
-                ax.scatter(freqL,pc,sidd,alpha=0.3,marker='o',s=20,c=color,zorder=order) # scatter
-        tt = dt.copy()
-        tt['SIDD'] = (dt['SIDD']/level).astype(int)*level
-        tm = tt.groupby(['SIDD']).mean().round(2)
-        for ii,sidd in enumerate(tm.index):
-            color = self.colL[ii%len(self.colL)]
-            ax.plot(freqL,tm.loc[sidd].values,sidd,alpha=0.8,lw=3,label=f'{sidd}')
-        ax.set_title(f'{wid}@{volt.replace("0","0.")}V {sigma}$\sigma$ ({len(dt)} smaples)')
-        ax.set_xlabel('Freq')
-        ax.set_ylabel('PassCore#')
-        ax.set_zlabel('SIDD')
-        ax.view_init(60,250)       
-        ax.legend(title='SIDD Level')
-        plt.subplots_adjust(left=0.08,bottom=0.08,right=0.95,top=0.95,wspace=0.01,hspace=0.01)
-        plt.show()
-        return dt
-
-    # scatter matrix (where cumHash>100)
-    def scatterMatrix(self,df,itemL,s=10,alpha=0.3): 
-        corr = df[itemL].corr().values.ravel()
+    
+    ### CP-WAT cross-domain features correlation & process recipe optimization
+    def surfaceContour(self,df,fx,fy,fz,fsize=(7,6),levels=10):
+        dt = df[[fx,fy,fz]].groupby(['WID']).mean() # apply wafer mean for reciple contour
+        dm = dt.groupby(by=[fx,fy]).mean().reset_index()
+        mm = dm[[fx,fy]].mean()
+        x,y,z = dm[[fx,fy,fz]].values.T
+        f,ax = plt.subplots(1,1)
+        f.set_size_inches(fsize)
+        su = ax.tricontourf(x,y,z,levels=levels) #np.linspace(trange[0],trange[1],20))
+        ax.scatter(mm[fx],mm[fy],marker='+',s=200,lw=2,c='y',alpha=0.8)
+        ax.text(mm[fx],mm[fy],f'{mm[[fx,fy]].values.round(3)}',c='w',fontsize=12)
+        name = '_'.join(df.index.names)
+        ax.set_title(f'{fz} {name}: {len(dm)} locations, {df.shape[0]:,} samples')
+        ax.set_xlabel(fx)
+        ax.set_ylabel(fy)
+        ax.grid(which='major',lw=1,color='r',alpha=0.3)
+        ax.grid(which='minor',lw=1,color='gray',ls=':',alpha=0.3)
+        ax.minorticks_on()  
+        #ax.set_zlim(bottom=0,top=512)
+        cb = f.colorbar(su,shrink=0.8,aspect=20) #ticks=range(0,520,50))
+        cb.ax.tick_params(labelsize=10)    
+        plt.tight_layout(rect=(0,0,1,0.98))
+    
+    def scatterMatrix(self,df,itemL,s=10,alpha=0.3,sub=10): 
+        corr = df[itemL].iloc[::sub].corr().values.ravel()
         axes = pd.plotting.scatter_matrix(
             df[itemL],figsize=(10,9),s=s,hist_kwds={'bins':30},alpha=alpha)
         for ii,ax in enumerate(axes.ravel()):
             ax.annotate(f'{corr[ii]:.2g}',(0.7,0.7),xycoords='axes fraction',ha='center',va='center',fontsize=12)
             ax.set_xlabel(ax.get_xlabel(),fontsize=10,rotation=0,color='b')
             ax.set_ylabel(ax.get_ylabel(),fontsize=10,rotation=0,color='b')
             ax.xaxis.set_label_coords(0.5,-0.2)
             ax.yaxis.set_label_coords(-0.1,0.5)
             #ax.xaxis.label.set_fontsize(8); ax.xaxis.label.set_rotation(30)
-        plt.subplots_adjust(left=0.08,bottom=0.1,right=0.98,top=0.96)
-        plt.suptitle(f'feature correlation matrix ({len(df)} samples)')
+        plt.suptitle(f'feature correlation ({len(df):,} samples, sub={sub})')
+        plt.tight_layout(rect=(0,0,1,1))
         return corr.round(3)
-
-    def pcmDensity3D(self,df,widL=None,fx='ROu',fy='SIDD',sigma=None,view=(60,240),bins=(10,10),rangeL=None):
-        widL = widL if widL is not None else df.index.unique().tolist()
-        if sigma!=None:
-            dt = self.filterData(df.loc[widL],itemL=[fx,fy],sigma=sigma)
-        else:
-            dt = df.loc[widL][[fx,fy]].dropna()
-        x,y = dt[fx].values,dt[fy].values
-        H,binx,biny = np.histogram2d(x,y,bins=bins,range=rangeL,normed=False)
-        gx,gy = np.meshgrid(binx[1:],biny[1:])
-        f = plt.figure(figsize=(11,9))
-        ax = Axes3D(f)
-        ax.contour(gx,gy,H.T,zdir='x',levels=30,offset=dt[fx].max()*1.1) 
-        ax.contour(gx,gy,H.T,zdir='y',levels=30,offset=0) 
-        ax.contour(gx,gy,H.T,levels=30,linewidths=2)  # line contour
-        cs = ax.contourf(gx,gy,H.T,levels=30,offset=0) # surface contour, project to z=0
-        f.colorbar(cs,extend='both',shrink=0.8) #,aspect=30)
-        #ax.clabel(cs,fmt='%2.3f',colors='b',fontsize=14,inline=True) # inline notation
-        ax.plot_surface(
-            gx,gy,H.T,zorder=0,alpha=0.6,
-            antialiased=False,linewidth=0,edgecolors='none',
-            cmap=plt.cm.Blues_r) #,cmap=plt.cm.viridis)
-        ax.set_title(f'PCM Histogram {sigma}$\sigma$ ({len(widL)} wafers)')
-        ax.set_xlabel(fx)
-        ax.set_ylabel(fy)
-        ax.set_zlabel('Density')
-        ax.view_init(view[0],view[1])
-        #plt.setp(cs.collections,linewidth=2)
-        plt.subplots_adjust(left=0.08,bottom=0.1,right=0.98,top=0.95)
-        plt.show()
-        return binx,biny,H.T
-
-    def pcmDensity2D(self,df,widL=None,fx='cumHash',fy='SIDD',sigma=None,bins=(20,20),rangeL=None):
-        widL = widL if widL is not None else df.index.unique().tolist()
-        if sigma!=None:
-            dt = self.filterData(df.loc[widL],itemL=[fx,fy],sigma=sigma)
-        else:
-            dt = df.loc[widL][[fx,fy]].dropna()
-        # projection contour
-        x,y = dt[fx].values,dt[fy].values
-        H,binx,biny = np.histogram2d(x,y,bins=bins,range=rangeL,normed=False)
-        gx,gy = np.meshgrid(binx[1:],biny[1:])
-        f,ax = plt.subplots()
-        f.set_size_inches((11,9))
-        #cs = ax.contour(gx,gy,H.T,levels=30,linewidths=3,alpha=0.7) # line contour
-        cs = ax.contourf(gx,gy,H.T,levels=30,alpha=0.7) # surface contour
-        f.colorbar(cs,extend='both',shrink=1)
-        ax.set_title(f'PCM Histogram {sigma}$\sigma$ ({len(widL)} wafers)')
-        ax.set_xlabel(fx)
-        ax.set_ylabel(fy)
-        plt.subplots_adjust(left=0.08,bottom=0.08,right=1.0,top=0.95)
-        plt.grid(which='major',lw=1,color='r',alpha=0.7)
-        plt.grid(which='minor',lw=1,color='gray',ls=':',alpha=0.5)
-        plt.minorticks_on()
-        plt.show()
-        return binx,biny,H.T
-    
-    def hardBinning(self,dt,fx='cumHash',fy='SIDD',bins=(6,8),rangeL=[(100,700),(1,9)],ylimit=1):
-        '''return hard-bin and soft-bin based on the specified XY bin ranges, when yield>ylimit'''
-        x,y = dt[fx].values,dt[fy].values
-        H,binx,biny = np.histogram2d(x,y,bins=bins,range=rangeL,normed=False)
-        gx1,gy1 = np.meshgrid(binx[:-1],biny[:-1])
-        gx2,gy2 = np.meshgrid(binx[1:],biny[1:])
-        rbin = pd.DataFrame({ # all avaliable bins
-            f'{fx}_Down':gx1.flatten(),f'{fx}_Up':gx2.flatten(),
-            f'{fy}_Down':gy1.flatten(),f'{fy}_Up':gy2.flatten(),
-            'Yield':H.T.flatten()*100/len(dt)})
-        rbin = rbin[rbin['Yield']>0].sort_values([f'{fx}_Down','Yield'],ascending=False)
-        rbin['BIN'] = np.arange(1,len(rbin)+1)
-        rbin = rbin.set_index(['BIN'])
-        hbin = rbin[rbin['Yield']>=ylimit] # remain yield > ylimit%
-        hbin['BIN'] = np.arange(1,len(hbin)+1)
-        hbin = hbin.set_index(['BIN'])
-        hbin['Yield'].sum()
-        return hbin,rbin
-
-    def pcmBinning(self,df,widL=None,fx='cumHash',fy='SIDD',sigma=None,outDir=None,bins=(20,20),rangeL=None,ylimit=1):
-        widL = widL if widL is not None else df.index.unique().tolist()
-        if sigma!=None:
-            #s1,s2 = sigma_percentage(sigma)
-            dt = self.filterData(df.loc[widL],itemL=[fx,fy],sigma=sigma)
-        else:
-            dt = df.loc[widL][[fx,fy]].dropna()
-        # projection contour
-        x,y = dt[fx].values,dt[fy].values
-        H,binx,biny = np.histogram2d(x,y,bins=(100,100),range=rangeL,normed=False)
-        gx,gy = np.meshgrid(binx[1:],biny[1:])
-        f,ax = plt.subplots()
-        f.set_size_inches((11,9))
-        #cs = ax.contour(gx,gy,H.T,levels=30,linewidths=3,alpha=0.7) # line contour
-        cs = ax.contourf(gx,gy,H.T,levels=30,linewidths=3,alpha=0.7) # surface contour
-        f.colorbar(cs,extend='both',shrink=1)
-        # binning
-        hbin,rbin = self.hardBinning(dt,fx,fy,bins=bins,rangeL=rangeL,ylimit=ylimit)
-        bx,by = hbin.iloc[:,0:2].mean(axis=1),hbin.iloc[:,2:4].mean(axis=1) # bin center coor
-        for i,(x,y) in enumerate(zip(bx,by)):
-            #plt.text(x-20,y-0.25,f'[{i+1:02d}]\n{hbin["Yield"][i+1]:.1f}%',fontsize=16,color='b',bbox={'edgecolor':'w','facecolor':'w','alpha':0.8,'pad':0})
-            plt.text(x,y,f'[{i+1:02d}]\n{hbin["Yield"][i+1]:.1f}%',fontsize=12,color='b',bbox={'edgecolor':'w','facecolor':'w','alpha':0.8,'pad':0})
-            print(f'BIN {i+1:02d}: {hbin["Yield"][i+1]:.1f}%')
-        ax.set_title(f'Binning Strategy ({len(widL)} wafers)')
-        ax.set_xlabel(fx)
-        ax.set_ylabel(fy)
-        plt.subplots_adjust(left=0.08,bottom=0.08,right=1.0,top=0.95)
-        plt.grid(which='major',lw=2,color='r',alpha=0.8)
-        plt.grid(which='minor',lw=1,color='gray',ls=':',alpha=0.5)
-        plt.minorticks_on()
-        plt.show()
-        return hbin,rbin
-
-    def mapCPMachine(self,df_cp,df_me,outCSV=None):
-        '''map CP DB (df_cp) with machine-efuse DB (df_me)'''
-        df_cp = df_cp.set_index(['LWID','X','Y'])
-        df_me['LWID'] = [f'{l}_{w}' for l,w in df_me[['LOTID','CPWID']].values]
-        df_me = df_me.set_index(['LWID','CPX','CPY'])
-        # grab mutually inclusive index first
-        idx = sorted(set(df_cp.index)&set(df_me.index))
-        print(f'total {len(idx):,d} mutually inclusive samples in both CP & machine DB')
-        dc = df_cp.loc[idx] # (376852, 31)
-        dm = df_me.loc[idx] # (376852, 14)
-        dx = pd.concat([dc,dm],axis=1) # (376852, 45)     
-        if outCSV!=None:
-            dx.reset_index().to_csv(outCSV,float_format='%g',index=False)
-            print(f'CP & machine mapping DB was saved into {outCSV}: {dx.shape}')
-        return dx
-
-cpanalyzer = CPAnalysis()
-
+        
+dtco = DTCO()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DTCO-0.1.2/libMetric/classLiberty.py` & `DTCO-0.1.3/libMetric/classLiberty.py`

 * *Files identical despite different names*

