# Comparing `tmp/easymms-0.1.5.tar.gz` & `tmp/easymms-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymms-0.1.5.tar", last modified: Fri Jun  2 00:34:21 2023, max compression
+gzip compressed data, was "easymms-0.1.6.tar", last modified: Fri Jun  2 22:23:55 2023, max compression
```

## Comparing `easymms-0.1.5.tar` & `easymms-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.154697 easymms-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-06-02 00:34:12.000000 easymms-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-02 00:34:21.150696 easymms-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-02 00:34:12.000000 easymms-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.150696 easymms-0.1.5/easymms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.150696 easymms-0.1.5/easymms/models/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/models/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/models/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/models/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.150696 easymms-0.1.5/easymms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:34:20.000000 easymms-0.1.5/easymms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 00:34:21.154697 easymms-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-02 00:34:12.000000 easymms-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.150696 easymms-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:12.000000 easymms-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-02 00:34:12.000000 easymms-0.1.5/tests/test_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 00:34:12.000000 easymms-0.1.5/tests/test_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:23:55.969623 easymms-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-06-02 22:23:47.000000 easymms-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-02 22:23:55.969623 easymms-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-02 22:23:47.000000 easymms-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:23:55.969623 easymms-0.1.6/easymms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 22:23:47.000000 easymms-0.1.6/easymms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-02 22:23:47.000000 easymms-0.1.6/easymms/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-02 22:23:47.000000 easymms-0.1.6/easymms/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:23:55.969623 easymms-0.1.6/easymms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:23:47.000000 easymms-0.1.6/easymms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-06-02 22:23:47.000000 easymms-0.1.6/easymms/models/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-02 22:23:47.000000 easymms-0.1.6/easymms/models/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-02 22:23:47.000000 easymms-0.1.6/easymms/models/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-02 22:23:47.000000 easymms-0.1.6/easymms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:23:55.969623 easymms-0.1.6/easymms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-02 22:23:55.000000 easymms-0.1.6/easymms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-02 22:23:55.000000 easymms-0.1.6/easymms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:23:55.000000 easymms-0.1.6/easymms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:23:55.000000 easymms-0.1.6/easymms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 22:23:55.000000 easymms-0.1.6/easymms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 22:23:55.000000 easymms-0.1.6/easymms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 22:23:55.969623 easymms-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-02 22:23:47.000000 easymms-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:23:55.969623 easymms-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 22:23:47.000000 easymms-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-02 22:23:47.000000 easymms-0.1.6/tests/test_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 22:23:47.000000 easymms-0.1.6/tests/test_tts.py
```

### Comparing `easymms-0.1.5/LICENSE` & `easymms-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easymms-0.1.5/PKG-INFO` & `easymms-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymms
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
 Project-URL: Source, https://abdeladim-s.github.io/easymms/
 Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
 Requires-Python: >=3.8
```

### Comparing `easymms-0.1.5/README.md` & `easymms-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `easymms-0.1.5/easymms/_logger.py` & `easymms-0.1.6/easymms/_logger.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.5/easymms/constants.py` & `easymms-0.1.6/easymms/constants.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.5/easymms/models/alignment.py` & `easymms-0.1.6/easymms/models/alignment.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 import logging
 import shutil
 import sys
 from pathlib import Path
 from typing import List
 import torch
 # fix importing from fairseq.examples
-import site
-sys.path.append(str(Path(site.getsitepackages()[0]) / 'fairseq'))
-try:
-    from fairseq.examples.mms.data_prep.align_and_segment import get_alignments
-    from fairseq.examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
-    from fairseq.examples.mms.data_prep.text_normalization import text_normalize
-except ImportError:
-    from examples.mms.data_prep.align_and_segment import get_alignments
-    from examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
-    from examples.mms.data_prep.text_normalization import text_normalize
+# import site
+# sys.path.append(str(Path(site.getsitepackages()[0]) / 'fairseq'))
+# try:
+#     from fairseq.examples.mms.data_prep.align_and_segment import get_alignments
+#     from fairseq.examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
+#     from fairseq.examples.mms.data_prep.text_normalization import text_normalize
+# except ImportError:
+#     from examples.mms.data_prep.align_and_segment import get_alignments
+#     from examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
+#     from examples.mms.data_prep.text_normalization import text_normalize
 
 from easymms import utils
 from easymms._logger import set_log_level
 from easymms.constants import PACKAGE_DATA_DIR, ALIGNMENT_MODEL_URL, ALIGNMENT_DICTIONARY_URL, UROMAN_URL, \
     UROMAN_DIR
 
 
@@ -75,14 +75,18 @@
         if dictionary is not None:
             self.dictionary_path = Path(dictionary)
         else:
             self.dictionary_path = Path(PACKAGE_DATA_DIR) / "ctc_alignment_mling_uroman_model.dict"
 
         self.model, self.dictionary = self._load_model_dict()
 
+        # clone Fairseq
+        easymms_utils.clone(constants.FAIRSEQ_URL, constants.FAIRSEQ_DIR)
+        sys.path.append(str(constants.FAIRSEQ_DIR.resolve()))
+
     def _load_model_dict(self):
         """
         Modified from <https://github.com/facebookresearch/fairseq/blob/main/examples/mms/data_prep/align_utils.py>
         to store the models in a consistent directory
 
         :return: None
         """
@@ -157,14 +161,22 @@
 
         :param media_file: the path of the media file, should be wav
         :param transcript: list of segments
         :param lang: language ISO code
         :param device: 'cuda' or 'cpu'
         :return: list of transcription timestamps
         """
+        # import
+        cwd = os.getcwd()
+        os.chdir(constants.FAIRSEQ_DIR)
+        from examples.mms.data_prep.align_and_segment import get_alignments
+        from examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
+        from examples.mms.data_prep.text_normalization import text_normalize
+        os.chdir(cwd)
+
         if device is None:
             device = 'cuda' if torch.cuda.is_available() else 'cpu'
         model = self.model.to(device)
         res = []
         logger.info(f"Aligning file {media_file} ...")
         norm_transcripts = [text_normalize(line.strip(), lang) for line in transcript]
         tokens = get_uroman_tokens(norm_transcripts, str(self.uroman_dir_path.resolve()), lang)
```

