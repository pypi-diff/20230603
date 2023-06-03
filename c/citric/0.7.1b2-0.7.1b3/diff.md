# Comparing `tmp/citric-0.7.1b2.tar.gz` & `tmp/citric-0.7.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citric-0.7.1b2.tar", max compression
+gzip compressed data, was "citric-0.7.1b3.tar", max compression
```

## Comparing `citric-0.7.1b2.tar` & `citric-0.7.1b3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-05-12 03:07:57.074755 citric-0.7.1b2/LICENSE
--rw-r--r--   0        0        0     4551 2023-05-12 03:07:57.074755 citric-0.7.1b2/README.md
--rw-r--r--   0        0        0     4393 2023-05-12 03:07:57.082755 citric-0.7.1b2/pyproject.toml
--rw-r--r--   0        0        0      399 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/__init__.py
--rw-r--r--   0        0        0     1509 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/_compat.py
--rw-r--r--   0        0        0    44916 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/client.py
--rw-r--r--   0        0        0     1739 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/enums.py
--rw-r--r--   0        0        0     1345 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/exceptions.py
--rw-r--r--   0        0        0     1055 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/method.py
--rw-r--r--   0        0        0     1171 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/objects.py
--rw-r--r--   0        0        0        0 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/py.typed
--rw-r--r--   0        0        0     6964 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/session.py
--rw-r--r--   0        0        0    14009 2023-05-12 03:07:57.082755 citric-0.7.1b2/src/citric/types.py
--rw-r--r--   0        0        0     6818 1970-01-01 00:00:00.000000 citric-0.7.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-01 04:42:30.650182 citric-0.7.1b3/LICENSE
+-rw-r--r--   0        0        0     4775 2023-06-01 04:42:30.650182 citric-0.7.1b3/README.md
+-rw-r--r--   0        0        0     4390 2023-06-01 04:42:30.654182 citric-0.7.1b3/pyproject.toml
+-rw-r--r--   0        0        0      399 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/__init__.py
+-rw-r--r--   0        0        0     1509 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/_compat.py
+-rw-r--r--   0        0        0    46924 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/client.py
+-rw-r--r--   0        0        0     1739 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/enums.py
+-rw-r--r--   0        0        0     1345 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/exceptions.py
+-rw-r--r--   0        0        0     1055 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/method.py
+-rw-r--r--   0        0        0     1171 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/objects.py
+-rw-r--r--   0        0        0        0 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/py.typed
+-rw-r--r--   0        0        0     6964 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/session.py
+-rw-r--r--   0        0        0    14009 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/types.py
+-rw-r--r--   0        0        0     6790 1970-01-01 00:00:00.000000 citric-0.7.1b3/PKG-INFO
```

### Comparing `citric-0.7.1b2/LICENSE` & `citric-0.7.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b2/README.md` & `citric-0.7.1b3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
   </a>
   <a href="https://github.com/edgarrmondragon/citric/blob/main/LICENSE">
     <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/citric"/>
   </a>
   <a href="https://citric.readthedocs.io/en/latest/?badge=latest">
     <img alt="Documentation Status" src="https://readthedocs.org/projects/citric/badge/?version=latest"/>
   </a>
+  <a href="https://github.com/charliermarsh/ruff">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
+  </a>
   <a href="https://codecov.io/gh/edgarrmondragon/citric">
     <img alt="codecov" src="https://codecov.io/gh/edgarrmondragon/citric/branch/main/graph/badge.svg"/>
   </a>
   <a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fedgarrmondragon%2Fcitric?ref=badge_shield">
     <img alt="FOSSA Status" src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fedgarrmondragon%2Fcitric.svg?type=shield"/>
   </a>
 </div>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                                    # Citric
-  [Tests] [pre-commit.ci_status] [License] [Documentation_Status] [codecov]
-                                [FOSSA_Status]
+    [Tests] [pre-commit.ci_status] [License] [Documentation_Status] [Ruff]
+                           [codecov] [FOSSA_Status]
       [PyPI_version] [Python_versions] [PyPI_-_Downloads] [PyPI_-_Format]
    [GitHub_languages] [GitHub repo size] [GitHub_stars] [Github_last-commit]
           A client to the [LimeSurvey Remote Control API 2](https://
      manual.limesurvey.org/RemoteControl_2_API), written in modern Python.
 ## Features - Supports the full RPC API via the [`Session` class](https://
 citric.readthedocs.io/en/latest/_api/citric/session/
 index.html#citric.session.Session). - Best effort to implement all the RPC
