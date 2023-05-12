# Comparing `tmp/citric-0.7.1b1.tar.gz` & `tmp/citric-0.7.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citric-0.7.1b1.tar", max compression
+gzip compressed data, was "citric-0.7.1b2.tar", max compression
```

## Comparing `citric-0.7.1b1.tar` & `citric-0.7.1b2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-04-11 05:24:40.664486 citric-0.7.1b1/LICENSE
--rw-r--r--   0        0        0     4491 2023-04-11 05:24:40.664486 citric-0.7.1b1/README.md
--rw-r--r--   0        0        0     4224 2023-04-11 05:24:40.668486 citric-0.7.1b1/pyproject.toml
--rw-r--r--   0        0        0      399 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/__init__.py
--rw-r--r--   0        0        0     1511 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/_compat.py
--rw-r--r--   0        0        0    44877 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/client.py
--rw-r--r--   0        0        0     1739 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/enums.py
--rw-r--r--   0        0        0     1345 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/exceptions.py
--rw-r--r--   0        0        0     1135 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/method.py
--rw-r--r--   0        0        0     1171 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/objects.py
--rw-r--r--   0        0        0        0 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/py.typed
--rw-r--r--   0        0        0     6984 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/session.py
--rw-r--r--   0        0        0    13839 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/types.py
--rw-r--r--   0        0        0     6806 1970-01-01 00:00:00.000000 citric-0.7.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-12 03:07:57.074755 citric-0.7.1b2/LICENSE
+-rw-r--r--   0        0        0     4551 2023-05-12 03:07:57.074755 citric-0.7.1b2/README.md
+-rw-r--r--   0        0        0     4393 2023-05-12 03:07:57.082755 citric-0.7.1b2/pyproject.toml
+-rw-r--r--   0        0        0      399 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/__init__.py
+-rw-r--r--   0        0        0     1509 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/_compat.py
+-rw-r--r--   0        0        0    44916 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/client.py
+-rw-r--r--   0        0        0     1739 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/enums.py
+-rw-r--r--   0        0        0     1345 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/exceptions.py
+-rw-r--r--   0        0        0     1055 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/method.py
+-rw-r--r--   0        0        0     1171 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/objects.py
+-rw-r--r--   0        0        0        0 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/py.typed
+-rw-r--r--   0        0        0     6964 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/session.py
+-rw-r--r--   0        0        0    14009 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/types.py
+-rw-r--r--   0        0        0     6818 1970-01-01 00:00:00.000000 citric-0.7.1b2/PKG-INFO
```

### Comparing `citric-0.7.1b1/LICENSE` & `citric-0.7.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b1/README.md` & `citric-0.7.1b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
 ## Features
 
 - Supports the full RPC API via the [`Session` class](https://citric.readthedocs.io/en/latest/_api/citric/session/index.html#citric.session.Session).
 - Best effort to implement all the RPC methods in the [`Client` class](https://citric.readthedocs.io/en/latest/_api/citric/client/index.html#citric.client.Client). See the [API coverage page](https://citric.readthedocs.io/en/latest/rpc_coverage.html) for details.
 - Easily export survey data to CSV files, [Pandas DataFrames](https://citric.readthedocs.io/en/latest/how-to.html#export-responses-to-a-pandas-dataframe) and [DuckDB databases](https://citric.readthedocs.io/en/latest/how-to.html#export-responses-to-a-duckdb-database-and-analyze-with-sql).
 - Easily [download survey files](https://citric.readthedocs.io/en/latest/how-to.html#get-files-uploaded-to-a-survey-and-move-them-to-s3) (e.g. images, audio, etc.) to a local directory.
+- Tested against LimeSurvey 6.0.0+ and 5.0.0+ LTS versions.
 
 ## Installation
 
 ```console
 $ pip install citric
 ```
```

#### html2text {}

```diff
@@ -13,16 +13,17 @@
 (https://citric.readthedocs.io/en/latest/rpc_coverage.html) for details. -
 Easily export survey data to CSV files, [Pandas DataFrames](https://
 citric.readthedocs.io/en/latest/how-to.html#export-responses-to-a-pandas-
 dataframe) and [DuckDB databases](https://citric.readthedocs.io/en/latest/how-
 to.html#export-responses-to-a-duckdb-database-and-analyze-with-sql). - Easily
 [download survey files](https://citric.readthedocs.io/en/latest/how-
 to.html#get-files-uploaded-to-a-survey-and-move-them-to-s3) (e.g. images,
-audio, etc.) to a local directory. ## Installation ```console $ pip install
-citric ``` ## Usage ```python from citric import Client with Client( "https://
+audio, etc.) to a local directory. - Tested against LimeSurvey 6.0.0+ and
+5.0.0+ LTS versions. ## Installation ```console $ pip install citric ``` ##
+Usage ```python from citric import Client with Client( "https://
 mylimesite.limequery.com/admin/remotecontrol", "myusername", "mypassword", ) as
 client: for survey in client.list_surveys(): print(survey["surveyls_title"])
 ``` ## Documentation Code samples and API documentation are available at
 [citric.readthedocs.io](https://citric.readthedocs.io/). ## Contributing If
 you'd like to contribute to this project, please see the [contributing guide]
 (https://citric.readthedocs.io/en/latest/contributing/getting-started.html). ##
 Credits - [Claudio Jolowicz][claudio] and [his amazing blog post][hypermodern].
```

### Comparing `citric-0.7.1b1/pyproject.toml` & `citric-0.7.1b2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,7 @@
-[tool.black]
-line-length = 88
-
-[tool.isort]
-include_trailing_comma = true
-known_first_party = "citric"
-multi_line_output = 3 # Vertical Hanging Indent
-profile = "black"
-src_paths = "citric"
-use_parentheses = true
-
-[tool.pytest.ini_options]
-addopts = '-vvv'
-markers = [
-  "integration_test: Integration and end-to-end tests",
-  "version(ref): Mark a test that depends on a specific version of LimeSurvey",
-  "xfail_mysql: Mark a test as expected to fail on MySQL",
-]
-
-[tool.coverage.paths]
-source = ["src", "*/site-packages"]
-
-[tool.coverage.run]
-branch = true
-source = ["citric"]
-
-[tool.coverage.report]
-exclude_lines = [
-    "pragma: no cover",
-    '''if (t\.)?TYPE_CHECKING:''',
-]
-fail_under = 90
-omit = [
-  "src/citric/types.py",
-]
-show_missing = true
-
-[tool.mypy]
-enable_incomplete_feature = "Unpack"
-warn_unreachable = true
-warn_unused_configs = true
-warn_unused_ignores = true
-
-[[tool.mypy.overrides]]
-ignore_missing_imports = true
-module = [
-  "nox.*",
-  "nox_poetry.*",
-  "pytest.*",
-]
-
 [tool.poetry]
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
@@ -73,55 +22,105 @@
 homepage = 'https://github.com/edgarrmondragon/citric'
 keywords = ["limesurvey", "json-rpc"]
 license = "MIT"
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 name = "citric"
 readme = "README.md"
 repository = 'https://github.com/edgarrmondragon/citric'
-version = "0.7.1-b1"
+version = "0.7.1-b2"
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/edgarrmondragon/citric/issues"
 
 [tool.poetry.dependencies]
 importlib_metadata = {version = ">=1.6", python = "<3.8"}
-python = "^3.7.0"
-requests = "^2.23.0"
+python = ">=3.7.0"
+requests = ">=2.23.0"
 
 # Docs
-furo = {version = "^2023.3.27", optional = true}
-myst-parser = {version = "^1.0.0", optional = true}
+furo = {version = ">=2023.3.27", optional = true}
+myst-parser = {version = ">=1.0.0,<2", optional = true}
 sphinx = {version = "<7", optional = true}
-sphinx-autoapi = {version = "^2.1.0", optional = true}
-sphinx-autobuild = {version = "^2021.3.14", optional = true}
-sphinx-autodoc-typehints = {version = "^1.22", optional = true}
-sphinx-copybutton = {version = "^0.5.1", optional = true}
+sphinx-autoapi = {version = ">=2.1.0,<3", optional = true}
+sphinx-autobuild = {version = ">=2021.3.14", optional = true}
+sphinx-autodoc-typehints = {version = ">=1.22,<2", optional = true}
+sphinx-copybutton = {version = ">=0.5.1,<1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
-codecov = "^2.1.4"
-colorama = "^0.4.5"
-coverage = {extras = ["toml"], version = "^7.0.1"}
-faker = "^18.3.1"
-pytest = "^7.1.2"
-pytest-github-actions-annotate-failures = "^0.1.7"
-safety = "^2.1.1"
-typing-extensions = {version = "^4.4.0", python = "<3.12"}
-xdoctest = "^1.0.2"
+colorama = ">=0.4.5,<1"
+coverage = {extras = ["toml"], version = ">=7.0.1,<8"}
+faker = ">=18.3.1,<19"
+pytest = ">=7.3.1,<8"
+pytest-github-actions-annotate-failures = ">=0.1.7,<0.3.0"
+safety = ">=2.1.1,<3"
+typing-extensions = {version = ">=4.4.0,<5", python = "<3.12"}
+xdoctest = ">=1.0.2,<2"
 
 [tool.poetry.extras]
 docs = [
   "furo",
   "myst-parser",
   "sphinx",
   "sphinx-autoapi",
   "sphinx-autobuild",
   "sphinx-autodoc-typehints",
   "sphinx-copybutton",
 ]
 
+[tool.black]
+line-length = 88
+
+[tool.isort]
+include_trailing_comma = true
+known_first_party = "citric"
+multi_line_output = 3 # Vertical Hanging Indent
+profile = "black"
+src_paths = "citric"
+use_parentheses = true
+
+[tool.pytest.ini_options]
+addopts = '-vvv'
+markers = [
+  "integration_test: Integration and end-to-end tests",
+  "version(ref): Mark a test that depends on a specific version of LimeSurvey",
+  "xfail_mysql: Mark a test as expected to fail on MySQL",
+]
+
+[tool.coverage.paths]
+source = ["src", "*/site-packages"]
+
+[tool.coverage.run]
+branch = true
+source = ["citric"]
+
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: no cover",
+    '''if (t\.)?TYPE_CHECKING:''',
+]
+fail_under = 90
+omit = [
+  "src/citric/types.py",
+]
+show_missing = true
+
+[tool.mypy]
+enable_incomplete_feature = "Unpack"
+warn_unreachable = true
+warn_unused_configs = true
+warn_unused_ignores = true
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = [
+  "nox.*",
+  "nox_poetry.*",
+  "pytest.*",
+]
+
 [tool.ruff]
 ignore = [
   "ANN101", # missing-type-self
   "DJ", # flake8-django
 ]
 line-length = 88
 select = ["ALL"]
@@ -151,14 +150,20 @@
 allow-star-arg-any = true
 mypy-init-return = true
 suppress-dummy-args = true
 
 [tool.ruff.flake8-errmsg]
 max-string-length = 30
 
+[tool.ruff.flake8-import-conventions]
+banned-from = ["typing"]
+
+[tool.ruff.flake8-import-conventions.extend-aliases]
+typing = "t"
+
 [tool.ruff.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 
 [tool.ruff.isort]
 known-first-party = ["citric"]
```

### Comparing `citric-0.7.1b1/src/citric/_compat.py` & `citric-0.7.1b2/src/citric/_compat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Compatibility functions and classes for different versions of LimeSurvey."""
 
 from __future__ import annotations
 
+import typing as t
 import warnings
 from functools import wraps
-from typing import Any, Callable
 
 __all__ = ["FutureVersionWarning", "future"]
 
 
 def _warning_message(next_version: str) -> tuple[str, ...]:
     """Format a warning message.
 
@@ -25,29 +25,29 @@
     )
 
 
 class FutureVersionWarning(UserWarning):
     """Warning for features only available in an unreleased version of LimeSurvey."""
 
 
-def future(version: str) -> Callable:
+def future(version: str) -> t.Callable:
     """Mark a function as only available in the current development build of LimeSurvey.
 
     Args:
         version: The earliest version of LimeSurvey that this function is
             available in.
 
     Returns:
         The wrapped function.
     """
     message = _warning_message(version)
 
-    def decorate(fn: Callable) -> Callable:
+    def decorate(fn: t.Callable) -> t.Callable:
         @wraps(fn)
-        def wrapper(*args: Any, **kwargs: Any) -> Callable:
+        def wrapper(*args: t.Any, **kwargs: t.Any) -> t.Callable:
             warnings.warn(
                 f"Method {fn.__name__} {''.join(message)}",
                 FutureVersionWarning,
                 stacklevel=2,
             )
             return fn(*args, **kwargs)
```

### Comparing `citric-0.7.1b1/src/citric/client.py` & `citric-0.7.1b2/src/citric/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 """Python API Client."""
 
 from __future__ import annotations
 
 import base64
 import datetime
 import io
+import typing as t
 from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, TypeVar
 
 import requests
 
 from citric import enums
 from citric.session import Session
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     import sys
     from os import PathLike
     from types import TracebackType
-    from typing import Any, BinaryIO, Generator, Iterable, Mapping, Sequence
 
     from typing_extensions import Unpack
 
     from citric import types
     from citric.objects import Participant
 
     if sys.version_info >= (3, 8):
-        from typing import Literal
+        from typing import Literal  # noqa: ICN003
     else:
         from typing_extensions import Literal
 
 
-_T = TypeVar("_T", bound="Client")
+_T = t.TypeVar("_T", bound="Client")
 
 
 @dataclass
 class QuestionReference:
     """Uploaded file question reference."""
 
     title: str
@@ -215,17 +214,17 @@
         """
         return self.__session.add_language(survey_id, language)
 
     def add_participants(
         self,
         survey_id: int,
         *,
-        participant_data: Sequence[Mapping[str, Any]],
+        participant_data: t.Sequence[t.Mapping[str, t.Any]],
         create_tokens: bool = True,
-    ) -> list[dict[str, Any]]:
+    ) -> list[dict[str, t.Any]]:
         """Add participants to a survey.
 
         Args:
             survey_id: Survey to add participants to.
             participant_data: Information to create participants with.
             create_tokens: Whether to create the participants with tokens.
 
@@ -313,16 +312,16 @@
             language,
             enums.NewSurveyType(survey_format),
         )
 
     def delete_participants(
         self,
         survey_id: int,
-        participant_ids: Sequence[int],
-    ) -> list[dict[str, Any]]:
+        participant_ids: t.Sequence[int],
+    ) -> list[dict[str, t.Any]]:
         """Add participants to a survey.
 
         Args:
             survey_id: Survey to delete participants to.
             participant_ids: Participant IDs to be deleted.
 
         Returns:
@@ -347,17 +346,17 @@
         Returns:
             Question mapping.
         """
         return {q["title"]: q for q in self.list_questions(survey_id)}
 
     @staticmethod
     def _map_response_keys(
-        response_data: Mapping[str, Any],
+        response_data: t.Mapping[str, t.Any],
         question_mapping: dict[str, types.QuestionsListElement],
-    ) -> dict[str, Any]:
+    ) -> dict[str, t.Any]:
         """Convert response keys to LimeSurvey's internal representation.
 
         Args:
             response_data: The response mapping.
             question_mapping: A mapping of question titles to question dictionaries.
 
         Returns:
@@ -403,28 +402,32 @@
         Returns:
             The id of the new group.
 
         .. versionadded:: 0.0.8
         """
         return self.__session.add_group(survey_id, title, description)
 
-    def _add_response(self, survey_id: int, response_data: Mapping[str, Any]) -> int:
+    def _add_response(
+        self,
+        survey_id: int,
+        response_data: t.Mapping[str, t.Any],
+    ) -> int:
         """Add a single response to a survey.
 
         Args:
             survey_id: Survey to add the response to.
             response_data: Single response as a mapping from question codes of the form
                 <SID>X<GID>X<QID> to response values.
 
         Returns:
             ID of the new response.
         """
         return int(self.__session.add_response(survey_id, response_data))
 
-    def add_response(self, survey_id: int, response_data: Mapping[str, Any]) -> int:
+    def add_response(self, survey_id: int, response_data: t.Mapping[str, t.Any]) -> int:
         """Add a single response to a survey.
 
         Args:
             survey_id: Survey to add the response to.
             response_data: Single response as a mapping.
 
         Returns:
@@ -436,15 +439,15 @@
         questions = self._get_question_mapping(survey_id)
         data = self._map_response_keys(response_data, questions)
         return self._add_response(survey_id, data)
 
     def add_responses(
         self,
         survey_id: int,
-        responses: Iterable[Mapping[str, Any]],
+        responses: t.Iterable[t.Mapping[str, t.Any]],
     ) -> list[int]:
         """Add multiple responses to a survey.
 
         Args:
             survey_id: Survey to add the response to.
             responses: Iterable of survey responses.
 
@@ -457,15 +460,15 @@
         questions = self._get_question_mapping(survey_id)
         for response in responses:
             data = self._map_response_keys(response, questions)
             response_id = self._add_response(survey_id, data)
             ids.append(response_id)
         return ids
 
-    def update_response(self, survey_id: int, response_data: dict[str, Any]) -> bool:
+    def update_response(self, survey_id: int, response_data: dict[str, t.Any]) -> bool:
         """Update a response.
 
         Args:
             survey_id: Survey to update the response in.
             response_data: Response data to update.
 
         Returns:
@@ -473,15 +476,15 @@
 
         .. versionadded:: 0.2.0
         """
         questions = self._get_question_mapping(survey_id)
         data = self._map_response_keys(response_data, questions)
         return self.__session.update_response(survey_id, data)
 
-    def copy_survey(self, survey_id: int, name: str) -> dict[str, Any]:
+    def copy_survey(self, survey_id: int, name: str) -> dict[str, t.Any]:
         """Copy a survey.
 
         Args:
             survey_id: ID of the source survey.
             name: Name of the new survey.
 
         Returns:
@@ -489,15 +492,15 @@
 
         .. versionadded:: 0.0.10
         """
         return self.__session.copy_survey(survey_id, name)
 
     def import_cpdb_participants(
         self,
-        participants: Sequence[Participant],
+        participants: t.Sequence[Participant],
         *,
         update: bool = False,
     ) -> types.CPDBParticipantImportResult:
         """Import CPDB participants.
 
         Args:
             participants: CPDB participant data.
@@ -609,15 +612,15 @@
         file_format: str | enums.ResponsesExportFormat = "json",
         language: str | None = None,
         completion_status: str | enums.SurveyCompletionStatus = "all",
         heading_type: str | enums.HeadingType = "code",
         response_type: str | enums.ResponseType = "short",
         from_response_id: int | None = None,
         to_response_id: int | None = None,
-        fields: Sequence[str] | None = None,
+        fields: t.Sequence[str] | None = None,
     ) -> bytes:
         """Export responses to a file-like object.
 
         Args:
             survey_id: Survey to add the response to.
             token: Optional participant token to get responses for.
             file_format: Type of export. One of PDF, CSV, XLS, DOC or JSON.
@@ -676,15 +679,15 @@
         file_format: str = "json",
         language: str | None = None,
         completion_status: str = "all",
         heading_type: str = "code",
         response_type: str = "short",
         from_response_id: int | None = None,
         to_response_id: int | None = None,
-        fields: Sequence[str] | None = None,
+        fields: t.Sequence[str] | None = None,
     ) -> int:
         """Save responses to a file.
 
         Args:
             filename: Target file path.
             survey_id: Survey to add the response to.
             token: Optional participant token to get responses for.
@@ -859,17 +862,17 @@
         .. versionadded:: 0.0.10
         """
         return self.__session.get_language_properties(survey_id, settings, language)
 
     def get_participant_properties(
         self,
         survey_id: int,
-        query: dict[str, Any] | int,
-        properties: Sequence[str] | None = None,
-    ) -> dict[str, Any]:
+        query: dict[str, t.Any] | int,
+        properties: t.Sequence[str] | None = None,
+    ) -> dict[str, t.Any]:
         """Get properties a single survey participant.
 
         Args:
             survey_id: Survey to get participants properties.
             query: Mapping of properties to query participants, or the token id
                 as an integer.
             properties: Which participant properties to retrieve.
@@ -1031,15 +1034,15 @@
         .. versionadded:: 0.0.10
         """
         return self.session.get_summary(survey_id)
 
     def get_survey_properties(
         self,
         survey_id: int,
-        properties: Sequence[str] | None = None,
+        properties: t.Sequence[str] | None = None,
     ) -> types.SurveyProperties:
         """Get properties of a survey.
 
         Args:
             survey_id: Survey to get properties.
             properties: Which survey properties to retrieve. If none, gets all fields.
 
@@ -1050,15 +1053,15 @@
         """
         return self.__session.get_survey_properties(survey_id, properties)
 
     def get_uploaded_files(
         self,
         survey_id: int,
         token: str | None = None,
-    ) -> dict[str, dict[str, Any]]:
+    ) -> dict[str, dict[str, t.Any]]:
         """Get a dictionary of files uploaded in a survey response.
 
         Args:
             survey_id: Survey for which to download files.
             token: Optional participant token to filter uploaded files.
 
         Returns:
@@ -1068,15 +1071,15 @@
         """
         return self.__session.get_uploaded_files(survey_id, token)
 
     def get_uploaded_file_objects(
         self,
         survey_id: int,
         token: str | None = None,
-    ) -> Generator[UploadedFile, None, None]:
+    ) -> t.Generator[UploadedFile, None, None]:
         """Iterate over uploaded files in a survey response.
 
         Args:
             survey_id: Survey for which to download files.
             token: Optional participant token to filter uploaded files.
 
         Yields:
@@ -1127,15 +1130,15 @@
             with Path(filepath).open("wb") as f:
                 f.write(file.content.read())
 
         return filepaths
 
     def import_group(
         self,
-        file: BinaryIO,
+        file: t.BinaryIO,
         survey_id: int,
         file_type: str | enums.ImportGroupType = "lsg",
     ) -> int:
         """Import group from a file.
 
         Create a new group from an exported LSG file.
 
@@ -1156,15 +1159,15 @@
             survey_id,
             contents,
             enums.ImportGroupType(file_type),
         )
 
     def import_question(
         self,
-        file: BinaryIO,
+        file: t.BinaryIO,
         survey_id: int,
         group_id: int,
     ) -> int:
         """Import question from a file.
 
         Create a new question from an exported LSQ file.
 
@@ -1186,15 +1189,15 @@
             group_id,
             contents,
             "lsq",
         )
 
     def import_survey(
         self,
-        file: BinaryIO,
+        file: t.BinaryIO,
         file_type: str | enums.ImportSurveyType = "lss",
         survey_name: str | None = None,
         survey_id: int | None = None,
     ) -> int:
         """Import survey from a file.
 
         Create a new survey from an exported LSS, CSV, TXT or LSA file.
