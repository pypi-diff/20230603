# Comparing `tmp/PySide2-Fluent-Widgets-0.9.3.tar.gz` & `tmp/PySide2-Fluent-Widgets-0.9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Fluent-Widgets-0.9.3.tar", last modified: Sat Jun  3 16:30:43 2023, max compression
+gzip compressed data, was "dist\PySide2-Fluent-Widgets-0.9.3.1.tar", last modified: Sat Jun  3 16:32:44 2023, max compression
```

## Comparing `PySide2-Fluent-Widgets-0.9.3.tar` & `PySide2-Fluent-Widgets-0.9.3.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:43.137255 PySide2-Fluent-Widgets-0.9.3/
--rw-rw-rw-   0        0        0    35821 2023-06-03 16:03:49.000000 PySide2-Fluent-Widgets-0.9.3/LICENSE
--rw-rw-rw-   0        0        0     4191 2023-06-03 16:30:43.136255 PySide2-Fluent-Widgets-0.9.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:42.940538 PySide2-Fluent-Widgets-0.9.3/PySide2_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4191 2023-06-03 16:30:42.000000 PySide2-Fluent-Widgets-0.9.3/PySide2_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3512 2023-06-03 16:30:42.000000 PySide2-Fluent-Widgets-0.9.3/PySide2_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 16:30:42.000000 PySide2-Fluent-Widgets-0.9.3/PySide2_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-06-03 16:30:42.000000 PySide2-Fluent-Widgets-0.9.3/PySide2_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-03 16:30:42.000000 PySide2-Fluent-Widgets-0.9.3/PySide2_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3381 2023-06-03 16:23:43.000000 PySide2-Fluent-Widgets-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:42.942543 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/
--rw-rw-rw-   0        0        0      501 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:42.947788 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  5168843 2023-06-03 16:25:34.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:42.995797 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      513 2023-05-23 16:16:16.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     1998 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10580 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0    18431 2023-05-19 15:03:57.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/deprecation.py
--rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      612 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0     8851 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4785 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-04-23 05:13:06.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0     4865 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7114 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      454 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:42.998642 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:43.013389 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-05-29 03:44:17.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2082 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21118 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7449 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19071 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5781 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:43.027243 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14725 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5269 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11331 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3205 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2492 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:43.039248 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2658 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5437 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1305 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:43.051046 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      381 2023-05-23 16:16:16.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     7536 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    19388 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    12892 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6032 2023-06-03 16:24:34.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/pivot.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:43.069275 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5314 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8029 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6028 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2838 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    13113 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1516 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-06-03 16:30:43.134115 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     1676 2023-06-03 16:03:50.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4596 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    18186 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     1615 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    14317 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7879 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0     1327 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    18492 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0      864 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0     9645 2023-06-03 16:26:19.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3854 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    30745 2023-06-03 16:25:13.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     7494 2023-06-03 16:25:18.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     1875 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2520 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17714 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     5151 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4644 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6335 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5795 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8964 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     8738 2023-06-03 16:25:21.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    10402 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2737 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/tree_view.py
--rw-rw-rw-   0        0        0       42 2023-06-03 16:30:43.138255 PySide2-Fluent-Widgets-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-06-03 16:23:58.000000 PySide2-Fluent-Widgets-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.861051 PySide2-Fluent-Widgets-0.9.3.1/
+-rw-rw-rw-   0        0        0    35821 2023-06-03 16:03:49.000000 PySide2-Fluent-Widgets-0.9.3.1/LICENSE
+-rw-rw-rw-   0        0        0     4193 2023-06-03 16:32:44.860051 PySide2-Fluent-Widgets-0.9.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.681486 PySide2-Fluent-Widgets-0.9.3.1/PySide2_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4193 2023-06-03 16:32:44.000000 PySide2-Fluent-Widgets-0.9.3.1/PySide2_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3512 2023-06-03 16:32:44.000000 PySide2-Fluent-Widgets-0.9.3.1/PySide2_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 16:32:44.000000 PySide2-Fluent-Widgets-0.9.3.1/PySide2_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-03 16:32:44.000000 PySide2-Fluent-Widgets-0.9.3.1/PySide2_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-03 16:32:44.000000 PySide2-Fluent-Widgets-0.9.3.1/PySide2_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3381 2023-06-03 16:23:43.000000 PySide2-Fluent-Widgets-0.9.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.684600 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/
+-rw-rw-rw-   0        0        0      503 2023-06-03 16:32:15.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.688126 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  5168843 2023-06-03 16:25:34.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.732977 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      513 2023-05-23 16:16:16.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10580 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0    18431 2023-05-19 15:03:57.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/deprecation.py
+-rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      612 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0     8851 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4785 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-04-23 05:13:06.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0     4865 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7114 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      454 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.734992 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.748526 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-05-29 03:44:17.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2082 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21118 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7449 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19071 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5781 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.764170 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14725 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5269 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11331 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3205 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2492 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.773697 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5437 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1305 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.786076 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      381 2023-05-23 16:16:16.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     7536 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    19388 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    12892 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6032 2023-06-03 16:24:34.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/pivot.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.802202 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5314 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8029 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6028 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2838 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    13113 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1516 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:32:44.857051 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     1676 2023-06-03 16:03:50.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4596 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    18186 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     1615 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    14317 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7879 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0     1327 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    18492 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0      864 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0     9645 2023-06-03 16:26:19.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3854 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    30745 2023-06-03 16:25:13.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     7494 2023-06-03 16:25:18.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     1875 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2520 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17714 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     5151 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4644 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6335 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5795 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8964 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     8738 2023-06-03 16:25:21.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    10402 2023-06-03 16:23:02.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2737 2023-06-03 16:23:14.000000 PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/tree_view.py
+-rw-rw-rw-   0        0        0       42 2023-06-03 16:32:44.861051 PySide2-Fluent-Widgets-0.9.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1262 2023-06-03 16:32:11.000000 PySide2-Fluent-Widgets-0.9.3.1/setup.py
```

### Comparing `PySide2-Fluent-Widgets-0.9.3/LICENSE` & `PySide2-Fluent-Widgets-0.9.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/PKG-INFO` & `PySide2-Fluent-Widgets-0.9.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Fluent-Widgets
-Version: 0.9.3
+Version: 0.9.3.1
 Summary: A fluent design widgets library based on PySide2
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 0.9.3 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 0.9.3.1 Summary: A
 fluent design widgets library based on PySide2 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2 Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2 Project-URL: Bug Tracker,
 https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyside2 fluent
 widgets Classifier: Programming Language :: Python :: 3 Classifier: License ::
