# Comparing `tmp/EnjoyAnimation-0.0.3.tar.gz` & `tmp/EnjoyAnimation-0.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnjoyAnimation-0.0.3.tar", last modified: Thu May 11 11:08:28 2023, max compression
+gzip compressed data, was "EnjoyAnimation-0.0.4b0.tar", last modified: Fri May 12 10:03:02 2023, max compression
```

## Comparing `EnjoyAnimation-0.0.3.tar` & `EnjoyAnimation-0.0.4b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:08:28.940386 EnjoyAnimation-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-11 11:08:28.926423 EnjoyAnimation-0.0.3/EnjoyAnimation/
--rw-rw-rw-   0        0        0    25359 2023-05-09 08:14:41.000000 EnjoyAnimation-0.0.3/EnjoyAnimation/EnjoyAnimation.py
--rw-rw-rw-   0        0        0       29 2023-05-09 08:30:32.000000 EnjoyAnimation-0.0.3/EnjoyAnimation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:08:28.937396 EnjoyAnimation-0.0.3/EnjoyAnimation.egg-info/
--rw-rw-rw-   0        0        0     2109 2023-05-11 11:08:28.000000 EnjoyAnimation-0.0.3/EnjoyAnimation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-11 11:08:28.000000 EnjoyAnimation-0.0.3/EnjoyAnimation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:08:28.000000 EnjoyAnimation-0.0.3/EnjoyAnimation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-11 11:08:28.000000 EnjoyAnimation-0.0.3/EnjoyAnimation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 11:08:28.000000 EnjoyAnimation-0.0.3/EnjoyAnimation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-05-09 08:14:41.000000 EnjoyAnimation-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2109 2023-05-11 11:08:28.940386 EnjoyAnimation-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1700 2023-05-09 08:14:41.000000 EnjoyAnimation-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 11:08:28.941383 EnjoyAnimation-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-05-11 11:08:25.000000 EnjoyAnimation-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:03:02.842722 EnjoyAnimation-0.0.4b0/
+drwxrwxrwx   0        0        0        0 2023-05-12 10:03:02.827655 EnjoyAnimation-0.0.4b0/EnjoyAnimation/
+-rw-rw-rw-   0        0        0    25605 2023-05-12 09:22:30.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation/EnjoyAnimation.py
+-rw-rw-rw-   0        0        0       29 2023-05-09 08:39:57.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:03:02.839145 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/
+-rw-rw-rw-   0        0        0     2834 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-05-06 02:32:29.000000 EnjoyAnimation-0.0.4b0/LICENSE
+-rw-rw-rw-   0        0        0     2834 2023-05-12 10:03:02.841148 EnjoyAnimation-0.0.4b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2423 2023-05-12 09:24:31.000000 EnjoyAnimation-0.0.4b0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 10:03:02.843640 EnjoyAnimation-0.0.4b0/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-05-12 09:50:44.000000 EnjoyAnimation-0.0.4b0/setup.py
```

### Comparing `EnjoyAnimation-0.0.3/EnjoyAnimation/EnjoyAnimation.py` & `EnjoyAnimation-0.0.4b0/EnjoyAnimation/EnjoyAnimation.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 require("nonebot_plugin_htmlrender")
 from nonebot_plugin_htmlrender import (
     text_to_pic,
 )
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
-plugin_version="beta 0.0.3"
+plugin_version="0.0.4b0"
 animation=on_command("番剧更新")
 animation_infor=on_command("番剧信息")
 search_number=on_command("番剧查询")
 animation_help=on_command("番剧帮助")
 upgrade_animation_today=on_command("今日新番")
-emmmm=on_keyword(keywords=["emm","233","hhh","哈哈哈","6","哦哦","奥奥","嗯嗯","哈哈","呃呃"])#5bCx5L2g5pW36KGN5oiR5piv5ZCn😅
+emmmm=on_keyword(keywords=["哦哦","奥奥","呃呃"])#5bCx5L2g5pW36KGN5oiR5piv5ZCn😅
 sub_drama=on_command("新增追番")
 sub_sub_drama=on_command("取消追番")
 sub_drama_list=on_command("我的追番")
 async def admin_check(event:MessageEvent) -> bool:
     animation_config=get_driver().config
     animation_admin=animation_config.animation_admin
     return animation_admin==event.user_id