@@ -1224,17 +1227,17 @@
     def list_participants(
         self,
         survey_id: int,
         *,
         start: int = 0,
         limit: int = 10,
         unused: bool = False,
-        attributes: Sequence[str] | bool = False,
-        conditions: Mapping[str, Any] | None = None,
-    ) -> list[dict[str, Any]]:
+        attributes: t.Sequence[str] | bool = False,
+        conditions: t.Mapping[str, t.Any] | None = None,
+    ) -> list[dict[str, t.Any]]:
         """Get participants in a survey.
 
         Args:
             survey_id: Survey to get participants from.
             start: Retrieve participants starting from this index (zero-indexed).
             limit: Maximum number of participants to retrieve.
             unused: Retrieve partipants with unused tokens.
@@ -1253,29 +1256,29 @@
             start,
             limit,
             unused,
             attributes,
             conditions or {},
         )
 
-    def list_users(self) -> list[dict[str, Any]]:
+    def list_users(self) -> list[dict[str, t.Any]]:
         """Get LimeSurvey users.
 
         Returns:
             List of users.
 
         .. versionadded:: 0.0.3
         """
         return self.__session.list_users()
 
     def list_groups(
         self,
         survey_id: int,
         language: str | None = None,
-    ) -> list[dict[str, Any]]:
+    ) -> list[dict[str, t.Any]]:
         """Get the IDs and all attributes of all question groups in a Survey.
 
         Args:
             survey_id: ID of the Survey containing the groups.
             language: Optional parameter language for multilingual groups.
 
         Returns:
