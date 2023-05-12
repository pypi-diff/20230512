# Comparing `tmp/lazycodr-0.1.1.tar.gz` & `tmp/lazycodr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycodr-0.1.1.tar", max compression
+gzip compressed data, was "lazycodr-0.1.2.tar", max compression
```

## Comparing `lazycodr-0.1.1.tar` & `lazycodr-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3282 2023-05-11 10:38:38.530131 lazycodr-0.1.1/README.md
--rw-r--r--   0        0        0      993 2023-05-11 11:47:31.284359 lazycodr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      435 2023-05-11 09:19:38.169467 lazycodr-0.1.1/src/lazycodr/cli/__init__.py
--rw-r--r--   0        0        0      708 2023-05-11 11:37:46.377666 lazycodr-0.1.1/src/lazycodr/cli/config.py
--rw-r--r--   0        0        0      841 2023-05-10 23:34:39.649616 lazycodr-0.1.1/src/lazycodr/cli/pr.py
--rw-r--r--   0        0        0      126 2023-05-10 23:26:25.337695 lazycodr-0.1.1/src/lazycodr/constants.py
--rw-r--r--   0        0        0      513 2023-05-10 23:26:05.445197 lazycodr-0.1.1/src/lazycodr/prompts/__init__.py
--rw-r--r--   0        0        0      295 2023-05-11 09:20:09.661178 lazycodr-0.1.1/src/lazycodr/prompts/templates/pr-generate-refine-init.jinja
--rw-r--r--   0        0        0      586 2023-05-11 09:20:09.661178 lazycodr-0.1.1/src/lazycodr/prompts/templates/pr-generate-refine-loop.jinja
--rw-r--r--   0        0        0     2961 2023-05-11 10:16:40.893987 lazycodr-0.1.1/src/lazycodr/utils.py
--rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 lazycodr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3306 2023-05-12 16:48:38.549507 lazycodr-0.1.2/README.md
+-rw-r--r--   0        0        0      994 2023-05-12 16:48:38.549507 lazycodr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      435 2023-05-12 16:48:38.549507 lazycodr-0.1.2/src/lazycodr/cli/__init__.py
+-rw-r--r--   0        0        0      708 2023-05-12 16:48:38.549507 lazycodr-0.1.2/src/lazycodr/cli/config.py
+-rw-r--r--   0        0        0      865 2023-05-12 16:48:38.549507 lazycodr-0.1.2/src/lazycodr/cli/pr.py
+-rw-r--r--   0        0        0      126 2023-05-12 16:48:38.549507 lazycodr-0.1.2/src/lazycodr/constants.py
+-rw-r--r--   0        0        0      513 2023-05-12 16:48:38.549507 lazycodr-0.1.2/src/lazycodr/prompts/__init__.py
+-rw-r--r--   0        0        0      295 2023-05-12 16:48:38.549507 lazycodr-0.1.2/src/lazycodr/prompts/templates/pr-generate-refine-init.jinja
+-rw-r--r--   0        0        0      586 2023-05-12 16:48:38.549507 lazycodr-0.1.2/src/lazycodr/prompts/templates/pr-generate-refine-loop.jinja
+-rw-r--r--   0        0        0     2961 2023-05-12 16:48:38.549507 lazycodr-0.1.2/src/lazycodr/utils.py
+-rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 lazycodr-0.1.2/PKG-INFO
```

### Comparing `lazycodr-0.1.1/README.md` & `lazycodr-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 2. Click on "Generate new token" in the top right corner.j
 3. Give your token a descriptive name and select the required scopes (for LazyCodr, you'll need `repo` and `user` scopes.
 4. Click "Generate token" at the bottom of the page and copy the generated token.
 
 After you have both your OpenAI API key and GitHub token, you can configure LazyCodr by running the following command:
 
 ```bash
-lazycodr config
+lazycodr config credentials
 ```
 
 This command will prompt you to enter your API key and GitHub token, which will be securely stored for future use.
 
 Now you're all set to use LazyCodr! 🚀
 
 
 ## Usage 📚
 
 1. Configure LazyCodr with your OpenAI API key and GitHub token:
 
 ```bash
-lazycodr config
+lazycodr config credentials
 ```
 
 2. Use LazyCodr to generate a pull request description:
 
 ```bash
 lazycodr pr generate <repo_name> <pr_number>
 ```
```

### Comparing `lazycodr-0.1.1/pyproject.toml` & `lazycodr-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 authors = ["JimZer <jimi.vaubien@protonmail.com>"]
 description = "A CLI tool to help lazy coders get the work done with AI (commit messages, pull requests ...)"
+homepage = "https://github.com/bitswired/lazycodr"
 name = "lazycodr"
 packages = [{include = "lazycodr", from = "src"}]
 readme = "README.md"
-version = "0.1.1"
 repository = "https://github.com/bitswired/lazycodr"
-homepage = "https://github.com/bitswired/lazycodr"
+version = "0.1.2"
+
 
 [tool.poetry.dependencies]
 httpx = "^0.24.0"
 jinja2 = "^3.1.2"
 langchain = "^0.0.163"
 openai = "^0.27.6"
 pydantic = "^1.10.7"
```

### Comparing `lazycodr-0.1.1/src/lazycodr/cli/config.py` & `lazycodr-0.1.2/src/lazycodr/cli/config.py`

 * *Files identical despite different names*

### Comparing `lazycodr-0.1.1/src/lazycodr/cli/pr.py` & `lazycodr-0.1.2/src/lazycodr/cli/pr.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
 
 app = typer.Typer()
 
 
 @app.command()
 def generate(repo_name: str, pr_number: int):
+    pr_template = typer.edit("<Enter PR template here>")
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
     ) as progress:
