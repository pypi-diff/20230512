# Comparing `tmp/copier_template_tester-1.2.0rc1.tar.gz` & `tmp/copier_template_tester-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copier_template_tester-1.2.0rc1.tar", max compression
+gzip compressed data, was "copier_template_tester-1.2.1.tar", max compression
```

## Comparing `copier_template_tester-1.2.0rc1.tar` & `copier_template_tester-1.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-04-08 20:25:06.309423 copier_template_tester-1.2.0rc1/LICENSE
--rw-r--r--   0        0        0      200 2023-04-22 07:58:19.015708 copier_template_tester-1.2.0rc1/copier_template_tester/__init__.py
--rw-r--r--   0        0        0      918 2023-04-22 05:52:45.492482 copier_template_tester-1.2.0rc1/copier_template_tester/_config.py
--rw-r--r--   0        0        0     1201 2023-04-22 06:45:54.453506 copier_template_tester-1.2.0rc1/copier_template_tester/_pre_commit_support.py
--rw-r--r--   0        0        0     2446 2023-04-22 07:58:02.422439 copier_template_tester-1.2.0rc1/copier_template_tester/_write_output.py
--rw-r--r--   0        0        0     2032 2023-04-22 07:05:15.639502 copier_template_tester-1.2.0rc1/copier_template_tester/main.py
--rw-r--r--   0        0        0     3438 2023-04-22 07:58:24.472597 copier_template_tester-1.2.0rc1/docs/README.md
--rw-r--r--   0        0        0     1511 2023-04-22 07:58:19.030665 copier_template_tester-1.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4491 1970-01-01 00:00:00.000000 copier_template_tester-1.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-11 02:39:27.384670 copier_template_tester-1.2.1/LICENSE
+-rw-r--r--   0        0        0      197 2023-05-12 00:01:00.006512 copier_template_tester-1.2.1/copier_template_tester/__init__.py
+-rw-r--r--   0        0        0      918 2023-04-27 21:50:31.592600 copier_template_tester-1.2.1/copier_template_tester/_config.py
+-rw-r--r--   0        0        0     1201 2023-05-11 23:45:19.757850 copier_template_tester-1.2.1/copier_template_tester/_pre_commit_support.py
+-rw-r--r--   0        0        0     4333 2023-05-11 23:58:25.770678 copier_template_tester-1.2.1/copier_template_tester/_write_output.py
+-rw-r--r--   0        0        0     2276 2023-05-11 02:36:41.502126 copier_template_tester-1.2.1/copier_template_tester/main.py
+-rw-r--r--   0        0        0     3438 2023-05-12 00:01:05.841697 copier_template_tester-1.2.1/docs/README.md
+-rw-r--r--   0        0        0     1505 2023-05-12 00:01:00.021997 copier_template_tester-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4488 1970-01-01 00:00:00.000000 copier_template_tester-1.2.1/PKG-INFO
```

### Comparing `copier_template_tester-1.2.0rc1/LICENSE` & `copier_template_tester-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.0rc1/copier_template_tester/_config.py` & `copier_template_tester-1.2.1/copier_template_tester/_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,12 +17,13 @@
         raise RuntimeError('CTT expected headers like: [output."<something>"]')
 
 
 @beartype
 def load_config(base_dir: Path) -> dict:  # type: ignore[type-arg]
     """Read the ctt config from `CWD`."""
     cfg_path = base_dir / 'ctt.toml'
-    if cfg_path.is_file():
-        config: dict = tomllib.loads(cfg_path.read_text())  # type: ignore[type-arg]
-        _validate_config(config)
-        return config
-    raise ValueError(f'No configuration file found. Expected: {cfg_path.absolute()}')  # pragma: no cover # noqa: EM102
+    if not cfg_path.is_file():  # pragma: no cover
+        msg = f'No configuration file found. Expected: {cfg_path.absolute()}'
+        raise ValueError(msg)
+    config: dict = tomllib.loads(cfg_path.read_text())  # type: ignore[type-arg]
+    _validate_config(config)
+    return config
```

### Comparing `copier_template_tester-1.2.0rc1/copier_template_tester/_pre_commit_support.py` & `copier_template_tester-1.2.1/copier_template_tester/_pre_commit_support.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.0rc1/copier_template_tester/_write_output.py` & `copier_template_tester-1.2.1/copier_template_tester/_write_output.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,95 @@
 """Template Directory Writer."""
 