@@ -51,101 +51,105 @@
     "User-Agent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.0.0"
 }
 animation_config=get_driver().config
 animation_tmp=animation_config.animation_time
 animation_default_return_img=animation_config.animation_default_return_img
 animation_hour=animation_tmp[0]
 animation_minute=animation_tmp[1]
+work_path=os.path.join(os.getcwd(),"data")#指向data路径
+pic_path=os.path.join(work_path,"Animation_pic")#指向pic路径
+animation_path=os.path.join(work_path,"animations.json")#指向animation.json文件路径
+User_setting_path=os.path.join(work_path,"User_setting.json")#指向user setting.json文件路径
+img_tmp_path=os.path.join(pic_path,"img.jpg")#指向临时图片路径
+os.makedirs(pic_path,exist_ok=True)
 
 def animation_informtions() -> None:#爬取番剧详细信息
-    with open("animations.json","w",encoding="utf-8") as f:
-        global month
+    with open(animation_path,"w",encoding="utf-8") as f:
         url="https://yuc.wiki/"+str(datetime.now().year)+(month[datetime.now().month-1])+"/"#拼接成当前季度番剧的查询网址
         url_html=requests.get(url=url,headers=yuc_header)
         url_txt=url_html.text
         url_structure=BeautifulSoup(url_txt,"html.parser")
         animation_all=url_structure.find_all("div",attrs={"style":"float:left"})
         classesX=["date_title","date_title_","date_title__"]
         data={}
-        os.makedirs("pic",exist_ok=True)
-        work_path="file:///"+os.getcwd()+"\\pic\\"
         def animation_information(classes):
             for animation_boki in animation_all:
                 try:
                     animation_name=animation_boki.find("td",attrs={"class":classes}).get_text()
                     animation_urls=animation_boki.find_all("a")
                     animation_pic_url=animation_boki.find("img")
                     animation_pic=requests.get(url=animation_pic_url["src"],headers=yuc_header)
                 except AttributeError:
                     continue
                 animation_href=[a["href"] for a in animation_urls]
-                with open (file=".\\pic\\img.jpg",mode="wb") as p:
+                with open (img_tmp_path,mode="wb") as p:
                     p.write(animation_pic.content)
                 try:
-                    os.rename(p.name,f".\\pic\\{animation_name}.jpg")
+                    os.rename(p.name,os.path.join(pic_path,f"{animation_name}.jpg"))
                 except:
-                    os.remove(".\\pic\\img.jpg")
+                    os.remove(img_tmp_path)
                     pass
                 try:
                     animation_date=str(datetime.now().year)+"/"+animation_boki.find("p",attrs={"class":"imgtext"}).get_text()[:-1]
                     animation_week=datetime.strptime(animation_date,"%Y/%m/%d").strftime("%A")
                     animation_times=animation_boki.find("p",attrs={"class":"imgep"}).get_text()[:-1]
                 except  AttributeError:
                     animation_date,animation_week,animation_times=None,None,None
                     pass
+                tmp=os.path.join(pic_path,f"{animation_name}.jpg")
                 animation_hrefs={"urls":animation_href,
-                                 "path":f"{work_path}{animation_name}.jpg",
+                                 "path":f"file:///{tmp}",
                                  "date":animation_date,
                                  "week":animation_week,
                                  "time":animation_times
                                  }
                 data[animation_name]=(animation_hrefs)
         for classes in classesX:
             animation_information(classes) 
         json.dump(data,f,indent=4,ensure_ascii=False)
 def r_animation_informations_name():#读取番剧json文本信息，读取番剧名称
-    with open("animations.json","r",encoding="utf-8") as r:
+    with open(animation_path,"r",encoding="utf-8") as r:
         work_r=json.load(r)
         return(work_r.keys())
 def r_animation_informations_num_to_name(number:int):#通过序列号查询名字
     return str(list(r_animation_informations_name())[number-1])
 def r_animation_information_path(names) ->str:#通过名称寻找路径
