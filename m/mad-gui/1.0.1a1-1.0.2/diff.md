# Comparing `tmp/mad_gui-1.0.1a1.tar.gz` & `tmp/mad_gui-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mad_gui-1.0.1a1.tar", max compression
+gzip compressed data, was "mad_gui-1.0.2.tar", max compression
```

## Comparing `mad_gui-1.0.1a1.tar` & `mad_gui-1.0.2.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0     1100 2022-07-18 17:31:44.111098 mad_gui-1.0.1a1/LICENSE
--rw-r--r--   0        0        0     2278 2022-07-18 17:31:44.111098 mad_gui-1.0.1a1/README_pypi.md
--rw-r--r--   0        0        0      301 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/__init__.py
--rw-r--r--   0        0        0      217 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/dialogs/__init__.py
--rw-r--r--   0        0        0     1925 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/dialogs/data_selector.py
--rw-r--r--   0        0        0     6910 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/dialogs/label_annotation_dialog.py
--rw-r--r--   0        0        0      245 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/dialogs/plugin_selection/__init__.py
--rw-r--r--   0        0        0    13512 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/dialogs/plugin_selection/load_data_dialog.py
--rw-r--r--   0        0        0     4436 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/dialogs/plugin_selection/plugin_selection_dialog.py
--rw-r--r--   0        0        0     4221 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/dialogs/user_information.py
--rw-r--r--   0        0        0      648 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/helper.py
--rw-r--r--   0        0        0     2143 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/key_event_handler.py
--rw-r--r--   0        0        0     2511 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/components/sidebar.py
--rw-r--r--   0        0        0      909 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/config/__init__.py
--rw-r--r--   0        0        0      304 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/config/settings.py
--rw-r--r--   0        0        0      777 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/config/theme.py
--rw-r--r--   0        0        0       76 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/models/__init__.py
--rw-r--r--   0        0        0     2499 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/models/global_data.py
--rw-r--r--   0        0        0      110 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/models/local/__init__.py
--rw-r--r--   0        0        0     6833 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/models/local/plot_data.py
--rw-r--r--   0        0        0      422 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/models/ui_state.py
--rw-r--r--   0        0        0      351 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/labels/__init__.py
--rw-r--r--   0        0        0    14379 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/labels/base_label.py
--rw-r--r--   0        0        0     8129 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/labels/labels.py
--rw-r--r--   0        0        0      240 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/plots/__init__.py
--rw-r--r--   0        0        0      989 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/plots/base_mode_handler.py
--rw-r--r--   0        0        0    13409 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/plots/base_plot.py
--rw-r--r--   0        0        0    20846 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/plots/sensor_plot.py
--rw-r--r--   0        0        0    11097 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/plots/sensor_plot_mode_handler.py
--rw-r--r--   0        0        0     3543 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/plots/video_plot.py
--rw-r--r--   0        0        0     1040 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plot_tools/plots/video_plot_mode_handler.py
--rw-r--r--   0        0        0      566 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plugins/__init__.py
--rw-r--r--   0        0        0    10424 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plugins/base.py
--rw-r--r--   0        0        0     6877 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plugins/example.py
--rw-r--r--   0        0        0      279 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/plugins/helper.py
--rw-r--r--   0        0        0       58 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/qt_designer/__init__.py
--rw-r--r--   0        0        0     1933 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/qt_designer/channel_selector.ui
--rw-r--r--   0        0        0    31016 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/algorithm.png
--rw-r--r--   0        0        0     1063 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/burger.png
--rw-r--r--   0        0        0     7748 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/camera.png
--rw-r--r--   0        0        0     7450 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/camera_light.png
--rw-r--r--   0        0        0     9019 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/export.png
--rw-r--r--   0        0        0    28229 2022-07-18 17:31:44.127098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/icon.png
--rw-r--r--   0        0        0    33097 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/label.png
--rw-r--r--   0        0        0    12745 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/logo_mad_man.png
--rw-r--r--   0        0        0     7392 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/open.png
--rw-r--r--   0        0        0    23115 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/reload.png
--rw-r--r--   0        0        0     3593 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/images/save.png
--rw-r--r--   0        0        0    10585 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/load.ui
--rw-r--r--   0        0        0    48842 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/main.ui
--rw-r--r--   0        0        0     2471 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/palette_btn.xml
--rw-r--r--   0        0        0     5420 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/palette_window.xml
--rw-r--r--   0        0        0    10862 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/plugin_selection.ui
--rw-r--r--   0        0        0     2227 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/ui_video.py
--rw-r--r--   0        0        0      523 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/window_buttons.qrc
--rw-r--r--   0        0        0   603290 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/qt_designer/window_buttons_rc.py
--rw-r--r--   0        0        0     2482 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/start_gui.py
--rw-r--r--   0        0        0     1843 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/state_keeper.py
--rw-r--r--   0        0        0        0 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/utils/__init__.py
--rw-r--r--   0        0        0     2902 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/utils/helper.py
--rw-r--r--   0        0        0     3765 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/utils/model_base.py
--rw-r--r--   0        0        0      522 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/windows/__init__.py
--rw-r--r--   0        0        0    30759 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/windows/main.py
--rw-r--r--   0        0        0     6890 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/mad_gui/windows/video_window.py
--rw-r--r--   0        0        0     1951 2022-07-18 17:31:44.131098 mad_gui-1.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     3606 2022-07-18 17:31:59.108575 mad_gui-1.0.1a1/setup.py
--rw-r--r--   0        0        0     3139 2022-07-18 17:31:59.108944 mad_gui-1.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-06-03 06:57:52.113863 mad_gui-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2278 2023-06-03 06:57:52.113863 mad_gui-1.0.2/README_pypi.md
+-rw-r--r--   0        0        0      301 2023-06-03 06:57:52.129863 mad_gui-1.0.2/mad_gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 06:57:52.129863 mad_gui-1.0.2/mad_gui/components/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-03 06:57:52.129863 mad_gui-1.0.2/mad_gui/components/dialogs/__init__.py
+-rw-r--r--   0        0        0     1925 2023-06-03 06:57:52.129863 mad_gui-1.0.2/mad_gui/components/dialogs/data_selector.py
+-rw-r--r--   0        0        0     7054 2023-06-03 06:57:52.129863 mad_gui-1.0.2/mad_gui/components/dialogs/label_annotation_dialog.py
+-rw-r--r--   0        0        0      245 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/components/dialogs/plugin_selection/__init__.py
+-rw-r--r--   0        0        0    13512 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/components/dialogs/plugin_selection/load_data_dialog.py
+-rw-r--r--   0        0        0     4436 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/components/dialogs/plugin_selection/plugin_selection_dialog.py
+-rw-r--r--   0        0        0     4221 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/components/dialogs/user_information.py
+-rw-r--r--   0        0        0      648 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/components/helper.py
+-rw-r--r--   0        0        0     2143 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/components/key_event_handler.py
+-rw-r--r--   0        0        0     2511 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/components/sidebar.py
+-rw-r--r--   0        0        0      909 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/config/__init__.py
+-rw-r--r--   0        0        0      304 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/config/settings.py
+-rw-r--r--   0        0        0      777 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/config/theme.py
+-rw-r--r--   0        0        0       76 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/models/__init__.py
+-rw-r--r--   0        0        0     2499 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/models/global_data.py
+-rw-r--r--   0        0        0      110 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/models/local/__init__.py
+-rw-r--r--   0        0        0     6833 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/models/local/plot_data.py
+-rw-r--r--   0        0        0      422 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/models/ui_state.py
+-rw-r--r--   0        0        0      351 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/labels/__init__.py
+-rw-r--r--   0        0        0    15205 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/labels/base_label.py
+-rw-r--r--   0        0        0     8282 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/labels/labels.py
+-rw-r--r--   0        0        0      240 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/plots/__init__.py
+-rw-r--r--   0        0        0     1041 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/plots/base_mode_handler.py
+-rw-r--r--   0        0        0    13383 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/plots/base_plot.py
+-rw-r--r--   0        0        0    20814 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/plots/sensor_plot.py
+-rw-r--r--   0        0        0    11673 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/plots/sensor_plot_mode_handler.py
+-rw-r--r--   0        0        0     3543 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/plots/video_plot.py
+-rw-r--r--   0        0        0     1040 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plot_tools/plots/video_plot_mode_handler.py
+-rw-r--r--   0        0        0      566 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plugins/__init__.py
+-rw-r--r--   0        0        0    10424 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plugins/base.py
+-rw-r--r--   0        0        0     6896 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plugins/example.py
+-rw-r--r--   0        0        0      279 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/plugins/helper.py
+-rw-r--r--   0        0        0       58 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/__init__.py
+-rw-r--r--   0        0        0     1933 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/channel_selector.ui
+-rw-r--r--   0        0        0    31016 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/algorithm.png
+-rw-r--r--   0        0        0     1063 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/burger.png
+-rw-r--r--   0        0        0     7748 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/camera.png
+-rw-r--r--   0        0        0     7450 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/camera_light.png
+-rw-r--r--   0        0        0     9019 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/export.png
+-rw-r--r--   0        0        0    28229 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/icon.png
+-rw-r--r--   0        0        0    33097 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/label.png
+-rw-r--r--   0        0        0    12745 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/logo_mad_man.png
+-rw-r--r--   0        0        0     7392 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/open.png
+-rw-r--r--   0        0        0    23115 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/reload.png
+-rw-r--r--   0        0        0     3593 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/images/save.png
+-rw-r--r--   0        0        0    10585 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/load.ui
+-rw-r--r--   0        0        0    48842 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/main.ui
+-rw-r--r--   0        0        0     2471 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/palette_btn.xml
+-rw-r--r--   0        0        0     5420 2023-06-03 06:57:52.133864 mad_gui-1.0.2/mad_gui/qt_designer/palette_window.xml
+-rw-r--r--   0        0        0    10862 2023-06-03 06:57:52.137864 mad_gui-1.0.2/mad_gui/qt_designer/plugin_selection.ui
+-rw-r--r--   0        0        0     2227 2023-06-03 06:57:52.137864 mad_gui-1.0.2/mad_gui/qt_designer/ui_video.py
+-rw-r--r--   0        0        0      523 2023-06-03 06:57:52.137864 mad_gui-1.0.2/mad_gui/qt_designer/window_buttons.qrc
+-rw-r--r--   0        0        0   603290 2023-06-03 06:57:52.137864 mad_gui-1.0.2/mad_gui/qt_designer/window_buttons_rc.py
+-rw-r--r--   0        0        0     2865 2023-06-03 06:57:52.137864 mad_gui-1.0.2/mad_gui/start_gui.py
+-rw-r--r--   0        0        0     1843 2023-06-03 06:57:52.137864 mad_gui-1.0.2/mad_gui/state_keeper.py
+-rw-r--r--   0        0        0        0 2023-06-03 06:57:52.137864 mad_gui-1.0.2/mad_gui/utils/__init__.py
+-rw-r--r--   0        0        0     2902 2023-06-03 06:57:52.137864 mad_gui-1.0.2/mad_gui/utils/helper.py
+-rw-r--r--   0        0        0     3765 2023-06-03 06:57:52.137864 mad_gui-1.0.2/mad_gui/utils/model_base.py
+-rw-r--r--   0        0        0      522 2023-06-03 06:57:52.141864 mad_gui-1.0.2/mad_gui/windows/__init__.py
+-rw-r--r--   0        0        0    30691 2023-06-03 06:57:52.141864 mad_gui-1.0.2/mad_gui/windows/main.py
+-rw-r--r--   0        0        0     6890 2023-06-03 06:57:52.141864 mad_gui-1.0.2/mad_gui/windows/video_window.py
+-rw-r--r--   0        0        0     1857 2023-06-03 06:57:52.141864 mad_gui-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3145 1970-01-01 00:00:00.000000 mad_gui-1.0.2/PKG-INFO
```

### Comparing `mad_gui-1.0.1a1/LICENSE` & `mad_gui-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/README_pypi.md` & `mad_gui-1.0.2/README_pypi.md`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/components/dialogs/data_selector.py` & `mad_gui-1.0.2/mad_gui/components/dialogs/data_selector.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/components/dialogs/label_annotation_dialog.py` & `mad_gui-1.0.2/mad_gui/components/dialogs/label_annotation_dialog.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,31 +4,40 @@
 from PySide2.QtWidgets import QButtonGroup, QDialog, QDialogButtonBox, QGroupBox, QHBoxLayout, QRadioButton, QVBoxLayout
 
 from typing import Any, Dict, List, Tuple, Union
 
 
 def depth(d):
     if isinstance(d, dict):
-        return 1 + (max(map(depth, d.values())) if d else 0)
-    return 0
+        if not d:
+            # empty dict
+            return 1
+        all_depths = (depth(v) for v in d.values())
+        return 1 + max(all_depths)
+    if isinstance(d, list):
+        return 1
+    if d is None:
+        return 0
+    raise ValueError(f"Unknown type {type(d)}")
 
 
 class NestedLabelSelectDialog(QDialog):
     """A Window with Radio Buttons or Checkboxes"""
 
     _max_depth: int
     _label_options: Union[List[str], Dict[str, Any]]
 
     latest_selection_: Tuple[str, ...] = ()
 
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, initial_selection: Tuple[str, ...] = None):
         super().__init__()
         self.parent = parent
         self.setWindowIcon(self.parent.windowIcon())
         self.setPalette(self.parent.palette())
+        self.initial_selection = initial_selection or NestedLabelSelectDialog.latest_selection_
         self.main_layout = QVBoxLayout()
         self.level_widgets: List[QVBoxLayout] = []
         self.level_button_group: List[QButtonGroup] = []
         self.buttons = QDialogButtonBox(parent=self)
         self.buttons.addButton("Ok", QDialogButtonBox.AcceptRole)
         self.buttons.addButton("Cancel", QDialogButtonBox.RejectRole)
         self.buttons.accepted.connect(self.accept)
@@ -38,46 +47,42 @@
 
         self.setLayout(self.main_layout)
 
     def _setup_layout(self):
         # Create emtpy layouts based max depth
         label_layout = QHBoxLayout()
         self.main_layout.addLayout(label_layout)
-        for i in range(self._max_depth + 1):
+        for i in range(self._max_depth):
             group_box = QGroupBox(parent=self, title=f"Level {i}")
             group_box.setPalette(self.palette())
             inner_layout = QVBoxLayout()
             inner_layout.addStretch()
             group_box.setLayout(inner_layout)
             label_layout.addWidget(group_box)
             self.level_widgets.append(inner_layout)
             button_group = QButtonGroup(parent=group_box)
             button_group.setObjectName(str(i))
             button_group.buttonToggled.connect(self._on_label_select)
             self.level_button_group.append(button_group)
 
         self.main_layout.addWidget(self.buttons)
         self._setup_level(self._get_level_keys(self._label_options), level=0)
-        if NestedLabelSelectDialog.latest_selection_:
-            for level, name_button in enumerate(NestedLabelSelectDialog.latest_selection_):
-                radiobutton = self.findChild(QRadioButton, name_button)
-                self.level_button_group[level].buttonToggled.emit(radiobutton, True)
 
-        self.level_button_group[0].buttons()[0].setFocus()
+        self.level_button_group[0].checkedButton().setFocus()
 
     def _on_label_select(self, value):
         if not value:
             return None
         level = int(self.sender().objectName())
         choices = self._get_choices(level + 1)
         if choices is not None:
             return self._setup_level(choices, level + 1)
         # We have a final choice.
         # We do nothing, but we need to cleanup all further levels"
-        for i in range(level + 1, self._max_depth + 1):
+        for i in range(level + 1, self._max_depth):
             self._clean_level(i)
 
         self.current_selection_ = tuple(b.checkedButton().objectName() for b in self.level_button_group[: level + 1])
         return None
 
     def _get_choices(self, level):
         if level == 0:
@@ -111,37 +116,36 @@
 
     def _setup_level(self, choices: List[str], level: int):
         widget = self.level_widgets[level]
         group = self.level_button_group[level]
 
         self._clean_level(level)
 
-        first_button = None
+        pre_selected = None
+
+        initial_choice_for_level = None
+        if self.initial_selection and len(self.initial_selection) > level:
+            initial_choice_for_level = self.initial_selection[level]
 
         for i, choice in enumerate(choices):
             button = QRadioButton(str(i + 1) + ": " + choice, parent=self)
             # This is required so that we can capture the space key
             button.installEventFilter(self)
             button.setObjectName(choice)
             if i == 0:
-                first_button = button
+                # per default we select the first button
+                pre_selected = button
+            if initial_choice_for_level == choice:
+                pre_selected = button
             # We insert instead of add to keep the stretch at the bottom
             widget.insertWidget(widget.count() - 1, button)
-            if (
-                NestedLabelSelectDialog.latest_selection_
-                and len(NestedLabelSelectDialog.latest_selection_) > level
-                and NestedLabelSelectDialog.latest_selection_[level] in choice
-            ):
-
-                button.setChecked(True)
             group.addButton(button)
 
         # Enable first checkbox:
-        if first_button is not None and not NestedLabelSelectDialog.latest_selection_:
-            first_button.setChecked(True)
+        pre_selected.setChecked(True)
 
     def get_label(self, label_options: Union[List[str], Dict[str, Any]]):
         self._max_depth = depth(label_options)
         self._label_options = label_options
         self._setup_layout()
         if self.exec_():
             NestedLabelSelectDialog.latest_selection_ = self.current_selection_
@@ -155,15 +159,19 @@
             self.accept()
             return
         if event.key() == Qt.Key_Escape:
             event.accept()
             self.reject()
             return
         current_focus = self.focusWidget().parentWidget()
-        level = self.level_widgets.index(current_focus.layout())
+        try:
+            level = self.level_widgets.index(current_focus.layout())
+        except ValueError:
+            # This happens if a widget is focused that is not part of the label selection
+            return
         choices = self._get_choices(level)
         # Number keys start at 49 to 59
         mapping = dict(zip(range(49, 59), choices))
         k_choice = mapping.get(event.key(), None)
         if k_choice is None:
             return
         button: QRadioButton = current_focus.findChild(QRadioButton, k_choice)
```