+import re
 import shutil
+from functools import lru_cache
 from pathlib import Path
 
 import copier
 import yaml
 from beartype import beartype
+from corallium.file_helpers import read_lines
 from corallium.log import get_logger
+from corallium.shell import capture_shell
 
 logger = get_logger()
 
+DEFAULT_TEMPLATE_FILE_NAME = 'copier.yaml'
+"""Default answer file name. Alternative is copier.yml."""
+
+
+DEFAULT_ANSWER_FILE_NAME = '.copier-answers.yml'
+"""Default answer file name.
+
+https://github.com/copier-org/copier/blob/7f05baf4f004a4876fb6158e1c532b28290146a4/copier/subproject.py#L39
+
+"""
+
 
 @beartype
 def _read_copier_template(base_dir: Path) -> dict:  # type: ignore[type-arg]
     """Locate and read the copier configuration file."""
-    copier_path = base_dir / 'copier.yaml'
+    copier_path = base_dir / DEFAULT_TEMPLATE_FILE_NAME
     if not copier_path.is_file():
         copier_path = copier_path.with_suffix('.yml')
-    if not copier_path.is_file():
-        msg = f"Can't find the copier answer file. Expected: {copier_path} (or .yaml)"
+    if not copier_path.is_file():  # pragma: no cover
+        msg = f"Can't find the copier template file. Expected: {copier_path} (or .yaml)"
         raise FileNotFoundError(msg)
 
     return yaml.safe_load(copier_path.read_text())  # type: ignore[no-any-return]
 
 
 @beartype
-def _remove_unique_values(*, src_path: Path, dst_path: Path) -> None:
-    """Remove unique values for deterministic 'ctt' output."""
+def _find_answers_file(*, src_path: Path, dst_path: Path) -> Path:
+    """Locate the copier answers file based on the copier template."""
     copier_config = _read_copier_template(src_path)
