# Comparing `tmp/falra_run_github-0.1.3.tar.gz` & `tmp/falra_run_github-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/falra_run_github-0.1.3.tar", last modified: Wed Apr 26 15:18:49 2023, max compression
+gzip compressed data, was "dist/falra_run_github-0.1.4.tar", last modified: Fri May 12 07:49:22 2023, max compression
```

## Comparing `falra_run_github-0.1.3.tar` & `falra_run_github-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:18:49.820818 falra_run_github-0.1.3/
--rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-26 15:18:49.820528 falra_run_github-0.1.3/PKG-INFO
--rw-r--r--   0 wengroy    (501) staff       (20)      984 2023-04-13 18:39:23.000000 falra_run_github-0.1.3/README.md
-drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:18:49.816282 falra_run_github-0.1.3/falra_run_github/
--rw-r--r--   0 wengroy    (501) staff       (20)        0 2023-03-09 00:23:54.000000 falra_run_github-0.1.3/falra_run_github/__init__.py
--rw-r--r--   0 wengroy    (501) staff       (20)       78 2023-04-13 18:03:18.000000 falra_run_github-0.1.3/falra_run_github/__main__.py
--rwxr-xr-x   0 wengroy    (501) staff       (20)     8896 2023-04-26 15:18:41.000000 falra_run_github-0.1.3/falra_run_github/main.py
-drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:18:49.820055 falra_run_github-0.1.3/falra_run_github.egg-info/
--rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/PKG-INFO
--rw-r--r--   0 wengroy    (501) staff       (20)      343 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/SOURCES.txt
--rw-r--r--   0 wengroy    (501) staff       (20)        1 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/dependency_links.txt
--rw-r--r--   0 wengroy    (501) staff       (20)       62 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/entry_points.txt
--rw-r--r--   0 wengroy    (501) staff       (20)      600 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/requires.txt
--rw-r--r--   0 wengroy    (501) staff       (20)       17 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/top_level.txt
--rw-r--r--   0 wengroy    (501) staff       (20)       38 2023-04-26 15:18:49.820911 falra_run_github-0.1.3/setup.cfg
--rwxr-xr-x   0 wengroy    (501) staff       (20)      439 2023-04-26 15:18:46.000000 falra_run_github-0.1.3/setup.py
+drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-05-12 07:49:22.158175 falra_run_github-0.1.4/
+-rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-05-12 07:49:22.157886 falra_run_github-0.1.4/PKG-INFO
+-rw-r--r--   0 wengroy    (501) staff       (20)      984 2023-04-13 18:39:23.000000 falra_run_github-0.1.4/README.md
+drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-05-12 07:49:22.153391 falra_run_github-0.1.4/falra_run_github/
+-rw-r--r--   0 wengroy    (501) staff       (20)        0 2023-03-09 00:23:54.000000 falra_run_github-0.1.4/falra_run_github/__init__.py
+-rw-r--r--   0 wengroy    (501) staff       (20)       78 2023-04-13 18:03:18.000000 falra_run_github-0.1.4/falra_run_github/__main__.py
+-rwxr-xr-x   0 wengroy    (501) staff       (20)     9013 2023-05-12 07:44:28.000000 falra_run_github-0.1.4/falra_run_github/main.py
+drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-05-12 07:49:22.157471 falra_run_github-0.1.4/falra_run_github.egg-info/
+-rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-05-12 07:49:21.000000 falra_run_github-0.1.4/falra_run_github.egg-info/PKG-INFO
+-rw-r--r--   0 wengroy    (501) staff       (20)      343 2023-05-12 07:49:21.000000 falra_run_github-0.1.4/falra_run_github.egg-info/SOURCES.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)        1 2023-05-12 07:49:21.000000 falra_run_github-0.1.4/falra_run_github.egg-info/dependency_links.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)       62 2023-05-12 07:49:21.000000 falra_run_github-0.1.4/falra_run_github.egg-info/entry_points.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)      600 2023-05-12 07:49:21.000000 falra_run_github-0.1.4/falra_run_github.egg-info/requires.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)       17 2023-05-12 07:49:21.000000 falra_run_github-0.1.4/falra_run_github.egg-info/top_level.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)       38 2023-05-12 07:49:22.158283 falra_run_github-0.1.4/setup.cfg
+-rwxr-xr-x   0 wengroy    (501) staff       (20)      439 2023-05-12 07:30:15.000000 falra_run_github-0.1.4/setup.py
```

### Comparing `falra_run_github-0.1.3/README.md` & `falra_run_github-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `falra_run_github-0.1.3/falra_run_github/main.py` & `falra_run_github-0.1.4/falra_run_github/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -54,45 +54,49 @@
         print("Git clone ...start")
         os.system(f"""git clone {repo_url} {local_path}""")
         print("Git clone ...success")
     except Exception as e:
         print(f"""[download_files_from_github] git clone fail.. skip! error:{e}""")
 
 
-def download_github_repo(repo_url, access_token, repo_name="repo"):
+def download_github_repo(repo_url, access_token, repo_name, work_dir=""):
     # 解析出 repo 的 owner 和 name
     _, owner, name = repo_url.rstrip('/').rsplit('/', 2)
 
     # 創建新目錄來存儲 repo 的內容
     if not os.path.exists("user-repo"):
         os.mkdir("user-repo")
-    repo_name = os.path.join("user-repo", repo_name)
-    if not os.path.exists(repo_name):
-        os.mkdir(repo_name)
+
+    if work_dir == "":
+        work_dir = repo_name
+
+    work_path = os.path.join("user-repo", work_dir)
+    if not os.path.exists(work_path):
+        os.mkdir(work_path)
 
     # 下載每個文件並存儲到本地
     try:
-        download_files_from_github(repo_url=repo_url, local_path=repo_name, token=access_token)
+        download_files_from_github(repo_url=repo_url, local_path=work_path, token=access_token)
     except Exception as e:
         # 如果 下載 產生錯誤，將錯誤訊息寫到檔案中
         print(f"""[Github download ERROR!!] repo_url:  {repo_url}. ERROR_msg：{e}""")
 
 
 def install_requirements(repo_name, requirements_file_path="requirements.txt"):
     # 獲取 main.py 的路徑
     repo_name = os.path.join("user-repo", repo_name)
     # todo: install requirements
     # 檢查 main.py 是否存在
     if not os.path.exists(requirements_file_path):
         print("reauirement install failed, requirements.txt not found")
     return
 
-def run_main_py(repo_name, output_file="falra_output.txt", py_name="main.py", arg=[]):
+def run_main_py(work_dir, output_file="falra_output.txt", py_name="main.py", arg=[]):
     # 獲取 main.py 的路徑
-    repo_name = os.path.join("user-repo", repo_name)
+    repo_name = os.path.join("user-repo", work_dir)
     # 已經更改為進入 repo 子資料夾去執行 main.py
     main_path = py_name
     #main_path = os.path.join(repo_name, py_name)
 
     # 設置子資料夾的路徑
     sub_dir = repo_name
 
@@ -143,19 +147,19 @@
         with open(output_file, "a") as f:
             f.write(error_msg)
 
     # 恢復到原始工作目錄
     os.chdir(current_dir)
 
 
-def query_output(repo_name, output_file="falra_output.txt"):
-    repo_name = os.path.join("user-repo", repo_name)
+def query_output(work_dir, output_file="falra_output.txt"):
+    work_dir = os.path.join("user-repo", work_dir)
     #print(f"""result_file = {repo_name}/{output_file}""")
     # 讀取檔案內容
-    output_file_path = f"""{repo_name}/{output_file}"""
+    output_file_path = f"""{work_dir}/{output_file}"""
     with open(output_file_path, 'r') as f:
         contents = f.read()
         print(contents)
         # 返回結果
         return contents
 
 
@@ -167,75 +171,75 @@
 
     for root, dirs, files in os.walk(folder_path, topdown=False):
         for file in files:
             os.remove(os.path.join(root, file))
         for dir in dirs:
             shutil.rmtree(os.path.join(root, dir))
 
-def main_run_github(repo_url, access_token, repo_name, py_name, arg_str):
+def main_run_github(repo_url, access_token, repo_name, work_dir, py_name, arg_str):
     # repo_url = sys.argv[1] # "https://github.com/my-account/my-repo"
     # access_token = sys.argv[2] # "access_token
     # repo_name = sys.argv[3] # 'my-repo'
     # py_name = sys.argv[4] # 'main.py'
     # arg_str = sys.argv[5] # "['argument']"
 
     # read parameters
     arg = []
     # 將字符串轉換為 list
     arg = ast.literal_eval(arg_str)
 
     # Download GitHub repo and save to local directory user-repo
     print("002 download_github_repo..")
-    download_github_repo(repo_url, access_token, repo_name)
+    download_github_repo(repo_url, access_token, repo_name, work_dir)
 
     # 創建 output 目錄來存儲執行結果
     #if not os.path.exists(repo_name):
     #    os.mkdir(repo_name)
     # 創建 output 目錄來存儲執行結果
     #output_dir = f"""{repo_name}/output"""
     #if not os.path.exists(output_dir):
     #    os.mkdir(output_dir)
 
     # 運行 main.py 並將輸出結果記錄到 repo 下的 falra_output.txt 檔案
     print("003 run_main_py..")
     output_file= f"""falra_output.txt"""
-    run_main_py(repo_name=repo_name, output_file=output_file, py_name=py_name, arg=arg)
+    run_main_py(work_dir=work_dir, output_file=output_file, py_name=py_name, arg=arg)
 
     # Query output
-    execution_result = query_output(repo_name=repo_name)
+    execution_result = query_output(work_dir=work_dir)
     print(execution_result)
     print("004 run_main_py done.")
 
 
 def main():
     parser = argparse.ArgumentParser(description='GitHub Executor')
     parser.add_argument('--action', type=str, required=True, choices=['start', 'output', 'clean', 'version'], help="The actions to execute")
     parser.add_argument('--repo_url', metavar='repo_url', type=str, help='URL of the GitHub repository')
     parser.add_argument('--access_token', metavar='access_token', type=str, help='Access token for the GitHub API')
     parser.add_argument('--user_id', metavar='user_id', type=str, help='user_id as string')
     parser.add_argument('--repo_name', metavar='repo_name', type=str, help='Name of the repository')
+    parser.add_argument('--work_dir', metavar='work_dir', type=str, help='work directory')
     parser.add_argument('--py_name', metavar='py_name', type=str, help='Name of the Python file to execute')
     parser.add_argument('--argument', metavar='argument', type=str, help='Arguments of the Python to execute as string')
 
     args = parser.parse_args()
 
     print(f"""Action = {args.action}""")
 
     if args.action == "start":
         if not args.repo_url:
             parser.error("Executing run_github requires --repo_url parameter")
         print(f"""001 start falra_run_github..""")
 
-        repo_path = args.repo_name
-        if args.user_id :
-            repo_path = f"""{args.user_id}_{args.repo_name}"""
+        work_dir = args.work_dir
 
         main_run_github(repo_url=args.repo_url,
                         access_token=args.access_token,
-                        repo_name=repo_path,
+                        repo_name=args.repo_name,
+                        work_dir=work_dir,
                         py_name=args.py_name,
                         arg_str=args.argument,
                         )
     elif args.action == "output":
         if not args.repo_name:
             parser.error("Executing output query requires --repo_name parameter")
         query_output(args.repo_name)
```

### Comparing `falra_run_github-0.1.3/falra_run_github.egg-info/requires.txt` & `falra_run_github-0.1.4/falra_run_github.egg-info/requires.txt`

 * *Files identical despite different names*