-    with open("animations.json","r",encoding="utf-8") as r:
+    with open(animation_path,"r",encoding="utf-8") as r:
         tmp=json.load(r)
         return tmp[names]["path"]
 def r_animation_information_url(names) -> str:#通过名称寻找网址
-    with open("animations.json","r",encoding="utf-8") as r:
+    with open(animation_path,"r",encoding="utf-8") as r:
         tmp=json.load(r)
         return(tmp[names]["urls"])
 def r_animation_information_date(names) -> str:#返回番剧首播日期
-    with open("animations.json","r",encoding="utf-8") as r:
+    with open(animation_path,"r",encoding="utf-8") as r:
         tmp=json.load(r)
         if tmp[names]["date"]==None:
             return ""
         return(tmp[names]["date"])
 def r_animation_information_week(names)->str:#返回番剧更新周几
-    with open("animations.json","r",encoding="utf-8") as r:
+    with open(animation_path,"r",encoding="utf-8") as r:
         tmp=json.load(r)
         if tmp[names]["week"]==None:
             return " "
         return(tmp[names]["week"])
 def r_animation_information_time(names)->str:#返回当日更新时间
-    with open("animations.json","r",encoding="utf-8") as r:
+    with open(animation_path,"r",encoding="utf-8") as r:
         tmp=json.load(r)
         if tmp[names]["time"]==None:
             return ""
         return(tmp[names]["time"])
 def file_json_store() -> None:#检测json文件是否存在,若存在则跳过，不存在则创建,
     try:
-        with open("animations.json","x",encoding="utf-8"):
+        with open(animation_path,"x",encoding="utf-8"):
             animation_informtions()
             return 0
     except:
         pass
-    with open("animations.json","r",encoding="utf-8") as f:
+    with open(animation_path,"r",encoding="utf-8") as f:
         tmp=json.load(f)
         tmp_y=datetime.strptime(tmp[list(tmp.keys())[0]]["date"],"%Y/%m/%d").strftime("%Y")
         tmp_m=datetime.strptime(tmp[list(tmp.keys())[0]]["date"],"%Y/%m/%d").strftime("%m")
         if int(tmp_y) != datetime.now().year or month[int(tmp_m)-1] != month[datetime.now().month]:
             animation_informtions()
         else:
             pass
@@ -222,72 +226,72 @@
     r_message=f"今日番剧【{today_week}】\n"+r_message
     try:
         await text_to_img(bot,message=r_message,group=group,user=user)
     except:
         await bot.finish(Message(f"可能被风控了捏！{random.choice(random_face)}"))
 def load_user_setting()->list:#返回用户设置
     try:
-        with open("User_setting.json","r",encoding="utf-8") as f:
+        with open(User_setting_path,"r",encoding="utf-8") as f:
             tmp=json.load(f)
             sub_qq_group=tmp["sub_qq_group"]
             Users_sub=tmp["Users_sub"]
             Users_sub_animation=tmp["Users_sub_animation"]
             sub_time=tmp["sub_time"]
             tmp_version=tmp["version"]
             return [sub_qq_group,Users_sub,Users_sub_animation,sub_time,tmp_version]
     except KeyError:
         return [None,None,None,None,None]
 def user_file_json():#检测是否存在用户配置文件 无则创建
     global plugin_version
-    if not os.path.exists("User_setting.json"):
-        with open("User_setting.json","w",encoding="utf-8") as r:
+    if not os.path.exists(User_setting_path):
+        with open(User_setting_path,"w",encoding="utf-8") as r:
             data_tmp={
                 "sub_qq_group":[],
                 "Users_sub":[],
                 "Users_sub_animation":{},
                 "sub_time":[],
                 "version":plugin_version
             }
             json.dump(data_tmp,r,indent=4,ensure_ascii=False) 
     try:
         if load_user_setting()[4]!=plugin_version:
-            with open("User_setting.json","r",encoding="utf-8") as f:
+            with open(User_setting_path,"r",encoding="utf-8") as f:
                 tmp=json.load(f)
                 for i in ["sub_qq_group","Users_sub","Users_sub_animation","sub_time","version"]:
                     if i not in list(tmp.keys()):
                         if i!="version":
                             tmp[i]=[]
                         else:
                             tmp[i]=plugin_version
                 tmp["version"]=plugin_version