-    # https://github.com/copier-org/copier/blob/7f05baf4f004a4876fb6158e1c532b28290146a4/copier/subproject.py#L39
-    answers_filename = copier_config.get('_answers_file') or '.copier-answers.yml'
-    answers_path = dst_path / answers_filename
-    lines = (  # noqa: ECE001
-        # Create a stable tag that copier will still utilize
-        f'{line.split("-")[0]}-0' if line.startswith('_commit') else line
-        for line in answers_path.read_text().split('\n')
-    )
+    answers_filename = copier_config.get('_answers_file') or DEFAULT_ANSWER_FILE_NAME
+    if '{{' in answers_filename:
+        # If the filename is created from the template, just grab the first match
+        search_name = re.sub(r'{{[^}]+}}', '*', answers_filename)
+        matches = [*dst_path.glob(search_name)]
+        if len(matches) != 1:  # pragma: no cover
+            msg = f"Can't find just one copier answers file matching {dst_path / search_name}. Found: {matches}"
+            raise ValueError(msg)
+        return matches[0]
+    return dst_path / answers_filename  # pragma: no cover
+
+
+@lru_cache(maxsize=3)
+@beartype
+def _resolve_git_root_dir(base_dir: Path) -> Path:
+    """Use git to list all untracked files."""
+    cmd = 'git rev-parse --show-toplevel'
+    output = capture_shell(cmd=cmd, cwd=base_dir)
+    return Path(output.strip())
+
+
+@beartype
+def _stabilize(line: str, answers_path: Path) -> str:  # noqa: CFQ004
+    # Convert _src_path to a deterministic relative path
+    if line.startswith('_src_path'):
+        raw_path = Path(line.split('_src_path:')[-1].strip())
+        ans_dir = answers_path.parent
+        if ans_dir.is_relative_to(raw_path):
+            count_rel = len(ans_dir.relative_to(raw_path).parts)
+            rel_path = '/'.join([*(['..'] * count_rel), raw_path.name])
+            return f'_src_path: {rel_path}'
+        return line
+    # Create a stable tag for '_commit' that copier will still utilize
+    if line.startswith('_commit'):
+        return f'{line.split("-")[0]}-0'
+    return line
+
+
+@beartype
+def _stabilize_answers_file(*, src_path: Path, dst_path: Path) -> None:  # noqa: CFQ004
+    """Ensure that the answers file is deterministic."""
+    answers_path = _find_answers_file(src_path=src_path, dst_path=dst_path)
+    lines = (_stabilize(_l, answers_path) for _l in read_lines(answers_path))
     answers_path.write_text('\n'.join(lines))
 
 
 @beartype
 def write_output(  # type: ignore[no-untyped-def]
     *,
     src_path: Path,
@@ -59,12 +109,13 @@
     kwargs.setdefault('quiet', False)
     kwargs.setdefault('vcs_ref', 'HEAD')
     copier.run_auto(str(src_path), dst_path, **kwargs)
     git_path = dst_path / '.git'
     if git_path.is_dir():  # pragma: no cover
         shutil.rmtree(git_path)
 
-    # Ensure deterministic output
+    # Reduce variability in the output
     try:
-        _remove_unique_values(src_path=src_path, dst_path=dst_path)
-    except FileNotFoundError as exc:
-        logger.error(str(exc))  # noqa: TRY400
+        _stabilize_answers_file(src_path=src_path, dst_path=dst_path)
+    except FileNotFoundError as exc:  # pragma: no cover
+        logger.warning(str(exc))  # noqa: TRY400
+        raise
```

### Comparing `copier_template_tester-1.2.0rc1/copier_template_tester/main.py` & `copier_template_tester-1.2.1/copier_template_tester/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,31 @@
 logger = get_logger()
 
 
 @beartype
 def run(*, base_dir: Path | None = None, check_untracked: bool = False) -> None:
     """Main class to run ctt."""
     base_dir = base_dir or Path.cwd()
+    logger.text(f'Starting Copier Template Tester for {base_dir}')
     config = load_config(base_dir)
     defaults = config.get('defaults', {})
 
     input_path = base_dir
     paths = set()
     for key, data in config['output'].items():
         output_path = base_dir / key
         output_path.mkdir(parents=True, exist_ok=True)
         paths.add(output_path)
-        logger.text(f'Creating: {output_path}')
+        logger.text(f'Using copier to create: {output_path}')
         write_output(src_path=input_path, dst_path=base_dir / output_path, data=defaults | data)
 
     if check_untracked:  # pragma: no cover
+        logger.text('Checking for untracked files')
         check_for_untracked(paths, base_dir)
+    logger.text('Completed Copier Template Tester. If files were modified, pre-commit will report a failure.')
 
 
 @beartype
 def run_cli() -> None:  # pragma: no cover
     """Accept CLI configuration for running ctt."""
     @beartype
     def dir_path(pth: str | None) -> Path:
```

### Comparing `copier_template_tester-1.2.0rc1/docs/README.md` & `copier_template_tester-1.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.0rc1/pyproject.toml` & `copier_template_tester-1.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.2.0rc1"
+version = "1.2.1"
 version_files = ["copier_template_tester/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
@@ -20,15 +20,15 @@
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "copier_template_tester"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/copier-template-tester"
-version = "1.2.0rc1"
+version = "1.2.1"
 
 [tool.poetry.dependencies]
 python = "^3.10.5"
 copier = ">=7.0.1"
 corallium = ">=0.2.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `copier_template_tester-1.2.0rc1/PKG-INFO` & `copier_template_tester-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copier-template-tester
-Version: 1.2.0rc1
+Version: 1.2.1
 Summary: Test copier templates
 Home-page: https://github.com/kyleking/copier-template-tester
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