```

### Comparing `citric-0.7.1b2/pyproject.toml` & `citric-0.7.1b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 homepage = 'https://github.com/edgarrmondragon/citric'
 keywords = ["limesurvey", "json-rpc"]
 license = "MIT"
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 name = "citric"
 readme = "README.md"
 repository = 'https://github.com/edgarrmondragon/citric'
-version = "0.7.1-b2"
+version = "0.7.1-b3"
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/edgarrmondragon/citric/issues"
 
 [tool.poetry.dependencies]
 importlib_metadata = {version = ">=1.6", python = "<3.8"}
 python = ">=3.7.0"
@@ -65,22 +65,14 @@
   "sphinx-autodoc-typehints",
   "sphinx-copybutton",
 ]
 
 [tool.black]
 line-length = 88
 
-[tool.isort]
-include_trailing_comma = true
-known_first_party = "citric"
-multi_line_output = 3 # Vertical Hanging Indent
-profile = "black"
-src_paths = "citric"
-use_parentheses = true
-
 [tool.pytest.ini_options]
 addopts = '-vvv'
 markers = [
   "integration_test: Integration and end-to-end tests",
   "version(ref): Mark a test that depends on a specific version of LimeSurvey",
   "xfail_mysql: Mark a test as expected to fail on MySQL",
 ]
@@ -113,14 +105,17 @@
 ignore_missing_imports = true
 module = [
   "nox.*",
   "nox_poetry.*",
   "pytest.*",
 ]
 
+[tool.codespell]
+skip = ".mypy_cache,.nox,.ruff_cache,build,docs/index.md,poetry.lock"
+
 [tool.ruff]
 ignore = [
   "ANN101", # missing-type-self
   "DJ", # flake8-django
 ]
 line-length = 88
 select = ["ALL"]
@@ -162,19 +157,23 @@
 
 [tool.ruff.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 
 [tool.ruff.isort]
 known-first-party = ["citric"]
+required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.mccabe]
 max-complexity = 5
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
+[tool.ruff.pylint]
+max-args = 10
+
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = [
   "poetry-core>=1",
 ]
```

### Comparing `citric-0.7.1b2/src/citric/_compat.py` & `citric-0.7.1b3/src/citric/_compat.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b2/src/citric/client.py` & `citric-0.7.1b3/src/citric/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,27 +152,31 @@
     def session(self) -> Session:
         """Low-level RPC session."""
         return self.__session
 
     def get_fieldmap(self, survey_id: int) -> dict:
         """Get fieldmap for a survey.
 
+        Calls :rpc_method:`get_fieldmap`.
+
         Args:
             survey_id: ID of survey to get fieldmap for.
 
         Returns:
             Dictionary mapping response keys to LimeSurvey internal representation.
 
         .. versionadded:: 0.3.0
         """
         return self.__session.get_fieldmap(survey_id)
 
     def activate_survey(self, survey_id: int) -> types.OperationStatus:
         """Activate a survey.
 
+        Calls :rpc_method:`activate_survey`.
+
         Args:
             survey_id: ID of survey to be activated.
 
         Returns:
             Status and plugin feedback.
 
         .. versionadded:: 0.0.1
@@ -184,28 +188,32 @@
         survey_id: int,
         attributes: list[int] | None = None,
     ) -> types.OperationStatus:
         """Initialise the survey participant table.
 
         New participant tokens may be later added.
 
+        Calls :rpc_method:`activate_tokens`.
+
         Args:
             survey_id: ID of survey to be activated.
             attributes: Optional list of participant attributes numbers to be activated.
 
         Returns:
             Status message.
 
         .. versionadded:: 0.0.1
         """
         return self.__session.activate_tokens(survey_id, attributes or [])
 
     def add_language(self, survey_id: int, language: str) -> types.OperationStatus:
         """Add a survey language.
 