-            with open("User_setting.json","w",encoding="utf-8") as f:
+            with open(User_setting_path,"w",encoding="utf-8") as f:
                 json.dump(tmp,f,indent=4,ensure_ascii=False) 
     except json.JSONDecodeError:
-        os.remove("User_setting.json")
+        os.remove(User_setting_path)
         user_file_json()
 user_file_json()
 async def add_user_sub_animation(bot:Bot,event:MessageEvent,numbers):#添加用户追番
     num_list=str(numbers).split(" ")
     msg=""
-    with open("User_setting.json","r",encoding="utf-8") as f:
+    with open(User_setting_path,"r",encoding="utf-8") as f:
         tmp_1=json.load(f)
         if str(event.user_id) not in list(tmp_1["Users_sub_animation"].keys()):
             tmp_1["Users_sub_animation"][str(event.user_id)]=[]
-    with open("User_setting.json","w",encoding="utf-8") as f:
+    with open(User_setting_path,"w",encoding="utf-8") as f:
         json.dump(tmp_1,f,indent=4,ensure_ascii=False)
     for i in num_list:
         try:
             if 0<=int(i)<=len(list(r_animation_informations_name())):
                 i_name=r_animation_informations_num_to_name(int(i))
-                with open("User_setting.json","r",encoding="utf-8") as f:
+                with open(User_setting_path,"r",encoding="utf-8") as f:
                     tmp=json.load(f)
                     if i_name not in tmp["Users_sub_animation"][str(event.user_id)]:
                         tmp["Users_sub_animation"][str(event.user_id)].append(i_name)
                         msg+=i_name+"\n"
-                with open("User_setting.json","w",encoding="utf-8") as f:
+                with open(User_setting_path,"w",encoding="utf-8") as f:
                     json.dump(tmp,f,indent=4,ensure_ascii=False)
         except:
             pass
     if msg:
         try:
             await bot.finish(f"{msg}\n已新增至【{event.user_id}】的追番列表")   
         except ActionFailed:
@@ -360,15 +364,15 @@
     bot=get_bot()
     for i in load_user_setting()[0]:
         await animation_today_(bot=bot,group=i)
     for i in load_user_setting()[1]:
         await animation_today_(bot=bot,user=i)
 @everyday_push.got("tmp",prompt=f"是否订阅每日推送 Y/N")#新增订阅
 async def everyday_push_setting(bot:Bot,event:MessageEvent):
-    with open("User_setting.json","r",encoding="utf-8") as f:
+    with open(User_setting_path,"r",encoding="utf-8") as f:
         tmp1=event.get_plaintext()
         tmp1_txt=str(tmp1)
         tmp_json=json.load(f)
         if (tmp1_txt) in ["y","Y","是","yes","Yes","1"]:
             try:
                 qq_group=int(event.group_id)
                 if (qq_group not in load_user_setting()[0]) and await (admin_check(event)):
@@ -384,19 +388,19 @@
                 if user_qq not in load_user_setting()[1]:
                     tmp_json["Users_sub"].append(user_qq)
                     await everyday_push.send(message=f'QQ：{user_qq}已新增至订阅')
                 else:
                     await everyday_push.send(message=f'QQ：{user_qq}不可重复订阅')
         else:
             await everyday_push.finish(message=random.choice(random_face))
-    with open("User_setting.json","w",encoding="utf-8") as f:
+    with open(User_setting_path,"w",encoding="utf-8") as f:
         json.dump(tmp_json,f,indent=4,ensure_ascii=False)
 @everyday_push_off.got("tmp",prompt=f"是否取消每日推送 Y/N")#取消订阅
 async def everyday_push_off_setting(bot:Bot,event:MessageEvent):
-    with open("User_setting.json","r",encoding="utf-8") as f:
+    with open(User_setting_path,"r",encoding="utf-8") as f:
         tmp1=event.get_plaintext()
         tmp1_txt=str(tmp1)
         tmp_json=json.load(f)
         if (tmp1_txt) in ["y","Y","是","yes","Yes","1"]:
             try:
                 qq_group=int(event.group_id)
                 if (qq_group in load_user_setting()[0]) and await (admin_check(event)):