@@ -1315,15 +1318,15 @@
             List of quotas.
 
         .. versionadded:: 0.6.0
         .. minlimesurvey:: 6.0.0
         """
         return self.session.list_quotas(survey_id)
 
-    def list_surveys(self, username: str | None = None) -> list[dict[str, Any]]:
+    def list_surveys(self, username: str | None = None) -> list[dict[str, t.Any]]:
         """Get all surveys or only those owned by a user.
 
         Args:
             username: Owner of the surveys to retrieve.
 
         Returns:
             List of surveys with basic information.
@@ -1331,15 +1334,15 @@
         .. versionadded:: 0.0.1
         """
         return self.__session.list_surveys(username)
 
     def list_survey_groups(
         self,
         username: str | None = None,
-    ) -> list[dict[str, Any]]:
+    ) -> list[dict[str, t.Any]]:
         """Get all survey groups or only those owned by a user.
 
         Args:
             username: Owner of the survey groups to retrieve.
 
         Returns:
             List of survey groups with basic information.
@@ -1367,15 +1370,15 @@
         return self.session.set_group_properties(group_id, properties)
 
     def set_language_properties(
         self,
         survey_id: int,
         language: str | None = None,
         **properties: Unpack[types.LanguageProperties],
-    ) -> dict[str, Any]:
+    ) -> dict[str, t.Any]:
         """Set properties of a survey language.
 
         Args:
             survey_id: ID of the survey for which to set the language properties.
             language: Language code.
             properties: Properties to set.
 
@@ -1385,17 +1388,17 @@
         .. versionadded:: 0.0.11
         """
         return self.session.set_language_properties(survey_id, properties, language)
 
     def set_participant_properties(
         self,
         survey_id: int,
-        token_query_properties: Mapping[str, Any] | int,
-        **token_data: Any,
-    ) -> dict[str, Any]:
+        token_query_properties: t.Mapping[str, t.Any] | int,
+        **token_data: t.Any,
+    ) -> dict[str, t.Any]:
         """Set properties of a participant. Only one particpant can be updated.
 
         Args:
             survey_id: ID of the survey to which the participant belongs.
             token_query_properties: Dictionary of properties to match the participant
                 or token ID.
             token_data: Properties to set.
@@ -1470,15 +1473,15 @@
         return self.session.set_survey_properties(survey_id, properties)
 
     def upload_file_object(
         self,
         survey_id: int,
         field: str,
         filename: str,
-        file: BinaryIO,
+        file: t.BinaryIO,
     ) -> types.FileUploadResult:
         """Upload a file to a LimeSurvey survey.
 
         Args:
             survey_id: ID of the survey to upload the file to.
             field: Field name to upload the file to.
             filename: Name of the file to upload.