+        Calls :rpc_method:`add_language`.
+
         Args:
             survey_id: ID of the Survey for which a language will be added.
             language: A valid language shortcut to add to the current Survey. If the
                 language already exists no error will be given.
 
         Returns:
             Status message.
@@ -219,14 +227,16 @@
         survey_id: int,
         *,
         participant_data: t.Sequence[t.Mapping[str, t.Any]],
         create_tokens: bool = True,
     ) -> list[dict[str, t.Any]]:
         """Add participants to a survey.
 
+        Calls :rpc_method:`add_participants`.
+
         Args:
             survey_id: Survey to add participants to.
             participant_data: Information to create participants with.
             create_tokens: Whether to create the participants with tokens.
 
         Returns:
             Information of newly created participants.
@@ -252,14 +262,16 @@
         autoload_url: bool = False,
         message: str = "",
         url: str = "",
         url_description: str = "",
     ) -> int:
         """Add a quota to a LimeSurvey survey.
 
+        Calls :rpc_method:`add_quota`.
+
         Args:
             survey_id: ID of the survey to add the quota to.
             name: Name of the quota.
             limit: Limit of the quota.
             active: Whether the quota is active.
             action: Action to take when the limit is reached.
             autoload_url: Whether to automatically load the URL.
@@ -290,14 +302,16 @@
         survey_id: int,
         title: str,
         language: str,
         survey_format: str | enums.NewSurveyType = "G",
     ) -> int:
         """Add a new empty survey.
 
+        Calls :rpc_method:`add_survey`.
+
         Args:
             survey_id: The desired ID of the Survey to add.
             title: Title of the new Survey.
             language: Default language of the Survey.
             survey_format: Question appearance format (A, G or S) for "All on one page",
                 "Group by Group", "Single questions", default to group by group (G).
 
@@ -316,14 +330,16 @@
     def delete_participants(
         self,
         survey_id: int,
         participant_ids: t.Sequence[int],
     ) -> list[dict[str, t.Any]]:
         """Add participants to a survey.
 
+        Calls :rpc_method:`delete_participants`.
+
         Args:
             survey_id: Survey to delete participants to.
             participant_ids: Participant IDs to be deleted.
 
         Returns:
             Information of removed participants.
 
@@ -390,14 +406,16 @@
             ): value
             for key, value in response_data.items()
         }
 
     def add_group(self, survey_id: int, title: str, description: str = "") -> int:
         """Add a new empty question group to a survey.
 
+        Calls :rpc_method:`add_group`.
+
         Args:
             survey_id: ID of the Survey to add the group.
             title: Name of the group.
             description: Optional description of the group.
 
         Returns:
             The id of the new group.
@@ -463,14 +481,16 @@
             response_id = self._add_response(survey_id, data)
             ids.append(response_id)
         return ids
 
     def update_response(self, survey_id: int, response_data: dict[str, t.Any]) -> bool:
         """Update a response.
 
+        Calls :rpc_method:`update_response`.
+
         Args:
             survey_id: Survey to update the response in.
             response_data: Response data to update.
 
         Returns:
             True if the response was updated, False otherwise.
 
@@ -479,14 +499,16 @@
         questions = self._get_question_mapping(survey_id)
         data = self._map_response_keys(response_data, questions)
         return self.__session.update_response(survey_id, data)
 
     def copy_survey(self, survey_id: int, name: str) -> dict[str, t.Any]:
         """Copy a survey.
 
+        Calls :rpc_method:`copy_survey`.
+
         Args:
             survey_id: ID of the source survey.
             name: Name of the new survey.
 
         Returns:
             Dictionary of status message and the new survey ID.
 
@@ -498,14 +520,16 @@
         self,
         participants: t.Sequence[Participant],
         *,
         update: bool = False,
     ) -> types.CPDBParticipantImportResult:
         """Import CPDB participants.
 
+        Calls :rpc_method:`cpd_importParticipants`.
+
         Args:
             participants: CPDB participant data.
             update: Whether to update existing participants.
 
         Returns:
             IDs of the new participants.
 
