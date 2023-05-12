# Comparing `tmp/gpt-review-0.9.0rc675.post1.tar.gz` & `tmp/gpt-review-0.9.0rc678.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.9.0rc675.post1.tar", last modified: Fri May 12 05:16:36 2023, max compression
+gzip compressed data, was "gpt-review-0.9.0rc678.post1.tar", last modified: Fri May 12 17:18:05 2023, max compression
```

## Comparing `gpt-review-0.9.0rc675.post1.tar` & `gpt-review-0.9.0rc678.post1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      336 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1995 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4200 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1862 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/README.md
--rw-r--r--   0        0        0     3561 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/action.yml
--rw-r--r--   0        0        0      307 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/azure.yaml.template
--rw-r--r--   0        0        0      218 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/config.summary.template.yml
--rw-r--r--   0        0        0      362 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/prompt.template.yml
--rw-r--r--   0        0        0     8500 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-12 05:16:35.817094 gpt-review-0.9.0rc675.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-12 05:16:35.817094 gpt-review-0.9.0rc675.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0     9454 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     3016 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5998 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     5981 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     3882 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0      788 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     8560 2023-05-12 05:16:27.972370 gpt-review-0.9.0rc675.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      894 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0     2639 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/src/gpt_review/context.py
--rw-r--r--   0        0        0      924 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0       33 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/src/gpt_review/prompts/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/src/gpt_review/prompts/_prompt.py
--rw-r--r--   0        0        0      349 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/src/gpt_review/prompts/prompt_bug.yaml
--rw-r--r--   0        0        0      362 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/src/gpt_review/prompts/prompt_coverage.yaml
--rw-r--r--   0        0        0      327 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/src/gpt_review/prompts/prompt_summary.yaml
--rw-r--r--   0        0        0      218 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     5421 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/mock.diff
--rw-r--r--   0        0        0      375 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/test_context.py
--rw-r--r--   0        0        0      612 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/test_git.py
--rw-r--r--   0        0        0     1443 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/test_github.py
--rw-r--r--   0        0        0     5388 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1467 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/test_report.py
--rw-r--r--   0        0        0      797 2023-05-12 05:16:27.976370 gpt-review-0.9.0rc675.post1/tests/test_review.py
--rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 gpt-review-0.9.0rc675.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1995 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4200 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-12 17:17:57.858049 gpt-review-0.9.0rc678.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1862 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/.pypirc
+-rw-r--r--   0        0        0      450 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/action.yml
+-rw-r--r--   0        0        0      307 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/azure.yaml.template
+-rw-r--r--   0        0        0      218 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/config.summary.template.yml
+-rw-r--r--   0        0        0      362 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/prompt.template.yml
+-rw-r--r--   0        0        0     8500 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-12 17:18:05.098146 gpt-review-0.9.0rc678.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-12 17:18:05.098146 gpt-review-0.9.0rc678.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0     9454 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     3016 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5998 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     5981 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     4014 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0      788 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     8560 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      894 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0     2639 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/context.py
+-rw-r--r--   0        0        0      924 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      349 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/prompts/prompt_bug.yaml
+-rw-r--r--   0        0        0      362 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/prompts/prompt_coverage.yaml
+-rw-r--r--   0        0        0      327 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/src/gpt_review/prompts/prompt_summary.yaml
+-rw-r--r--   0        0        0      218 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     5421 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/mock.diff
+-rw-r--r--   0        0        0      375 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/test_context.py
+-rw-r--r--   0        0        0      612 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1443 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5388 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1467 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/test_report.py
+-rw-r--r--   0        0        0      797 2023-05-12 17:17:57.862049 gpt-review-0.9.0rc678.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 gpt-review-0.9.0rc678.post1/PKG-INFO
```

### Comparing `gpt-review-0.9.0rc675.post1/.devcontainer/devcontainer.json` & `gpt-review-0.9.0rc678.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.9.0rc678.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.github/dependabot.yml` & `gpt-review-0.9.0rc678.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.github/pull_request_template.md` & `gpt-review-0.9.0rc678.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.github/workflows/codeql.yml` & `gpt-review-0.9.0rc678.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.9.0rc678.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.9.0rc678.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.github/workflows/python.yml` & `gpt-review-0.9.0rc678.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.github/workflows/test-action.yml` & `gpt-review-0.9.0rc678.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.gitignore` & `gpt-review-0.9.0rc678.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/.vscode/settings.json` & `gpt-review-0.9.0rc678.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/LICENSE` & `gpt-review-0.9.0rc678.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/README.md` & `gpt-review-0.9.0rc678.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/action.yml` & `gpt-review-0.9.0rc678.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/pyproject.toml` & `gpt-review-0.9.0rc678.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/_ask.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/_git.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/_github.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/_llama_index.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/_openai.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/_openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,18 @@
             presence_penalty=presence_penalty,
         )
         return completion.choices[0].message.content  # type: ignore
     except RateLimitError as error:
         if retry < C.MAX_RETRIES:
             logging.warning("Call to GPT failed due to rate limit, retry attempt %s of %s", retry, C.MAX_RETRIES)
 
-            wait_time = int(error.headers["Retry-After"]) if error.headers["Retry-After"] else retry * 10
+            wait_time = (
+                int(error.headers["Retry-After"]) * 2 * (1 + retry / C.MAX_RETRIES)
+                if error.headers["Retry-After"]
+                else retry * (10 + pow(2, retry / C.MAX_RETRIES))
+            )
             logging.warning("Waiting for %s seconds before retrying.", wait_time)
 
             time.sleep(wait_time)
 
             return _call_gpt(prompt, temperature, max_tokens, top_p, frequency_penalty, presence_penalty, retry + 1)
         raise RateLimitError("Retry limit exceeded") from error
```

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/_repository.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/_review.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/constants.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/context.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/context.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/main.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/src/gpt_review/prompts/_prompt.py` & `gpt-review-0.9.0rc678.post1/src/gpt_review/prompts/_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/tests/conftest.py` & `gpt-review-0.9.0rc678.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/tests/mock.diff` & `gpt-review-0.9.0rc678.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/tests/test_git.py` & `gpt-review-0.9.0rc678.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/tests/test_github.py` & `gpt-review-0.9.0rc678.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/tests/test_gpt_cli.py` & `gpt-review-0.9.0rc678.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/tests/test_llama_index.py` & `gpt-review-0.9.0rc678.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/tests/test_openai.py` & `gpt-review-0.9.0rc678.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/tests/test_report.py` & `gpt-review-0.9.0rc678.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/tests/test_review.py` & `gpt-review-0.9.0rc678.post1/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc675.post1/PKG-INFO` & `gpt-review-0.9.0rc678.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.9.0rc675.post1
+Version: 0.9.0rc678.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.9.0rc675.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.9.0rc678.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

