# Comparing `tmp/hatch_build_scripts-0.0.3.tar.gz` & `tmp/hatch_build_scripts-0.0.4.tar.gz`

## Comparing `hatch_build_scripts-0.0.3.tar` & `hatch_build_scripts-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/pull_request_template.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/ISSUE_TEMPLATE/issue-form.yml
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/workflows/.hatch-run.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/workflows/check.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/hatch_build_scripts/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/hatch_build_scripts/hooks.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/hatch_build_scripts/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/tests/test_plugin.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/tests/utils.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/LICENSE
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/README.md
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/.github/pull_request_template.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/.github/ISSUE_TEMPLATE/issue-form.yml
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/.github/workflows/.hatch-run.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/.github/workflows/check.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/hatch_build_scripts/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/hatch_build_scripts/hooks.py
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/hatch_build_scripts/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/tests/test_plugin.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/tests/utils.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/README.md
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.4/PKG-INFO
```

### Comparing `hatch_build_scripts-0.0.3/.github/FUNDING.yml` & `hatch_build_scripts-0.0.4/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.3/.github/ISSUE_TEMPLATE/issue-form.yml` & `hatch_build_scripts-0.0.4/.github/ISSUE_TEMPLATE/issue-form.yml`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.3/.github/workflows/.hatch-run.yml` & `hatch_build_scripts-0.0.4/.github/workflows/.hatch-run.yml`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.3/.github/workflows/check.yml` & `hatch_build_scripts-0.0.4/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.3/.github/workflows/publish.yml` & `hatch_build_scripts-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.3/hatch_build_scripts/plugin.py` & `hatch_build_scripts-0.0.4/hatch_build_scripts/plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 import logging
 import os
 import shutil
-from dataclasses import MISSING, dataclass, fields
+from collections.abc import Sequence
+from dataclasses import MISSING, asdict, dataclass, fields
 from functools import cached_property
 from pathlib import Path
 from subprocess import run