@@ -544,14 +568,16 @@
         .. minlimesurvey:: 5.3.4
         """
         return self.__session.delete_language(survey_id, language)
 
     def delete_quota(self, quota_id: int) -> types.OperationStatus:
         """Delete a LimeSurvey quota.
 
+        Calls :rpc_method:`delete_quota`.
+
         Args:
             quota_id: ID of the quota to delete.
 
         Returns:
             True if the quota was deleted.
 
         .. versionadded:: 0.6.0
@@ -576,39 +602,43 @@
         .. versionadded:: 0.0.2
         """
         return self.__session.delete_response(survey_id, response_id)
 
     def delete_question(self, question_id: int) -> int:
         """Delete a survey.
 
+        Calls :rpc_method:`delete_question`.
+
         Args:
             question_id: ID of Question to delete.
 
         Returns:
             ID of the deleted question.
 
         .. versionadded:: 0.1.0
         .. minlimesurvey:: 5.3.19
         """
         return self.__session.delete_question(question_id)
 
     def delete_survey(self, survey_id: int) -> types.OperationStatus:
         """Delete a survey.
 
+        Calls :rpc_method:`delete_survey`.
+
         Args:
             survey_id: Survey to delete.
 
         Returns:
             Status message.
 
         .. versionadded:: 0.0.1
         """
         return self.__session.delete_survey(survey_id)
 
-    def export_responses(
+    def export_responses(  # noqa: PLR0913
         self,
         survey_id: int,
         *,
         token: str | None = None,
         file_format: str | enums.ResponsesExportFormat = "json",
         language: str | None = None,
         completion_status: str | enums.SurveyCompletionStatus = "all",
@@ -616,14 +646,16 @@
         response_type: str | enums.ResponseType = "short",
         from_response_id: int | None = None,
         to_response_id: int | None = None,
         fields: t.Sequence[str] | None = None,
     ) -> bytes:
         """Export responses to a file-like object.
 
+        Calls :rpc_method:`export_responses`.
+
         Args:
             survey_id: Survey to add the response to.
             token: Optional participant token to get responses for.
             file_format: Type of export. One of PDF, CSV, XLS, DOC or JSON.
             language: Export responses made to this language version of the survey.
             completion_status: Incomplete, complete or all.
             heading_type: Use response codes, long or abbreviated titles.
@@ -666,15 +698,15 @@
                 enums.ResponseType(response_type),
                 from_response_id,
                 to_response_id,
                 fields,
             ),
         )
 
-    def save_responses(
+    def save_responses(  # noqa: PLR0913
         self,
         filename: PathLike,
         survey_id: int,
         *,
         token: str | None = None,
         file_format: str = "json",
         language: str | None = None,
@@ -728,14 +760,16 @@
         file_format: str | enums.StatisticsExportFormat = "pdf",
         language: str | None = None,
         graph: bool = False,
         group_ids: list[int] | None = None,
     ) -> bytes:
         """Export survey statistics.
 
+        Calls :rpc_method:`export_statistics`.
+
         Args:
             survey_id: ID of the Survey.
             file_format: Type of documents the exported statistics should be.
                 Defaults to "pdf".
             language: Language of the survey to use (default from Survey).
                 Defaults to None.
             graph: Export graphs. Defaults to False.
@@ -797,14 +831,16 @@
         survey_id: int,
         period: Literal["day", "hour"] | enums.TimelineAggregationPeriod,
         start: datetime.datetime,
         end: datetime.datetime | None = None,
     ) -> dict[str, int]:
         """Export survey submission timeline.
 
+        Calls :rpc_method:`export_timeline`.
+
         Args:
             survey_id: ID of the Survey.
             period: Granularity level for aggregation submission counts.
             start: Start datetime.
             end: End datetime.
 
         Returns:
@@ -826,14 +862,16 @@
         group_id: int,
         *,
         settings: list[str] | None = None,
         language: str | None = None,
     ) -> types.GroupProperties:
         """Get the properties of a group of a survey.
 
+        Calls :rpc_method:`get_group_properties`.
+
         Args:
             group_id: ID of the group to get properties of.
             settings: Properties to get, default to all.
             language: Parameter language for multilingual groups.
 
         Returns:
             Dictionary of group properties.
@@ -867,14 +905,16 @@
         self,
         survey_id: int,
         query: dict[str, t.Any] | int,
         properties: t.Sequence[str] | None = None,
     ) -> dict[str, t.Any]:
         """Get properties a single survey participant.
 