```

### Comparing `citric-0.7.1b1/src/citric/enums.py` & `citric-0.7.1b2/src/citric/enums.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b1/src/citric/exceptions.py` & `citric-0.7.1b2/src/citric/exceptions.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b1/src/citric/method.py` & `citric-0.7.1b2/src/citric/method.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """RPC methods."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Generic, TypeVar
+import typing as t
 
-if TYPE_CHECKING:
-    from typing import Any, Callable
+T = t.TypeVar("T")
 
-T = TypeVar("T")
 
-
-class Method(Generic[T]):
+class Method(t.Generic[T]):
     """RPC method."""
 
-    def __init__(self, caller: Callable[[str], T], name: str) -> None:
+    def __init__(self, caller: t.Callable[[str], T], name: str) -> None:
         """Instantiate an RPC method."""
         self.__caller = caller
         self.__name = name
 
     def __getattr__(self, name: str) -> Method:
         """Get nested method.
 
@@ -29,15 +26,15 @@
 
         >>> method = Method(print, "some_method")
         >>> method.nested("x", "y")
         some_method.nested x y
         """
         return Method(self.__caller, f"{self.__name}.{name}")
 
-    def __call__(self, *params: Any) -> T:
+    def __call__(self, *params: t.Any) -> T:
         """Call RPC method.
 
         Args:
             params: RPC method parameters.
 
         Returns:
             An RPC result.