### Comparing `mad_gui-1.0.1a1/mad_gui/components/dialogs/plugin_selection/load_data_dialog.py` & `mad_gui-1.0.2/mad_gui/components/dialogs/plugin_selection/load_data_dialog.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/components/dialogs/plugin_selection/plugin_selection_dialog.py` & `mad_gui-1.0.2/mad_gui/components/dialogs/plugin_selection/plugin_selection_dialog.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/components/dialogs/user_information.py` & `mad_gui-1.0.2/mad_gui/components/dialogs/user_information.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/components/helper.py` & `mad_gui-1.0.2/mad_gui/components/helper.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/components/key_event_handler.py` & `mad_gui-1.0.2/mad_gui/components/key_event_handler.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/components/sidebar.py` & `mad_gui-1.0.2/mad_gui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/config/__init__.py` & `mad_gui-1.0.2/mad_gui/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/config/theme.py` & `mad_gui-1.0.2/mad_gui/config/theme.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/models/global_data.py` & `mad_gui-1.0.2/mad_gui/models/global_data.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/models/local/plot_data.py` & `mad_gui-1.0.2/mad_gui/models/local/plot_data.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/plot_tools/labels/base_label.py` & `mad_gui-1.0.2/mad_gui/plot_tools/labels/base_label.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pyqtgraph import mkPen
 from PySide2.QtGui import QColor, QHoverEvent, QMouseEvent, Qt
 
 from mad_gui.components.dialogs import UserInformation
 from mad_gui.components.dialogs.label_annotation_dialog import NestedLabelSelectDialog
 from mad_gui.config import Config
 from mad_gui.state_keeper import StateKeeper