+        Calls :rpc_method:`get_participant_properties`.
+
         Args:
             survey_id: Survey to get participants properties.
             query: Mapping of properties to query participants, or the token id
                 as an integer.
             properties: Which participant properties to retrieve.
 
         Returns:
@@ -889,14 +929,16 @@
         question_id: int,
         *,
         settings: list[str] | None = None,
         language: str | None = None,
     ) -> types.QuestionProperties:
         """Get properties of a question in a survey.
 
+        Calls :rpc_method:`get_question_properties`.
+
         Args:
             question_id: ID of the question to get properties.
             settings: Properties to get, default to all.
             language: Parameter language for multilingual questions.
 
         Returns:
             Dictionary of question properties.
@@ -909,14 +951,16 @@
         self,
         quota_id: int,
         settings: list[str] | None = None,
         language: str | None = None,
     ) -> types.QuotaProperties:
         """Get properties of a LimeSurvey quota.
 
+        Calls :rpc_method:`get_quota_properties`.
+
         Args:
             quota_id: ID of the quota to get properties for.
             settings: Properties to get, default to all.
             language: Parameter language for multilingual quotas.
 
         Returns:
             Quota properties.
@@ -929,28 +973,32 @@
     def get_response_ids(
         self,
         survey_id: int,
         token: str,
     ) -> list[int]:
         """Find response IDs given a survey ID and a token.
 
+        Calls :rpc_method:`get_response_ids`.
+
         Args:
             survey_id: Survey to get responses from.
             token: Participant for which to get response IDs.
 
         Returns:
             A list of response IDs.
 
         .. versionadded:: 0.0.1
         """
         return self.__session.get_response_ids(survey_id, token)
 
     def get_available_site_settings(self) -> list[str]:
         """Get all available site settings.
 
+        Calls :rpc_method:`get_available_site_settings`.
+
         Returns:
             A list of all the available site settings.
 
         .. versionadded:: 0.6.0
         .. minlimesurvey:: 6.0.0
         """
         return self.session.get_available_site_settings()
@@ -1021,14 +1069,16 @@
         langs: str = self._get_site_setting("restrictToLanguages")
 
         return langs.split(" ") if langs else None
 
     def get_summary(self, survey_id: int) -> dict[str, int]:
         """Get survey summary.
 
+        Calls :rpc_method:`get_summary`.
+
         Args:
             survey_id: ID of the survey to get summary of.
 
         Returns:
             Mapping of survey statistics.
 
         .. versionadded:: 0.0.10
@@ -1038,14 +1088,16 @@
     def get_survey_properties(
         self,
         survey_id: int,
         properties: t.Sequence[str] | None = None,
     ) -> types.SurveyProperties:
         """Get properties of a survey.
 
+        Calls :rpc_method:`get_survey_properties`.
+
         Args:
             survey_id: Survey to get properties.
             properties: Which survey properties to retrieve. If none, gets all fields.
 
         Returns:
             Dictionary of survey properties.
 
@@ -1056,14 +1108,16 @@
     def get_uploaded_files(
         self,
         survey_id: int,
         token: str | None = None,
     ) -> dict[str, dict[str, t.Any]]:
         """Get a dictionary of files uploaded in a survey response.
 
+        Calls :rpc_method:`get_uploaded_files`.
+
         Args:
             survey_id: Survey for which to download files.
             token: Optional participant token to filter uploaded files.
 
         Returns:
             Dictionary with uploaded files metadata.
 
@@ -1140,14 +1194,16 @@
     ) -> int:
         """Import group from a file.
 
         Create a new group from an exported LSG file.
 
         TODO: Check support for custom name and description.
 