@@ -412,15 +416,15 @@
                 if user_qq in load_user_setting()[1]:
                     tmp_json["Users_sub"].remove(user_qq)
                     await everyday_push_off.send(message=f'QQ：{user_qq}已取消订阅')
                 else:
                     await everyday_push_off.send(message=f'QQ：{user_qq}无订阅信息')
         else:
             await everyday_push_off.finish(message=random.choice(random_face))
-    with open("User_setting.json","w",encoding="utf-8") as f:
+    with open(User_setting_path,"w",encoding="utf-8") as f:
         json.dump(tmp_json,f,indent=4,ensure_ascii=False)
 @emmmm.handle()#u know,that's right
 async def emm():
     await emmmm.finish(message=Message(random.choice(random_face)))
 @sub_drama.handle()#新增追番
 async def sub_dramas(bot:Bot,event:MessageEvent,numbers:Message=CommandArg()):
     if str(numbers):
@@ -451,15 +455,15 @@
     for i in sub_list:
         num+=1
         msg+=f"{num}，{i}\n"
     await text_to_img(sub_sub_drama,msg)
     await sub_sub_drama.send(f"请发送编号捏{random.choice(random_face)}#")
 @sub_sub_drama.got("key")
 async def sub_sub_list_get(bot:Bot,event:MessageEvent):
-    with open("User_setting.json","r",encoding="utf-8") as f:
+    with open(User_setting_path,"r",encoding="utf-8") as f:
         sub_list=event.get_plaintext().split(" ")
         tmp=json.load(f)
         msg,remove_ani="",[]
         if "all" in sub_list:
             tmp["Users_sub_animation"].pop(str(event.user_id))
             for i in sub_list:
                 msg+=i+"\n"
@@ -474,15 +478,15 @@
             if not tmp["Users_sub_animation"][str(event.user_id)]:
                 tmp["Users_sub_animation"].pop(str(event.user_id))
         for i in remove_ani:
             msg+=i+'\n'
         msg=f"已取消追番：\n{msg}"
         if not remove_ani:
             await sub_sub_drama.finish(random.choice(random_face))
-    with open("User_setting.json","w",encoding="utf-8") as f:
+    with open(User_setting_path,"w",encoding="utf-8") as f:
         json.dump(tmp,f,indent=4,ensure_ascii=False)
     await text_to_img(sub_sub_drama,msg)
     await sub_sub_drama.finish()
 @scheduler.scheduled_job("interval",minutes=1)#追番更新提醒
 async def user_sub():
     sub_list=load_user_setting()[2]
     for qq_user in sub_list:
```

### Comparing `EnjoyAnimation-0.0.3/EnjoyAnimation.egg-info/PKG-INFO` & `EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnjoyAnimation
-Version: 0.0.3
+Version: 0.0.4b0
 Summary: 基于nonebot与gocqhttp的动漫番剧插件
 Home-page: https://github.com/small-bili/nonebot-plugin-EnjoyAnimation
 Author: slexce
 Author-email: sim69732@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -15,15 +15,36 @@
 
 ### 插件依赖
 插件：```nonebot-plugin-apscheduler nonebot-plugin-htmlrender```
 
 库：```bs4 requests```
 
 ### 安装插件
-由于并没有上传至PyPI，只能手动安装
+#### 自动安装
+
+安装此插件：
+```
+pip install EnjoyAnimation
+（若镜像站没有则使用以下指令进行安装）
+pip install --index-url https://pypi.org/simple EnjoyAnimation
+```
+安装第三方插件依赖：
+请在bot根目录运行此指令
+```
+nb plugin install nonebot-plugin-apscheduler
+```
+```
+nb plugin install nonebot-plugin-htmlrender
+```
+添加插件：
+```
+在pyproject.toml文件中将EnjoyAnimation添加进plugins中
+plugins = ["EnjoyAnimation"]
+```
+#### 手动安装
 
 1. 安装第三方库
 ```
 pip install bs4
 ```
 ```
 pip install requests
@@ -43,27 +64,28 @@
 ```
 plugin_dirs = ["src/plugins"]
 ```
 ### 配置插件
 
 插件有三项必须配置项
 
-配置文件为.env.dev（默认为此文件，.env中可以修改）文件
+配置文件为.env.X（默认为[初学者模式创建时]```.env.prof```或者[插件作者创建时]```.env.dev```，具体```.env```中可以修改）文件
 ```
 animation_admin=123456789            #管理员qq号
 animation_time= [8,30]               #订阅提醒时间，[0~23,0~59]
 animation_default_return_img=false   #一些番剧信息是否以图片发送（配置为false时，检测到风控会自动以图片进行发送）
 ```
 ### 插件使用
 ```
     Commands:【可选参数】
