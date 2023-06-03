# Comparing `tmp/robopianist-1.0.8.tar.gz` & `tmp/robopianist-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robopianist-1.0.8.tar", last modified: Thu Apr  6 15:37:07 2023, max compression
+gzip compressed data, was "robopianist-1.0.9.tar", last modified: Sat Jun  3 19:57:18 2023, max compression
```

## Comparing `robopianist-1.0.8.tar` & `robopianist-1.0.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.233737 robopianist-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-06 15:36:14.000000 robopianist-1.0.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-06 15:36:14.000000 robopianist-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-06 15:36:14.000000 robopianist-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-06 15:37:07.233737 robopianist-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-06 15:36:14.000000 robopianist-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-06 15:36:14.000000 robopianist-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.213736 robopianist-1.0.8/robopianist/
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.213736 robopianist-1.0.8/robopianist/models/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.213736 robopianist-1.0.8/robopianist/models/arenas/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/arenas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/arenas/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/arenas/stage_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.213736 robopianist-1.0.8/robopianist/models/hands/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/hands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/hands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/hands/shadow_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/hands/shadow_hand_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/hands/shadow_hand_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.213736 robopianist-1.0.8/robopianist/models/hands/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.213736 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.221737 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   341254 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/f_distal_pst.obj
--rw-r--r--   0 runner    (1001) docker     (123)    34351 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/f_knuckle.obj
--rw-r--r--   0 runner    (1001) docker     (123)    25738 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/f_middle.obj
--rw-r--r--   0 runner    (1001) docker     (123)    64846 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/f_proximal.obj
--rw-r--r--   0 runner    (1001) docker     (123)    80342 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/forearm_0.obj
--rw-r--r--   0 runner    (1001) docker     (123)  1285964 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/forearm_1.obj
--rw-r--r--   0 runner    (1001) docker     (123)    26812 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/forearm_collision.obj
--rw-r--r--   0 runner    (1001) docker     (123)    88696 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/lf_metacarpal.obj
--rw-r--r--   0 runner    (1001) docker     (123)   118690 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/mounting_plate.obj
--rw-r--r--   0 runner    (1001) docker     (123)   775747 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/palm.obj
--rw-r--r--   0 runner    (1001) docker     (123)   300842 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/th_distal_pst.obj
--rw-r--r--   0 runner    (1001) docker     (123)    75080 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/th_middle.obj
--rw-r--r--   0 runner    (1001) docker     (123)    23772 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/th_proximal.obj
--rw-r--r--   0 runner    (1001) docker     (123)   110838 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/wrist.obj
--rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/left_hand.xml
--rw-r--r--   0 runner    (1001) docker     (123)    17873 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/right_hand.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/scene_left.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/scene_right.xml
--rw-r--r--   0 runner    (1001) docker     (123)  1315458 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/shadow_hand.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.221737 robopianist-1.0.8/robopianist/models/piano/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/piano/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/piano/midi_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/piano/piano.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/piano/piano_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/piano/piano_mjcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/models/piano/piano_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.221737 robopianist-1.0.8/robopianist/music/
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.225737 robopianist-1.0.8/robopianist/music/data/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.225737 robopianist-1.0.8/robopianist/music/data/rousseau/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/data/rousseau/nocturne-trimmed.mid
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/data/rousseau/twinkle-twinkle-trimmed.mid
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/midi_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/midi_file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/midi_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/music_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/piano_roll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/music/synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.225737 robopianist-1.0.8/robopianist/soundfonts/
--rw-r--r--   0 runner    (1001) docker     (123)  5969788 2023-04-06 15:36:57.000000 robopianist-1.0.8/robopianist/soundfonts/TimGM6mb.sf2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.229737 robopianist-1.0.8/robopianist/suite/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/composite_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/suite_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.229737 robopianist-1.0.8/robopianist/suite/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/tasks/piano_with_one_shadow_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)    18464 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/tasks/piano_with_shadow_hands.py
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/tasks/piano_with_shadow_hands_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/tasks/self_actuated_piano.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/tasks/self_actuated_piano_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/variations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/suite/variations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.233737 robopianist-1.0.8/robopianist/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.233737 robopianist-1.0.8/robopianist/viewer/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/gui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/gui/fullscreen_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/gui/glfw_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    24076 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/user_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    21431 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/viewer/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.233737 robopianist-1.0.8/robopianist/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/wrappers/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-06 15:36:14.000000 robopianist-1.0.8/robopianist/wrappers/sound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:37:07.213736 robopianist-1.0.8/robopianist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-06 15:37:07.000000 robopianist-1.0.8/robopianist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-06 15:37:07.000000 robopianist-1.0.8/robopianist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:37:07.000000 robopianist-1.0.8/robopianist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-06 15:37:07.000000 robopianist-1.0.8/robopianist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:37:07.000000 robopianist-1.0.8/robopianist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-06 15:37:07.000000 robopianist-1.0.8/robopianist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 15:37:07.000000 robopianist-1.0.8/robopianist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 15:37:07.233737 robopianist-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-06 15:36:14.000000 robopianist-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.349764 robopianist-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-03 19:56:10.000000 robopianist-1.0.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-03 19:56:10.000000 robopianist-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-03 19:56:10.000000 robopianist-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-06-03 19:57:18.349764 robopianist-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-03 19:56:10.000000 robopianist-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-03 19:56:10.000000 robopianist-1.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.325764 robopianist-1.0.9/robopianist/
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.325764 robopianist-1.0.9/robopianist/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.325764 robopianist-1.0.9/robopianist/models/arenas/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/arenas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/arenas/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/arenas/stage_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.325764 robopianist-1.0.9/robopianist/models/hands/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/hands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/hands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/hands/shadow_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/hands/shadow_hand_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/hands/shadow_hand_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.321764 robopianist-1.0.9/robopianist/models/hands/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.325764 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.333764 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   341254 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/f_distal_pst.obj
+-rw-r--r--   0 runner    (1001) docker     (123)    34351 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/f_knuckle.obj
+-rw-r--r--   0 runner    (1001) docker     (123)    25738 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/f_middle.obj
+-rw-r--r--   0 runner    (1001) docker     (123)    64846 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/f_proximal.obj
+-rw-r--r--   0 runner    (1001) docker     (123)    80342 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/forearm_0.obj
+-rw-r--r--   0 runner    (1001) docker     (123)  1285964 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/forearm_1.obj
+-rw-r--r--   0 runner    (1001) docker     (123)    26812 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/forearm_collision.obj
+-rw-r--r--   0 runner    (1001) docker     (123)    88696 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/lf_metacarpal.obj
+-rw-r--r--   0 runner    (1001) docker     (123)   118690 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/mounting_plate.obj
+-rw-r--r--   0 runner    (1001) docker     (123)   775747 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/palm.obj
+-rw-r--r--   0 runner    (1001) docker     (123)   300842 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/th_distal_pst.obj
+-rw-r--r--   0 runner    (1001) docker     (123)    75080 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/th_middle.obj
+-rw-r--r--   0 runner    (1001) docker     (123)    23772 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/th_proximal.obj
+-rw-r--r--   0 runner    (1001) docker     (123)   110838 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/wrist.obj
+-rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/left_hand.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    17873 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/right_hand.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/scene_left.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/scene_right.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  1315458 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/shadow_hand.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.337764 robopianist-1.0.9/robopianist/models/piano/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/piano/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/piano/midi_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/piano/piano.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/piano/piano_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/piano/piano_mjcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/models/piano/piano_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.337764 robopianist-1.0.9/robopianist/music/
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.337764 robopianist-1.0.9/robopianist/music/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.337764 robopianist-1.0.9/robopianist/music/data/rousseau/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/data/rousseau/nocturne-trimmed.mid
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/data/rousseau/twinkle-twinkle-trimmed.mid
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/midi_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/midi_file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/midi_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/music_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/piano_roll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/music/synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.337764 robopianist-1.0.9/robopianist/soundfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)  5969788 2023-06-03 19:57:08.000000 robopianist-1.0.9/robopianist/soundfonts/TimGM6mb.sf2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.345764 robopianist-1.0.9/robopianist/suite/
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/composite_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/suite_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.345764 robopianist-1.0.9/robopianist/suite/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16038 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/tasks/piano_with_one_shadow_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/tasks/piano_with_shadow_hands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/tasks/piano_with_shadow_hands_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/tasks/self_actuated_piano.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/tasks/self_actuated_piano_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/variations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/suite/variations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.349764 robopianist-1.0.9/robopianist/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.349764 robopianist-1.0.9/robopianist/viewer/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/gui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/gui/fullscreen_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/gui/glfw_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24076 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/user_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21431 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/viewer/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.349764 robopianist-1.0.9/robopianist/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/wrappers/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-03 19:56:10.000000 robopianist-1.0.9/robopianist/wrappers/sound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:18.325764 robopianist-1.0.9/robopianist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-06-03 19:57:18.000000 robopianist-1.0.9/robopianist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-03 19:57:18.000000 robopianist-1.0.9/robopianist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:57:18.000000 robopianist-1.0.9/robopianist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-03 19:57:18.000000 robopianist-1.0.9/robopianist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:57:18.000000 robopianist-1.0.9/robopianist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-03 19:57:18.000000 robopianist-1.0.9/robopianist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 19:57:18.000000 robopianist-1.0.9/robopianist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 19:57:18.349764 robopianist-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-03 19:56:10.000000 robopianist-1.0.9/setup.py
```

### Comparing `robopianist-1.0.8/CITATION.cff` & `robopianist-1.0.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/LICENSE` & `robopianist-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/PKG-INFO` & `robopianist-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robopianist
-Version: 1.0.8
+Version: 1.0.9
 Summary: A benchmark for high-dimensional robot control
 Home-page: https://github.com/google-research/robopianist
 Author: Kevin Zakka
 Author-email: kevinarmandzakka@gmail.com
 Maintainer: Kevin Zakka
 Maintainer-email: kevinarmandzakka@gmail.com
 License: Apache License 2.0