```

### Comparing `PySide2-Fluent-Widgets-0.9.3/PySide2_Fluent_Widgets.egg-info/PKG-INFO` & `PySide2-Fluent-Widgets-0.9.3.1/PySide2_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Fluent-Widgets
-Version: 0.9.3
+Version: 0.9.3.1
 Summary: A fluent design widgets library based on PySide2
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 0.9.3 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 0.9.3.1 Summary: A
 fluent design widgets library based on PySide2 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2 Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2 Project-URL: Bug Tracker,
 https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyside2 fluent
 widgets Classifier: Programming Language :: Python :: 3 Classifier: License ::
```

### Comparing `PySide2-Fluent-Widgets-0.9.3/PySide2_Fluent_Widgets.egg-info/SOURCES.txt` & `PySide2-Fluent-Widgets-0.9.3.1/PySide2_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/README.md` & `PySide2-Fluent-Widgets-0.9.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/_rc/resource.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/__init__.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/animation.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/auto_wrap.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/config.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/deprecation.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/exception_handler.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/font.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/icon.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/image_utils.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/overload.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/router.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/smooth_scroll.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/common/style_sheet.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/calendar_picker.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/calendar_view.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/date_picker.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/picker_base.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/date_time/time_picker.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/color_dialog.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/dialog.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/dialog_box/message_dialog.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/layout/expand_layout.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/layout/flow_layout.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/layout/v_box_layout.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/navigation_interface.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/navigation_panel.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/navigation_widget.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/navigation/pivot.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/__init__.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/expand_setting_card.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/options_setting_card.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/setting_card.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/settings/setting_card_group.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/__init__.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/acrylic_label.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/button.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/check_box.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/combo_box.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/icon_widget.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/info_bar.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/label.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/line_edit.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/list_view.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/menu.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/progress_bar.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/progress_ring.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/scroll_area.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/scroll_bar.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/slider.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/spin_box.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/stacked_widget.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/state_tool_tip.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/switch_button.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/table_view.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/tool_tip.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/qfluentwidgets/components/widgets/tree_view.py` & `PySide2-Fluent-Widgets-0.9.3.1/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-0.9.3/setup.py` & `PySide2-Fluent-Widgets-0.9.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Fluent-Widgets",
-    version="0.9.3",
+    version="0.9.3.1",
     keywords="pyside2 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PySide2",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