-from typing import Optional
+from typing import Optional, Union, Sequence
 
 
 class InvalidStartEnd(Exception):
     pass
 
 
 class NoLabelSelected(Exception):
@@ -25,15 +25,15 @@
     max_height = 1
     descriptions: dict = {}
 
     def __init__(
         self,
         parent,
         pos,
-        description: Optional[str] = None,
+        description: Optional[Union[str, Sequence[str]]] = None,
         belongs_to_region_label: Optional[bool] = False,
         min_height: Optional[float] = 0,
         max_height: Optional[float] = 1,
     ):
         self.parent = parent
         self.removable = False
         self.belongs_to_region_label = belongs_to_region_label
@@ -69,15 +69,25 @@
 
     def mousePressEvent(self, event: QMouseEvent):  # noqa: N802
         if self.removable:
             self.parent.removeItem(self)
             self.parent.setCursor(Qt.ArrowCursor)
         elif self.movable:
             super().mousePressEvent(event)
-            self.setPos(self.parent.snap_to_sample(self.pos().x()))
+            if event.modifiers() == Qt.ControlModifier:
+                try:
+                    description = edit_label_description(
+                        descriptions=self.descriptions, parent=self.parent.parent, initial=self.description
+                    )
+                except NoLabelSelected:
+                    pass
+                else:
+                    self.description = description
+            else:
+                self.setPos(self.parent.snap_to_sample(self.pos().x()))
 
     def mouseDragEvent(self, ev):  # noqa: N802
         super().mouseDragEvent(ev)
         self.setPos(self.parent.snap_to_sample(self.pos().x()))
 
     def make_editable(self):
         self.removable = False