```

### Comparing `citric-0.7.1b1/src/citric/objects.py` & `citric-0.7.1b2/src/citric/objects.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b1/src/citric/session.py` & `citric-0.7.1b2/src/citric/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Low level wrapper for connecting to the LSRC2."""
 
 from __future__ import annotations
 
 import json
 import logging
 import random
-from typing import TYPE_CHECKING, Any, TypeVar
+import typing as t
 
 import requests
 
 from citric.exceptions import (
     InvalidJSONResponseError,
     LimeSurveyApiError,
     LimeSurveyStatusError,
     ResponseMismatchError,
     RPCInterfaceNotEnabledError,
 )
 from citric.method import Method
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     from types import TracebackType
 
     from citric.types import Result, RPCResponse
 
 __all__ = ["Session"]
 
 GET_SESSION_KEY = "get_session_key"
-_T = TypeVar("_T", bound="Session")
+_T = t.TypeVar("_T", bound="Session")
 
 logger = logging.getLogger(__name__)
 
 
 def handle_rpc_errors(result: Result, error: str | None) -> None:
     """Handle RPC errors.
 
@@ -127,15 +127,15 @@
         """RPC session key."""
         return self.__key
 
     def __getattr__(self, name: str) -> Method[Result]:
         """Magic method dispatcher."""
         return Method(self.rpc, name)
 