### Comparing `easymms-0.1.5/easymms/models/asr.py` & `easymms-0.1.6/easymms/models/asr.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,40 +5,41 @@
 This file contains a class definition to use the ASR models from [Meta's Massively Multilingual Speech (MMS) project](https://github.com/facebookresearch/fairseq/tree/main/examples/mms)
 """
 
 __author__ = "Abdeladim S."
 __copyright__ = "Copyright 2023,"
 
 
+import os
 import atexit
 import json
 import re
 import sys
 import tempfile
 import logging
 from pathlib import Path
 from typing import Union, List
 import torch
 from omegaconf import OmegaConf
 from pydub import AudioSegment
 from pydub.utils import mediainfo
 
 # fix importing from fairseq.examples
-import site
-sys.path.append(str(Path(site.getsitepackages()[0]) / 'fairseq'))
-try:
-    from fairseq.examples.speech_recognition.new.infer import hydra_main
-except ImportError:
-    from examples.speech_recognition.new.infer import hydra_main
+# import site
+# sys.path.append(str(Path(site.getsitepackages()[0]) / 'fairseq'))
+# try:
+#     from fairseq.examples.speech_recognition.new.infer import hydra_main
+# except ImportError:
+#     from examples.speech_recognition.new.infer import hydra_main
 
 
-from easymms import utils
+from easymms import utils as easymms_utils
 from easymms._logger import set_log_level
 from easymms.models.alignment import AlignmentModel
-from easymms.constants import CFG, HYPO_WORDS_FILE, MMS_LANGS_FILE
+from easymms import constants
 
 logger = logging.getLogger(__name__)
 
 
 class ASRModel:
     """
     MMS ASR class model
@@ -61,24 +62,48 @@
                  model: str,
                  log_level: int = logging.INFO):
         """
         :param model: path to the asr model <https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr>
         :param log_level: log level
         """
         set_log_level(log_level)
-        self.cfg = CFG.copy()
+        self.cfg = constants.CFG.copy()
         self.model = Path(model)
         self.cfg['common_eval']['path'] = str(self.model.resolve())
 
         self.tmp_dir = tempfile.TemporaryDirectory()
         self.tmp_dir_path = Path(self.tmp_dir.name)
         atexit.register(self._cleanup)
 
         self.wer = None
 
+
+
+    def _setup(self):
+        """
+        Helper function to setup different required packages
+        :return: None
+        """
+        # clone Fairseq
+        easymms_utils.clone(constants.FAIRSEQ_URL, constants.FAIRSEQ_DIR)
+        fairseq_dir = str(constants.FAIRSEQ_DIR.resolve())
+        sys.path.append(fairseq_dir)
+        try:
+            from fairseq.data.data_utils_fast import (
+                batch_by_size_fn,
+                batch_by_size_vec,
+                batch_fixed_shapes_fast,
+            )
+        except ImportError:
+            # we need to build the extension
+            from distutils.core import run_setup
+            run_setup(str((constants.FAIRSEQ_DIR / 'setup.py').resolve()), script_args=['build_ext', '--inplace'],
+                      stop_after='run')
+
+
     def _cleanup(self) -> None:
         """
         cleans up the temp_dir
         :return: None
         """
         self.tmp_dir.cleanup()
 