@@ -131,15 +141,15 @@
     def __init__(
         self,
         start: int,
         end: int,
         parent,
         events: Optional[pd.Series] = None,
         identifier: int = None,
-        description: Optional[str] = None,
+        description: Optional[Union[str, Sequence[str]]] = None,
         **_kwargs,  # underscore to prevent pylint form triggering
     ):
         pg.LinearRegionItem.__init__(self)
         self.parent = parent
         self.setMovable(False)
         self._set_border_colors(start, end)
         self._set_border_positions(start, end)
@@ -172,15 +182,15 @@
                 description = ", ".join(self.description)
             else:
                 description = self.description
             self.setToolTip(f"{self.name}: {description}")
         self.setEnabled(False)
 
     def _set_events(self, events: pd.DataFrame):
-        for event, pos in events.iteritems():
+        for event, pos in events.items():
             if pos is None:
                 return
             self.event_labels[event] = BaseEventLabel(
                 parent=self.parent,
                 pos=pos,
                 description=event,
                 min_height=self.min_height,
@@ -199,15 +209,20 @@
                 UserInformation.inform(
                     f"MaD GUI is not aware of descriptions for the class {self.name}. Thus, you can not edit the "
                     f"description.",
                     help_link="https://mad-gui.readthedocs.io/en/latest/troubleshooting.html#mad-gui-is-not-aware-of-"
                     "descriptions-for-the-class",
                 )
                 return
-            self.edit_label_description()
+            try:
+                self.description = edit_label_description(
+                    descriptions=self.descriptions, parent=self.parent.parent, initial=self.description
+                )
+            except NoLabelSelected:
+                pass
 
     def _hover_event(self, ev):
         """Coloring if mouse hovers of the stride"""
         # such that only borders of this element will be movable
         # and not the one of the neighbour
         self.setEnabled(True)
 
@@ -230,27 +245,14 @@
         return QColor(0, 255, 0, 50)
 
     def _description_to_str(self):
         if isinstance(self.description, tuple):
             return ", ".join(self.description)
         return self.description
 
-    def edit_label_description(self):
-        """Setting the type of the activity to one given in the consts file.
-
-        Called by :meth:`mad_gui.plot_tools.SensorPlot._finish_adding_activity` or if the user clicks on the label while
-        being in edit mode. The emitted signal is caught by :meth:`mad_gui.MainWindow.ask_for_label_type`.
-        """
-        # the activities should be set by passing a `Settings` object which inherits from mad_gui.config.BaseSettings
-        # and has an attribute `ACTIVITIES`, see our developer guidelines for more information
-        new_description = NestedLabelSelectDialog(parent=self.parent.parent).get_label(self.descriptions)
-        if not new_description:
-            raise NoLabelSelected("Invalid description selected for label")
-        self.description = new_description
-
     def _set_removable(self, removable: bool):
         self.removable = removable
         if not removable:
             self.setBrush(self.standard_brush)
 
     def _set_editable(self, editable: bool):
         self.editable = editable
@@ -376,7 +378,29 @@
                 self.setEnabled(False)
             if event.exit and self.mouseHovering:
                 self.parent.setCursor(Qt.PointingHandCursor)
                 self.setMouseHover(True)
             elif event.exit and not self.mouseHovering:
                 self.parent.setCursor(Qt.ArrowCursor)
                 self.setEnabled(True)
+
+
+def edit_label_description(descriptions, parent, initial=None):
+    """Setting the type of the activity to one given in the consts file.
+
+    Called by :meth:`mad_gui.plot_tools.SensorPlot._finish_adding_activity` or if the user clicks on the label while
+    being in edit mode. The emitted signal is caught by :meth:`mad_gui.MainWindow.ask_for_label_type`.
+    """
+    if initial is None:
+        pass
+    elif isinstance(initial, str):
+        initial = (initial,)
+    else:
+        initial = tuple(initial)
+
+    # the activities should be set by passing a `Settings` object which inherits from mad_gui.config.BaseSettings
+    # and has an attribute `ACTIVITIES`, see our developer guidelines for more information
+    new_description = NestedLabelSelectDialog(parent=parent, initial_selection=initial).get_label(descriptions)
+    if not new_description:
+        raise NoLabelSelected("Invalid description selected for label")
+
+    return new_description
```

### Comparing `mad_gui-1.0.1a1/mad_gui/plot_tools/labels/labels.py` & `mad_gui-1.0.2/mad_gui/plot_tools/labels/labels.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from typing import Callable, Optional, Type
+
 import numpy as np
 import pandas as pd
 import pyqtgraph as pg
 from PySide2.QtGui import QBrush, QColor, QLinearGradient, Qt
 from PySide2.QtWidgets import QWidget
 
 from mad_gui.config import Config
-from mad_gui.plot_tools.labels.base_label import BaseRegionLabel, InvalidStartEnd
+from mad_gui.plot_tools.labels.base_label import BaseRegionLabel, InvalidStartEnd, edit_label_description
 from mad_gui.state_keeper import StateKeeper
-from typing import Callable, Optional, Type
 
 
 class SegmentedStrideLabel(BaseRegionLabel):
     """Stride labels that only have a start and an end.
 
     This class can for example be used to generate stride labels as suggested by Barth et al. [1]_. This label looks
     like an :class:`RegionLabel`, just that it is placed in the area of `self.min_height` to
@@ -184,28 +185,30 @@
     def finalize(self):
         start, end = self.getRegion()
         if self.post_process is not None:
             end = self.post_process(end)
 
         if start == end:
             raise InvalidStartEnd()
-        events_series = pd.Series()
+        events_series = []
         for event in self.events:
             s = pd.Series(data=event.pos().x() * self.sampling_rate_hz, index=event.description)
-            events_series = events_series.append(s)
+            events_series.append(s)
         final_label = self.label_class(
             identifier=self.label_id,
             start=start * self.sampling_rate_hz,
             end=end * self.sampling_rate_hz,
             parent=self.label_parent,
-            events=events_series,
+            events=pd.concat(events_series) if events_series else None,
         )
         if self.label_class.descriptions:
             # If it is an activity label, we need to select the activity type
-            final_label.edit_label_description()
+            final_label.description = edit_label_description(
+                descriptions=final_label.descriptions, parent=final_label.parent.parent
+            )
         return final_label
 
 
 class SynchronizationLabel(BaseRegionLabel):
     def __init__(self, start, end, parent=None):
         super().__init__(start=start, end=end, parent=parent)
```

### Comparing `mad_gui-1.0.1a1/mad_gui/plot_tools/plots/base_mode_handler.py` & `mad_gui-1.0.2/mad_gui/plot_tools/plots/base_mode_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from typing import TYPE_CHECKING
+
 import pyqtgraph as pg
 from PySide2.QtGui import QCursor
 from PySide2.QtWidgets import QApplication
 
-from mad_gui.plot_tools.plots.base_plot import BasePlot
+if TYPE_CHECKING:
+    from mad_gui.plot_tools.plots import SensorPlot
 
 
 class BaseModeHandler:
     mode: str
 
-    def __init__(self, plot: BasePlot):
+    def __init__(self, plot: "SensorPlot"):
         self.plot = plot
         # This makes sure that the correct plot has focus when entering a new mode and can accept keyboard inputs
         # TODO: Should this be handled here on an application level?
         pos = QCursor.pos()
         active_widget = QApplication.widgetAt(pos)
         if active_widget:
             active_widget.setFocus()
```

### Comparing `mad_gui-1.0.1a1/mad_gui/plot_tools/plots/base_plot.py` & `mad_gui-1.0.2/mad_gui/plot_tools/plots/base_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,43 +51,43 @@
         #    return
         # df = self.plot_data.annotations["events"].data
         # for _, event in df.iterrows():
         #    pos = self.snap_to_sample(event.pos / self.plot_data.sampling_rate_hz)
         #    self.addItem(BaseEventLabel(pos=pos, span=(event.min_height, event.max_height), parent=self))
         if event_classes is None:
             return
-        event_ranges = pd.DataFrame()
+        event_ranges = []
         for event_class in event_classes:
             if event_class.name not in self.plot_data.annotations.keys():
                 self.plot_data.annotations[event_class.name] = AnnotationData()
             self.set_events(event_class, self.plot_data.annotations[event_class.name].data)
 
             event_range = pd.DataFrame(
                 index=[event_class.name],
                 data=[[event_class.min_height, event_class.max_height]],
                 columns=["min_height", "max_height"],
             )
-            event_ranges = event_ranges.append(event_range)
-        self.event_ranges = event_ranges
+            event_ranges.append(event_range)
+        self.event_ranges = pd.concat(event_ranges)
 
     def _initialize_labels(self, labels: List):
-        label_ranges = pd.DataFrame()
+        label_ranges = []
 
         for label_class in labels:
             if hasattr(self.plot_data, "annotations"):
                 self._ensure_annotations_available(label_class)
                 self.set_labels(label_class, self.plot_data.annotations[label_class.name].data)
 
             label_range = pd.DataFrame(
                 index=[label_class.name],
                 data=[[label_class.min_height, label_class.max_height]],
                 columns=["min_height", "max_height"],
             )
-            label_ranges = label_ranges.append(label_range)
-        self.label_ranges = label_ranges
+            label_ranges.append(label_range)
+        self.label_ranges = pd.concat(label_ranges)
 
     def _ensure_annotations_available(self, label_class: Union[BaseRegionLabel, BaseEventLabel]):
         if label_class.name not in self.plot_data.annotations.keys():
             self.plot_data.annotations[label_class.name] = AnnotationData()
 
     @Slot(BaseEventLabel, pd.DataFrame)
     def set_events(self, label_class: Type[BaseEventLabel], df: pd.DataFrame):
@@ -134,15 +134,15 @@
                     self.addItem(event)
 
     @staticmethod
     def _enforce_columns(activity: pd.Series, necessary_columns: List) -> pd.Series:
         # make sure all required fields are available
         for parameter in necessary_columns:
             if parameter not in activity.index:
-                activity = activity.append(pd.Series(data=[None], index=[parameter]))
+                activity = pd.concat([activity, pd.Series(data=[None], index=[parameter])])
         return activity
 
     def set_title(self, title: str):
         """Set the title, which will be shown centered on the top of the plot.
 
         Parameters
         ----------
```

### Comparing `mad_gui-1.0.1a1/mad_gui/plot_tools/plots/sensor_plot.py` & `mad_gui-1.0.2/mad_gui/plot_tools/plots/sensor_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,18 +339,17 @@
     def delete_item(self, item: QObject):
         if self.event_labels:
             for event in self.event_labels.values():
                 self.parent.removeItem(event)
         self.removeItem(item)
 
     def keyPressEvent(self, ev):  # noqa
-        # Camelcase method overwrites qt method
-        self.mode_handler.handle_key_press(ev)
-        # This is important! As it will forward unhandled events to the parent!
-        super().keyPressEvent(ev)
+        if not self.mode_handler.handle_key_press(ev):
+            # This is important! As it will forward unhandled events to the parent!
+            super().keyPressEvent(ev)
 
     def mousePressEvent(self, ev):  # noqa
         # Camelcase method overwrites qt method
         self.mode_handler.handle_mouse_click(ev)
 
     def mouseMoveEvent(self, ev):  # noqa
         # Camelcase method overwrites qt method
```

### Comparing `mad_gui-1.0.1a1/mad_gui/plot_tools/plots/sensor_plot_mode_handler.py` & `mad_gui-1.0.2/mad_gui/plot_tools/plots/sensor_plot_mode_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from __future__ import annotations
 
-from pyqtgraph import InfiniteLine, mkPen
+from typing import Optional
+
 from PySide2.QtCore import QEvent, Qt
 from PySide2.QtGui import QMouseEvent
+from pyqtgraph import InfiniteLine, mkPen
 
-from mad_gui.components.dialogs import NestedLabelSelectDialog
 from mad_gui.components.dialogs.user_information import UserInformation
 from mad_gui.config import Config
 from mad_gui.plot_tools.labels import PartialLabel
-from mad_gui.plot_tools.labels.base_label import BaseEventLabel, BaseRegionLabel, InvalidStartEnd, NoLabelSelected
+from mad_gui.plot_tools.labels.base_label import (
+    BaseEventLabel,
+    BaseRegionLabel,
+    InvalidStartEnd,
+    NoLabelSelected,
+    edit_label_description,
+)
 from mad_gui.plot_tools.plots.base_mode_handler import BaseModeHandler
-from typing import Optional
 
 
 class AddModeHandler(BaseModeHandler):
     mode = "add"
     _partial_label: Optional[PartialLabel] = None
     _potential_start: Optional[InfiniteLine] = None
 
@@ -61,15 +67,22 @@
                 Qt.MouseButton.LeftButton,
                 ev.modifiers(),
                 Qt.MouseEventSource.MouseEventSynthesizedByApplication,
             )
             self.handle_mouse_click(e, pos=local)
             ev.accept()
             e.accept()