-    def rpc(self, method: str, *params: Any) -> Result:
+    def rpc(self, method: str, *params: t.Any) -> Result:
         """Execute RPC method on LimeSurvey, with optional token authentication.
 
         Any method, except for `get_session_key`.
 
         Args:
             method: Name of the method to call.
             params: Positional arguments of the RPC method.
@@ -148,15 +148,15 @@
 
         # Methods requiring authentication
         return self._invoke(method, self.key, *params)
 
     def _invoke(
         self,
         method: str,
-        *params: Any,
+        *params: t.Any,
     ) -> Result:
         """Execute a LimeSurvey RPC with a JSON payload.
 
         Args:
             method: Name of the method to call.
             params: Positional arguments of the RPC method.
```

### Comparing `citric-0.7.1b1/src/citric/types.py` & `citric-0.7.1b2/src/citric/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 
 from __future__ import annotations
 
 import sys
 import typing as t
 
 if sys.version_info >= (3, 8):
-    from typing import Literal, TypedDict
+    from typing import Literal, TypedDict  # noqa: ICN003
 else:
     from typing_extensions import Literal, TypedDict
 
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias  # noqa: ICN003
+else:
+    from typing_extensions import TypeAlias
+
 if t.TYPE_CHECKING:
     from citric import enums
 