@@ -14,16 +14,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # RoboPianist: A Benchmark for High-Dimensional Robot Control
 
@@ -36,15 +37,15 @@
 [docs-badge]: https://github.com/google-research/robopianist/actions/workflows/docs.yml/badge.svg
 [tests]: https://github.com/google-research/robopianist/actions/workflows/ci.yml
 [docs]: https://google-research.github.io/robopianist/
 [pypi-versions-badge]: https://img.shields.io/pypi/pyversions/robopianist
 [pypi-badge]: https://badge.fury.io/py/robopianist.svg
 [pypi]: https://pypi.org/project/robopianist/
 
-![RoboPianist teaser image](./docs/teaser1x3.jpeg)
+[![Video](http://img.youtube.com/vi/VBFn_Gg0yD8/hqdefault.jpg)](https://youtu.be/VBFn_Gg0yD8)
 
 RoboPianist is a new benchmarking suite for high-dimensional control, targeted at testing high spatial and temporal precision, coordination, and planning, all with an underactuated system frequently making-and-breaking contacts. The proposed challenge is *mastering the piano* through bi-manual dexterity, using a pair of simulated anthropomorphic robot hands.
 
 This codebase contains software and tasks for the benchmark, and is powered by [MuJoCo](https://mujoco.org/).
 
 - [Getting Started](#getting-started)
 - [Installation](#installation)
@@ -63,17 +64,15 @@
 
 We've created an introductory [Colab](https://colab.research.google.com/github/google-research/robopianist/blob/main/tutorial.ipynb) notebook that demonstrates how to use RoboPianist. It includes code for loading and customizing a piano playing task, and a demonstration of a pretrained policy playing a short snippet of *Twinkle Twinkle Little Star*. Click the button below to get started!
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/google-research/robopianist/blob/main/tutorial.ipynb)
 
 ## Installation
 
-RoboPianist is supported on both Linux and macOS and can be installed with Python 3.8 up to 3.10. We recommend using [Miniconda](https://docs.conda.io/en/latest/miniconda.html) to manage your Python environment.
-
-**3.11 will be supported once the numba team resolves [#8304](https://github.com/numba/numba/issues/8304).**
+RoboPianist is supported on both Linux and macOS and can be installed with Python >= 3.8. We recommend using [Miniconda](https://docs.conda.io/en/latest/miniconda.html) to manage your Python environment.
 
 ### Install from source
 
 The recommended way to install this package is from source. Start by cloning the repository:
 
 ```bash
 git clone https://github.com/google-research/robopianist.git && cd robopianist
@@ -141,18 +140,18 @@
 See [docs/faq.md](docs/faq.md) for a list of frequently asked questions.
 
 ## Citing RoboPianist
 
 If you use RoboPianist in your work, please use the following citation:
 
 ```bibtex
-@software{zakka2023robopianist,
+@article{zakka2023robopianist,
   author = {Zakka, Kevin and Smith, Laura and Gileadi, Nimrod and Howell, Taylor and Peng, Xue Bin and Singh, Sumeet and Tassa, Yuval and Florence, Pete and Zeng, Andy and Abbeel, Pieter},
   title = {{RoboPianist: A Benchmark for High-Dimensional Robot Control}},
-  url = {https://github.com/google-research/robopianist},
+  journal = {arXiv preprint arXiv:2304.04150},
   year = {2023},
 }
 ```
 
 ## Acknowledgements
 
 We would like to thank the following people for making this project possible:
@@ -160,10 +159,10 @@
 - [Philipp Wu](https://www.linkedin.com/in/wuphilipp/) and [Mohit Shridhar](https://mohitshridhar.com/) for being a constant source of inspiration and support.
 - [Ilya Kostrikov](https://www.kostrikov.xyz/) for constantly raising the bar for RL engineering and for invaluable debugging help.
 - The [Magenta](https://magenta.tensorflow.org/) team for helpful pointers and feedback.
 - The [MuJoCo](https://mujoco.org/) team for the development of the MuJoCo physics engine and their support throughout the project.
 
 ## License and Disclaimer
 
-[MuJoco Menagerie](https://github.com/deepmind/mujoco_menagerie)'s license can be found [here](https://github.com/deepmind/mujoco_menagerie/blob/main/LICENSE). Soundfont licensing information can be found [here](docs/soundfonts.md). MIDI licensing information can be found [here](docs/dataset). All other code is licensed under an [Apache-2.0 License](LICENSE).
+[MuJoco Menagerie](https://github.com/deepmind/mujoco_menagerie)'s license can be found [here](https://github.com/deepmind/mujoco_menagerie/blob/main/LICENSE). Soundfont licensing information can be found [here](docs/soundfonts.md). MIDI licensing information can be found [here](docs/dataset.md). All other code is licensed under an [Apache-2.0 License](LICENSE).
 
 This is not an officially supported Google product.
```

### Comparing `robopianist-1.0.8/README.md` & `robopianist-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [docs-badge]: https://github.com/google-research/robopianist/actions/workflows/docs.yml/badge.svg
 [tests]: https://github.com/google-research/robopianist/actions/workflows/ci.yml
 [docs]: https://google-research.github.io/robopianist/
 [pypi-versions-badge]: https://img.shields.io/pypi/pyversions/robopianist
 [pypi-badge]: https://badge.fury.io/py/robopianist.svg
 [pypi]: https://pypi.org/project/robopianist/
 
-![RoboPianist teaser image](./docs/teaser1x3.jpeg)
+[![Video](http://img.youtube.com/vi/VBFn_Gg0yD8/hqdefault.jpg)](https://youtu.be/VBFn_Gg0yD8)
 
 RoboPianist is a new benchmarking suite for high-dimensional control, targeted at testing high spatial and temporal precision, coordination, and planning, all with an underactuated system frequently making-and-breaking contacts. The proposed challenge is *mastering the piano* through bi-manual dexterity, using a pair of simulated anthropomorphic robot hands.
 
 This codebase contains software and tasks for the benchmark, and is powered by [MuJoCo](https://mujoco.org/).
 
 - [Getting Started](#getting-started)
 - [Installation](#installation)
@@ -36,17 +36,15 @@
 
 We've created an introductory [Colab](https://colab.research.google.com/github/google-research/robopianist/blob/main/tutorial.ipynb) notebook that demonstrates how to use RoboPianist. It includes code for loading and customizing a piano playing task, and a demonstration of a pretrained policy playing a short snippet of *Twinkle Twinkle Little Star*. Click the button below to get started!
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/google-research/robopianist/blob/main/tutorial.ipynb)
 
 ## Installation
 
-RoboPianist is supported on both Linux and macOS and can be installed with Python 3.8 up to 3.10. We recommend using [Miniconda](https://docs.conda.io/en/latest/miniconda.html) to manage your Python environment.
-
-**3.11 will be supported once the numba team resolves [#8304](https://github.com/numba/numba/issues/8304).**
+RoboPianist is supported on both Linux and macOS and can be installed with Python >= 3.8. We recommend using [Miniconda](https://docs.conda.io/en/latest/miniconda.html) to manage your Python environment.
 
 ### Install from source
 
 The recommended way to install this package is from source. Start by cloning the repository:
 
 ```bash
 git clone https://github.com/google-research/robopianist.git && cd robopianist
@@ -114,18 +112,18 @@
 See [docs/faq.md](docs/faq.md) for a list of frequently asked questions.
 
 ## Citing RoboPianist
 
 If you use RoboPianist in your work, please use the following citation:
 
 ```bibtex
-@software{zakka2023robopianist,
+@article{zakka2023robopianist,
   author = {Zakka, Kevin and Smith, Laura and Gileadi, Nimrod and Howell, Taylor and Peng, Xue Bin and Singh, Sumeet and Tassa, Yuval and Florence, Pete and Zeng, Andy and Abbeel, Pieter},
   title = {{RoboPianist: A Benchmark for High-Dimensional Robot Control}},
-  url = {https://github.com/google-research/robopianist},
+  journal = {arXiv preprint arXiv:2304.04150},
   year = {2023},
 }
 ```
 
 ## Acknowledgements
 
 We would like to thank the following people for making this project possible:
@@ -133,10 +131,10 @@
 - [Philipp Wu](https://www.linkedin.com/in/wuphilipp/) and [Mohit Shridhar](https://mohitshridhar.com/) for being a constant source of inspiration and support.
 - [Ilya Kostrikov](https://www.kostrikov.xyz/) for constantly raising the bar for RL engineering and for invaluable debugging help.
 - The [Magenta](https://magenta.tensorflow.org/) team for helpful pointers and feedback.
 - The [MuJoCo](https://mujoco.org/) team for the development of the MuJoCo physics engine and their support throughout the project.
 
 ## License and Disclaimer
 
-[MuJoco Menagerie](https://github.com/deepmind/mujoco_menagerie)'s license can be found [here](https://github.com/deepmind/mujoco_menagerie/blob/main/LICENSE). Soundfont licensing information can be found [here](docs/soundfonts.md). MIDI licensing information can be found [here](docs/dataset). All other code is licensed under an [Apache-2.0 License](LICENSE).
+[MuJoco Menagerie](https://github.com/deepmind/mujoco_menagerie)'s license can be found [here](https://github.com/deepmind/mujoco_menagerie/blob/main/LICENSE). Soundfont licensing information can be found [here](docs/soundfonts.md). MIDI licensing information can be found [here](docs/dataset.md). All other code is licensed under an [Apache-2.0 License](LICENSE).
 
 This is not an officially supported Google product.
```

### Comparing `robopianist-1.0.8/robopianist/__init__.py` & `robopianist-1.0.9/robopianist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from pathlib import Path
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 # Path to the root of the project.
 _PROJECT_ROOT = Path(__file__).parent.parent
 
 # Path to the soundfont directory.
 _SOUNDFONT_PATH = _PROJECT_ROOT / "robopianist" / "soundfonts"
```

### Comparing `robopianist-1.0.8/robopianist/cli.py` & `robopianist-1.0.9/robopianist/cli.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/__init__.py` & `robopianist-1.0.9/robopianist/models/__init__.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/arenas/__init__.py` & `robopianist-1.0.9/robopianist/models/arenas/__init__.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/arenas/stage.py` & `robopianist-1.0.9/robopianist/models/arenas/stage.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/arenas/stage_test.py` & `robopianist-1.0.9/robopianist/models/arenas/stage_test.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/__init__.py` & `robopianist-1.0.9/robopianist/models/hands/__init__.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/base.py` & `robopianist-1.0.9/robopianist/models/hands/base.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/shadow_hand.py` & `robopianist-1.0.9/robopianist/models/hands/shadow_hand.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/shadow_hand_constants.py` & `robopianist-1.0.9/robopianist/models/hands/shadow_hand_constants.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/shadow_hand_test.py` & `robopianist-1.0.9/robopianist/models/hands/shadow_hand_test.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/LICENSE` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/LICENSE`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/README.md` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/README.md`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/f_distal_pst.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/f_distal_pst.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/f_knuckle.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/f_knuckle.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/f_middle.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/f_middle.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/f_proximal.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/f_proximal.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/forearm_0.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/forearm_0.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/forearm_1.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/forearm_1.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/forearm_collision.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/forearm_collision.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/lf_metacarpal.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/lf_metacarpal.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/mounting_plate.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/mounting_plate.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/palm.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/palm.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/th_distal_pst.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/th_distal_pst.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/th_middle.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/th_middle.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/th_proximal.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/th_proximal.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/assets/wrist.obj` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/assets/wrist.obj`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/left_hand.xml` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/left_hand.xml`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/right_hand.xml` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/right_hand.xml`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/scene_left.xml` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/scene_left.xml`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/scene_right.xml` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/scene_right.xml`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/hands/third_party/shadow_hand/shadow_hand.png` & `robopianist-1.0.9/robopianist/models/hands/third_party/shadow_hand/shadow_hand.png`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/piano/__init__.py` & `robopianist-1.0.9/robopianist/models/piano/__init__.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/piano/midi_module.py` & `robopianist-1.0.9/robopianist/models/piano/midi_module.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/piano/piano.py` & `robopianist-1.0.9/robopianist/models/piano/piano.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/piano/piano_constants.py` & `robopianist-1.0.9/robopianist/models/piano/piano_constants.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/piano/piano_mjcf.py` & `robopianist-1.0.9/robopianist/models/piano/piano_mjcf.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/models/piano/piano_test.py` & `robopianist-1.0.9/robopianist/models/piano/piano_test.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/__init__.py` & `robopianist-1.0.9/robopianist/music/__init__.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/audio.py` & `robopianist-1.0.9/robopianist/music/audio.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/constants.py` & `robopianist-1.0.9/robopianist/music/constants.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/data/README.md` & `robopianist-1.0.9/robopianist/music/data/README.md`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/data/rousseau/nocturne-trimmed.mid` & `robopianist-1.0.9/robopianist/music/data/rousseau/nocturne-trimmed.mid`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/data/rousseau/twinkle-twinkle-trimmed.mid` & `robopianist-1.0.9/robopianist/music/data/rousseau/twinkle-twinkle-trimmed.mid`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/library.py` & `robopianist-1.0.9/robopianist/music/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
         8,
         2,
         9,
         6,
         8,
         6,
         5,
-        2,
+        7,
         1,
         9,
         6,
         8,
         6,
         5,
         0,
@@ -449,15 +449,15 @@
         6,
         5,
         0,
         3,
         2,
         1,
         0,
-        2,
+        7,
         4,
         9,
         6,
         8,
         6,
         5,
         0,
```

### Comparing `robopianist-1.0.8/robopianist/music/midi_file.py` & `robopianist-1.0.9/robopianist/music/midi_file.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/midi_file_test.py` & `robopianist-1.0.9/robopianist/music/midi_file_test.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/midi_message.py` & `robopianist-1.0.9/robopianist/music/midi_message.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/music_test.py` & `robopianist-1.0.9/robopianist/music/music_test.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/piano_roll.py` & `robopianist-1.0.9/robopianist/music/piano_roll.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/music/synthesizer.py` & `robopianist-1.0.9/robopianist/music/synthesizer.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/soundfonts/TimGM6mb.sf2` & `robopianist-1.0.9/robopianist/soundfonts/TimGM6mb.sf2`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/suite/__init__.py` & `robopianist-1.0.9/robopianist/suite/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """RoboPianist suite."""
 
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Mapping, Optional, Union
 
 from dm_control import composer
 from mujoco_utils import composer_utils
 
 from robopianist import music
 from robopianist.suite.tasks import piano_with_shadow_hands
 
@@ -51,15 +51,15 @@
     environment_name: str,
     midi_file: Optional[Path] = None,
     seed: Optional[int] = None,
     stretch: float = 1.0,
     shift: int = 0,
     recompile_physics: bool = False,
     legacy_step: bool = True,
-    task_kwargs: Optional[Dict[str, Any]] = None,
+    task_kwargs: Optional[Mapping[str, Any]] = None,
 ) -> composer.Environment:
     """Loads a RoboPianist environment.
 
     Args:
         environment_name: Name of the environment to load. Must be of the form
             "RoboPianist-repertoire-150-<name>-v0", where <name> is the name of a
             PIG dataset MIDI file in camel case notation.
```

### Comparing `robopianist-1.0.8/robopianist/suite/composite_reward.py` & `robopianist-1.0.9/robopianist/suite/composite_reward.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/suite/suite_test.py` & `robopianist-1.0.9/robopianist/suite/suite_test.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/suite/tasks/__init__.py` & `robopianist-1.0.9/robopianist/suite/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/suite/tasks/base.py` & `robopianist-1.0.9/robopianist/suite/tasks/base.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/suite/tasks/piano_with_one_shadow_hand.py` & `robopianist-1.0.9/robopianist/suite/tasks/piano_with_one_shadow_hand.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                 bounds=(0, _KEY_CLOSE_ENOUGH_TO_PRESSED),
                 margin=(_KEY_CLOSE_ENOUGH_TO_PRESSED * 10),
                 sigmoid="gaussian",
             )
             rew += 0.5 * rews.mean()
         # If there's any false positive, the remaining 0.5 reward is lost.
         off = np.flatnonzero(1 - self._goal_current[:-1])
-        rew += 0.5 * (1 - self.piano.activation[off].any())
+        rew += 0.5 * (1 - float(self.piano.activation[off].any()))
         return rew
 
     def _compute_fingering_reward(self, physics) -> float:
         """Reward for minimizing the distance between the fingers and the keys."""
 
         def _distance_finger_to_key(
             hand_keys: List[Tuple[int, int]], hand
```

### Comparing `robopianist-1.0.8/robopianist/suite/tasks/piano_with_shadow_hands.py` & `robopianist-1.0.9/robopianist/suite/tasks/piano_with_shadow_hands.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 # Energy penalty coefficient.
 _ENERGY_PENALTY_COEF = 5e-3
 
 # Transparency of fingertip geoms.
 _FINGERTIP_ALPHA = 1.0
 
+# Bounds for the uniform distribution from which initial hand offset is sampled.
+_POSITION_OFFSET = 0.05
+
 
 class PianoWithShadowHands(base.PianoTask):
     def __init__(
         self,
         midi: midi_file.MidiFile,
         n_steps_lookahead: int = 1,
         n_seconds_lookahead: Optional[float] = None,
@@ -53,14 +56,15 @@
         initial_buffer_time: float = 0.0,
         disable_fingering_reward: bool = False,
         disable_forearm_reward: bool = False,
         disable_colorization: bool = False,
         disable_hand_collisions: bool = False,
         augmentations: Optional[Sequence[base_variation.Variation]] = None,
         energy_penalty_coef: float = _ENERGY_PENALTY_COEF,
+        randomize_hand_positions: bool = False,
         **kwargs,
     ) -> None:
         """Task constructor.
 
         Args:
             midi: A `MidiFile` object.
             n_steps_lookahead: Number of timesteps to look ahead when computing the
@@ -82,14 +86,16 @@
             disable_colorization: If True, disables the colorization of the fingertips
                 and corresponding keys.
             disable_hand_collisions: If True, disables collisions between the two hands.
             augmentations: A list of `Variation` objects that will be applied to the
                 MIDI file at the beginning of each episode. If None, no augmentations
                 will be applied.
             energy_penalty_coef: Coefficient for the energy penalty.
+            randomize_hand_positions: If True, randomizes the initial position of the
+                hands at the beginning of each episode.
         """
         super().__init__(arena=stage.Stage(), **kwargs)
 
         self._midi = midi
         self._initial_midi = midi
         self._n_steps_lookahead = n_steps_lookahead
         if n_seconds_lookahead is not None:
@@ -103,14 +109,15 @@
         )
         self._disable_forearm_reward = disable_forearm_reward
         self._wrong_press_termination = wrong_press_termination
         self._disable_colorization = disable_colorization
         self._disable_hand_collisions = disable_hand_collisions
         self._augmentations = augmentations
         self._energy_penalty_coef = energy_penalty_coef
+        self._randomize_hand_positions = randomize_hand_positions
 
         if not disable_fingering_reward and not disable_colorization:
             self._colorize_fingertips()
         if disable_hand_collisions:
             self._disable_collisions_between_hands()
         self._reset_quantities_at_episode_init()
         self._reset_trajectory()  # Important: call before adding observables.
@@ -152,17 +159,17 @@
         self._sustains = note_traj.sustains
 
     # Composer methods.
 
     def initialize_episode(
         self, physics: mjcf.Physics, random_state: np.random.RandomState
     ) -> None:
-        del physics  # Unused.
         self._maybe_change_midi(random_state)
         self._reset_quantities_at_episode_init()
+        self._randomize_initial_hand_positions(physics, random_state)
 
     def before_step(
         self,
         physics: mjcf.Physics,
         action: np.ndarray,
         random_state: np.random.RandomState,
     ) -> None:
@@ -277,15 +284,15 @@
                 bounds=(0, _KEY_CLOSE_ENOUGH_TO_PRESSED),
                 margin=(_KEY_CLOSE_ENOUGH_TO_PRESSED * 10),
                 sigmoid="gaussian",
             )
             rew += 0.5 * rews.mean()
         # If there are any false positives, the remaining 0.5 reward is lost.
         off = np.flatnonzero(1 - self._goal_current[:-1])
-        rew += 0.5 * (1 - self.piano.activation[off].any())
+        rew += 0.5 * (1 - float(self.piano.activation[off].any()))
         return rew
 
     def _compute_fingering_reward(self, physics: mjcf.Physics) -> float:
         """Reward for minimizing the distance between the fingers and the keys."""
 
         def _distance_finger_to_key(
             hand_keys: List[Tuple[int, int]], hand
@@ -429,7 +436,17 @@
                 # the contype and conaffinity of the hand geoms that are already
                 # disabled (i.e., the visual geoms).
                 commit_defaults(geom, ["contype", "conaffinity"])
                 if geom.contype == 0 and geom.conaffinity == 0:
                     continue
                 geom.conaffinity = 0
                 geom.contype = 1
+
+    def _randomize_initial_hand_positions(
+        self, physics: mjcf.Physics, random_state: np.random.RandomState
+    ) -> None:
+        """Randomize the initial position of the hands."""
+        if not self._randomize_hand_positions:
+            return
+        offset = random_state.uniform(low=-_POSITION_OFFSET, high=_POSITION_OFFSET)
+        for hand in [self.right_hand, self.left_hand]:
+            hand.shift_pose(physics, (0, offset, 0))
```

### Comparing `robopianist-1.0.8/robopianist/suite/tasks/piano_with_shadow_hands_test.py` & `robopianist-1.0.9/robopianist/suite/tasks/piano_with_shadow_hands_test.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/suite/tasks/self_actuated_piano.py` & `robopianist-1.0.9/robopianist/suite/tasks/self_actuated_piano.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/suite/tasks/self_actuated_piano_test.py` & `robopianist-1.0.9/robopianist/suite/tasks/self_actuated_piano_test.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/suite/variations.py` & `robopianist-1.0.9/robopianist/suite/variations.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/suite/variations_test.py` & `robopianist-1.0.9/robopianist/suite/variations_test.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/__init__.py` & `robopianist-1.0.9/robopianist/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/application.py` & `robopianist-1.0.9/robopianist/viewer/application.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/figures.py` & `robopianist-1.0.9/robopianist/viewer/figures.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/gui/__init__.py` & `robopianist-1.0.9/robopianist/viewer/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/gui/base.py` & `robopianist-1.0.9/robopianist/viewer/gui/base.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/gui/fullscreen_quad.py` & `robopianist-1.0.9/robopianist/viewer/gui/fullscreen_quad.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/gui/glfw_gui.py` & `robopianist-1.0.9/robopianist/viewer/gui/glfw_gui.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/renderer.py` & `robopianist-1.0.9/robopianist/viewer/renderer.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/runtime.py` & `robopianist-1.0.9/robopianist/viewer/runtime.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/user_input.py` & `robopianist-1.0.9/robopianist/viewer/user_input.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/util.py` & `robopianist-1.0.9/robopianist/viewer/util.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/viewer.py` & `robopianist-1.0.9/robopianist/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/viewer/views.py` & `robopianist-1.0.9/robopianist/viewer/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,17 @@
     Args:
         data: A deque of floats or sequences of floats. Sequences of floats get plotted
             as multiple lines on the same figure.
         linename: A list of strings, one for each line in the time series if storing
             sequences of floats. Will be used to annotate the legend.
     """
 
-    data: Deque[Union[float, Sequence[float]]] = deque(maxlen=mujoco.mjMAXLINE)
+    data: Deque[Union[float, Sequence[float]]] = field(
+        default_factory=lambda: deque(maxlen=mujoco.mjMAXLINE)
+    )
     linename: List[str] = field(default_factory=list)
 
     def add(self, value: float) -> None:
         self.data.append(value)
 
     def add_dict(self, data: Dict[str, float]) -> None:
         # Sort the keys to ensure consistent ordering.
```

### Comparing `robopianist-1.0.8/robopianist/wrappers/__init__.py` & `robopianist-1.0.9/robopianist/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/wrappers/evaluation.py` & `robopianist-1.0.9/robopianist/wrappers/evaluation.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist/wrappers/sound.py` & `robopianist-1.0.9/robopianist/wrappers/sound.py`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/robopianist.egg-info/PKG-INFO` & `robopianist-1.0.9/robopianist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robopianist
-Version: 1.0.8
+Version: 1.0.9
 Summary: A benchmark for high-dimensional robot control
 Home-page: https://github.com/google-research/robopianist
 Author: Kevin Zakka
 Author-email: kevinarmandzakka@gmail.com
 Maintainer: Kevin Zakka
 Maintainer-email: kevinarmandzakka@gmail.com
 License: Apache License 2.0
@@ -14,16 +14,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # RoboPianist: A Benchmark for High-Dimensional Robot Control
 
@@ -36,15 +37,15 @@
 [docs-badge]: https://github.com/google-research/robopianist/actions/workflows/docs.yml/badge.svg
 [tests]: https://github.com/google-research/robopianist/actions/workflows/ci.yml
 [docs]: https://google-research.github.io/robopianist/
 [pypi-versions-badge]: https://img.shields.io/pypi/pyversions/robopianist
 [pypi-badge]: https://badge.fury.io/py/robopianist.svg
 [pypi]: https://pypi.org/project/robopianist/
 
-![RoboPianist teaser image](./docs/teaser1x3.jpeg)
+[![Video](http://img.youtube.com/vi/VBFn_Gg0yD8/hqdefault.jpg)](https://youtu.be/VBFn_Gg0yD8)
 
 RoboPianist is a new benchmarking suite for high-dimensional control, targeted at testing high spatial and temporal precision, coordination, and planning, all with an underactuated system frequently making-and-breaking contacts. The proposed challenge is *mastering the piano* through bi-manual dexterity, using a pair of simulated anthropomorphic robot hands.
 
 This codebase contains software and tasks for the benchmark, and is powered by [MuJoCo](https://mujoco.org/).
 
 - [Getting Started](#getting-started)
 - [Installation](#installation)
@@ -63,17 +64,15 @@
 
 We've created an introductory [Colab](https://colab.research.google.com/github/google-research/robopianist/blob/main/tutorial.ipynb) notebook that demonstrates how to use RoboPianist. It includes code for loading and customizing a piano playing task, and a demonstration of a pretrained policy playing a short snippet of *Twinkle Twinkle Little Star*. Click the button below to get started!
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/google-research/robopianist/blob/main/tutorial.ipynb)
 
 ## Installation
 
-RoboPianist is supported on both Linux and macOS and can be installed with Python 3.8 up to 3.10. We recommend using [Miniconda](https://docs.conda.io/en/latest/miniconda.html) to manage your Python environment.
-
-**3.11 will be supported once the numba team resolves [#8304](https://github.com/numba/numba/issues/8304).**
+RoboPianist is supported on both Linux and macOS and can be installed with Python >= 3.8. We recommend using [Miniconda](https://docs.conda.io/en/latest/miniconda.html) to manage your Python environment.
 
 ### Install from source
 
 The recommended way to install this package is from source. Start by cloning the repository:
 
 ```bash
 git clone https://github.com/google-research/robopianist.git && cd robopianist
@@ -141,18 +140,18 @@
 See [docs/faq.md](docs/faq.md) for a list of frequently asked questions.
 
 ## Citing RoboPianist
 
 If you use RoboPianist in your work, please use the following citation:
 
 ```bibtex
-@software{zakka2023robopianist,
+@article{zakka2023robopianist,
   author = {Zakka, Kevin and Smith, Laura and Gileadi, Nimrod and Howell, Taylor and Peng, Xue Bin and Singh, Sumeet and Tassa, Yuval and Florence, Pete and Zeng, Andy and Abbeel, Pieter},
   title = {{RoboPianist: A Benchmark for High-Dimensional Robot Control}},
-  url = {https://github.com/google-research/robopianist},
+  journal = {arXiv preprint arXiv:2304.04150},
   year = {2023},
 }
 ```
 
 ## Acknowledgements
 
 We would like to thank the following people for making this project possible:
@@ -160,10 +159,10 @@
 - [Philipp Wu](https://www.linkedin.com/in/wuphilipp/) and [Mohit Shridhar](https://mohitshridhar.com/) for being a constant source of inspiration and support.
 - [Ilya Kostrikov](https://www.kostrikov.xyz/) for constantly raising the bar for RL engineering and for invaluable debugging help.
 - The [Magenta](https://magenta.tensorflow.org/) team for helpful pointers and feedback.
 - The [MuJoCo](https://mujoco.org/) team for the development of the MuJoCo physics engine and their support throughout the project.
 
 ## License and Disclaimer
 
-[MuJoco Menagerie](https://github.com/deepmind/mujoco_menagerie)'s license can be found [here](https://github.com/deepmind/mujoco_menagerie/blob/main/LICENSE). Soundfont licensing information can be found [here](docs/soundfonts.md). MIDI licensing information can be found [here](docs/dataset). All other code is licensed under an [Apache-2.0 License](LICENSE).
+[MuJoco Menagerie](https://github.com/deepmind/mujoco_menagerie)'s license can be found [here](https://github.com/deepmind/mujoco_menagerie/blob/main/LICENSE). Soundfont licensing information can be found [here](docs/soundfonts.md). MIDI licensing information can be found [here](docs/dataset.md). All other code is licensed under an [Apache-2.0 License](LICENSE).
 
 This is not an officially supported Google product.
```

### Comparing `robopianist-1.0.8/robopianist.egg-info/SOURCES.txt` & `robopianist-1.0.9/robopianist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robopianist-1.0.8/setup.py` & `robopianist-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 author = "Kevin Zakka"
 
 author_email = "kevinarmandzakka@gmail.com"
 
@@ -90,15 +91,15 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords=keywords,
     url=f"https://github.com/google-research/{name}",
     license="Apache License 2.0",
     license_files=("LICENSE",),
     packages=find_packages(exclude=["examples"]),
-    python_requires=">=3.8, <3.11",
+    python_requires=">=3.8",
     install_requires=core_requirements,
     include_package_data=True,
     classifiers=classifiers,
     extras_require={
         "test": test_requirements,
         "dev": dev_requirements,
     },
```