-        ev.accept()
+            return True
+        if ev.key() == Qt.Key_Escape:
+            ev.accept()
+            if self._partial_label is not None:
+                self._clear_partial_label()
+                # This indicates that the event will not probagate further
+                return True
+        return False
 
     def handle_mouse_movement(self, ev):
         if not self._active:
             return
         if self._partial_label is None or not self.plot.inside_plot_range(self.plot.get_mouse_pos_from_event(ev)):
             self._reposition_potential_start(ev)
             super(AddModeHandler, self).handle_mouse_movement(ev)  # pylint: disable=super-with-arguments
@@ -81,15 +94,21 @@
     def deactivate(self):
         self._active = False
         self._clear_partial_label()
 
     def _add_event_to_region(self, position: float):
         # self._partial_label
         label_class = self.plot.inside_label_range(position)
-        description = NestedLabelSelectDialog(parent=self.plot.parent.parent).get_label(label_class.event_descriptions)
+        try:
+            description = edit_label_description(
+                descriptions=label_class.event_descriptions, parent=self.plot.parent.parent
+            )
+        except NoLabelSelected:
+            # If people press cancel we do nothing
+            return
         new_event = BaseEventLabel(
             parent=self.plot,
             pos=position * self.plot.plot_data.sampling_rate_hz,
             min_height=label_class.min_height,
             max_height=label_class.max_height,
             description=description,
         )