-Result = t.Any
-YesNo = Literal["Y", "N"]
+Result: TypeAlias = t.Any
+YesNo: TypeAlias = Literal["Y", "N"]
 
 
 class FileUploadResult(TypedDict):
     """File upload result.
 
     Keys:
         success: Whether the file was uploaded successfully.
```

### Comparing `citric-0.7.1b1/PKG-INFO` & `citric-0.7.1b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: citric
-Version: 0.7.1b1
+Version: 0.7.1b2
 Summary: A client to the LimeSurvey Remote Control API 2, written in modern Python.
 Home-page: https://github.com/edgarrmondragon/citric
 License: MIT
 Keywords: limesurvey,json-rpc
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
 Maintainer-email: edgarrm358@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.7.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -28,23 +28,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: docs
-Requires-Dist: furo (>=2023.3.27,<2024.0.0) ; extra == "docs"
+Requires-Dist: furo (>=2023.3.27) ; extra == "docs"
 Requires-Dist: importlib_metadata (>=1.6) ; python_version < "3.8"
-Requires-Dist: myst-parser (>=1.0.0,<2.0.0) ; extra == "docs"
-Requires-Dist: requests (>=2.23.0,<3.0.0)
+Requires-Dist: myst-parser (>=1.0.0,<2) ; extra == "docs"
+Requires-Dist: requests (>=2.23.0)
 Requires-Dist: sphinx (<7) ; extra == "docs"
-Requires-Dist: sphinx-autoapi (>=2.1.0,<3.0.0) ; extra == "docs"
-Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints (>=1.22,<2.0) ; extra == "docs"
-Requires-Dist: sphinx-copybutton (>=0.5.1,<0.6.0) ; extra == "docs"
+Requires-Dist: sphinx-autoapi (>=2.1.0,<3) ; extra == "docs"
+Requires-Dist: sphinx-autobuild (>=2021.3.14) ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints (>=1.22,<2) ; extra == "docs"
+Requires-Dist: sphinx-copybutton (>=0.5.1,<1) ; extra == "docs"
 Project-URL: Documentation, https://citric.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/edgarrmondragon/citric/issues
 Project-URL: Repository, https://github.com/edgarrmondragon/citric
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -105,14 +105,15 @@
 
 ## Features
 
 - Supports the full RPC API via the [`Session` class](https://citric.readthedocs.io/en/latest/_api/citric/session/index.html#citric.session.Session).
 - Best effort to implement all the RPC methods in the [`Client` class](https://citric.readthedocs.io/en/latest/_api/citric/client/index.html#citric.client.Client). See the [API coverage page](https://citric.readthedocs.io/en/latest/rpc_coverage.html) for details.
 - Easily export survey data to CSV files, [Pandas DataFrames](https://citric.readthedocs.io/en/latest/how-to.html#export-responses-to-a-pandas-dataframe) and [DuckDB databases](https://citric.readthedocs.io/en/latest/how-to.html#export-responses-to-a-duckdb-database-and-analyze-with-sql).
 - Easily [download survey files](https://citric.readthedocs.io/en/latest/how-to.html#get-files-uploaded-to-a-survey-and-move-them-to-s3) (e.g. images, audio, etc.) to a local directory.
+- Tested against LimeSurvey 6.0.0+ and 5.0.0+ LTS versions.
 
 ## Installation
 
 ```console
 $ pip install citric
 ```
```

#### html2text {}

```diff
@@ -1,35 +1,34 @@
-Metadata-Version: 2.1 Name: citric Version: 0.7.1b1 Summary: A client to the
+Metadata-Version: 2.1 Name: citric Version: 0.7.1b2 Summary: A client to the
 LimeSurvey Remote Control API 2, written in modern Python. Home-page: https://
 github.com/edgarrmondragon/citric License: MIT Keywords: limesurvey,json-rpc
 Author: Edgar RamÃ­rez-MondragÃ³n Author-email: edgarrm358@gmail.com
 Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email: edgarrm358@gmail.com
-Requires-Python: >=3.7.0,<4.0.0 Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Programming Language :: Python
-:: Implementation :: PyPy Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Typing :: Typed Provides-Extra: docs
-Requires-Dist: furo (>=2023.3.27,<2024.0.0) ; extra == "docs" Requires-Dist:
-importlib_metadata (>=1.6) ; python_version < "3.8" Requires-Dist: myst-parser
-(>=1.0.0,<2.0.0) ; extra == "docs" Requires-Dist: requests (>=2.23.0,<3.0.0)
-Requires-Dist: sphinx (<7) ; extra == "docs" Requires-Dist: sphinx-autoapi
-(>=2.1.0,<3.0.0) ; extra == "docs" Requires-Dist: sphinx-autobuild
-(>=2021.3.14,<2022.0.0) ; extra == "docs" Requires-Dist: sphinx-autodoc-
-typehints (>=1.22,<2.0) ; extra == "docs" Requires-Dist: sphinx-copybutton
-(>=0.5.1,<0.6.0) ; extra == "docs" Project-URL: Documentation, https://
+Requires-Python: >=3.7.0 Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Typing :: Typed Provides-Extra: docs Requires-
+Dist: furo (>=2023.3.27) ; extra == "docs" Requires-Dist: importlib_metadata
+(>=1.6) ; python_version < "3.8" Requires-Dist: myst-parser (>=1.0.0,<2) ;
+extra == "docs" Requires-Dist: requests (>=2.23.0) Requires-Dist: sphinx (<7) ;
+extra == "docs" Requires-Dist: sphinx-autoapi (>=2.1.0,<3) ; extra == "docs"
+Requires-Dist: sphinx-autobuild (>=2021.3.14) ; extra == "docs" Requires-Dist:
+sphinx-autodoc-typehints (>=1.22,<2) ; extra == "docs" Requires-Dist: sphinx-
+copybutton (>=0.5.1,<1) ; extra == "docs" Project-URL: Documentation, https://
 citric.readthedocs.io Project-URL: Issue Tracker, https://github.com/
 edgarrmondragon/citric/issues Project-URL: Repository, https://github.com/
 edgarrmondragon/citric Description-Content-Type: text/markdown
                                    # Citric
   [Tests] [pre-commit.ci_status] [License] [Documentation_Status] [codecov]
                                 [FOSSA_Status]
       [PyPI_version] [Python_versions] [PyPI_-_Downloads] [PyPI_-_Format]
@@ -44,16 +43,17 @@
 (https://citric.readthedocs.io/en/latest/rpc_coverage.html) for details. -
 Easily export survey data to CSV files, [Pandas DataFrames](https://
 citric.readthedocs.io/en/latest/how-to.html#export-responses-to-a-pandas-
 dataframe) and [DuckDB databases](https://citric.readthedocs.io/en/latest/how-
 to.html#export-responses-to-a-duckdb-database-and-analyze-with-sql). - Easily
 [download survey files](https://citric.readthedocs.io/en/latest/how-
 to.html#get-files-uploaded-to-a-survey-and-move-them-to-s3) (e.g. images,
-audio, etc.) to a local directory. ## Installation ```console $ pip install
-citric ``` ## Usage ```python from citric import Client with Client( "https://
+audio, etc.) to a local directory. - Tested against LimeSurvey 6.0.0+ and
+5.0.0+ LTS versions. ## Installation ```console $ pip install citric ``` ##
+Usage ```python from citric import Client with Client( "https://
 mylimesite.limequery.com/admin/remotecontrol", "myusername", "mypassword", ) as
 client: for survey in client.list_surveys(): print(survey["surveyls_title"])
 ``` ## Documentation Code samples and API documentation are available at
 [citric.readthedocs.io](https://citric.readthedocs.io/). ## Contributing If
 you'd like to contribute to this project, please see the [contributing guide]
 (https://citric.readthedocs.io/en/latest/contributing/getting-started.html). ##
 Credits - [Claudio Jolowicz][claudio] and [his amazing blog post][hypermodern].
```