+        Calls :rpc_method:`import_group`.
+
         Args:
             file: File object.
             survey_id: The ID of the Survey that the question will belong to.
             file_type: Type of file. One of LSS, CSV, TXT and LSA.
 
         Returns:
             The ID of the new group.
@@ -1169,14 +1225,16 @@
     ) -> int:
         """Import question from a file.
 
         Create a new question from an exported LSQ file.
 
         TODO: Check support for additional fields like custom title, text, etc.
 
+        Calls :rpc_method:`import_question`.
+
         Args:
             file: File object.
             survey_id: The ID of the Survey that the question will belong to.
             group_id: The ID of the Group that the question will belong to.
 
         Returns:
             The ID of the new question.
@@ -1198,14 +1256,16 @@
         survey_name: str | None = None,
         survey_id: int | None = None,
     ) -> int:
         """Import survey from a file.
 
         Create a new survey from an exported LSS, CSV, TXT or LSA file.
 
+        Calls :rpc_method:`import_survey`.
+
         Args:
             file: File object.
             file_type: Type of file. One of LSS, CSV, TXT and LSA.
             survey_name: Override the new survey name.
             survey_id: Desired ID of the new survey. A different ID will be used if
                 there is already a survey with this ID.
 
@@ -1232,19 +1292,21 @@
         limit: int = 10,
         unused: bool = False,
         attributes: t.Sequence[str] | bool = False,
         conditions: t.Mapping[str, t.Any] | None = None,
     ) -> list[dict[str, t.Any]]:
         """Get participants in a survey.
 
+        Calls :rpc_method:`list_participants`.
+
         Args:
             survey_id: Survey to get participants from.
             start: Retrieve participants starting from this index (zero-indexed).
             limit: Maximum number of participants to retrieve.
-            unused: Retrieve partipants with unused tokens.
+            unused: Retrieve participants with unused tokens.
             attributes: Extra participant attributes to include in the result.
             conditions: Dictionary of conditions to limit the list.
 
         Returns:
             List of participants with basic information.
 
         .. versionadded:: 0.0.1
@@ -1259,28 +1321,32 @@
             attributes,
             conditions or {},
         )
 
     def list_users(self) -> list[dict[str, t.Any]]:
         """Get LimeSurvey users.
 
+        Calls :rpc_method:`list_users`.
+
         Returns:
             List of users.
 
         .. versionadded:: 0.0.3
         """
         return self.__session.list_users()
 
     def list_groups(
         self,
         survey_id: int,
         language: str | None = None,
     ) -> list[dict[str, t.Any]]:
         """Get the IDs and all attributes of all question groups in a Survey.
 
+        Calls :rpc_method:`list_groups`.
+
         Args:
             survey_id: ID of the Survey containing the groups.
             language: Optional parameter language for multilingual groups.
 
         Returns:
             List of question groups.
 
@@ -1292,14 +1358,16 @@
         self,
         survey_id: int,
         group_id: int | None = None,
         language: str | None = None,
     ) -> list[types.QuestionsListElement]:
         """Get questions in a survey, in a specific group or all.
 
+        Calls :rpc_method:`list_questions`.
+
         Args:
             survey_id: Survey.
             group_id: Question group.
             language: Retrieve question text, description, etc. in this language.
 
         Returns:
             List of questions with basic information.
@@ -1307,28 +1375,32 @@
         .. versionadded:: 0.0.1
         """
         return self.__session.list_questions(survey_id, group_id, language)
 
     def list_quotas(self, survey_id: int) -> list[types.QuotaListElement]:
         """Get all quotas for a LimeSurvey survey.
 
+        Calls :rpc_method:`list_quotas`.
+
         Args:
             survey_id: ID of the survey to get quotas for.
 
         Returns:
             List of quotas.
 
         .. versionadded:: 0.6.0
         .. minlimesurvey:: 6.0.0
         """
         return self.session.list_quotas(survey_id)
 
     def list_surveys(self, username: str | None = None) -> list[dict[str, t.Any]]:
         """Get all surveys or only those owned by a user.
 
+        Calls :rpc_method:`list_surveys`.
+
         Args:
             username: Owner of the surveys to retrieve.
 
         Returns:
             List of surveys with basic information.
 
         .. versionadded:: 0.0.1
@@ -1337,14 +1409,16 @@
 
     def list_survey_groups(
         self,
         username: str | None = None,
     ) -> list[dict[str, t.Any]]:
         """Get all survey groups or only those owned by a user.
 