@@ -100,23 +119,26 @@
         plot = self.plot
         if self._partial_label:
             self._add_event_to_region(pos)
             return
         event_class = plot.inside_event_range(pos)
         if not event_class:
             return
+        try:
+            description = edit_label_description(descriptions=event_class.descriptions, parent=self.plot.parent)
+        except NoLabelSelected:
+            # If people press cancel we do nothing
+            return
         if getattr(event_class, "snap_to_min", False):
             position = self.plot.snap_to_min(pos.x())
         elif getattr(event_class, "snap_to_max", False):
             position = self.plot.snap_to_max(pos.x())
         else:
             position = self.plot.snap_to_sample(pos.x())
 
-        description = NestedLabelSelectDialog(parent=self.plot.parent).get_label(event_class.descriptions)
-
         new_event = event_class(
             parent=self.plot,
             pos=position * self.plot.plot_data.sampling_rate_hz,
             min_height=event_class.min_height,
             max_height=event_class.max_height,
             description=description,
         )
@@ -137,25 +159,27 @@
         # TODO: This might be a dumb idea, as this will delete your partial label, if you click in the wrong region
         self._clear_partial_label()
         self._start_new_label(pos)
 
     def _start_new_label(self, pos):
         plot = self.plot
         label_class = self.plot.inside_label_range(pos)