-    #番剧信息 【当前季度的番剧】
-    #番剧更新 【强制更新番剧信息】
-    #今日新番 【今日更新的番剧】
-    #新增订阅 【订阅=追番提醒】
-    #取消订阅
+    番剧帮助 （查看指令用法）
+    番剧信息 （当前季度的番剧）
+    番剧更新 （强制更新番剧信息）
+    今日新番 （今日更新的番剧）
+    新增订阅 （订阅=追番提醒）
+    取消订阅 （取消追番提醒）
     ==================== 
-    #番剧查询 【番剧信息中的序号】
-    #新增追番 【番剧信息中的序号】
-    #我的追番 【查看追番列表】
-    #取消追番
+    番剧查询 【番剧信息中的序号，如12 23 4 51这种数字列表】
+    新增追番 【番剧信息中的序号，也支持数字列表】
+    我的追番 （查看追番列表）
+    取消追番 【追番中的番剧序号，支持数字列表】
 ```
```

### Comparing `EnjoyAnimation-0.0.3/LICENSE` & `EnjoyAnimation-0.0.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `EnjoyAnimation-0.0.3/PKG-INFO` & `EnjoyAnimation-0.0.4b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnjoyAnimation
-Version: 0.0.3
+Version: 0.0.4b0
 Summary: 基于nonebot与gocqhttp的动漫番剧插件
 Home-page: https://github.com/small-bili/nonebot-plugin-EnjoyAnimation
 Author: slexce
 Author-email: sim69732@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -15,15 +15,36 @@
 
 ### 插件依赖
 插件：```nonebot-plugin-apscheduler nonebot-plugin-htmlrender```
 
 库：```bs4 requests```
 
 ### 安装插件
-由于并没有上传至PyPI，只能手动安装
+#### 自动安装
+
+安装此插件：
+```
+pip install EnjoyAnimation
+（若镜像站没有则使用以下指令进行安装）
+pip install --index-url https://pypi.org/simple EnjoyAnimation
+```
+安装第三方插件依赖：
+请在bot根目录运行此指令
+```
+nb plugin install nonebot-plugin-apscheduler
+```
+```
+nb plugin install nonebot-plugin-htmlrender
+```
+添加插件：
+```
+在pyproject.toml文件中将EnjoyAnimation添加进plugins中
+plugins = ["EnjoyAnimation"]
+```
+#### 手动安装
 
 1. 安装第三方库
 ```
 pip install bs4
 ```
 ```
 pip install requests
@@ -43,27 +64,28 @@
 ```
 plugin_dirs = ["src/plugins"]
 ```
 ### 配置插件
 
 插件有三项必须配置项
 
-配置文件为.env.dev（默认为此文件，.env中可以修改）文件
+配置文件为.env.X（默认为[初学者模式创建时]```.env.prof```或者[插件作者创建时]```.env.dev```，具体```.env```中可以修改）文件
 ```
 animation_admin=123456789            #管理员qq号
 animation_time= [8,30]               #订阅提醒时间，[0~23,0~59]
 animation_default_return_img=false   #一些番剧信息是否以图片发送（配置为false时，检测到风控会自动以图片进行发送）
 ```
 ### 插件使用
 ```
     Commands:【可选参数】
