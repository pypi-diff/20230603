# Comparing `tmp/fgo_api_types-2023.5.31.14.20.7.tar.gz` & `tmp/fgo_api_types-2023.6.3.17.24.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.5.31.14.20.7.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.6.3.17.24.33.tar", max compression
```

## Comparing `fgo_api_types-2023.5.31.14.20.7.tar` & `fgo_api_types-2023.6.3.17.24.33.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-05-31 14:19:45.134564 fgo_api_types-2023.5.31.14.20.7/LICENSE
--rw-r--r--   0        0        0      449 2023-05-31 14:19:45.134564 fgo_api_types-2023.5.31.14.20.7/README.md
--rw-r--r--   0        0        0        0 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/common.py
--rw-r--r--   0        0        0    38038 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/enums.py
--rw-r--r--   0        0        0   157892 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    75688 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50619 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-05-31 14:20:07.279860 fgo_api_types-2023.5.31.14.20.7/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-05-31 14:20:07.631875 fgo_api_types-2023.5.31.14.20.7/pyproject.toml
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.5.31.14.20.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-03 17:24:12.099063 fgo_api_types-2023.6.3.17.24.33/LICENSE
+-rw-r--r--   0        0        0      449 2023-06-03 17:24:12.099063 fgo_api_types-2023.6.3.17.24.33/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38038 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   157892 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    76303 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50619 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-06-03 17:24:34.019460 fgo_api_types-2023.6.3.17.24.33/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.6.3.17.24.33/PKG-INFO
```

### Comparing `fgo_api_types-2023.5.31.14.20.7/LICENSE` & `fgo_api_types-2023.6.3.17.24.33/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/basic.py` & `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/common.py` & `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/enums.py` & `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/gameenums.py` & `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/nice.py` & `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,14 +619,29 @@
     idx: int
     condType: NiceCondType
     condTargetId: int
     condNum: int
     condGroup: int
 
 
+class NiceSkillSvt(BaseModelORJson):
+    svtId: int  # 9400920,
+    num: int  # 1,
+    priority: int  # 1,
+    script: Optional[dict[str, Any]] = None
+    strengthStatus: int  # 1,
+    condQuestId: int  # 0,
+    condQuestPhase: int  # 0,
+    condLv: int = 0  # 0,
+    condLimitCount: int  # 0,
+    eventId: int  # 0,
+    flag: int  # 0
+    releaseConditions: list[NiceSvtSkillRelease]
+
+
 class NiceSkill(BaseModelORJson):
     id: int
     num: int = -1
     name: str
     originalName: str
     ruby: str
     detail: Optional[str] = None
@@ -640,15 +655,15 @@
     condLimitCount: int = -1
     icon: Optional[HttpUrl] = None
     coolDown: list[int]
     actIndividuality: list[NiceTrait]
     script: NiceSkillScript
     extraPassive: list[ExtraPassive]
     skillAdd: list[NiceSkillAdd]
-    releaseConditions: list[NiceSvtSkillRelease] = []
+    skillSvts: list[NiceSkillSvt] = []
     aiIds: Optional[dict[AiType, list[int]]] = None
     groupOverwrites: list[NiceSkillGroupOverwrite] | None = None
     functions: list[NiceFunction]
 
 
 class NpGain(BaseModel):
     buster: list[int]
@@ -2311,22 +2326,32 @@
 
 class NiceQuestPhaseAiNpc(BaseModelORJson):
     npc: NpcServant
     detail: QuestEnemy | None = None
     aiIds: list[int]
 
 
+class NiceQuestPhaseOverwriteEquipSkill(BaseModelORJson):
+    lv: int
+    id: int
+
+
+class NiceQuestPhaseOverwriteEquipSkills(BaseModelORJson):
+    iconId: int
+    skills: list[NiceQuestPhaseOverwriteEquipSkill]
+
+
 class NiceQuestPhaseExtraDetail(BaseModelORJson):
     questSelect: list[int] | None = None
     singleForceSvtId: int | None = None
     hintTitle: str | None = None
     hintMessage: str | None = None
     aiNpc: NiceQuestPhaseAiNpc | None = None
     aiMultiNpc: list[NiceQuestPhaseAiNpc] | None = None
-    overwriteEquipSkills: dict | None = None
+    overwriteEquipSkills: NiceQuestPhaseOverwriteEquipSkills | None = None
 
 
 class NiceRestriction(BaseModelORJson):
     id: int
     name: str
     type: NiceRestrictionType
     rangeType: NiceRestrictionRangeType
```

### Comparing `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/raw.py` & `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/rayshift.py` & `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.20.7/fgo_api_types/search.py` & `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.31.14.20.7/pyproject.toml` & `fgo_api_types-2023.6.3.17.24.33/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.05.31.14.20.07"
+version = "2023.06.03.17.24.33"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.5.31.14.20.7/PKG-INFO` & `fgo_api_types-2023.6.3.17.24.33/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.5.31.14.20.7
+Version: 2023.6.3.17.24.33
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