-        if getattr(label_class, "snap_to_min", False) and getattr(label_class, "snap_to_max", False):
+        post_process = plot.snap_to_sample
+
+        snap_to_min = getattr(label_class, "snap_to_min", False)
+        snap_to_max = getattr(label_class, "snap_to_max", False)
+        if snap_to_min and snap_to_max:
             UserInformation.inform(
                 f"The class {label_class} is configured to snap to minimum AND maximum. Please "
                 f"only set one of those to attributes to `True`. Snapping is deactivated for now."
             )
-        elif getattr(label_class, "snap_to_min", False):
+        elif snap_to_min:
             post_process = plot.snap_to_min
-        elif getattr(label_class, "snap_to_max", False):
+        elif snap_to_max:
             post_process = plot.snap_to_max
-        else:
-            post_process = plot.snap_to_sample
 
         if self._partial_label:
             self._clear_partial_label()
         self._partial_label = PartialLabel(
             raw_start=pos.x(),
             sampling_rate_hz=plot.plot_data.sampling_rate_hz,
             label_class=label_class,
@@ -207,16 +231,16 @@
             self._potential_start = InfiniteLine(snapped_pos, pen=mkPen(255, 0, 255, 150, width=2, style=Qt.DashLine))
             self._potential_start.span = (
                 event_class.min_height,
                 event_class.max_height,
             )
             self.plot.addItem(self._potential_start)
 
-    def _clear_partial_label(self):
-        if self._potential_start is not None:
+    def _clear_partial_label(self, labels_only=False):
+        if labels_only is not True and self._potential_start is not None:
             self.plot.delete_item(self._potential_start)
             self._potential_start = None
         if self._partial_label is not None:
             for event in self._partial_label.events:
                 self.plot.delete_item(event)
             self.plot.delete_item(self._partial_label)
             self._partial_label = None
```

### Comparing `mad_gui-1.0.1a1/mad_gui/plot_tools/plots/video_plot.py` & `mad_gui-1.0.2/mad_gui/plot_tools/plots/video_plot.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/plot_tools/plots/video_plot_mode_handler.py` & `mad_gui-1.0.2/mad_gui/plot_tools/plots/video_plot_mode_handler.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/plugins/__init__.py` & `mad_gui-1.0.2/mad_gui/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/plugins/base.py` & `mad_gui-1.0.2/mad_gui/plugins/base.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/plugins/example.py` & `mad_gui-1.0.2/mad_gui/plugins/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 from PySide2.QtWidgets import QFileDialog
 
 from mad_gui.components.dialogs import UserInformation
 from mad_gui.models import GlobalData
 from mad_gui.models.local import PlotData
 from mad_gui.plot_tools.labels import BaseRegionLabel, BaseEventLabel
 from mad_gui.plugins.base import BaseAlgorithm, BaseExporter, BaseImporter
-from typing import Dict
-
 from mad_gui.state_keeper import StateKeeper
+from typing import Dict
 
 
 class ActivityLabel(BaseRegionLabel):
     min_height = 0.8
     max_height = 1
     name = "Activity"
     descriptions = {"Jump": None, "Walk": ["Slow", "Normal", "Fast"]}
@@ -27,14 +26,15 @@
     max_height = 1
     name = "Peak"
     descriptions = {"Positive peak": None, "Negative peak": None}
     snap_to_min = False
 
 
 class Stride(BaseRegionLabel):
+    name = "Stride"
     min_height = 0
     max_height = 0.75
 
 
 class ExampleImporter(BaseImporter):
     """An exemplary importer.
```

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/channel_selector.ui` & `mad_gui-1.0.2/mad_gui/qt_designer/channel_selector.ui`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/algorithm.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/algorithm.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/burger.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/burger.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/camera.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/camera.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/camera_light.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/camera_light.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/export.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/export.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/icon.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/icon.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/label.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/label.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/logo_mad_man.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/logo_mad_man.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/open.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/open.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/reload.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/reload.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/images/save.png` & `mad_gui-1.0.2/mad_gui/qt_designer/images/save.png`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/load.ui` & `mad_gui-1.0.2/mad_gui/qt_designer/load.ui`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/main.ui` & `mad_gui-1.0.2/mad_gui/qt_designer/main.ui`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/palette_btn.xml` & `mad_gui-1.0.2/mad_gui/qt_designer/palette_btn.xml`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/palette_window.xml` & `mad_gui-1.0.2/mad_gui/qt_designer/palette_window.xml`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/plugin_selection.ui` & `mad_gui-1.0.2/mad_gui/qt_designer/plugin_selection.ui`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/ui_video.py` & `mad_gui-1.0.2/mad_gui/qt_designer/ui_video.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/window_buttons.qrc` & `mad_gui-1.0.2/mad_gui/qt_designer/window_buttons.qrc`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/qt_designer/window_buttons_rc.py` & `mad_gui-1.0.2/mad_gui/qt_designer/window_buttons_rc.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/start_gui.py` & `mad_gui-1.0.2/mad_gui/start_gui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import sys
 from pathlib import Path
 
+import pyqtgraph
 from PySide2.QtWidgets import QApplication
 
 from mad_gui.config import BaseSettings, BaseTheme
 from mad_gui.plot_tools.labels import BaseEventLabel, BaseRegionLabel
 from mad_gui.plugins.base import BasePlugin
 from mad_gui.plugins.example import (
     EnergyCalculator,
@@ -28,14 +29,15 @@
         EnergyCalculator,
         ExampleExporter,
     ),
     labels: Optional[Sequence[BaseRegionLabel]] = (ActivityLabel, Stride),
     events: Optional[Sequence[BaseEventLabel]] = (MyEvent,),
     settings: Optional[Type[BaseSettings]] = BaseSettings,
     theme: Optional[Type[BaseTheme]] = BaseTheme,
+    use_opengl: bool = True,
 ):
     """Use this function to start the GUI and pass your plugins, like importers and algorithms to it.
 
     Please look at the `See Also` section below, to learn more about how to create objects of the classes you can
     pass to this function.
 
     Parameters
@@ -50,18 +52,23 @@
         :class:`~mad_gui.plugins.BaseAlgorithm`.
     labels
         The region labels you want to use. They inherit from :class:`~mad_gui.plot_tools.labels.BaseRegionLabel`.
     settings
         Change some settings like the snap range, if you set your label's `snap_to_min` or `snap_to_max` to `True`
     theme
         Change the two main colors (light and dark) of the GUI using this
+    use_opengl
+        If you want to use OpenGL for the plots, set this to `True`.
+        On some operating systems, this makes zooming and scrolling much smoother.
+        However, under Linux this can cause degraded performance, so you can set it to `False` there.
 
 
     """
     # Create the Qt Application
+    pyqtgraph.setConfigOptions(useOpenGL=use_opengl, useNumba=True)
     app = QApplication(sys.argv)
     form = MainWindow(
         parent=app, data_dir=data_dir, settings=settings, theme=theme, plugins=plugins, labels=labels, events=events
     )
     form.show()
 
     sys.exit(app.exec_())
```

### Comparing `mad_gui-1.0.1a1/mad_gui/state_keeper.py` & `mad_gui-1.0.2/mad_gui/state_keeper.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/utils/helper.py` & `mad_gui-1.0.2/mad_gui/utils/helper.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/utils/model_base.py` & `mad_gui-1.0.2/mad_gui/utils/model_base.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/windows/__init__.py` & `mad_gui-1.0.2/mad_gui/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/mad_gui/windows/main.py` & `mad_gui-1.0.2/mad_gui/windows/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,14 @@
     import pyi_splash  # noqa
 
     pyi_splash.close()
 except ModuleNotFoundError:
     # we only need to import this when we are in a .exe, see pyinstaller docs
     pass
 
-# helps to make plot zooming smooth even when line width >1
-pg.setConfigOption("useOpenGL", True)
-
 # CI can't handle openGL
 if os.environ.get("GITHUB_CI"):
     pg.setConfigOption("useOpenGL", False)
 
 # Make sure that graphs are properly scaled when having multiple screens
 QApplication.setAttribute(Qt.AA_EnableHighDpiScaling)
 os.environ["QT_AUTO_SCREEN_SCALE_FACTOR"] = "1"
@@ -317,17 +314,19 @@
         if getattr(Config.settings, "SENSORS_SYNCHRONIZED", False):
             for plot in self.sensor_plots.values():
                 if plot == main_plot:
                     continue
                 plot.sync_info = main_plot.sync_info
         self._link_plots()
 
+        all_sync = []
         for plot_name, plot in self.sensor_plots.items():
-            sync = pd.concat([sync, pd.DataFrame(data=plot.sync_info, columns=[plot_name + "_sample"])], axis=1)
-        sync = pd.concat([sync, pd.DataFrame(data=self.video_plot.sync_info, columns=["video_ms"])], axis=1)
+            all_sync.append(pd.DataFrame(data=plot.sync_info, columns=[plot_name + "_sample"]))
+        all_sync.append(pd.DataFrame(data=self.video_plot.sync_info, columns=["video_ms"]))
+        sync = pd.concat(all_sync, axis=1)
         self.VideoWindow.set_sync(self.video_plot.sync_info["start"], self.video_plot.sync_info["end"])
         file_name, _ = QFileDialog.getSaveFileName(self, "Save Synchronization File", filter="*.xlsx")
         if file_name is None:
             return
         sync.to_excel(file_name)
         for plot in self.sensor_plots.values():
             plot.adapt_to_opening_video_window()
```

### Comparing `mad_gui-1.0.1a1/mad_gui/windows/video_window.py` & `mad_gui-1.0.2/mad_gui/windows/video_window.py`

 * *Files identical despite different names*

### Comparing `mad_gui-1.0.1a1/pyproject.toml` & `mad_gui-1.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mad_gui"
-version = "1.0.1-a1"
+version = "1.0.2"
 description = "Python GUI for annotating and processing time series data."
 authors = [
     "Malte Ollenschlaeger <malte.ollenschlaeger@fau.de>",
     "Arne Kuederle <arne.kuederle@fau.de>",
     "Ann-Kristin Seifer <ann-kristin.seifer@fau.de>"
 ]
 readme = "README_pypi.md"
@@ -14,27 +14,25 @@
 	"Intended Audience :: Science/Research",
 	"Topic :: Scientific/Engineering",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
-# we just initialize empty Dataframes, so we do not specify a verison here
-pandas = "*"  
-pyqtgraph = "0.11.0"
+pandas = ">=1.2"
+pyqtgraph = "0.13.1"
 PySide2 = "5.15.1"
 typing-extensions = "^3.10.0"
 sphinx-qt-documentation = "^0.3"
 python-vlc = "^3.0.16120"
 
 [tool.poetry.dev-dependencies]
 openpyxl = "^3.0.6"
 pytest = "^6.2.2"
 numpy = "^1.19.2"
-pandas = "^1.2.4"
 black = "^22.3.0"
 doit = "^0.33.1"
 isort = "4.2.5"
 pytest-cov = "^2.11.1"
 pytest-qt = "^3.3.0"
 Sphinx = "^3.5.1"
 recommonmark = "^0.7.1"
```

### Comparing `mad_gui-1.0.1a1/PKG-INFO` & `mad_gui-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mad-gui
-Version: 1.0.1a1
+Version: 1.0.2
 Summary: Python GUI for annotating and processing time series data.
 Home-page: https://github.com/mad-lab-fau/mad-gui
 Author: Malte Ollenschlaeger
 Author-email: malte.ollenschlaeger@fau.de
 Requires-Python: >=3.8,<3.10
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: PySide2 (==5.15.1)
-Requires-Dist: pandas
-Requires-Dist: pyqtgraph (==0.11.0)
+Requires-Dist: pandas (>=1.2)
+Requires-Dist: pyqtgraph (==0.13.1)
 Requires-Dist: python-vlc (>=3.0.16120,<4.0.0)
 Requires-Dist: sphinx-qt-documentation (>=0.3,<0.4)
 Requires-Dist: typing-extensions (>=3.10.0,<4.0.0)
 Project-URL: Repository, https://github.com/mad-lab-fau/mad-gui
 Description-Content-Type: text/markdown
 
 # MaD GUI
```