@@ -142,14 +167,36 @@
         :param timestamps_type: Once of (`segment`, `word` or `char`) if `align` is set to True, this will be used to fragment the raw text
         :param max_segment_len: the maximum length of the fragmented segments
         :param cfg: configuration dict in case you want to use a custom configuration, see [CFG](#Constants.CFG)
 
         :return: List of transcription text in the same order as input files
         """
         processed_files = self._prepare_media_files(media_files)
+        cwd = os.getcwd()
+        # clone Fairseq
+        easymms_utils.clone(constants.FAIRSEQ_URL, constants.FAIRSEQ_DIR)
+        fairseq_dir = str(constants.FAIRSEQ_DIR.resolve())
+        sys.path.append(fairseq_dir)
+        os.chdir(fairseq_dir)
+        # import
+        from examples.speech_recognition.new.infer import hydra_main
+        try:
+            from fairseq.data.data_utils_fast import (
+                batch_by_size_fn,
+                batch_by_size_vec,
+                batch_fixed_shapes_fast,
+            )
+        except ImportError:
+            # we need to build the extension
+            logger.info("Bulding required extensions, this may take a while ...")
+            from distutils.core import run_setup
+            run_setup(str((constants.FAIRSEQ_DIR / 'setup.py').resolve()), script_args=['build_ext', '--inplace'],
+                      stop_after='run')
+
+
         self._setup_tmp_dir(processed_files)
         # edit cfg
         if cfg is None:
             self.cfg['task']['data'] = self.cfg['decoding']['results_path'] = str(self.tmp_dir_path.resolve())
             self.cfg['dataset']['gen_subset'] = f'{lang}:dev'
             if device is None:
                 if torch.cuda.is_available():
@@ -162,42 +209,44 @@
                 self.cfg['common']['cpu'] = True
             if device == 'tpu':
                 self.cfg['common']['tpu'] = True
             cfg = OmegaConf.structured(self.cfg)
 
         self.wer = hydra_main(cfg)
         # get results: will just read from hypo.word as I don't want to change fairseq repo to get the hypo array
-        hypo_file = self.tmp_dir_path / HYPO_WORDS_FILE
+        hypo_file = self.tmp_dir_path / constants.HYPO_WORDS_FILE
         res = []
         with open(hypo_file) as hw:
             hypos = hw.readlines()
             outputs = self._reorder_decode(hypos)
             transcripts = [line[1].strip() for line in outputs]
         if align:
             align_model = AlignmentModel()
             for i in range(len(transcripts)):
                 media_file = processed_files[i][0]
-                transcript = utils.get_transcript_segments(transcripts[i], timestamps_type, max_segment_len=max_segment_len)
+                transcript = easymms_utils.get_transcript_segments(transcripts[i], timestamps_type, max_segment_len=max_segment_len)
                 segments = align_model.align(media_file=media_file,
                                              transcript=transcript,
                                              lang=lang,
                                              device=device)
                 res.append(segments)
         else:
             res = transcripts
+
+        os.chdir(cwd)
         return res
 
     @staticmethod
     def get_supported_langs() -> List[str]:
         """
         Helper function to get supported ISO 693-3 languages by the ASR model
         Source <https://dl.fbaipublicfiles.com/mms/misc/language_coverage_mms.html>
         :return: list of supported languages
         """
-        with open(MMS_LANGS_FILE) as f:
+        with open(constants.MMS_LANGS_FILE) as f:
             data = json.load(f)
             return [key for key in data if data[key]['ASR']]
 
     @staticmethod
     def _reorder_decode(hypos):
         """
         Helper method to reorder the `hypos`, see @bekarys0504 comment in
```

### Comparing `easymms-0.1.5/easymms/models/tts.py` & `easymms-0.1.6/easymms/models/tts.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.5/easymms/utils.py` & `easymms-0.1.6/easymms/utils.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.5/easymms.egg-info/PKG-INFO` & `easymms-0.1.6/easymms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymms
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
 Project-URL: Source, https://abdeladim-s.github.io/easymms/
 Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
 Requires-Python: >=3.8
```

### Comparing `easymms-0.1.5/setup.py` & `easymms-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 
 setup(
     name="easymms",
-    version="0.1.5",
+    version="0.1.6",
     author="Abdeladim Sadiki",
     description="A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project",
     long_description=long_description,
     ext_modules=[],
     zip_safe=False,
     python_requires=">=3.8",
     packages=find_packages('.'),
```

### Comparing `easymms-0.1.5/tests/test_asr.py` & `easymms-0.1.6/tests/test_asr.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.5/tests/test_tts.py` & `easymms-0.1.6/tests/test_tts.py`

 * *Files identical despite different names*