-        pr_template = typer.edit()
         progress.add_task(description="Getting diff...", total=None)
         pr_diff = get_pr_diff(repo_name, pr_number)
+
         progress.add_task(description="Generating PR description...", total=None)
         res = generate_pr(pr_diff, pr_template)
+
         md = Markdown(res)
         console.print(md, width=90)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `lazycodr-0.1.1/src/lazycodr/prompts/__init__.py` & `lazycodr-0.1.2/src/lazycodr/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `lazycodr-0.1.1/src/lazycodr/prompts/templates/pr-generate-refine-loop.jinja` & `lazycodr-0.1.2/src/lazycodr/prompts/templates/pr-generate-refine-loop.jinja`

 * *Files identical despite different names*

### Comparing `lazycodr-0.1.1/src/lazycodr/utils.py` & `lazycodr-0.1.2/src/lazycodr/utils.py`

 * *Files identical despite different names*

### Comparing `lazycodr-0.1.1/PKG-INFO` & `lazycodr-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycodr
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI tool to help lazy coders get the work done with AI (commit messages, pull requests ...)
 Home-page: https://github.com/bitswired/lazycodr
 Author: JimZer
 Author-email: jimi.vaubien@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -56,28 +56,28 @@
 2. Click on "Generate new token" in the top right corner.j
 3. Give your token a descriptive name and select the required scopes (for LazyCodr, you'll need `repo` and `user` scopes.
 4. Click "Generate token" at the bottom of the page and copy the generated token.
 
 After you have both your OpenAI API key and GitHub token, you can configure LazyCodr by running the following command:
 
 ```bash
-lazycodr config
+lazycodr config credentials
 ```
 
 This command will prompt you to enter your API key and GitHub token, which will be securely stored for future use.
 
 Now you're all set to use LazyCodr! 🚀
 
 
 ## Usage 📚
 
 1. Configure LazyCodr with your OpenAI API key and GitHub token:
 
 ```bash
-lazycodr config
+lazycodr config credentials
 ```
 
 2. Use LazyCodr to generate a pull request description:
 
 ```bash
 lazycodr pr generate <repo_name> <pr_number>
 ```
```