+        Calls :rpc_method:`list_survey_groups`.
+
         Args:
             username: Owner of the survey groups to retrieve.
 
         Returns:
             List of survey groups with basic information.
 
         .. versionadded:: 0.0.2
@@ -1354,14 +1428,16 @@
     def set_group_properties(
         self,
         group_id: int,
         **properties: Unpack[types.GroupProperties],
     ) -> dict[str, bool]:
         """Set properties of a group.
 
+        Calls :rpc_method:`set_group_properties`.
+
         Args:
             group_id: ID of the group.
             properties: Properties to set.
 
         Returns:
             Mapping of property names to whether they were set successfully.
 
@@ -1373,14 +1449,16 @@
         self,
         survey_id: int,
         language: str | None = None,
         **properties: Unpack[types.LanguageProperties],
     ) -> dict[str, t.Any]:
         """Set properties of a survey language.
 
+        Calls :rpc_method:`set_language_properties`.
+
         Args:
             survey_id: ID of the survey for which to set the language properties.
             language: Language code.
             properties: Properties to set.
 
         Returns:
             Mapping with status and updated properties.
@@ -1391,15 +1469,17 @@
 
     def set_participant_properties(
         self,
         survey_id: int,
         token_query_properties: t.Mapping[str, t.Any] | int,
         **token_data: t.Any,
     ) -> dict[str, t.Any]:
-        """Set properties of a participant. Only one particpant can be updated.
+        """Set properties of a participant. Only one participant can be updated.
+
+        Calls :rpc_method:`set_participant_properties`.
 
         Args:
             survey_id: ID of the survey to which the participant belongs.
             token_query_properties: Dictionary of properties to match the participant
                 or token ID.
             token_data: Properties to set.
 
@@ -1457,14 +1537,16 @@
     def set_survey_properties(
         self,
         survey_id: int,
         **properties: Unpack[types.SurveyProperties],
     ) -> dict[str, bool]:
         """Set properties of a survey.
 
+        Calls :rpc_method:`set_survey_properties`.
+
         Args:
             survey_id: ID of the survey to set the properties of.
             properties: Properties to set.
 
         Returns:
             Mapping of property names to whether they were set successfully.
 
@@ -1477,14 +1559,16 @@
         survey_id: int,
         field: str,
         filename: str,
         file: t.BinaryIO,
     ) -> types.FileUploadResult:
         """Upload a file to a LimeSurvey survey.
 
+        Calls :rpc_method:`upload_file`.
+
         Args:
             survey_id: ID of the survey to upload the file to.
             field: Field name to upload the file to.
             filename: Name of the file to upload.
             file: File-like object to upload.
 
         Returns:
```

### Comparing `citric-0.7.1b2/src/citric/enums.py` & `citric-0.7.1b3/src/citric/enums.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b2/src/citric/exceptions.py` & `citric-0.7.1b3/src/citric/exceptions.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b2/src/citric/method.py` & `citric-0.7.1b3/src/citric/method.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b2/src/citric/objects.py` & `citric-0.7.1b3/src/citric/objects.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b2/src/citric/session.py` & `citric-0.7.1b3/src/citric/session.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b2/src/citric/types.py` & `citric-0.7.1b3/src/citric/types.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b2/PKG-INFO` & `citric-0.7.1b3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citric
-Version: 0.7.1b2
+Version: 0.7.1b3
 Summary: A client to the LimeSurvey Remote Control API 2, written in modern Python.
 Home-page: https://github.com/edgarrmondragon/citric
 License: MIT
 Keywords: limesurvey,json-rpc
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
@@ -17,20 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: docs
 Requires-Dist: furo (>=2023.3.27) ; extra == "docs"
 Requires-Dist: importlib_metadata (>=1.6) ; python_version < "3.8"