-from typing import Any, Sequence
+from typing import Any
 
 import pathspec
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
-logger = logging.getLogger(__name__)
+log = logging.getLogger(__name__)
+log_level = logging.getLevelName(os.getenv("HATCH_BUILD_SCRIPTS_LOG_LEVEL", "INFO"))
+log.setLevel(log_level)
 
 
 class BuildScriptsHook(BuildHookInterface):
     PLUGIN_NAME = "build-scripts"
 
     def initialize(
         self,
@@ -26,36 +29,42 @@
         created: set[Path] = set()
 
         all_scripts = load_scripts(self.config)
 
         for script in all_scripts:
             if script.clean_out_dir:
                 out_dir = Path(self.root, script.out_dir)
-                logger.info(f"Cleaning {out_dir}")
+                log.debug(f"Cleaning {out_dir}")
                 shutil.rmtree(out_dir, ignore_errors=True)
             elif script.clean_artifacts:
                 for out_file in script.out_files(self.root):
+                    log.debug(f"Cleaning {out_file}")
                     out_file.unlink(missing_ok=True)
 
         for script in all_scripts:
+            log.debug(f"Script config: {asdict(script)}")
             work_dir = Path(self.root, script.work_dir)
             out_dir = Path(self.root, script.out_dir)
             out_dir.mkdir(parents=True, exist_ok=True)
 
             for cmd in script.commands:
+                log.info(f"Running command: {cmd}")
                 run(cmd, cwd=str(work_dir), check=True, shell=True)  # noqa: S602
 
-            logger.info(f"Copying artifacts to {out_dir}")
-            for artifact_file in script.artifact_files():
-                src_file = work_dir / artifact_file
-                out_file = out_dir / artifact_file
+            log.info(f"Copying artifacts to {out_dir}")
+            for work_file in script.work_files(self.root, relative=True):
+                src_file = work_dir / work_file
+                out_file = out_dir / work_file
+                log.debug(f"Copying {src_file} to {out_file}")
                 if src_file not in created:
                     out_file.parent.mkdir(parents=True, exist_ok=True)
                     shutil.copyfile(src_file, out_file)
                     created.add(out_file)
+                else:
+                    log.debug(f"Skipping {src_file} - already exists")
 
             build_data["artifacts"].append(str(out_dir.relative_to(self.root)))
 
 
 def load_scripts(config: dict[str, Any]) -> Sequence[OneScriptConfig]:
     script_defaults = dataclass_defaults(OneScriptConfig)
     script_defaults.update({k: config[k] for k in script_defaults if k in config})
@@ -87,35 +96,40 @@
     clean_out_dir: bool = False
     """Whether to clean the output directory before running the scripts"""
 
     def __post_init__(self) -> None:
         self.out_dir = conv_path(self.out_dir)
         self.work_dir = conv_path(self.work_dir)
 
-    def work_files(self, root: str | Path) -> Sequence[Path]:
-        """Get the files that will be used by the script."""
-        work_dir = Path(root, self.work_dir)
-        if not work_dir.exists():
+    def work_files(self, root: str | Path, *, relative: bool = False) -> Sequence[Path]:
+        """Get files in the work directory that match the artifacts spec."""
+        abs_dir = Path(root, self.work_dir)
+        if not abs_dir.exists():
             return []
-        return [Path(root, self.work_dir, f) for f in self.artifacts_spec.match_tree(work_dir)]
-
-    def out_files(self, root: str | Path) -> Sequence[Path]:
-        """Get the files that will be created by the script."""
-        out_dir = Path(root, self.out_dir)
-        if not out_dir.exists():
+        return [
+            Path(f) if relative else abs_dir / f
+            for f in self.artifacts_spec.match_tree(abs_dir)
+        ]
+
+    def out_files(self, root: str | Path, *, relative: bool = False) -> Sequence[Path]:
+        """Get files in the output directory that match the artifacts spec."""
+        abs_dir = Path(root, self.out_dir)
+        if not abs_dir.exists():
             return []
-        return [Path(root, self.out_dir, f) for f in self.artifacts_spec.match_tree(out_dir)]
-
-    def artifact_files(self) -> Sequence[Path]:
-        return [Path(conv_path(p)) for p in self.artifacts_spec.match_tree(self.work_dir)]
+        return [
+            Path(f) if relative else abs_dir / f
+            for f in self.artifacts_spec.match_tree(abs_dir)
+        ]
 
     @cached_property
     def artifacts_spec(self) -> pathspec.PathSpec:
         """A pathspec for the artifacts."""
-        return pathspec.PathSpec.from_lines(pathspec.patterns.GitWildMatchPattern, self.artifacts)
+        return pathspec.PathSpec.from_lines(
+            pathspec.patterns.GitWildMatchPattern, self.artifacts
+        )
 
 
 def dataclass_defaults(obj: Any) -> dict[str, Any]:
     defaults: dict[str, Any] = {}
     for f in fields(obj):
         if f.default is not MISSING:
             defaults[f.name] = f.default
```

### Comparing `hatch_build_scripts-0.0.3/tests/test_plugin.py` & `hatch_build_scripts-0.0.4/tests/test_plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from hatch_build_scripts.plugin import OneScriptConfig
 
 from .utils import create_project
 
 
 def test_plugin(tmpdir):
-    (tmpdir / "some-dir").mkdir()
-    (tmpdir / "another-dir").mkdir()
+    tmp_lib_dir = tmpdir / "lib"
+    tmp_lib_dir.mkdir()
 
-    some_dir_out = tmpdir / "some-dir-out"
+    (tmp_lib_dir / "some-dir").mkdir()
+    (tmp_lib_dir / "another-dir").mkdir()
+
+    some_dir_out = tmp_lib_dir / "some-dir-out"
     some_dir_out.mkdir()
     # we expect that this file will not be cleaned
     (some_dir_out / "module.py").write_text('print("hello")', "utf-8")
     # we expect that this file will be cleaned
     (some_dir_out / "f3.txt").write_text("this should be cleaned", "utf-8")
 
-    another_dir_out = tmpdir / "another-dir-out"
+    another_dir_out = tmp_lib_dir / "another-dir-out"
     another_dir_out.mkdir()
     # we expect that this file will be cleaned
     (another_dir_out / "module.py").write_text('print("hello")', "utf-8")
 
     proj = create_project(
-        tmpdir,
+        tmp_lib_dir,
         [
             OneScriptConfig(
                 out_dir="fake",
                 commands=["echo 'hello world' > fake.txt"],
                 artifacts=["fake.txt"],
             ),
             OneScriptConfig(
@@ -48,14 +51,18 @@
                 clean_out_dir=True,
             ),
         ],
     )
 
     proj.build()
 
+    extract_dir = tmpdir / "extract"
+    extract_dir.mkdir()
+
     with proj.dist() as dist:
-        files = {file.filename for file in dist.filelist}
+        dist.extractall(extract_dir)
+
+        assert (extract_dir / "fake" / "fake.txt").exists()
+        assert (extract_dir / "some-dir-out" / "module.py").exists()
 
-        assert "fake/fake.txt" in files
-        assert "some-dir-out/module.py" in files
-        assert "another-dir-out/module.py" not in files
-        assert "some-dir-out/f3.txt" not in files
+        assert not (extract_dir / "some-dir-out" / "f3.txt").exists()
+        assert not (extract_dir / "another-dir-out" / "module.py").exists()
```

### Comparing `hatch_build_scripts-0.0.3/tests/utils.py` & `hatch_build_scripts-0.0.4/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import subprocess
 import sys
 import zipfile
+from collections.abc import Iterator, Sequence
 from contextlib import contextmanager
 from dataclasses import asdict
 from pathlib import Path
-from typing import Iterator, Sequence
 
 import toml
 
 import hatch_build_scripts
 from hatch_build_scripts.plugin import OneScriptConfig
 
 ROOT_DIR = Path(__file__).parent.parent
@@ -49,27 +49,29 @@
 
 class FakeProject:
     def __init__(self, path: Path) -> None:
         self.path = path
 
     def build(self) -> None:
         subprocess.run(
-            [  # noqa: S603
+            [
                 sys.executable,
                 "-m",
                 "pip",
                 "cache",
                 "remove",
                 hatch_build_scripts.__name__,
             ],
             cwd=self.path,
             check=True,
         )
         subprocess.run(
-            [sys.executable, "-m", "hatch", "build"], cwd=self.path, check=True  # noqa: S603
+            [sys.executable, "-m", "hatch", "build"],
+            cwd=self.path,
+            check=True,
         )
 
     @contextmanager
     def dist(self) -> Iterator[zipfile.ZipFile]:
         files = list((self.path / "dist").glob("*.whl"))
         assert len(files) == 1
         with zipfile.ZipFile(str(files[0])) as whl:
```

### Comparing `hatch_build_scripts-0.0.3/.gitignore` & `hatch_build_scripts-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.3/LICENSE` & `hatch_build_scripts-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.3/README.md` & `hatch_build_scripts-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.3/pyproject.toml` & `hatch_build_scripts-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -56,32 +56,30 @@
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:hatch_build_scripts tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
-fmt = [
+fix = [
   "black {args:.}",
   "ruff --fix {args:.}",
   "style",
 ]
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
-target-version = ["py37"]
-line-length = 100
+target-version = ["py39"]
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
-line-length = 100
+target-version = "py39"
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
@@ -124,8 +122,8 @@
 known-first-party = ["hatch_build_scripts"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
-"tests/**/*" = ["PLR2004", "S101", "TID252"]
+"tests/**/*" = ["PLR2004", "S101", "TID252", "S603"]
```

### Comparing `hatch_build_scripts-0.0.3/PKG-INFO` & `hatch_build_scripts-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-build-scripts
-Version: 0.0.3
+Version: 0.0.4
 Summary: A plugin for Hatch for writing build scripts
 Project-URL: Documentation, https://github.com/rmorshea/hatch-build-scripts#readme
 Project-URL: Issues, https://github.com/rmorshea/hatch-build-scripts/issues
 Project-URL: Source, https://github.com/rmorshea/hatch-build-scripts
 Author-email: rmorshea <ryan.morshead@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