-    #番剧信息 【当前季度的番剧】
-    #番剧更新 【强制更新番剧信息】
-    #今日新番 【今日更新的番剧】
-    #新增订阅 【订阅=追番提醒】
-    #取消订阅
+    番剧帮助 （查看指令用法）
+    番剧信息 （当前季度的番剧）
+    番剧更新 （强制更新番剧信息）
+    今日新番 （今日更新的番剧）
+    新增订阅 （订阅=追番提醒）
+    取消订阅 （取消追番提醒）
     ==================== 
-    #番剧查询 【番剧信息中的序号】
-    #新增追番 【番剧信息中的序号】
-    #我的追番 【查看追番列表】
-    #取消追番
+    番剧查询 【番剧信息中的序号，如12 23 4 51这种数字列表】
+    新增追番 【番剧信息中的序号，也支持数字列表】
+    我的追番 （查看追番列表）
+    取消追番 【追番中的番剧序号，支持数字列表】
 ```
```

### Comparing `EnjoyAnimation-0.0.3/README.md` & `EnjoyAnimation-0.0.4b0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,36 @@
 
 ### 插件依赖
 插件：```nonebot-plugin-apscheduler nonebot-plugin-htmlrender```
 
 库：```bs4 requests```
 
 ### 安装插件
-由于并没有上传至PyPI，只能手动安装
+#### 自动安装
+
+安装此插件：
+```
+pip install EnjoyAnimation
+（若镜像站没有则使用以下指令进行安装）
+pip install --index-url https://pypi.org/simple EnjoyAnimation
+```
+安装第三方插件依赖：
+请在bot根目录运行此指令
+```
+nb plugin install nonebot-plugin-apscheduler
+```
+```
+nb plugin install nonebot-plugin-htmlrender
+```
+添加插件：
+```
+在pyproject.toml文件中将EnjoyAnimation添加进plugins中
+plugins = ["EnjoyAnimation"]
+```
+#### 手动安装
 
 1. 安装第三方库
 ```
 pip install bs4
 ```
 ```
 pip install requests
@@ -31,27 +52,28 @@
 ```
 plugin_dirs = ["src/plugins"]
 ```
 ### 配置插件
 
 插件有三项必须配置项
 
-配置文件为.env.dev（默认为此文件，.env中可以修改）文件
+配置文件为.env.X（默认为[初学者模式创建时]```.env.prof```或者[插件作者创建时]```.env.dev```，具体```.env```中可以修改）文件
 ```
 animation_admin=123456789            #管理员qq号
 animation_time= [8,30]               #订阅提醒时间，[0~23,0~59]
 animation_default_return_img=false   #一些番剧信息是否以图片发送（配置为false时，检测到风控会自动以图片进行发送）
 ```
 ### 插件使用
 ```
     Commands:【可选参数】
-    #番剧信息 【当前季度的番剧】
-    #番剧更新 【强制更新番剧信息】
-    #今日新番 【今日更新的番剧】
-    #新增订阅 【订阅=追番提醒】
-    #取消订阅
+    番剧帮助 （查看指令用法）
+    番剧信息 （当前季度的番剧）
+    番剧更新 （强制更新番剧信息）
+    今日新番 （今日更新的番剧）
+    新增订阅 （订阅=追番提醒）
+    取消订阅 （取消追番提醒）
     ==================== 
-    #番剧查询 【番剧信息中的序号】
-    #新增追番 【番剧信息中的序号】
-    #我的追番 【查看追番列表】
-    #取消追番
+    番剧查询 【番剧信息中的序号，如12 23 4 51这种数字列表】
+    新增追番 【番剧信息中的序号，也支持数字列表】
+    我的追番 （查看追番列表）
+    取消追番 【追番中的番剧序号，支持数字列表】
 ```
```

### Comparing `EnjoyAnimation-0.0.3/setup.py` & `EnjoyAnimation-0.0.4b0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r",encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["bs4","requests"] # 这里填依赖包信息
-VERSION="0.0.3"
+VERSION="0.0.4b0"
 
 setup(
     name="",
-    version="0.0.3",
+    version=VERSION,
     author="slexce",
     author_email="sim69732@gmail.com",
     description="基于nonebot与gocqhttp的动漫番剧插件",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/small-bili/nonebot-plugin-EnjoyAnimation",
     packages=find_packages(),
```