@@ -59,14 +54,17 @@
   </a>
   <a href="https://github.com/edgarrmondragon/citric/blob/main/LICENSE">
     <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/citric"/>
   </a>
   <a href="https://citric.readthedocs.io/en/latest/?badge=latest">
     <img alt="Documentation Status" src="https://readthedocs.org/projects/citric/badge/?version=latest"/>
   </a>
+  <a href="https://github.com/charliermarsh/ruff">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
+  </a>
   <a href="https://codecov.io/gh/edgarrmondragon/citric">
     <img alt="codecov" src="https://codecov.io/gh/edgarrmondragon/citric/branch/main/graph/badge.svg"/>
   </a>
   <a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fedgarrmondragon%2Fcitric?ref=badge_shield">
     <img alt="FOSSA Status" src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fedgarrmondragon%2Fcitric.svg?type=shield"/>
   </a>
 </div>
```

#### html2text {}

```diff
@@ -1,40 +1,37 @@
-Metadata-Version: 2.1 Name: citric Version: 0.7.1b2 Summary: A client to the
+Metadata-Version: 2.1 Name: citric Version: 0.7.1b3 Summary: A client to the
 LimeSurvey Remote Control API 2, written in modern Python. Home-page: https://
 github.com/edgarrmondragon/citric License: MIT Keywords: limesurvey,json-rpc
 Author: Edgar RamÃ­rez-MondragÃ³n Author-email: edgarrm358@gmail.com
 Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python ::
-Implementation :: CPython Classifier: Programming Language :: Python ::
-Implementation :: PyPy Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Classifier: Typing :: Typed Provides-Extra: docs Requires-
-Dist: furo (>=2023.3.27) ; extra == "docs" Requires-Dist: importlib_metadata
-(>=1.6) ; python_version < "3.8" Requires-Dist: myst-parser (>=1.0.0,<2) ;
-extra == "docs" Requires-Dist: requests (>=2.23.0) Requires-Dist: sphinx (<7) ;
-extra == "docs" Requires-Dist: sphinx-autoapi (>=2.1.0,<3) ; extra == "docs"
-Requires-Dist: sphinx-autobuild (>=2021.3.14) ; extra == "docs" Requires-Dist:
-sphinx-autodoc-typehints (>=1.22,<2) ; extra == "docs" Requires-Dist: sphinx-
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed Provides-Extra: docs Requires-Dist: furo
+(>=2023.3.27) ; extra == "docs" Requires-Dist: importlib_metadata (>=1.6) ;
+python_version < "3.8" Requires-Dist: myst-parser (>=1.0.0,<2) ; extra ==
+"docs" Requires-Dist: requests (>=2.23.0) Requires-Dist: sphinx (<7) ; extra ==
+"docs" Requires-Dist: sphinx-autoapi (>=2.1.0,<3) ; extra == "docs" Requires-
+Dist: sphinx-autobuild (>=2021.3.14) ; extra == "docs" Requires-Dist: sphinx-
+autodoc-typehints (>=1.22,<2) ; extra == "docs" Requires-Dist: sphinx-
 copybutton (>=0.5.1,<1) ; extra == "docs" Project-URL: Documentation, https://
 citric.readthedocs.io Project-URL: Issue Tracker, https://github.com/
 edgarrmondragon/citric/issues Project-URL: Repository, https://github.com/
 edgarrmondragon/citric Description-Content-Type: text/markdown
                                    # Citric
-  [Tests] [pre-commit.ci_status] [License] [Documentation_Status] [codecov]
-                                [FOSSA_Status]
+    [Tests] [pre-commit.ci_status] [License] [Documentation_Status] [Ruff]
+                           [codecov] [FOSSA_Status]
       [PyPI_version] [Python_versions] [PyPI_-_Downloads] [PyPI_-_Format]
    [GitHub_languages] [GitHub repo size] [GitHub_stars] [Github_last-commit]
           A client to the [LimeSurvey Remote Control API 2](https://
      manual.limesurvey.org/RemoteControl_2_API), written in modern Python.
 ## Features - Supports the full RPC API via the [`Session` class](https://
 citric.readthedocs.io/en/latest/_api/citric/session/
 index.html#citric.session.Session). - Best effort to implement all the RPC
```

