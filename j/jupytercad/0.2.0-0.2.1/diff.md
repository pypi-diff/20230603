# Comparing `tmp/jupytercad-0.2.0.tar.gz` & `tmp/jupytercad-0.2.1.tar.gz`

## Comparing `jupytercad-0.2.0.tar` & `jupytercad-0.2.1.tar`

### file list

```diff
@@ -1,402 +1,708 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupytercad-0.2.0/.eslintignore
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 jupytercad-0.2.0/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupytercad-0.2.0/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupytercad-0.2.0/.prettierrc
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupytercad-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0    18904 2020-02-02 00:00:00.000000 jupytercad-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 jupytercad-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.2.0/RELEASE.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupytercad-0.2.0/install.json
--rw-r--r--   0        0        0   196437 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad-screenshot.png
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad-0.2.0/lerna.json
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 jupytercad-0.2.0/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.0/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupytercad-0.2.0/tsconfig.eslint.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.2.0/tsconfigbase.json
--rw-r--r--   0        0        0   423974 2020-02-02 00:00:00.000000 jupytercad-0.2.0/yarn.lock
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupytercad-0.2.0/etc/jupyter/jupyter_server_config.d/jupytercad.json
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/_version.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/fcstd_ydoc.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/jcad_ydoc.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/cadapp/__init__.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/cadapp/cadapp.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/cadapp/utils.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/cadapp/templates/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/__init__.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/loader.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/base_prop.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_angle.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_bool.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_distance.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_geometrylist.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_length.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_link.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_link_list.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_map.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_partshape.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/property_placement.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/geometry/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/geometry/geom_circle.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/freecad/props/geometry/geom_linesegment.py
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/package.json
--rw-r--r--   0        0        0    52115 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/184.6f76dd957e411be19baa.js
--rw-r--r--   0        0        0    86711 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/213.778b3209dbe7ec5470b6.js
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/268.16c8a4126908b03651f0.js
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/358.45fb46ea24bb44ba7fa9.js
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js
--rw-r--r--   0        0        0    59793 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/422.39a95e19d3a414516796.js
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js
--rw-r--r--   0        0        0   124214 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/544.5c918f69ee5ea6e28e28.js
--rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/643.850e055919134443b4fa.js
--rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js.LICENSE.txt
--rw-r--r--   0        0        0    12563 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/711.2093084af91b1879c5ac.js
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js
--rw-r--r--   0        0        0   183517 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js
--rw-r--r--   0        0        0   116747 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/733.89a6a4e0561966230286.js
--rw-r--r--   0        0        0    31683 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js.LICENSE.txt
--rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/816.00326e9e5f2436d0d67f.js
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js
--rw-r--r--   0        0        0   254953 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/842.116bb3340768f53ea709.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/842.116bb3340768f53ea709.js.LICENSE.txt
--rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js
--rw-r--r--   0        0        0   623572 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/955.a084e75defa008fca238.js
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/955.a084e75defa008fca238.js.LICENSE.txt
--rw-r--r--   0        0        0   114029 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js
--rw-r--r--   0        0        0  5065593 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/jupytercad.opencascade.wasm
--rw-r--r--   0        0        0    13050 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/remoteEntry.3d94847557dd157537a5.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/style.js
--rw-r--r--   0        0        0    67994 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/__init__.py
--rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/cad_document.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/utils.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/y_connector.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/box.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/cone.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/cut.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/cylinder.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/extrusion.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/fuse.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/geomCircle.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/geomLineSegment.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/intersection.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/jcad.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/placement.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/sketch.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/sphere.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.2.0/jupytercad/notebook/objects/_schema/torus.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 jupytercad-0.2.0/scripts/bump-version.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/package.json
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/tsconfig.json
--rw-r--r--   0        0        0    98468 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/webpack.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/bootstrap.d.ts
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/bootstrap.js
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/main.d.ts
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/main.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/sharedscope.d.ts
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/sharedscope.js
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/style.js
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/app.d.ts
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/app.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/shell.d.ts
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/shell.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/browser/index.d.ts
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/browser/index.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/launcher/index.d.ts
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/launcher/index.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/index.d.ts
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/index.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.d.ts
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.js
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/titleWidget.d.ts
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/titleWidget.js
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.d.ts
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.js
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/paths/index.d.ts
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/paths/index.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/bootstrap.d.ts
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/bootstrap.js
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/main.d.ts
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/main.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/sharedscope.d.ts
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/sharedscope.js
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/app.d.ts
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/app.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/shell.d.ts
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/shell.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/browser/index.d.ts
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/browser/index.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/launcher/index.d.ts
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/launcher/index.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/index.d.ts
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.d.ts
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.js
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/titleWidget.d.ts
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/titleWidget.js
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.d.ts
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.js
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/paths/index.d.ts
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/paths/index.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/bootstrap.ts
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/main.ts
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/sharedscope.ts
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/app/app.ts
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/app/shell.ts
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/browser/index.ts
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/launcher/index.ts
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/mainmenu/menuWidget.ts
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/mainmenu/titleWidget.tsx
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/mainmenu/userWidget.tsx
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/paths/index.ts
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-app/style/index.js
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/extension.webpack.config.js
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/package.json
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/schema.js
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/tsconfig.json
--rw-r--r--   0        0        0   187724 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/tsconfig.worker.json
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/worker.webpack.config.js
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/commands.d.ts
--rw-r--r--   0        0        0    23175 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/commands.js
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/factory.d.ts
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/factory.js
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/formdialog.d.ts
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/formdialog.js
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/index.d.ts
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/index.js
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/mainview.d.ts
--rw-r--r--   0        0        0    37791 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/mainview.js
--rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/model.d.ts
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/model.js
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/token.d.ts
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/token.js
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/tools.d.ts
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/tools.js
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/types.d.ts
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/types.js
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/widget.d.ts
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/widget.js
--rw-r--r--   0        0        0    86564 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker.js
--rw-r--r--   0        0        0    26960 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/_interface/forms.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/message.d.ts
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/message.js
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/model.d.ts
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/model.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/view.d.ts
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/view.js
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/fcplugin/modelfactory.js
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/fcplugin/plugins.d.ts
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/fcplugin/plugins.js
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/jcadplugin/plugins.d.ts
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/jcadplugin/plugins.js
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/index.d.ts
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/index.js
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/model.js
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/token.js
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/view.js
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/annotations.d.ts
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/annotations.js
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/formbuilder.js
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/header.d.ts
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/header.js
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/leftpanel.js
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/model.d.ts
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/model.js
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/objectproperties.d.ts
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/objectproperties.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/objecttree.d.ts
--rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/objecttree.js
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/rightpanel.d.ts
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/rightpanel.js
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/box.json
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/cone.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/cut.json
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/cylinder.json
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/extrusion.json
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/fuse.json
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/geomCircle.json
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/geomLineSegment.json
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/intersection.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/jcad.json
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/placement.json
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/sketch.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/sphere.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/torus.json
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/helper.d.ts
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/helper.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/panzoom.d.ts
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/panzoom.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketcherdialog.d.ts
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketchermodel.js
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts
--rw-r--r--   0        0        0    19357 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/types.d.ts
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/types.js
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/elements/circle.d.ts
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/elements/circle.js
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/elements/line.d.ts
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/elements/line.js
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/elements/point.d.ts
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/elements/point.js
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/toolbar/widget.d.ts
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/toolbar/widget.js
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/actions.d.ts
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/actions.js
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/occapi.d.ts
--rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/occapi.js
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/occparser.d.ts
--rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/occparser.js
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/operatorcache.d.ts
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/operatorcache.js
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/types.d.ts
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/types.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/utils.d.ts
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/utils.js
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/worker.d.ts
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/worker.js
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/geometry/geomCircle.d.ts
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.d.ts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.js
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/commands.ts
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/factory.ts
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/formdialog.tsx
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/index.ts
--rw-r--r--   0        0        0    34821 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/mainview.tsx
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/model.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/svg.d.ts
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/token.ts
--rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/tools.ts
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/types.ts
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/widget.tsx
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/box.d.ts
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/cone.d.ts
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/cut.d.ts
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/cylinder.d.ts
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/extrusion.d.ts
--rw-r--r--   0        0        0    19613 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/forms.json
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/fuse.d.ts
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/geomCircle.d.ts
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/intersection.d.ts
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/jcad.d.ts
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/placement.d.ts
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/sketch.d.ts
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/sphere.d.ts
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/torus.d.ts
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/annotation/message.tsx
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/annotation/model.ts
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/annotation/view.tsx
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/fcplugin/modelfactory.ts
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/fcplugin/plugins.ts
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/jcadplugin/plugins.ts
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/index.ts
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/model.ts
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/token.ts
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/view.ts
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/annotations.tsx
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/formbuilder.tsx
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/header.tsx
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/leftpanel.tsx
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/model.ts
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/objectproperties.tsx
--rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/objecttree.tsx
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/rightpanel.tsx
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/box.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/cone.json
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/cut.json
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/cylinder.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/extrusion.json
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/fuse.json
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/geomCircle.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/geomLineSegment.json
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/intersection.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/jcad.json
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/placement.json
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/sketch.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/sphere.json
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/schema/torus.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/helper.tsx
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/panzoom.ts
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/sketchermodel.ts
--rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/types.ts
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/elements/circle.ts
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/elements/line.ts
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/elements/point.ts
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/toolbar/widget.tsx
--rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/worker/actions.ts
--rw-r--r--   0        0        0    10134 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/worker/occapi.ts
--rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/worker/occparser.ts
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/worker/operatorcache.ts
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/worker/types.ts
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/worker/utils.ts
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/worker/worker.ts
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/src/worker/geometry/geomLineSegment.ts
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/index.js
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/axes.svg
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/box.svg
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/cone.svg
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/cut.svg
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/cylinder.svg
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/extrusion.svg
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/intersection.svg
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/jvcontrol.svg
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/minimize.svg
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/sphere.svg
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/torus.svg
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/union.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/visibility.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-extension/style/icon/visibilityOff.svg
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-opencascade/build.yml
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-opencascade/build_opencascade.js
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-opencascade/package.json
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-opencascade/lib/build.yml
--rw-r--r--   0        0        0   129654 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts
--rw-r--r--   0        0        0   123823 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.version
--rwxr-xr-x   0        0        0  5065593 2020-02-02 00:00:00.000000 jupytercad-0.2.0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.0/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupytercad-0.2.0/LICENSE
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 jupytercad-0.2.0/README.md
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 jupytercad-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 jupytercad-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.1/.eslintignore
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 jupytercad-0.2.1/.eslintrc.js
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 jupytercad-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupytercad-0.2.1/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupytercad-0.2.1/.prettierrc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupytercad-0.2.1/.yarnrc.yml
+-rw-r--r--   0        0        0    20726 2020-02-02 00:00:00.000000 jupytercad-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 jupytercad-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.2.1/RELEASE.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupytercad-0.2.1/install.json
+-rw-r--r--   0        0        0   196437 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad-screenshot.png
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad-0.2.1/lerna.json
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 jupytercad-0.2.1/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.1/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupytercad-0.2.1/tsconfig.eslint.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.2.1/tsconfigbase.json
+-rw-r--r--   0        0        0   423942 2020-02-02 00:00:00.000000 jupytercad-0.2.1/yarn.lock
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupytercad-0.2.1/etc/jupyter/jupyter_server_config.d/jupytercad.json
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/_version.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/fcstd_ydoc.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/jcad_ydoc.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/cadapp.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/utils.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/application-extension/package.json.orig
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/application-extension/property-inspector.json
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/application-extension/top-bar.json
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/notification.json
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/package.json.orig
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/sanitizer.json
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/utilityCommands.json
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/workspaces.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/codemirror-extension/package.json.orig
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/codemirror-extension/plugin.json
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/package.json.orig
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/plugin.json
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/package.json.orig
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/widget.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/package.json.orig
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/plugin.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/package.json.orig
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/plugin.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/package.json.orig
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/plugin.json
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/103.app.js
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1053.app.js
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1058.app.js
+-rw-r--r--   0        0        0   302401 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1072.app.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1072.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1152.app.js
+-rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1208.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1210.app.js
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1222.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1227.app.js
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1278.app.js
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1286.app.js
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/13.app.js
+-rw-r--r--   0        0        0    20577 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1320.app.js
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1322.app.js
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1377.app.js
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1403.app.js
+-rw-r--r--   0        0        0     9838 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/15.app.js
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/151.app.js
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1567.app.js
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1580.app.js
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1581.app.js
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1623.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1729.app.js
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1746.app.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1770.app.js
+-rw-r--r--   0        0        0    60948 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1880.app.js
+-rw-r--r--   0        0        0     9036 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1882.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/1935.app.js
+-rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2033.app.js
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2042.app.js
+-rw-r--r--   0        0        0    24578 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2075.app.js
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2100.app.js
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2106.app.js
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2185.app.js
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2194.app.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2266.app.js
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2284.app.js
+-rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/23.app.js
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/231.app.js
+-rw-r--r--   0        0        0    77242 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2318.app.js
+-rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2488.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2502.app.js
+-rw-r--r--   0        0        0    39462 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2553.app.js
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2563.app.js
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2628.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2667.app.js
+-rw-r--r--   0        0        0    13343 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2687.app.js
+-rw-r--r--   0        0        0    25924 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/274.app.js
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/275.app.js
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2784.app.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2784.app.js.LICENSE.txt
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2805.app.js
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/288.app.js
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/2970.app.js
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3007.app.js
+-rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3093.app.js
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3159.app.js
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3191.app.js
+-rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3192.app.js
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3206.app.js
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3211.app.js
+-rw-r--r--   0        0        0   432933 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/330.app.js
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3312.app.js
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3316.app.js
+-rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3324.app.js
+-rw-r--r--   0        0        0   171985 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3326.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3330.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3397.app.js
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3466.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3499.app.js
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3500.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/351.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3540.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3542.app.js
+-rw-r--r--   0        0        0   169327 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/358.app.js
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/360.app.js
+-rw-r--r--   0        0        0  1020115 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3656.app.js
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3656.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3726.app.js
+-rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/373c04fd2418f5c77eea.eot
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3811.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3851.app.js
+-rw-r--r--   0        0        0    61590 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3855.app.js
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/386.app.js
+-rw-r--r--   0        0        0    46084 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3872.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3880.app.js
+-rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/3f6d3488cf65374f6f67.woff
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4024.app.js
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4040.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4065.app.js
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4073.app.js
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4123.app.js
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4282.app.js
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4283.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4299.app.js
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4351.app.js
+-rw-r--r--   0        0        0    16452 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4359.app.js
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4391.app.js
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4403.app.js
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4462.app.js
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4476.app.js
+-rw-r--r--   0        0        0   143645 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/450.app.js
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4608.app.js
+-rw-r--r--   0        0        0    18653 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4651.app.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4651.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4654.app.js
+-rw-r--r--   0        0        0    23079 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4679.app.js
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4702.app.js
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4718.app.js
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4808.app.js
+-rw-r--r--   0        0        0    15011 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/484.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4874.app.js
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4878.app.js
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4935.app.js
+-rw-r--r--   0        0        0    27298 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4965.app.js
+-rw-r--r--   0        0        0    69298 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4973.app.js
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4973.app.js.LICENSE.txt
+-rw-r--r--   0        0        0    22107 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/4982.app.js
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5002.app.js
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5024.app.js
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/504.app.js
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5101.app.js
+-rw-r--r--   0        0        0    94906 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5148.app.js
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5172.app.js
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5176.app.js
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5223.app.js
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5225.app.js
+-rw-r--r--   0        0        0    86931 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5231.app.js
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5263.app.js
+-rw-r--r--   0        0        0   101929 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5340.app.js
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5393.app.js
+-rw-r--r--   0        0        0   180936 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5430.app.js
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5433.app.js
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5445.app.js
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5513.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5514.app.js
+-rw-r--r--   0        0        0    18861 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5544.app.js
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5556.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/558.app.js
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5681.app.js
+-rw-r--r--   0        0        0    68549 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5708.app.js
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5764.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5817.app.js
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5876.app.js
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5882.app.js
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/5882.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6146.app.js
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6151.app.js
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6186.app.js
+-rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6196.app.js
+-rw-r--r--   0        0        0   179936 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6328.app.js
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6410.app.js
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6483.app.js
+-rw-r--r--   0        0        0    30696 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6510.app.js
+-rw-r--r--   0        0        0    37190 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6645.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6686.app.js
+-rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6770.app.js
+-rw-r--r--   0        0        0    49485 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6778.app.js
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6782.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6808.app.js
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6833.app.js
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6835.app.js
+-rw-r--r--   0        0        0    99172 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6914.app.js
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/6970.app.js
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7058.app.js
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7111.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7127.app.js
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7149.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7174.app.js
+-rw-r--r--   0        0        0    27083 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7233.app.js
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7236.app.js
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7294.app.js
+-rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/730.app.js
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7377.app.js
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7379.app.js
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7424.app.js
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7469.app.js
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7498.app.js
+-rw-r--r--   0        0        0    33625 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7526.app.js
+-rw-r--r--   0        0        0    40106 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7529.app.js
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7600.app.js
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/765.app.js
+-rw-r--r--   0        0        0    22254 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7664.app.js
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7710.app.js
+-rw-r--r--   0        0        0   277483 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/78.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7806.app.js
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7860.app.js
+-rw-r--r--   0        0        0   199353 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7869.app.js
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7882.app.js
+-rw-r--r--   0        0        0    16715 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7884.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7955.app.js
+-rw-r--r--   0        0        0   103425 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/7991.app.js
+-rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/79d088064beb3826054f.eot
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8090.app.js
+-rw-r--r--   0        0        0    47563 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8124.app.js
+-rw-r--r--   0        0        0    54614 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8138.app.js
+-rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/819.app.js
+-rw-r--r--   0        0        0    17084 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8227.app.js
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8307.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8342.app.js
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8409.app.js
+-rw-r--r--   0        0        0    25262 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8423.app.js
+-rw-r--r--   0        0        0    25112 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8441.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8442.app.js
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/846.app.js
+-rw-r--r--   0        0        0    66111 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8466.app.js
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8496.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8518.app.js
+-rw-r--r--   0        0        0    17922 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8561.app.js
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8576.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8615.app.js
+-rw-r--r--   0        0        0    40918 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8640.app.js
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8658.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8662.app.js
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8763.app.js
+-rw-r--r--   0        0        0    39773 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8769.app.js
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8782.app.js
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8803.app.js
+-rw-r--r--   0        0        0   292717 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/882.app.js
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8866.app.js
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8877.app.js
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8914.app.js
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8953.app.js
+-rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/8ea8791754915a898a31.woff2
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9036.app.js
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9060.app.js
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9117.app.js
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9172.app.js
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9304.app.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9308.app.js
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9319.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9369.app.js
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9397.app.js
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9406.app.js
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9472.app.js
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9473.app.js
+-rw-r--r--   0        0        0   253965 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9491.app.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9491.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9513.app.js
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9583.app.js
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9631.app.js
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9636.app.js
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9672.app.js
+-rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9674eb1bd55047179038.svg
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9715.app.js
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9787.app.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9787.app.js.LICENSE.txt
+-rw-r--r--   0        0        0    10153 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9811.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9822.app.js
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9827.app.js
+-rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9834b82ad26e2a37583d.woff2
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9866.app.js
+-rw-r--r--   0        0        0    59178 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9877.app.js
+-rw-r--r--   0        0        0   138733 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9908.app.js
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9908.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9932.app.js
+-rw-r--r--   0        0        0    22523 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9961.app.js
+-rw-r--r--   0        0        0   569460 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9976.app.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/9976.app.js.LICENSE.txt
+-rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/a3b9817780214caf01e8.svg
+-rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/af6397503fcefbd61397.ttf
+-rw-r--r--   0        0        0    29197 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/app.js
+-rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/be0a084962d8066884f7.svg
+-rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/cb9e9e693192413cde2b.woff
+-rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/cda59d6efffa685830fd.ttf
+-rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/e4299464e7b012968eed.eot
+-rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/e42a88444448ac3d6054.woff2
+-rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/e8711bbb871afd8e9dea.ttf
+-rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/static/f9217f66874b0c01cd8c.woff
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/templates/index.html
+-rw-r--r--   0        0        0    17760 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/themes/@jupyterlab/theme-dark-extension/index.js
+-rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/cadapp/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/loader.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/base_prop.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_angle.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_bool.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_distance.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_geometrylist.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_length.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_link.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_link_list.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_map.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_partshape.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/property_placement.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/geometry/__init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/geometry/geom_circle.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/freecad/props/geometry/geom_linesegment.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/package.json
+-rw-r--r--   0        0        0    52115 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/184.6f76dd957e411be19baa.js
+-rw-r--r--   0        0        0    86711 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/213.778b3209dbe7ec5470b6.js
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/268.16c8a4126908b03651f0.js
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/358.45fb46ea24bb44ba7fa9.js
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js
+-rw-r--r--   0        0        0    59793 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/422.39a95e19d3a414516796.js
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js
+-rw-r--r--   0        0        0   124222 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/544.f90bd90ee4b5fdf48162.js
+-rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/643.850e055919134443b4fa.js
+-rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js.LICENSE.txt
+-rw-r--r--   0        0        0    12563 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/711.2093084af91b1879c5ac.js
+-rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js
+-rw-r--r--   0        0        0   183517 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js
+-rw-r--r--   0        0        0   116747 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/733.89a6a4e0561966230286.js
+-rw-r--r--   0        0        0    31683 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js.LICENSE.txt
+-rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/816.00326e9e5f2436d0d67f.js
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js
+-rw-r--r--   0        0        0   254953 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/842.116bb3340768f53ea709.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/842.116bb3340768f53ea709.js.LICENSE.txt
+-rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js
+-rw-r--r--   0        0        0   623572 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/955.a084e75defa008fca238.js
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/955.a084e75defa008fca238.js.LICENSE.txt
+-rw-r--r--   0        0        0   114029 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js
+-rw-r--r--   0        0        0  5065593 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/jupytercad.opencascade.wasm
+-rw-r--r--   0        0        0    13044 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/remoteEntry.e8080149ddd48fae3b49.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/style.js
+-rw-r--r--   0        0        0    67994 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/__init__.py
+-rw-r--r--   0        0        0    22888 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/cad_document.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/utils.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/y_connector.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/box.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/cone.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/cut.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/cylinder.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/extrusion.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/fuse.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/geomCircle.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/geomLineSegment.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/intersection.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/jcad.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/placement.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/sketch.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/sphere.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.2.1/jupytercad/notebook/objects/_schema/torus.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupytercad-0.2.1/scripts/bump-version.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/package.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/tsconfig.json
+-rw-r--r--   0        0        0    98468 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/webpack.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/bootstrap.d.ts
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/bootstrap.js
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/main.d.ts
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/main.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/sharedscope.d.ts
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/sharedscope.js
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/style.js
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/app.d.ts
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/app.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/shell.d.ts
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/shell.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/browser/index.d.ts
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/browser/index.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/launcher/index.d.ts
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/launcher/index.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/index.d.ts
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/index.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.d.ts
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.js
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/titleWidget.d.ts
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/titleWidget.js
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.d.ts
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.js
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/paths/index.d.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/paths/index.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/bootstrap.d.ts
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/bootstrap.js
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/main.d.ts
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/main.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/sharedscope.d.ts
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/sharedscope.js
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/app.d.ts
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/app.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/shell.d.ts
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/shell.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/browser/index.d.ts
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/browser/index.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/launcher/index.d.ts
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/launcher/index.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/index.d.ts
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.d.ts
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.js
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/titleWidget.d.ts
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/titleWidget.js
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.d.ts
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.js
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/paths/index.d.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/paths/index.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/bootstrap.ts
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/main.ts
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/sharedscope.ts
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/app/app.ts
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/app/shell.ts
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/browser/index.ts
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/launcher/index.ts
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/mainmenu/menuWidget.ts
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/mainmenu/titleWidget.tsx
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/mainmenu/userWidget.tsx
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/paths/index.ts
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-app/style/index.js
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/extension.webpack.config.js
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/package.json
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/schema.js
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/tsconfig.json
+-rw-r--r--   0        0        0   187724 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/tsconfig.worker.json
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/worker.webpack.config.js
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/commands.d.ts
+-rw-r--r--   0        0        0    23175 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/commands.js
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/factory.d.ts
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/factory.js
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/formdialog.d.ts
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/formdialog.js
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/index.d.ts
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/index.js
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/mainview.d.ts
+-rw-r--r--   0        0        0    37791 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/mainview.js
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/model.d.ts
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/model.js
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/token.d.ts
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/token.js
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/tools.d.ts
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/tools.js
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/types.d.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/types.js
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/widget.d.ts
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/widget.js
+-rw-r--r--   0        0        0    86564 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker.js
+-rw-r--r--   0        0        0    26960 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/_interface/forms.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/message.d.ts
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/message.js
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/model.d.ts
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/model.js
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/view.d.ts
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/view.js
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/fcplugin/modelfactory.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/fcplugin/plugins.d.ts
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/fcplugin/plugins.js
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/jcadplugin/plugins.d.ts
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/jcadplugin/plugins.js
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/index.d.ts
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/index.js
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/model.js
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/token.js
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/view.js
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/annotations.d.ts
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/annotations.js
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/formbuilder.js
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/header.d.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/header.js
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/leftpanel.js
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/model.d.ts
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/model.js
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/objectproperties.d.ts
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/objectproperties.js
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/objecttree.d.ts
+-rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/objecttree.js
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/rightpanel.d.ts
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/rightpanel.js
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/box.json
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/cone.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/cut.json
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/cylinder.json
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/extrusion.json
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/fuse.json
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/geomCircle.json
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/geomLineSegment.json
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/intersection.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/jcad.json
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/placement.json
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/sketch.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/sphere.json
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/torus.json
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/helper.d.ts
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/helper.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/panzoom.d.ts
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/panzoom.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketcherdialog.d.ts
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketchermodel.js
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts
+-rw-r--r--   0        0        0    19357 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/types.d.ts
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/types.js
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/elements/circle.d.ts
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/elements/circle.js
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/elements/line.d.ts
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/elements/line.js
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/elements/point.d.ts
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/elements/point.js
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/toolbar/widget.d.ts
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/toolbar/widget.js
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/actions.d.ts
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/actions.js
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/occapi.d.ts
+-rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/occapi.js
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/occparser.d.ts
+-rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/occparser.js
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/operatorcache.d.ts
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/operatorcache.js
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/types.d.ts
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/types.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/utils.d.ts
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/utils.js
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/worker.d.ts
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/worker.js
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/geometry/geomCircle.d.ts
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.d.ts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.js
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/commands.ts
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/factory.ts
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/formdialog.tsx
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/index.ts
+-rw-r--r--   0        0        0    34821 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/mainview.tsx
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/model.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/svg.d.ts
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/token.ts
+-rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/tools.ts
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/types.ts
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/widget.tsx
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/box.d.ts
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/cone.d.ts
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/cut.d.ts
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/cylinder.d.ts
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/extrusion.d.ts
+-rw-r--r--   0        0        0    19613 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/forms.json
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/fuse.d.ts
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/geomCircle.d.ts
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/intersection.d.ts
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/jcad.d.ts
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/placement.d.ts
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/sketch.d.ts
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/sphere.d.ts
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/torus.d.ts
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/annotation/message.tsx
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/annotation/model.ts
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/annotation/view.tsx
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/fcplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/fcplugin/plugins.ts
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/jcadplugin/plugins.ts
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/index.ts
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/model.ts
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/token.ts
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/view.ts
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/annotations.tsx
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/formbuilder.tsx
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/header.tsx
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/leftpanel.tsx
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/model.ts
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/objectproperties.tsx
+-rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/objecttree.tsx
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/rightpanel.tsx
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/box.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/cone.json
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/cut.json
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/cylinder.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/extrusion.json
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/fuse.json
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/geomCircle.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/geomLineSegment.json
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/intersection.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/jcad.json
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/placement.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/sketch.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/sphere.json
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/schema/torus.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/helper.tsx
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/panzoom.ts
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/sketchermodel.ts
+-rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/types.ts
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/elements/circle.ts
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/elements/line.ts
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/elements/point.ts
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/toolbar/widget.tsx
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/worker/actions.ts
+-rw-r--r--   0        0        0    10134 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/worker/occapi.ts
+-rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/worker/occparser.ts
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/worker/operatorcache.ts
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/worker/types.ts
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/worker/utils.ts
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/worker/worker.ts
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/src/worker/geometry/geomLineSegment.ts
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/index.js
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/axes.svg
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/box.svg
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/cone.svg
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/cut.svg
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/cylinder.svg
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/extrusion.svg
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/intersection.svg
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/jvcontrol.svg
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/minimize.svg
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/sphere.svg
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/torus.svg
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/union.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/visibility.svg
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-extension/style/icon/visibilityOff.svg
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-opencascade/build.yml
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-opencascade/build_opencascade.js
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-opencascade/package.json
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-opencascade/lib/build.yml
+-rw-r--r--   0        0        0   129654 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts
+-rw-r--r--   0        0        0   123823 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-opencascade/lib/jupytercad.opencascade.version
+-rwxr-xr-x   0        0        0  5065593 2020-02-02 00:00:00.000000 jupytercad-0.2.1/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupytercad-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 jupytercad-0.2.1/README.md
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 jupytercad-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 jupytercad-0.2.1/PKG-INFO
```

### Comparing `jupytercad-0.2.0/.eslintrc.js` & `jupytercad-0.2.1/.eslintrc.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,14 @@
 module.exports = {
     extends: [
         'eslint:recommended',
         'plugin:@typescript-eslint/eslint-recommended',
         'plugin:@typescript-eslint/recommended',
-        'plugin:prettier/recommended'
+        'plugin:prettier/recommended',
+        'prettier'
     ],
     parser: '@typescript-eslint/parser',
     parserOptions: {
         project: 'tsconfig.eslint.json',
         sourceType: 'module'
     },
     plugins: ['@typescript-eslint'],
```

### Comparing `jupytercad-0.2.0/CHANGELOG.md` & `jupytercad-0.2.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,38 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.2.1
+
+([Full Changelog](https://github.com/QuantStack/jupytercad/compare/v0.2.0...ec0b05cb38d16a1a8fc0a853a53328c4a05542dd))
+
+### Bugs fixed
+
+- Fix missing static files in cad app [#181](https://github.com/QuantStack/jupytercad/pull/181) ([@trungleduc](https://github.com/trungleduc))
+- NPM Package version fix [#173](https://github.com/QuantStack/jupytercad/pull/173) ([@martinRenou](https://github.com/martinRenou))
+
+### Maintenance and upkeep improvements
+
+- Simplify bump version script [#178](https://github.com/QuantStack/jupytercad/pull/178) ([@martinRenou](https://github.com/martinRenou))
+- Fix file paths in Notebook.ipynb [#176](https://github.com/QuantStack/jupytercad/pull/176) ([@davidbrochart](https://github.com/davidbrochart))
+- Add releaser action and pre-commit config [#172](https://github.com/QuantStack/jupytercad/pull/172) ([@trungleduc](https://github.com/trungleduc))
+
+### Documentation improvements
+
+- Add docstrings [#177](https://github.com/QuantStack/jupytercad/pull/177) ([@martinRenou](https://github.com/martinRenou))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/QuantStack/jupytercad/graphs/contributors?from=2023-06-02&to=2023-06-02&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Adavidbrochart+updated%3A2023-06-02..2023-06-02&type=Issues) | [@github-actions](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Agithub-actions+updated%3A2023-06-02..2023-06-02&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3AmartinRenou+updated%3A2023-06-02..2023-06-02&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Atrungleduc+updated%3A2023-06-02..2023-06-02&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.2.0
 
 ([Full Changelog](https://github.com/QuantStack/jupytercad/compare/@jupytercad/jupytercad-app@0.1.0...65c8ba939c9b1f86bf3dbd18f5d2eeb3fb67597e))
 
 ### Enhancements made
 
 - Add backend installation check [#168](https://github.com/QuantStack/jupytercad/pull/168) ([@trungleduc](https://github.com/trungleduc))
@@ -38,16 +65,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/QuantStack/jupytercad/graphs/contributors?from=2023-05-17&to=2023-06-02&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Agithub-actions+updated%3A2023-05-17..2023-06-02&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3AmartinRenou+updated%3A2023-05-17..2023-06-02&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Atrungleduc+updated%3A2023-05-17..2023-06-02&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.0
 
 No merged PRs
 
 ## 0.1.0rc0
 
 No merged PRs
```

### Comparing `jupytercad-0.2.0/CONTRIBUTING.md` & `jupytercad-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/RELEASE.md` & `jupytercad-0.2.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad-screenshot.png` & `jupytercad-0.2.1/jupytercad-screenshot.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/package.json` & `jupytercad-0.2.1/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'scripts'": "{'bump:js:version': 'lerna version --no-push --force-publish --no-git-tag-version "*

 * *              "--yes'}",*

 * * "'version'": "'0.2.1'"}*

```diff
@@ -39,22 +39,23 @@
         "@jupyterlab/services": " ^7.0.0",
         "@lumino/coreutils": "^2.0.0"
     },
     "scripts": {
         "build": "lerna run build",
         "build:prod": "lerna run build:prod",
         "build:test": "lerna run build:test",
+        "bump:js:version": "lerna version --no-push --force-publish --no-git-tag-version --yes",
         "clean": "lerna run clean",
         "clean:all": "lerna run clean:all",
         "eslint": "eslint . --ext .ts,.tsx --cache --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "lint": "jlpm run prettier && jlpm run eslint",
         "lint:check": "jlpm run prettier:check && jlpm run eslint:check",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "prettier --list-different \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "test": "lerna run test"
     },
-    "version": "0.2.0",
+    "version": "0.2.1",
     "workspaces": [
         "packages/*"
     ]
 }
```

### Comparing `jupytercad-0.2.0/tsconfigbase.json` & `jupytercad-0.2.1/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/yarn.lock` & `jupytercad-0.2.1/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -818,15 +818,15 @@
   resolution: "@jupytercad/jupytercad-app@workspace:packages/jupytercad-app"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.3
     "@jupyter/collaboration": ^1.0.0-alpha.7
     "@jupyter/docprovider": ^1.0.0-alpha.8
     "@jupyter/ydoc": ^0.3.4 || ^1.0.2
-    "@jupytercad/jupytercad-extension": ^0.2.0-alpha.0
+    "@jupytercad/jupytercad-extension": ^0.2.1
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/application-extension": ^4.0.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/apputils-extension": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/codemirror": ^4.0.0
     "@jupyterlab/codemirror-extension": ^4.0.0
@@ -867,24 +867,24 @@
     tsc-watch: ^6.0.0
     typescript: ^5
     webpack: ^5.76.3
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupytercad/jupytercad-extension@^0.2.0-alpha.0, @jupytercad/jupytercad-extension@workspace:packages/jupytercad-extension":
+"@jupytercad/jupytercad-extension@^0.2.1, @jupytercad/jupytercad-extension@workspace:packages/jupytercad-extension":
   version: 0.0.0-use.local
   resolution: "@jupytercad/jupytercad-extension@workspace:packages/jupytercad-extension"
   dependencies:
     "@apidevtools/json-schema-ref-parser": ^9.0.9
     "@deathbeds/jupyterlab-rjsf": ^1.1.0
     "@jupyter/collaboration": ^1.0.0-alpha.7
     "@jupyter/docprovider": ^1.0.0-alpha.8
     "@jupyter/ydoc": ^0.3.4 || ^1.0.2
-    "@jupytercad/jupytercad-opencascade": ^0.2.0-alpha.0
+    "@jupytercad/jupytercad-opencascade": ^0.2.1
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/docregistry": ^4.0.0
     "@jupyterlab/filebrowser": ^4.0.0
     "@jupyterlab/launcher": ^4.0.0
@@ -917,15 +917,15 @@
     ts-loader: ^9.2.6
     typescript: ^5
     uuid: ^8.3.2
     webpack: ^5.76.3
   languageName: unknown
   linkType: soft
 
-"@jupytercad/jupytercad-opencascade@^0.2.0-alpha.0, @jupytercad/jupytercad-opencascade@workspace:packages/jupytercad-opencascade":
+"@jupytercad/jupytercad-opencascade@^0.2.1, @jupytercad/jupytercad-opencascade@workspace:packages/jupytercad-opencascade":
   version: 0.0.0-use.local
   resolution: "@jupytercad/jupytercad-opencascade@workspace:packages/jupytercad-opencascade"
   dependencies:
     js-yaml: ^4.1.0
     rimraf: ^3.0.2
   languageName: unknown
   linkType: soft
```

### Comparing `jupytercad-0.2.0/jupytercad/fcstd_ydoc.py` & `jupytercad-0.2.1/jupytercad/fcstd_ydoc.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 
 from jupytercad.freecad.loader import FCStd
 
 
 class YFCStd(YBaseDoc):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._ysource = self._ydoc.get_text('source')
-        self._yobjects = self._ydoc.get_array('objects')
-        self._yoptions = self._ydoc.get_map('options')
-        self._ymeta = self._ydoc.get_map('metadata')
+        self._ysource = self._ydoc.get_text("source")
+        self._yobjects = self._ydoc.get_array("objects")
+        self._yoptions = self._ydoc.get_map("options")
+        self._ymeta = self._ydoc.get_map("metadata")
         self._virtual_file = FCStd()
 
     @property
     def objects(self) -> Y.YArray:
         return self._yobjects
 
     def version(self) -> str:
-        return '0.1.0'
-    
+        return "0.1.0"
+
     def get(self):
-        fc_objects = json.loads(self._yobjects.to_json()) 
+        fc_objects = json.loads(self._yobjects.to_json())
         options = json.loads(self._yoptions.to_json())
         meta = json.loads(self._ymeta.to_json())
 
         self._virtual_file.save(fc_objects, options, meta)
         return self._virtual_file.sources
 
     def set(self, value):
@@ -38,23 +38,31 @@
         objects = []
 
         for obj in virtual_file.objects:
             objects.append(Y.YMap(obj))
         with self._ydoc.begin_transaction() as t:
             length = len(self._yobjects)
             self._yobjects.delete_range(t, 0, length)
-            #workaround for https://github.com/y-crdt/ypy/issues/126:
-            #self._yobjects.extend(t, objects)
+            # workaround for https://github.com/y-crdt/ypy/issues/126:
+            # self._yobjects.extend(t, objects)
             for o in objects:
                 self._yobjects.append(t, o)
             self._yoptions.update(t, virtual_file.options.items())
             self._ymeta.update(t, virtual_file.metadata.items())
 
     def observe(self, callback: Callable[[str, Any], None]):
         self.unobserve()
-        self._subscriptions[self._ystate] = self._ystate.observe(partial(callback, "state"))
-        self._subscriptions[self._ysource] = self._ysource.observe(partial(callback, "source"))
+        self._subscriptions[self._ystate] = self._ystate.observe(
+            partial(callback, "state")
+        )
+        self._subscriptions[self._ysource] = self._ysource.observe(
+            partial(callback, "source")
+        )
         self._subscriptions[self._yobjects] = self._yobjects.observe_deep(
             partial(callback, "objects")
         )
-        self._subscriptions[self._yoptions] = self._yoptions.observe(partial(callback, "options"))
-        self._subscriptions[self._ymeta] = self._ymeta.observe_deep(partial(callback, "meta"))
+        self._subscriptions[self._yoptions] = self._yoptions.observe(
+            partial(callback, "options")
+        )
+        self._subscriptions[self._ymeta] = self._ymeta.observe_deep(
+            partial(callback, "meta")
+        )
```

### Comparing `jupytercad-0.2.0/jupytercad/jcad_ydoc.py` & `jupytercad-0.2.1/jupytercad/jcad_ydoc.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import y_py as Y
 from jupyter_ydoc.ybasedoc import YBaseDoc
 
 
 class YJCad(YBaseDoc):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._ysource = self._ydoc.get_text('source')
-        self._yobjects = self._ydoc.get_array('objects')
-        self._yoptions = self._ydoc.get_map('options')
-        self._ymeta = self._ydoc.get_map('metadata')
+        self._ysource = self._ydoc.get_text("source")
+        self._yobjects = self._ydoc.get_array("objects")
+        self._yoptions = self._ydoc.get_map("options")
+        self._ymeta = self._ydoc.get_map("metadata")
 
     def version(self) -> str:
-        return '0.1.0'
+        return "0.1.0"
 
     def get(self) -> str:
         """
         Returns the content of the document.
         :return: Document's content.
         :rtype: Any
         """
@@ -34,28 +34,36 @@
         """
         Sets the content of the document.
         :param value: The content of the document.
         :type value: Any
         """
         valueDict = json.loads(value)
         newObj = []
-        for obj in valueDict['objects']:
+        for obj in valueDict["objects"]:
             newObj.append(Y.YMap(obj))
         with self._ydoc.begin_transaction() as t:
             length = len(self._yobjects)
             self._yobjects.delete_range(t, 0, length)
             # workaround for https://github.com/y-crdt/ypy/issues/126:
-            #self._yobjects.extend(t, newObj)
+            # self._yobjects.extend(t, newObj)
             for o in newObj:
                 self._yobjects.append(t, o)
-            self._yoptions.update(t, valueDict['options'].items())
-            self._ymeta.update(t, valueDict['metadata'].items())
+            self._yoptions.update(t, valueDict["options"].items())
+            self._ymeta.update(t, valueDict["metadata"].items())
 
     def observe(self, callback: Callable[[str, Any], None]):
         self.unobserve()
-        self._subscriptions[self._ystate] = self._ystate.observe(partial(callback, "state"))
-        self._subscriptions[self._ysource] = self._ysource.observe(partial(callback, "source"))
+        self._subscriptions[self._ystate] = self._ystate.observe(
+            partial(callback, "state")
+        )
+        self._subscriptions[self._ysource] = self._ysource.observe(
+            partial(callback, "source")
+        )
         self._subscriptions[self._yobjects] = self._yobjects.observe_deep(
             partial(callback, "objects")
         )
-        self._subscriptions[self._yoptions] = self._yoptions.observe(partial(callback, "options"))
-        self._subscriptions[self._ymeta] = self._ymeta.observe(partial(callback, "meta"))
+        self._subscriptions[self._yoptions] = self._yoptions.observe(
+            partial(callback, "options")
+        )
+        self._subscriptions[self._ymeta] = self._ymeta.observe(
+            partial(callback, "meta")
+        )
```

### Comparing `jupytercad-0.2.0/jupytercad/cadapp/cadapp.py` & `jupytercad-0.2.1/jupytercad/cadapp/cadapp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 import json
 import os
 
 import tornado
 from jupyter_server.base.handlers import APIHandler, JupyterHandler
-from jupyter_server.extension.handler import (ExtensionHandlerJinjaMixin,
-                                              ExtensionHandlerMixin)
+from jupyter_server.extension.handler import (
+    ExtensionHandlerJinjaMixin,
+    ExtensionHandlerMixin,
+)
 from jupyterlab_server import LabServerApp
 
 from .._version import __version__
 from .utils import get_page_config
 
 HERE = os.path.dirname(__file__)
 
 
 class CADHandler(ExtensionHandlerJinjaMixin, ExtensionHandlerMixin, JupyterHandler):
     """Handle requests between the main app page and notebook server."""
 
     def get(self):
         """Get the main page for the application's interface."""
         page_config = get_page_config(self.base_url, self.name)
-        page_config['token'] = self.settings['token']
+        page_config["token"] = self.settings["token"]
         return self.write(
             self.render_template(
-                'index.html',
+                "index.html",
                 static=self.static_url,
                 base_url=self.base_url,
-                token=self.settings['token'],
+                token=self.settings["token"],
                 page_config=page_config,
             )
         )
 
 
 class BackendCheckHandler(APIHandler):
     @tornado.web.authenticated
     def post(self):
         body = self.get_json_body()
-        backend = body.get('backend')
-        if backend == 'FreeCAD':
+        backend = body.get("backend")
+        if backend == "FreeCAD":
             fc_installed = True
             try:
-                import freecad
+                pass
             except ImportError:
                 fc_installed = False
-            self.finish(json.dumps({'installed': fc_installed}))
-        elif backend == 'JCAD':
-            self.finish(json.dumps({'installed': True}))
+            self.finish(json.dumps({"installed": fc_installed}))
+        elif backend == "JCAD":
+            self.finish(json.dumps({"installed": True}))
         else:
-            self.finish(json.dumps({'installed': False}))
+            self.finish(json.dumps({"installed": False}))
 
-class CadApp(LabServerApp):
 
-    extension_url = '/cad'
-    default_url = '/cad'
+class CadApp(LabServerApp):
+    extension_url = "/cad"
+    default_url = "/cad"
     app_url = "/cad"
     load_other_extensions = True
     name = "cad"
-    app_name = 'JupyterCAD'
-    static_dir = os.path.join(HERE, 'static')
-    templates_dir = os.path.join(HERE, 'templates')
+    app_name = "JupyterCAD"
+    static_dir = os.path.join(HERE, "static")
+    templates_dir = os.path.join(HERE, "templates")
     app_version = __version__
-    app_settings_dir = os.path.join(HERE, 'static', 'application_settings')
-    schemas_dir = os.path.join(HERE, 'schemas')
-    themes_dir = os.path.join(HERE, 'themes')
-    user_settings_dir = os.path.join(HERE, 'static', 'user_settings')
-    workspaces_dir = os.path.join(HERE, 'static', 'workspaces')
+    app_settings_dir = os.path.join(HERE, "static", "application_settings")
+    schemas_dir = os.path.join(HERE, "schemas")
+    themes_dir = os.path.join(HERE, "themes")
+    user_settings_dir = os.path.join(HERE, "static", "user_settings")
+    workspaces_dir = os.path.join(HERE, "static", "workspaces")
 
     def initialize_handlers(self):
         """Add cad handler to Lab Server's handler list."""
-        self.handlers.append(('/cad', CADHandler))
-        self.handlers.append(('/cad/backend-check', BackendCheckHandler))
+        self.handlers.append(("/cad", CADHandler))
+        self.handlers.append(("/cad/backend-check", BackendCheckHandler))
         super().initialize_handlers()
 
 
 main = CadApp.launch_instance
```

### Comparing `jupytercad-0.2.0/jupytercad/cadapp/utils.py` & `jupytercad-0.2.1/jupytercad/cadapp/utils.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/cadapp/templates/index.html` & `jupytercad-0.2.1/jupytercad/cadapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/freecad/loader.py` & `jupytercad-0.2.1/jupytercad/freecad/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import base64
-import json
 import logging
 import os
 import tempfile
 import traceback
 from typing import Dict, List, Type
 
 from . import props as Props
@@ -24,23 +23,23 @@
     options = {}
 
     for obj_name, data in guidata.items():
         obj_options = {}
 
         # We need to make a special case to "GuiCameraSettings" because freecad's
         # OfflineRenderingUtils mixes the camera settings with 3D objects
-        if obj_name == 'GuiCameraSettings':
+        if obj_name == "GuiCameraSettings":
             options[obj_name] = data
             continue
 
-        if 'ShapeColor' in data:
-            obj_options['color'] = list(data['ShapeColor']['value'])
+        if "ShapeColor" in data:
+            obj_options["color"] = list(data["ShapeColor"]["value"])
 
-        if 'Visibility' in data:
-            obj_options['visibility'] = data['Visibility']['value']
+        if "Visibility" in data:
+            obj_options["visibility"] = data["Visibility"]["value"]
 
         options[obj_name] = obj_options
 
     return options
 
 
 def _options_to_guidata(options):
@@ -48,36 +47,36 @@
     gui_data = {}
 
     for obj_name, data in options.items():
         obj_data = {}
 
         # We need to make a special case to "GuiCameraSettings" because freecad's
         # OfflineRenderingUtils mixes the camera settings with 3D objects
-        if obj_name == 'GuiCameraSettings':
+        if obj_name == "GuiCameraSettings":
             options[obj_name] = data
             continue
 
-        if 'color' in data:
-            obj_data['ShapeColor'] = dict(
-                type='App::PropertyColor', value=tuple(data['color'])
+        if "color" in data:
+            obj_data["ShapeColor"] = dict(
+                type="App::PropertyColor", value=tuple(data["color"])
             )
 
-        if 'visibility' in data:
-            obj_data['Visibility'] = dict(
-                type='App::PropertyBool', value=data['visibility']
+        if "visibility" in data:
+            obj_data["Visibility"] = dict(
+                type="App::PropertyBool", value=data["visibility"]
             )
 
         gui_data[obj_name] = obj_data
 
     return gui_data
 
 
 class FCStd:
     def __init__(self) -> None:
-        self._sources = ''
+        self._sources = ""
         self._objects = []
         self._options = {}
         self._metadata = {}
         self._id = None
         self._visible = True
         self._prop_handlers: Dict[str, Type[BaseProp]] = {}
         for Cls in Props.__dict__.values():
@@ -100,25 +99,25 @@
     def options(self):
         return self._options
 
     def load(self, base64_content: str) -> None:
         if not fc:
             return
         self._sources = base64_content
-        with tempfile.NamedTemporaryFile(delete=False, suffix='.FCStd') as tmp:
+        with tempfile.NamedTemporaryFile(delete=False, suffix=".FCStd") as tmp:
             file_content = base64.b64decode(base64_content)
             tmp.write(file_content)
 
         fc_file = fc.app.openDocument(tmp.name)
 
         # Get metadata
         self._metadata = fc_file.Meta
 
         # Get GuiData (metadata from the GuiDocument.xml file)
-        self._options['guidata'] = _guidata_to_options(
+        self._options["guidata"] = _guidata_to_options(
             OfflineRenderingUtils.getGuiData(tmp.name)
         )
 
         # Get objects
         self._objects = []
         for obj in fc_file.Objects:
             self._objects.append(self._fc_to_jcad_obj(obj))
@@ -126,63 +125,61 @@
         os.remove(tmp.name)
 
     def save(self, objects: List, options: Dict, metadata: Dict) -> None:
         try:
             if not fc or len(self._sources) == 0:
                 return
 
-            with tempfile.NamedTemporaryFile(
-                delete=False, suffix='.FCStd'
-            ) as tmp:
+            with tempfile.NamedTemporaryFile(delete=False, suffix=".FCStd") as tmp:
                 file_content = base64.b64decode(self._sources)
                 tmp.write(file_content)
             fc_file = fc.app.openDocument(tmp.name)
             fc_file.Meta = metadata
-            new_objs = dict([(o['name'], o) for o in objects])
+            new_objs = dict([(o["name"], o) for o in objects])
 
             current_objs = dict([(o.Name, o) for o in fc_file.Objects])
 
             to_remove = [x for x in current_objs if x not in new_objs]
             to_add = [x for x in new_objs if x not in current_objs]
             for obj_name in to_remove:
                 fc_file.removeObject(obj_name)
             for obj_name in to_add:
                 py_obj = new_objs[obj_name]
-                fc_file.addObject(py_obj['shape'], py_obj['name'])
+                fc_file.addObject(py_obj["shape"], py_obj["name"])
             to_update = [x for x in new_objs if x in current_objs] + to_add
 
             for obj_name in to_update:
                 py_obj = new_objs[obj_name]
 
-                fc_obj = fc_file.getObject(py_obj['name'])
+                fc_obj = fc_file.getObject(py_obj["name"])
 
-                for prop, jcad_prop_value in py_obj['parameters'].items():
+                for prop, jcad_prop_value in py_obj["parameters"].items():
                     prop_type = fc_obj.getTypeIdOfProperty(prop)
                     prop_handler = self._prop_handlers.get(prop_type, None)
                     if prop_handler is not None:
                         fc_value = prop_handler.jcad_to_fc(
                             jcad_prop_value,
                             jcad_object=objects,
                             fc_prop=getattr(fc_obj, prop),
                             fc_object=fc_obj,
                             fc_file=fc_file,
                         )
                         if fc_value:
                             try:
                                 setattr(fc_obj, prop, fc_value)
-                            except:
+                            except Exception:
                                 pass
 
             OfflineRenderingUtils.save(
                 fc_file,
-                guidata=_options_to_guidata(options.get('guidata', {})),
+                guidata=_options_to_guidata(options.get("guidata", {})),
             )
 
             fc_file.recompute()
-            with open(tmp.name, 'rb') as f:
+            with open(tmp.name, "rb") as f:
                 encoded = base64.b64encode(f.read())
                 self._sources = encoded.decode()
             os.remove(tmp.name)
         except Exception:
             print(traceback.print_exc())
 
     def _fc_to_jcad_obj(self, obj) -> Dict:
@@ -196,9 +193,9 @@
             prop_type = obj.getTypeIdOfProperty(prop)
             prop_value = getattr(obj, prop)
             prop_handler = self._prop_handlers.get(prop_type, None)
             if prop_handler is not None and prop_value is not None:
                 value = prop_handler.fc_to_jcad(prop_value, fc_object=obj)
             else:
                 value = None
-            obj_data['parameters'][prop] = value
+            obj_data["parameters"][prop] = value
         return obj_data
```

### Comparing `jupytercad-0.2.0/jupytercad/freecad/props/base_prop.py` & `jupytercad-0.2.1/jupytercad/freecad/props/base_prop.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/freecad/props/property_geometrylist.py` & `jupytercad-0.2.1/jupytercad/freecad/props/property_geometrylist.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .base_prop import BaseProp
 from .geometry import geom_handlers
 
 
 class Part_PropertyGeometryList(BaseProp):
     @staticmethod
     def name() -> str:
-        return 'Part::PropertyGeometryList'
+        return "Part::PropertyGeometryList"
 
     @staticmethod
     def fc_to_jcad(prop_value: List, **kwargs) -> Any:
         ret = []
         for geo in prop_value:
             if geo.TypeId in geom_handlers:
                 ret.append(geom_handlers[geo.TypeId].fc_to_jcad(geo))
@@ -22,25 +22,25 @@
         # We do not handle the case of adding or removing yet.
         n_objects = len(fc_prop)
 
         n_new_objects = len(prop_value)
         if n_objects > 0 and n_objects == n_new_objects:
             # Update existing geometries
             for idx, jcad_geo in enumerate(prop_value):
-                if jcad_geo['TypeId'] in geom_handlers:
-                    geom_handlers[jcad_geo['TypeId']].jcad_to_fc(
+                if jcad_geo["TypeId"] in geom_handlers:
+                    geom_handlers[jcad_geo["TypeId"]].jcad_to_fc(
                         jcad_geo, fc_object=fc_prop[idx]
                     )
             return fc_prop
 
         if n_objects == 0 and n_new_objects > 0:
             # Create new geometries
             for jcad_geo in prop_value:
-                if jcad_geo['TypeId'] in geom_handlers:
-                    fc_geo = geom_handlers[jcad_geo['TypeId']].jcad_to_fc(
+                if jcad_geo["TypeId"] in geom_handlers:
+                    fc_geo = geom_handlers[jcad_geo["TypeId"]].jcad_to_fc(
                         jcad_geo, fc_object=None
                     )
 
                     fc_prop.append(fc_geo)
 
             return fc_prop
```

### Comparing `jupytercad-0.2.0/jupytercad/freecad/props/property_partshape.py` & `jupytercad-0.2.1/jupytercad/freecad/props/property_partshape.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .base_prop import BaseProp
 
 
 class Part_PropertyPartShape(BaseProp):
     @staticmethod
     def name() -> str:
-        return 'Part::PropertyPartShape'
+        return "Part::PropertyPartShape"
 
     @staticmethod
     def fc_to_jcad(prop_value: Any, **kwargs) -> Any:
         buffer = StringIO()
         prop_value.exportBrep(buffer)
         return buffer.getvalue()
```

### Comparing `jupytercad-0.2.0/jupytercad/freecad/props/property_placement.py` & `jupytercad-0.2.1/jupytercad/freecad/props/property_placement.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 except ImportError:
     fc = None
 
 
 class App_PropertyPlacement(BaseProp):
     @staticmethod
     def name() -> str:
-        return 'App::PropertyPlacement'
+        return "App::PropertyPlacement"
 
     @staticmethod
     def fc_to_jcad(prop_value: Any, **kwargs) -> Any:
         return {
-            'Position': [
+            "Position": [
                 prop_value.Base.x,
                 prop_value.Base.y,
                 prop_value.Base.z,
             ],
-            'Axis': [
+            "Axis": [
                 prop_value.Rotation.Axis.x,
                 prop_value.Rotation.Axis.y,
                 prop_value.Rotation.Axis.z,
             ],
-            'Angle': 180 * prop_value.Rotation.Angle / math.pi,
+            "Angle": 180 * prop_value.Rotation.Angle / math.pi,
         }
 
     @staticmethod
     def jcad_to_fc(prop_value: Any, **kwargs) -> Any:
         if not fc:
             return
 
-        base = fc.app.Base.Vector(prop_value['Position'])
-        axis = fc.app.Base.Vector(prop_value['Axis'])
-        angle = prop_value['Angle']
+        base = fc.app.Base.Vector(prop_value["Position"])
+        axis = fc.app.Base.Vector(prop_value["Axis"])
+        angle = prop_value["Angle"]
         return fc.app.Placement(base, axis, angle)
```

### Comparing `jupytercad-0.2.0/jupytercad/freecad/props/geometry/geom_circle.py` & `jupytercad-0.2.1/jupytercad/freecad/props/geometry/geom_circle.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,52 +8,52 @@
 except ImportError:
     fc = None
 
 
 class Part_GeomCircle(BaseProp):
     @staticmethod
     def name() -> str:
-        return 'Part::GeomCircle'
+        return "Part::GeomCircle"
 
     @staticmethod
     def fc_to_jcad(prop_value: Any, **kwargs) -> Any:
         center = prop_value.Center
         radius = prop_value.Radius
         angle = prop_value.AngleXU
         normal = prop_value.Axis
         return {
-            'TypeId': Part_GeomCircle.name(),
-            'CenterX': center.x,
-            'CenterY': center.y,
-            'CenterZ': center.z,
-            'NormalX': normal.x,
-            'NormalY': normal.y,
-            'NormalZ': normal.z,
-            'AngleXU': angle,
-            'Radius': radius,
+            "TypeId": Part_GeomCircle.name(),
+            "CenterX": center.x,
+            "CenterY": center.y,
+            "CenterZ": center.z,
+            "NormalX": normal.x,
+            "NormalY": normal.y,
+            "NormalZ": normal.z,
+            "AngleXU": angle,
+            "Radius": radius,
         }
 
     @staticmethod
     def jcad_to_fc(prop_value: Dict, fc_object: Any, **kwargs) -> Any:
         if not fc:
             return
         Center = fc.app.Base.Vector(
-            prop_value['CenterX'],
-            prop_value['CenterY'],
-            prop_value['CenterZ'],
+            prop_value["CenterX"],
+            prop_value["CenterY"],
+            prop_value["CenterZ"],
         )
 
         Axis = fc.app.Base.Vector(
-            prop_value['NormalX'],
-            prop_value['NormalY'],
-            prop_value['NormalZ'],
+            prop_value["NormalX"],
+            prop_value["NormalY"],
+            prop_value["NormalZ"],
         )
 
-        Radius = prop_value['Radius']
+        Radius = prop_value["Radius"]
         if fc_object:
             fc_object.Center = Center
             fc_object.Axis = Axis
-            fc_object.AngleXU = prop_value['AngleXU']
+            fc_object.AngleXU = prop_value["AngleXU"]
             fc_object.Radius = Radius
             return None
         else:
             return Part.Circle(Center, Axis, Radius)
```

### Comparing `jupytercad-0.2.0/jupytercad/freecad/props/geometry/geom_linesegment.py` & `jupytercad-0.2.1/jupytercad/freecad/props/geometry/geom_linesegment.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 except ImportError:
     fc = None
 
 
 class Part_GeomLineSegment(BaseProp):
     @staticmethod
     def name() -> str:
-        return 'Part::GeomLineSegment'
+        return "Part::GeomLineSegment"
 
     @staticmethod
     def fc_to_jcad(prop_value: Any, **kwargs) -> Any:
         start = prop_value.StartPoint
         end = prop_value.EndPoint
 
         return {
-            'TypeId': Part_GeomLineSegment.name(),
-            'StartX': start.x,
-            'StartY': start.y,
-            'StartZ': start.z,
-            'EndX': end.x,
-            'EndY': end.y,
-            'EndZ': end.z,
+            "TypeId": Part_GeomLineSegment.name(),
+            "StartX": start.x,
+            "StartY": start.y,
+            "StartZ": start.z,
+            "EndX": end.x,
+            "EndY": end.y,
+            "EndZ": end.z,
         }
 
     @staticmethod
     def jcad_to_fc(prop_value: Dict, fc_object: Any, **kwargs) -> Any:
         if not fc:
             return
         StartPoint = fc.app.Base.Vector(
-            prop_value['StartX'], prop_value['StartY'], prop_value['StartZ']
+            prop_value["StartX"], prop_value["StartY"], prop_value["StartZ"]
         )
         EndPoint = fc.app.Base.Vector(
-            prop_value['EndX'], prop_value['EndY'], prop_value['EndZ']
+            prop_value["EndX"], prop_value["EndY"], prop_value["EndZ"]
         )
         if fc_object:
             fc_object.StartPoint = StartPoint
             fc_object.EndPoint = EndPoint
             return None
         else:
             return Part.LineSegment(StartPoint, EndPoint)
```

### Comparing `jupytercad-0.2.0/jupytercad/labextension/package.json` & `jupytercad-0.2.1/jupytercad/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9741927083333334%*

 * *Differences: {"'dependencies'": "{'@jupytercad/jupytercad-opencascade': '^0.2.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e8080149ddd48fae3b49.js'}}",*

 * * "'version'": "'0.2.1'"}*

```diff
@@ -6,15 +6,15 @@
         "url": "https://github.com/QuantStack/jupytercad/issues"
     },
     "dependencies": {
         "@deathbeds/jupyterlab-rjsf": "^1.1.0",
         "@jupyter/collaboration": "^1.0.0-alpha.7",
         "@jupyter/docprovider": "^1.0.0-alpha.8",
         "@jupyter/ydoc": "^0.3.4 || ^1.0.2",
-        "@jupytercad/jupytercad-opencascade": "^0.2.0-alpha.0",
+        "@jupytercad/jupytercad-opencascade": "^0.2.1",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -57,15 +57,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/QuantStack/jupytercad",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3d94847557dd157537a5.js",
+            "load": "static/remoteEntry.e8080149ddd48fae3b49.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../jupytercad/labextension",
         "sharedPackages": {
             "yjs": {
                 "bundled": false,
@@ -113,9 +113,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0-alpha.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/184.6f76dd957e411be19baa.js` & `jupytercad-0.2.1/jupytercad/labextension/static/184.6f76dd957e411be19baa.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/213.778b3209dbe7ec5470b6.js` & `jupytercad-0.2.1/jupytercad/labextension/static/213.778b3209dbe7ec5470b6.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/268.16c8a4126908b03651f0.js` & `jupytercad-0.2.1/jupytercad/labextension/static/268.16c8a4126908b03651f0.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js` & `jupytercad-0.2.1/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/358.45fb46ea24bb44ba7fa9.js` & `jupytercad-0.2.1/jupytercad/labextension/static/358.45fb46ea24bb44ba7fa9.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js` & `jupytercad-0.2.1/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js` & `jupytercad-0.2.1/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/422.39a95e19d3a414516796.js` & `jupytercad-0.2.1/jupytercad/labextension/static/422.39a95e19d3a414516796.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js` & `jupytercad-0.2.1/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/544.5c918f69ee5ea6e28e28.js` & `jupytercad-0.2.1/jupytercad/labextension/static/544.f90bd90ee4b5fdf48162.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -236,22 +236,22 @@
                         AngleXU: 0
                     }
                 }
             }
             var x = n(59474),
                 C = n(3020),
                 j = n(36258);
-            const P = '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px"><g class="jp-icon3" fill="#616161"><g><path d="M2,6c0.55,0,1-0.45,1-1V4c0-0.55,0.45-1,1-1h1c0.55,0,1-0.45,1-1S5.55,1,5,1H4C2.34,1,1,2.34,1,4v1C1,5.55,1.45,6,2,6z"/><path d="M5,21H4c-0.55,0-1-0.45-1-1v-1c0-0.55-0.45-1-1-1c-0.55,0-1,0.45-1,1v1c0,1.66,1.34,3,3,3h1c0.55,0,1-0.45,1-1 S5.55,21,5,21z"/><path d="M20,1h-1c-0.55,0-1,0.45-1,1s0.45,1,1,1h1c0.55,0,1,0.45,1,1v1c0,0.55,0.45,1,1,1c0.55,0,1-0.45,1-1V4 C23,2.34,21.66,1,20,1z"/><path d="M22,18c-0.55,0-1,0.45-1,1v1c0,0.55-0.45,1-1,1h-1c-0.55,0-1,0.45-1,1s0.45,1,1,1h1c1.66,0,3-1.34,3-3v-1 C23,18.45,22.55,18,22,18z"/><path d="M19,14.87V9.13c0-0.72-0.38-1.38-1-1.73l-5-2.88c-0.31-0.18-0.65-0.27-1-0.27s-0.69,0.09-1,0.27L6,7.39 C5.38,7.75,5,8.41,5,9.13v5.74c0,0.72,0.38,1.38,1,1.73l5,2.88c0.31,0.18,0.65,0.27,1,0.27s0.69-0.09,1-0.27l5-2.88 C18.62,16.25,19,15.59,19,14.87z M11,17.17l-4-2.3v-4.63l4,2.33V17.17z M12,10.84L8.04,8.53L12,6.25l3.96,2.28L12,10.84z M17,14.87l-4,2.3v-4.6l4-2.33V14.87z"/></g></g></svg>',
+            const P = '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px"><g class="jp-icon3" fill="#616161"><g><path d="M2,6c0.55,0,1-0.45,1-1V4c0-0.55,0.45-1,1-1h1c0.55,0,1-0.45,1-1S5.55,1,5,1H4C2.34,1,1,2.34,1,4v1C1,5.55,1.45,6,2,6z"/><path d="M5,21H4c-0.55,0-1-0.45-1-1v-1c0-0.55-0.45-1-1-1c-0.55,0-1,0.45-1,1v1c0,1.66,1.34,3,3,3h1c0.55,0,1-0.45,1-1 S5.55,21,5,21z"/><path d="M20,1h-1c-0.55,0-1,0.45-1,1s0.45,1,1,1h1c0.55,0,1,0.45,1,1v1c0,0.55,0.45,1,1,1c0.55,0,1-0.45,1-1V4 C23,2.34,21.66,1,20,1z"/><path d="M22,18c-0.55,0-1,0.45-1,1v1c0,0.55-0.45,1-1,1h-1c-0.55,0-1,0.45-1,1s0.45,1,1,1h1c1.66,0,3-1.34,3-3v-1 C23,18.45,22.55,18,22,18z"/><path d="M19,14.87V9.13c0-0.72-0.38-1.38-1-1.73l-5-2.88c-0.31-0.18-0.65-0.27-1-0.27s-0.69,0.09-1,0.27L6,7.39 C5.38,7.75,5,8.41,5,9.13v5.74c0,0.72,0.38,1.38,1,1.73l5,2.88c0.31,0.18,0.65,0.27,1,0.27s0.69-0.09,1-0.27l5-2.88 C18.62,16.25,19,15.59,19,14.87z M11,17.17l-4-2.3v-4.63l4,2.33V17.17z M12,10.84L8.04,8.53L12,6.25l3.96,2.28L12,10.84z M17,14.87l-4,2.3v-4.6l4-2.33V14.87z"/></g></g></svg>\n',
                 S = new c.LabIcon({
                     name: "jupytercad:control-light",
                     svgstr: P
                 }),
                 M = new c.LabIcon({
                     name: "jupytercad:minimize-icon",
-                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="20" width="20"><path class="jp-icon3" fill="#616161" d="M5 11.75v-1.5h10v1.5Z"/></svg>'
+                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="20" width="20"><path class="jp-icon3" fill="#616161" d="M5 11.75v-1.5h10v1.5Z"/></svg>\n'
                 }),
                 A = new c.LabIcon({
                     name: "jupytercad:box-icon",
                     svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   width="14.3"\n   viewBox="0 0 21.45 14.3"\n   version="1.1"\n   height="14.3"\n   xmlns="http://www.w3.org/2000/svg"\n   xmlns:svg="http://www.w3.org/2000/svg">\n  <g\n     class="jp-icon3"\n     fill="#616161"\n     transform="translate(0.75039085,0.49939006)">\n    <path\n       d="M 0.97460938,-0.32421875 A 0.97509752,0.97509752 0 0 0 0,0.65039062 V 15.650391 A 0.97509752,0.97509752 0 0 0 0.97460938,16.625 H 15.974609 a 0.97509752,0.97509752 0 0 0 0.97461,-0.974609 V 0.65039062 a 0.97509752,0.97509752 0 0 0 -0.97461,-0.97460937 z M 1.9492187,1.625 H 15 V 14.675781 H 1.9492187 Z"\n       />\n    <path\n       d="M 3.9746094,-3.3242188 A 0.97500002,0.97500002 0 0 0 3,-2.3496094 0.97500002,0.97500002 0 0 0 3.9746094,-1.375 H 18 v 13.621094 l -2.714844,2.714844 a 0.97500002,0.97500002 0 0 0 0,1.378906 0.97500002,0.97500002 0 0 0 1.378906,0 l 3,-3 a 0.97509752,0.97509752 0 0 0 0.285157,-0.689453 V -2.3496094 a 0.97509752,0.97509752 0 0 0 -0.97461,-0.9746094 z"\n       />\n    <path\n       d="m 18.974609,-3.3242188 a 0.97500002,0.97500002 0 0 0 -0.689453,0.2851563 l -3,3 a 0.97500002,0.97500002 0 0 0 0,1.3789062 0.97500002,0.97500002 0 0 0 1.378906,0 l 3,-2.9999999 a 0.97500002,0.97500002 0 0 0 0,-1.3789063 0.97500002,0.97500002 0 0 0 -0.689453,-0.2851563 z"\n       />\n    <path\n       d="m 3.9746094,-3.3242188 a 0.97500002,0.97500002 0 0 0 -0.6894531,0.2851563 l -3.00000005,3 a 0.97500002,0.97500002 0 0 0 0,1.3789062 0.97500002,0.97500002 0 0 0 1.37890625,0 l 3,-2.9999999 a 0.97500002,0.97500002 0 0 0 0,-1.3789063 0.97500002,0.97500002 0 0 0 -0.6894531,-0.2851563 z"\n       />\n    <path\n       d="M 3.9746094,-1.2421875 A 0.97500002,0.97500002 0 0 0 3,-0.26757813 V 1.6835937 A 0.97500002,0.97500002 0 0 0 3.9746094,2.6582031 0.97500002,0.97500002 0 0 0 4.9492187,1.6835937 V -0.26757813 A 0.97500002,0.97500002 0 0 0 3.9746094,-1.2421875 Z m 0,5.8496094 A 0.97500002,0.97500002 0 0 0 3,5.5820312 V 7.5332031 A 0.97500002,0.97500002 0 0 0 3.9746094,8.5078125 0.97500002,0.97500002 0 0 0 4.9492187,7.5332031 V 5.5820312 A 0.97500002,0.97500002 0 0 0 3.9746094,4.6074219 Z m 0,5.8496091 A 0.97500002,0.97500002 0 0 0 3,11.433594 v 0.8125 l -0.2324219,0.232422 a 0.97500002,0.97500002 0 0 0 0,1.378906 0.97500002,0.97500002 0 0 0 1.3789063,0 L 4.6640625,13.339844 A 0.97509752,0.97509752 0 0 0 4.9492187,12.650391 V 11.433594 A 0.97500002,0.97500002 0 0 0 3.9746094,10.457031 Z"\n       />\n    <path\n       d="M 3.9746094,11.675781 A 0.97500002,0.97500002 0 0 0 3,12.650391 0.97500002,0.97500002 0 0 0 3.9746094,13.625 h 0.9746093 a 0.97500002,0.97500002 0 0 0 0.9765625,-0.974609 0.97500002,0.97500002 0 0 0 -0.9765625,-0.97461 z m 4.875,0 A 0.97500002,0.97500002 0 0 0 7.875,12.650391 0.97500002,0.97500002 0 0 0 8.8496094,13.625 h 1.9511716 a 0.97500002,0.97500002 0 0 0 0.97461,-0.974609 0.97500002,0.97500002 0 0 0 -0.97461,-0.97461 z m 5.8496096,0 a 0.97500002,0.97500002 0 0 0 -0.97461,0.97461 0.97500002,0.97500002 0 0 0 0.97461,0.974609 h 1.951172 A 0.97500002,0.97500002 0 0 0 17.625,12.650391 0.97500002,0.97500002 0 0 0 16.650391,11.675781 Z"\n       />\n  </g>\n</svg>\n'
                 }),
                 O = new c.LabIcon({
                     name: "jupytercad:cone-icon",
@@ -892,15 +892,15 @@
                     })), super({
                         title: e.title,
                         body: i,
                         buttons: [o.Dialog.cancelButton()]
                     }), this.addClass("jpcad-property-FormDialog")
                 }
             }
-            const ee = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the box":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
+            const ee = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the box":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
             var te = function(e, t) {
                 var n = {};
                 for (var s in e) Object.prototype.hasOwnProperty.call(e, s) && t.indexOf(s) < 0 && (n[s] = e[s]);
                 if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                     var o = 0;
                     for (s = Object.getOwnPropertySymbols(e); o < s.length; o++) t.indexOf(s[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, s[o]) && (n[s[o]] = e[s[o]])
                 }
@@ -2615,19 +2615,19 @@
             function tt() {
                 const e = document.createElement("h2");
                 return e.textContent = "-", e
             }
             var nt = n(8743);
             const st = new c.LabIcon({
                     name: "jupytercad:visibilityIcon",
-                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 0 24 24" width="24">\n    <path d="M0 0h24v24H0V0z" fill="none" />\n    <path class="jp-icon3" d="M12 6c3.79 0 7.17 2.13 8.82 5.5C19.17 14.87 15.79 17 12 17s-7.17-2.13-8.82-5.5C4.83 8.13 8.21 6 12 6m0-2C7 4 2.73 7.11 1 11.5 2.73 15.89 7 19 12 19s9.27-3.11 11-7.5C21.27 7.11 17 4 12 4zm0 5c1.38 0 2.5 1.12 2.5 2.5S13.38 14 12 14s-2.5-1.12-2.5-2.5S10.62 9 12 9m0-2c-2.48 0-4.5 2.02-4.5 4.5S9.52 16 12 16s4.5-2.02 4.5-4.5S14.48 7 12 7z" fill="none" />\n</svg>'
+                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 0 24 24" width="24">\n    <path d="M0 0h24v24H0V0z" fill="none" />\n    <path class="jp-icon3" d="M12 6c3.79 0 7.17 2.13 8.82 5.5C19.17 14.87 15.79 17 12 17s-7.17-2.13-8.82-5.5C4.83 8.13 8.21 6 12 6m0-2C7 4 2.73 7.11 1 11.5 2.73 15.89 7 19 12 19s9.27-3.11 11-7.5C21.27 7.11 17 4 12 4zm0 5c1.38 0 2.5 1.12 2.5 2.5S13.38 14 12 14s-2.5-1.12-2.5-2.5S10.62 9 12 9m0-2c-2.48 0-4.5 2.02-4.5 4.5S9.52 16 12 16s4.5-2.02 4.5-4.5S14.48 7 12 7z" fill="none" />\n</svg>\n'
                 }),
                 ot = new c.LabIcon({
                     name: "jupytercad:visibilityOffIcon",
-                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 0 24 24" width="24">\n    <path d="M0 0h24v24H0V0zm0 0h24v24H0V0zm0 0h24v24H0V0zm0 0h24v24H0V0z" fill="none" />\n    <path class="jp-icon3" d="M12 6c3.79 0 7.17 2.13 8.82 5.5-.59 1.22-1.42 2.27-2.41 3.12l1.41 1.41c1.39-1.23 2.49-2.77 3.18-4.53C21.27 7.11 17 4 12 4c-1.27 0-2.49.2-3.64.57l1.65 1.65C10.66 6.09 11.32 6 12 6zm-1.07 1.14L13 9.21c.57.25 1.03.71 1.28 1.28l2.07 2.07c.08-.34.14-.7.14-1.07C16.5 9.01 14.48 7 12 7c-.37 0-.72.05-1.07.14zM2.01 3.87l2.68 2.68C3.06 7.83 1.77 9.53 1 11.5 2.73 15.89 7 19 12 19c1.52 0 2.98-.29 4.32-.82l3.42 3.42 1.41-1.41L3.42 2.45 2.01 3.87zm7.5 7.5l2.61 2.61c-.04.01-.08.02-.12.02-1.38 0-2.5-1.12-2.5-2.5 0-.05.01-.08.01-.13zm-3.4-3.4l1.75 1.75c-.23.55-.36 1.15-.36 1.78 0 2.48 2.02 4.5 4.5 4.5.63 0 1.23-.13 1.77-.36l.98.98c-.88.24-1.8.38-2.75.38-3.79 0-7.17-2.13-8.82-5.5.7-1.43 1.72-2.61 2.93-3.53z" fill="none" />\n</svg>'
+                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 0 24 24" width="24">\n    <path d="M0 0h24v24H0V0zm0 0h24v24H0V0zm0 0h24v24H0V0zm0 0h24v24H0V0z" fill="none" />\n    <path class="jp-icon3" d="M12 6c3.79 0 7.17 2.13 8.82 5.5-.59 1.22-1.42 2.27-2.41 3.12l1.41 1.41c1.39-1.23 2.49-2.77 3.18-4.53C21.27 7.11 17 4 12 4c-1.27 0-2.49.2-3.64.57l1.65 1.65C10.66 6.09 11.32 6 12 6zm-1.07 1.14L13 9.21c.57.25 1.03.71 1.28 1.28l2.07 2.07c.08-.34.14-.7.14-1.07C16.5 9.01 14.48 7 12 7c-.37 0-.72.05-1.07.14zM2.01 3.87l2.68 2.68C3.06 7.83 1.77 9.53 1 11.5 2.73 15.89 7 19 12 19c1.52 0 2.98-.29 4.32-.82l3.42 3.42 1.41-1.41L3.42 2.45 2.01 3.87zm7.5 7.5l2.61 2.61c-.04.01-.08.02-.12.02-1.38 0-2.5-1.12-2.5-2.5 0-.05.01-.08.01-.13zm-3.4-3.4l1.75 1.75c-.23.55-.36 1.15-.36 1.78 0 2.48 2.02 4.5 4.5 4.5.63 0 1.23-.13 1.77-.36l.98.98c-.88.24-1.8.38-2.75.38-3.79 0-7.17-2.13-8.82-5.5.7-1.43 1.72-2.61 2.93-3.53z" fill="none" />\n</svg>\n'
                 }),
                 it = {
                     labTheme: {
                         text: {
                             fontSize: "14px",
                             fontFamily: "var(--jp-ui-font-family)",
                             color: "var(--jp-ui-font-color1)",
```

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/643.850e055919134443b4fa.js` & `jupytercad-0.2.1/jupytercad/labextension/static/643.850e055919134443b4fa.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js` & `jupytercad-0.2.1/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/711.2093084af91b1879c5ac.js` & `jupytercad-0.2.1/jupytercad/labextension/static/711.2093084af91b1879c5ac.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js` & `jupytercad-0.2.1/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js` & `jupytercad-0.2.1/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/733.89a6a4e0561966230286.js` & `jupytercad-0.2.1/jupytercad/labextension/static/733.89a6a4e0561966230286.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js` & `jupytercad-0.2.1/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js` & `jupytercad-0.2.1/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js` & `jupytercad-0.2.1/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/816.00326e9e5f2436d0d67f.js` & `jupytercad-0.2.1/jupytercad/labextension/static/816.00326e9e5f2436d0d67f.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js` & `jupytercad-0.2.1/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/842.116bb3340768f53ea709.js` & `jupytercad-0.2.1/jupytercad/labextension/static/842.116bb3340768f53ea709.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js` & `jupytercad-0.2.1/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js` & `jupytercad-0.2.1/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/955.a084e75defa008fca238.js` & `jupytercad-0.2.1/jupytercad/labextension/static/955.a084e75defa008fca238.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js` & `jupytercad-0.2.1/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/jupytercad.opencascade.wasm` & `jupytercad-0.2.1/jupytercad/labextension/static/jupytercad.opencascade.wasm`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/remoteEntry.3d94847557dd157537a5.js` & `jupytercad-0.2.1/jupytercad/labextension/static/remoteEntry.e8080149ddd48fae3b49.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, d, n, o, f, l, c, u, i, s, b, p, h, m, v, y, j, g, P, w, _, x, O, S = {
-            8634: (e, r, t) => {
+            21306: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(651), t.e(78), t.e(963), t.e(29), t.e(662), t.e(930), t.e(647), t.e(387), t.e(544)]).then((() => () => t(38790))),
                         "./extension": () => Promise.all([t.e(651), t.e(78), t.e(963), t.e(29), t.e(662), t.e(930), t.e(647), t.e(387), t.e(544)]).then((() => () => t(38790))),
                         "./style": () => Promise.all([t.e(847), t.e(643)]).then((() => () => t(76643)))
                     },
                     d = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -70,15 +70,15 @@
         294: "454be2b126053f634b3b",
         358: "45fb46ea24bb44ba7fa9",
         379: "5df518c877987fc7ca0c",
         387: "4b2774fa163561009f77",
         391: "b0cccbdfb86a0129bdc4",
         406: "5ed89c99d9b3043c85c0",
         422: "39a95e19d3a414516796",
-        544: "5c918f69ee5ea6e28e28",
+        544: "f90bd90ee4b5fdf48162",
         643: "850e055919134443b4fa",
         647: "de9d2ebc968580177a57",
         651: "3736a4bd9cf2725cc067",
         662: "5542c04bd2cba2e92de1",
         711: "2093084af91b1879c5ac",
         712: "3d4b32523dbb4dff584d",
         730: "5a8c1aad713514a0a596",
@@ -104,15 +104,15 @@
         294: "454be2b126053f634b3b",
         358: "45fb46ea24bb44ba7fa9",
         379: "5df518c877987fc7ca0c",
         387: "4b2774fa163561009f77",
         391: "b0cccbdfb86a0129bdc4",
         406: "5ed89c99d9b3043c85c0",
         422: "39a95e19d3a414516796",
-        544: "5c918f69ee5ea6e28e28",
+        544: "f90bd90ee4b5fdf48162",
         643: "850e055919134443b4fa",
         647: "de9d2ebc968580177a57",
         651: "3736a4bd9cf2725cc067",
         662: "5542c04bd2cba2e92de1",
         711: "2093084af91b1879c5ac",
         712: "3d4b32523dbb4dff584d",
         730: "5a8c1aad713514a0a596",
@@ -183,15 +183,15 @@
                         (!f || !f.loaded && (!a != !f.eager ? a : o > f.from)) && (d[r] = {
                             get: t,
                             from: o,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (f("@deathbeds/jupyterlab-rjsf", "1.1.0", (() => Promise.all([k.e(184), k.e(29), k.e(662), k.e(294), k.e(387)]).then((() => () => k(46184))))), f("@jupyter/docprovider", "1.0.0-alpha.8", (() => Promise.all([k.e(78), k.e(711), k.e(662), k.e(930), k.e(647)]).then((() => () => k(44711))))), f("@jupytercad/jupytercad-extension", "0.2.0-alpha.0", (() => Promise.all([k.e(651), k.e(78), k.e(963), k.e(29), k.e(662), k.e(930), k.e(647), k.e(387), k.e(544)]).then((() => () => k(38790))))), f("@naisutech/react-tree", "3.1.0", (() => Promise.all([k.e(733), k.e(29), k.e(778), k.e(406)]).then((() => () => k(74733))))), f("@rjsf/core", "3.2.1", (() => Promise.all([k.e(651), k.e(842), k.e(29)]).then((() => () => k(28842))))), f("d3-color", "3.1.0", (() => k.e(52).then((() => () => k(37052))))), f("styled-components", "5.3.10", (() => Promise.all([k.e(761), k.e(29), k.e(816)]).then((() => () => k(69761))))), f("three-mesh-bvh", "0.5.24", (() => Promise.all([k.e(422), k.e(391)]).then((() => () => k(31422))))), f("three", "0.135.0", (() => k.e(955).then((() => () => k(12955))))), f("uuid", "8.3.2", (() => k.e(712).then((() => () => k(67712)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (f("@deathbeds/jupyterlab-rjsf", "1.1.0", (() => Promise.all([k.e(184), k.e(29), k.e(662), k.e(294), k.e(387)]).then((() => () => k(46184))))), f("@jupyter/docprovider", "1.0.0-alpha.8", (() => Promise.all([k.e(78), k.e(711), k.e(662), k.e(930), k.e(647)]).then((() => () => k(44711))))), f("@jupytercad/jupytercad-extension", "0.2.1", (() => Promise.all([k.e(651), k.e(78), k.e(963), k.e(29), k.e(662), k.e(930), k.e(647), k.e(387), k.e(544)]).then((() => () => k(38790))))), f("@naisutech/react-tree", "3.1.0", (() => Promise.all([k.e(733), k.e(29), k.e(778), k.e(406)]).then((() => () => k(74733))))), f("@rjsf/core", "3.2.1", (() => Promise.all([k.e(651), k.e(842), k.e(29)]).then((() => () => k(28842))))), f("d3-color", "3.1.0", (() => k.e(52).then((() => () => k(37052))))), f("styled-components", "5.3.10", (() => Promise.all([k.e(761), k.e(29), k.e(816)]).then((() => () => k(69761))))), f("three-mesh-bvh", "0.5.24", (() => Promise.all([k.e(422), k.e(391)]).then((() => () => k(31422))))), f("three", "0.135.0", (() => k.e(955).then((() => () => k(12955))))), f("uuid", "8.3.2", (() => k.e(712).then((() => () => k(67712)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -399,10 +399,10 @@
                     f && f(k)
                 }
                 for (r && r(t); l < n.length; l++) d = n[l], k.o(e, d) && e[d] && e[d][0](), e[d] = 0
             },
             t = self.webpackChunk_jupytercad_jupytercad_extension = self.webpackChunk_jupytercad_jupytercad_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), k.nc = void 0;
-    var T = k(8634);
+    var T = k(21306);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupytercad/jupytercad-extension"] = T
 })();
```

### Comparing `jupytercad-0.2.0/jupytercad/labextension/static/third-party-licenses.json` & `jupytercad-0.2.1/jupytercad/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/box.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/box.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  box.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 from . import placement
```

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/cone.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/sphere.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # generated by datamodel-codegen:
-#   filename:  cone.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   filename:  sphere.json
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 from . import placement
 
 
-class ICone(BaseModel):
+class ISphere(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    Radius1: float = Field(..., description='The bottom radius of the cone')
-    Radius2: float = Field(..., description='The top radius of the cone')
-    Height: float = Field(..., description='The height of the cone')
-    Angle: float = Field(..., description='The angle of the cone')
+    Radius: float = Field(..., description='The radius of the sphere')
+    Angle1: float = Field(..., description='The angle of the sphere')
+    Angle2: float = Field(..., description='The angle of the sphere')
+    Angle3: float = Field(..., description='The angle of the sphere')
     Placement: placement.Model
```

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/cylinder.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/cylinder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  cylinder.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 from . import placement
```

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/extrusion.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/extrusion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  extrusion.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from typing import List
 
 from pydantic import BaseModel, Extra, Field
```

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/geomCircle.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/geomCircle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  geomCircle.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 
 class IGeomCircle(BaseModel):
```

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/geomLineSegment.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/geomLineSegment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  geomLineSegment.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 
 class IGeomLineSegment(BaseModel):
```

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/jcad.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/jcad.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  jcad.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Extra, Field, constr
```

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/sketch.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/sketch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  sketch.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Extra, Field
```

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/sphere.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/cone.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # generated by datamodel-codegen:
-#   filename:  sphere.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   filename:  cone.json
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 from . import placement
 
 
-class ISphere(BaseModel):
+class ICone(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    Radius: float = Field(..., description='The radius of the sphere')
-    Angle1: float = Field(..., description='The angle of the sphere')
-    Angle2: float = Field(..., description='The angle of the sphere')
-    Angle3: float = Field(..., description='The angle of the sphere')
+    Radius1: float = Field(..., description='The bottom radius of the cone')
+    Radius2: float = Field(..., description='The top radius of the cone')
+    Height: float = Field(..., description='The height of the cone')
+    Angle: float = Field(..., description='The angle of the cone')
     Placement: placement.Model
```

### Comparing `jupytercad-0.2.0/jupytercad/notebook/objects/_schema/torus.py` & `jupytercad-0.2.1/jupytercad/notebook/objects/_schema/torus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  torus.json
-#   timestamp: 2023-06-02T10:14:00+00:00
+#   timestamp: 2023-06-03T08:59:50+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 from . import placement
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/package.json` & `jupytercad-0.2.1/packages/jupytercad-app/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9611204013377926%*

 * *Differences: {"'dependencies'": "{'@jupytercad/jupytercad-extension': '^0.2.1'}", "'version'": "'0.2.1'"}*

```diff
@@ -4,15 +4,15 @@
     },
     "dependencies": {
         "@codemirror/state": "^6.2.0",
         "@codemirror/view": "^6.9.3",
         "@jupyter/collaboration": "^1.0.0-alpha.7",
         "@jupyter/docprovider": "^1.0.0-alpha.8",
         "@jupyter/ydoc": "^0.3.4 || ^1.0.2",
-        "@jupytercad/jupytercad-extension": "^0.2.0-alpha.0",
+        "@jupytercad/jupytercad-extension": "^0.2.1",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/application-extension": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/apputils-extension": "^4.0.0",
         "@jupyterlab/codemirror": "^4.0.0",
         "@jupyterlab/codemirror-extension": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
@@ -82,9 +82,9 @@
         "watch:webpack": "webpack --watch"
     },
     "sideEffects": [
         "style/**/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.2.0-alpha.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/tsconfig.tsbuildinfo` & `jupytercad-0.2.1/packages/jupytercad-app/tsconfig.tsbuildinfo`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/webpack.config.js` & `jupytercad-0.2.1/packages/jupytercad-app/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/build/main.js` & `jupytercad-0.2.1/packages/jupytercad-app/build/main.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/build/style.js` & `jupytercad-0.2.1/packages/jupytercad-app/build/style.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/build/app/app.d.ts` & `jupytercad-0.2.1/packages/jupytercad-app/build/app/app.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/build/app/app.js` & `jupytercad-0.2.1/packages/jupytercad-app/build/app/app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/browser/index.js` & `jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/browser/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/launcher/index.js` & `jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/launcher/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/index.js` & `jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.js` & `jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.js` & `jupytercad-0.2.1/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/lib/main.js` & `jupytercad-0.2.1/packages/jupytercad-app/lib/main.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/lib/app/app.d.ts` & `jupytercad-0.2.1/packages/jupytercad-app/lib/app/app.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/lib/app/app.js` & `jupytercad-0.2.1/packages/jupytercad-app/lib/app/app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/browser/index.js` & `jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/browser/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/launcher/index.js` & `jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/launcher/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js` & `jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.js` & `jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.js` & `jupytercad-0.2.1/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/src/main.ts` & `jupytercad-0.2.1/packages/jupytercad-app/src/main.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/src/app/app.ts` & `jupytercad-0.2.1/packages/jupytercad-app/src/app/app.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/browser/index.ts` & `jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/browser/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/launcher/index.ts` & `jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/launcher/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts` & `jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/mainmenu/menuWidget.ts` & `jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/mainmenu/menuWidget.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/src/app/plugins/mainmenu/userWidget.tsx` & `jupytercad-0.2.1/packages/jupytercad-app/src/app/plugins/mainmenu/userWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-app/style/base.css` & `jupytercad-0.2.1/packages/jupytercad-app/style/base.css`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/extension.webpack.config.js` & `jupytercad-0.2.1/packages/jupytercad-extension/extension.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/package.json` & `jupytercad-0.2.1/packages/jupytercad-extension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.974609375%*

 * *Differences: {"'dependencies'": "{'@jupytercad/jupytercad-opencascade': '^0.2.1'}", "'version'": "'0.2.1'"}*

```diff
@@ -6,15 +6,15 @@
         "url": "https://github.com/QuantStack/jupytercad/issues"
     },
     "dependencies": {
         "@deathbeds/jupyterlab-rjsf": "^1.1.0",
         "@jupyter/collaboration": "^1.0.0-alpha.7",
         "@jupyter/docprovider": "^1.0.0-alpha.8",
         "@jupyter/ydoc": "^0.3.4 || ^1.0.2",
-        "@jupytercad/jupytercad-opencascade": "^0.2.0-alpha.0",
+        "@jupytercad/jupytercad-opencascade": "^0.2.1",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -108,9 +108,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0-alpha.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/schema.js` & `jupytercad-0.2.1/packages/jupytercad-extension/schema.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/tsconfig.tsbuildinfo` & `jupytercad-0.2.1/packages/jupytercad-extension/tsconfig.tsbuildinfo`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999728732638888%*

 * *Differences: {"'program'": "{'fileInfos': {insert: [(656, "*

 * *              "'804b1f55cc6092cbae7d61fd9eae3c8b8ecc49d4839ed508c4ed6977430c487e')], delete: "*

 * *              '[656]}}'}*

```diff
@@ -11779,15 +11779,15 @@
                 "signature": "b0b2e26f6c0af31421caacaa42d50526b8472ab99c53a2e084623ba38f018cf1",
                 "version": "7d699ee11551656103fc9d2aa490dbba77007338910bfb0d1efa6e2cd95719a8"
             },
             {
                 "signature": "7b2d5be885bc8529df052b09cd46b2d783d292837815f61bbce6ea1c257c99bf",
                 "version": "2b3def2e55b1a604998b3d2b204ff5e64790974fcf9821564ec67222093337d4"
             },
-            "9c46b0ebf6d7295b23249f8d0b7d999a7b684f13686a50fbd42d0e7dc87e8dba",
+            "804b1f55cc6092cbae7d61fd9eae3c8b8ecc49d4839ed508c4ed6977430c487e",
             {
                 "signature": "5570335ff6452229406838ff2c0cf08a6736e1e1064d0c4c8dcef0dd0e490592",
                 "version": "4d72f3934a62e515ef8284df1522b9bccc3c2bbc0a8c81329ee5c11ba9300e1f"
             },
             "9f3c5498245c38c9016a369795ec5ef1768d09db63643c8dba9656e5ab294825",
             "2d225e7bda2871c066a7079c88174340950fb604f624f2586d3ea27bb9e5f4ff",
             "6a785f84e63234035e511817dd48ada756d984dd8f9344e56eb8b2bdcd8fd001",
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/worker.webpack.config.js` & `jupytercad-0.2.1/packages/jupytercad-extension/worker.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/commands.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/commands.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/commands.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/commands.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/factory.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/factory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/factory.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/factory.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/formdialog.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/formdialog.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/formdialog.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/formdialog.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/index.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/mainview.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/mainview.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/mainview.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/mainview.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/model.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/model.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/tools.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/tools.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/tools.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/tools.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/types.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/types.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/widget.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/widget.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/widget.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/widget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/_interface/forms.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/_interface/forms.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -343,67 +343,14 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::MultiFuse": {
-        "type": "object",
-        "required": [
-            "Shapes",
-            "Refine",
-            "Placement"
-        ],
-        "additionalProperties": false,
-        "properties": {
-            "Shapes": {
-                "type": "array",
-                "description": "The shapes of the individual elements",
-                "fcType": "App::PropertyLinkList",
-                "items": {
-                    "type": "string"
-                }
-            },
-            "Refine": {
-                "type": "boolean",
-                "description": "Refine shape"
-            },
-            "Placement": {
-                "type": "object",
-                "description": "Placement of the box",
-                "additionalProperties": false,
-                "required": [
-                    "Position",
-                    "Axis",
-                    "Angle"
-                ],
-                "properties": {
-                    "Position": {
-                        "type": "array",
-                        "description": "Position of the Placement",
-                        "items": {
-                            "type": "number"
-                        }
-                    },
-                    "Axis": {
-                        "type": "array",
-                        "description": "Axis of the Placement",
-                        "items": {
-                            "type": "number"
-                        }
-                    },
-                    "Angle": {
-                        "type": "number",
-                        "description": "Angle of the Placement"
-                    }
-                }
-            }
-        }
-    },
     "Part::Extrusion": {
         "type": "object",
         "required": [
             "Base",
             "Dir",
             "LengthFwd",
             "LengthRev",
@@ -464,26 +411,26 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::MultiCommon": {
+    "Part::MultiFuse": {
         "type": "object",
         "required": [
             "Shapes",
             "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
             "Shapes": {
                 "type": "array",
-                "description": "The objects to intersect",
+                "description": "The shapes of the individual elements",
                 "fcType": "App::PropertyLinkList",
                 "items": {
                     "type": "string"
                 }
             },
             "Refine": {
                 "type": "boolean",
@@ -517,104 +464,34 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Sphere": {
+    "Part::MultiCommon": {
         "type": "object",
         "required": [
-            "Radius",
-            "Angle1",
-            "Angle2",
-            "Angle3",
+            "Shapes",
+            "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Radius": {
-                "type": "number",
-                "description": "The radius of the sphere"
-            },
-            "Angle1": {
-                "type": "number",
-                "description": "The angle of the sphere"
-            },
-            "Angle2": {
-                "type": "number",
-                "description": "The angle of the sphere"
-            },
-            "Angle3": {
-                "type": "number",
-                "description": "The angle of the sphere"
-            },
-            "Placement": {
-                "type": "object",
-                "description": "Placement of the box",
-                "additionalProperties": false,
-                "required": [
-                    "Position",
-                    "Axis",
-                    "Angle"
-                ],
-                "properties": {
-                    "Position": {
-                        "type": "array",
-                        "description": "Position of the Placement",
-                        "items": {
-                            "type": "number"
-                        }
-                    },
-                    "Axis": {
-                        "type": "array",
-                        "description": "Axis of the Placement",
-                        "items": {
-                            "type": "number"
-                        }
-                    },
-                    "Angle": {
-                        "type": "number",
-                        "description": "Angle of the Placement"
-                    }
+            "Shapes": {
+                "type": "array",
+                "description": "The objects to intersect",
+                "fcType": "App::PropertyLinkList",
+                "items": {
+                    "type": "string"
                 }
-            }
-        }
-    },
-    "Part::Torus": {
-        "type": "object",
-        "required": [
-            "Radius1",
-            "Radius2",
-            "Angle1",
-            "Angle2",
-            "Angle3",
-            "Placement"
-        ],
-        "additionalProperties": false,
-        "properties": {
-            "Radius1": {
-                "type": "number",
-                "description": "The radius of the torus"
-            },
-            "Radius2": {
-                "type": "number",
-                "description": "The radius of the torus"
             },
-            "Angle1": {
-                "type": "number",
-                "description": "The angle of the torus"
-            },
-            "Angle2": {
-                "type": "number",
-                "description": "The angle of the torus"
-            },
-            "Angle3": {
-                "type": "number",
-                "description": "The angle of the torus"
+            "Refine": {
+                "type": "boolean",
+                "description": "Refine shape"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -792,14 +669,137 @@
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
+                    "Axis",
+                    "Angle"
+                ],
+                "properties": {
+                    "Position": {
+                        "type": "array",
+                        "description": "Position of the Placement",
+                        "items": {
+                            "type": "number"
+                        }
+                    },
+                    "Axis": {
+                        "type": "array",
+                        "description": "Axis of the Placement",
+                        "items": {
+                            "type": "number"
+                        }
+                    },
+                    "Angle": {
+                        "type": "number",
+                        "description": "Angle of the Placement"
+                    }
+                }
+            }
+        }
+    },
+    "Part::Sphere": {
+        "type": "object",
+        "required": [
+            "Radius",
+            "Angle1",
+            "Angle2",
+            "Angle3",
+            "Placement"
+        ],
+        "additionalProperties": false,
+        "properties": {
+            "Radius": {
+                "type": "number",
+                "description": "The radius of the sphere"
+            },
+            "Angle1": {
+                "type": "number",
+                "description": "The angle of the sphere"
+            },
+            "Angle2": {
+                "type": "number",
+                "description": "The angle of the sphere"
+            },
+            "Angle3": {
+                "type": "number",
+                "description": "The angle of the sphere"
+            },
+            "Placement": {
+                "type": "object",
+                "description": "Placement of the box",
+                "additionalProperties": false,
+                "required": [
+                    "Position",
+                    "Axis",
+                    "Angle"
+                ],
+                "properties": {
+                    "Position": {
+                        "type": "array",
+                        "description": "Position of the Placement",
+                        "items": {
+                            "type": "number"
+                        }
+                    },
+                    "Axis": {
+                        "type": "array",
+                        "description": "Axis of the Placement",
+                        "items": {
+                            "type": "number"
+                        }
+                    },
+                    "Angle": {
+                        "type": "number",
+                        "description": "Angle of the Placement"
+                    }
+                }
+            }
+        }
+    },
+    "Part::Torus": {
+        "type": "object",
+        "required": [
+            "Radius1",
+            "Radius2",
+            "Angle1",
+            "Angle2",
+            "Angle3",
+            "Placement"
+        ],
+        "additionalProperties": false,
+        "properties": {
+            "Radius1": {
+                "type": "number",
+                "description": "The radius of the torus"
+            },
+            "Radius2": {
+                "type": "number",
+                "description": "The radius of the torus"
+            },
+            "Angle1": {
+                "type": "number",
+                "description": "The angle of the torus"
+            },
+            "Angle2": {
+                "type": "number",
+                "description": "The angle of the torus"
+            },
+            "Angle3": {
+                "type": "number",
+                "description": "The angle of the torus"
+            },
+            "Placement": {
+                "type": "object",
+                "description": "Placement of the box",
+                "additionalProperties": false,
+                "required": [
+                    "Position",
                     "Axis",
                     "Angle"
                 ],
                 "properties": {
                     "Position": {
                         "type": "array",
                         "description": "Position of the Placement",
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/message.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/message.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/model.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/model.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/annotation/view.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/annotation/view.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/fcplugin/modelfactory.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/fcplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/fcplugin/plugins.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/fcplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/jcadplugin/plugins.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/jcadplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/index.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/model.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/view.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/view.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/annotations.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/annotations.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/annotations.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/annotations.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/formbuilder.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/formbuilder.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/leftpanel.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/leftpanel.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/model.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/model.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/objectproperties.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/objectproperties.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/objecttree.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/objecttree.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/panelview/rightpanel.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/panelview/rightpanel.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/box.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/box.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/cone.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/cone.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/cut.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/cut.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/cylinder.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/cylinder.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/extrusion.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/extrusion.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/fuse.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/fuse.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/geomCircle.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/geomCircle.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/geomLineSegment.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/geomLineSegment.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/intersection.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/intersection.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/jcad.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/jcad.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/placement.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/placement.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/sketch.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/sketch.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/sphere.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/sphere.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/schema/torus.json` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/schema/torus.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/helper.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/helper.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/helper.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/helper.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/panzoom.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/panzoom.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketchermodel.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketchermodel.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/sketcher/types.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/sketcher/types.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/toolbar/widget.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/toolbar/widget.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/toolbar/widget.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/toolbar/widget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/actions.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/actions.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/actions.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/actions.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/occapi.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/occapi.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/occapi.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/occapi.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/occparser.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/occparser.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/occparser.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/occparser.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/operatorcache.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/operatorcache.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/types.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/types.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/worker.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/worker.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js` & `jupytercad-0.2.1/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/commands.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/factory.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/formdialog.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/formdialog.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/index.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/mainview.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/mainview.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/model.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/tools.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/tools.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/types.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/widget.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/box.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/box.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/cone.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/cone.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/cut.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/cut.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/cylinder.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/cylinder.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/extrusion.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/extrusion.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/forms.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/forms.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -343,67 +343,14 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::MultiFuse": {
-        "type": "object",
-        "required": [
-            "Shapes",
-            "Refine",
-            "Placement"
-        ],
-        "additionalProperties": false,
-        "properties": {
-            "Shapes": {
-                "type": "array",
-                "description": "The shapes of the individual elements",
-                "fcType": "App::PropertyLinkList",
-                "items": {
-                    "type": "string"
-                }
-            },
-            "Refine": {
-                "type": "boolean",
-                "description": "Refine shape"
-            },
-            "Placement": {
-                "type": "object",
-                "description": "Placement of the box",
-                "additionalProperties": false,
-                "required": [
-                    "Position",
-                    "Axis",
-                    "Angle"
-                ],
-                "properties": {
-                    "Position": {
-                        "type": "array",
-                        "description": "Position of the Placement",
-                        "items": {
-                            "type": "number"
-                        }
-                    },
-                    "Axis": {
-                        "type": "array",
-                        "description": "Axis of the Placement",
-                        "items": {
-                            "type": "number"
-                        }
-                    },
-                    "Angle": {
-                        "type": "number",
-                        "description": "Angle of the Placement"
-                    }
-                }
-            }
-        }
-    },
     "Part::Extrusion": {
         "type": "object",
         "required": [
             "Base",
             "Dir",
             "LengthFwd",
             "LengthRev",
@@ -464,26 +411,26 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::MultiCommon": {
+    "Part::MultiFuse": {
         "type": "object",
         "required": [
             "Shapes",
             "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
             "Shapes": {
                 "type": "array",
-                "description": "The objects to intersect",
+                "description": "The shapes of the individual elements",
                 "fcType": "App::PropertyLinkList",
                 "items": {
                     "type": "string"
                 }
             },
             "Refine": {
                 "type": "boolean",
@@ -517,104 +464,34 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Sphere": {
+    "Part::MultiCommon": {
         "type": "object",
         "required": [
-            "Radius",
-            "Angle1",
-            "Angle2",
-            "Angle3",
+            "Shapes",
+            "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Radius": {
-                "type": "number",
-                "description": "The radius of the sphere"
-            },
-            "Angle1": {
-                "type": "number",
-                "description": "The angle of the sphere"
-            },
-            "Angle2": {
-                "type": "number",
-                "description": "The angle of the sphere"
-            },
-            "Angle3": {
-                "type": "number",
-                "description": "The angle of the sphere"
-            },
-            "Placement": {
-                "type": "object",
-                "description": "Placement of the box",
-                "additionalProperties": false,
-                "required": [
-                    "Position",
-                    "Axis",
-                    "Angle"
-                ],
-                "properties": {
-                    "Position": {
-                        "type": "array",
-                        "description": "Position of the Placement",
-                        "items": {
-                            "type": "number"
-                        }
-                    },
-                    "Axis": {
-                        "type": "array",
-                        "description": "Axis of the Placement",
-                        "items": {
-                            "type": "number"
-                        }
-                    },
-                    "Angle": {
-                        "type": "number",
-                        "description": "Angle of the Placement"
-                    }
+            "Shapes": {
+                "type": "array",
+                "description": "The objects to intersect",
+                "fcType": "App::PropertyLinkList",
+                "items": {
+                    "type": "string"
                 }
-            }
-        }
-    },
-    "Part::Torus": {
-        "type": "object",
-        "required": [
-            "Radius1",
-            "Radius2",
-            "Angle1",
-            "Angle2",
-            "Angle3",
-            "Placement"
-        ],
-        "additionalProperties": false,
-        "properties": {
-            "Radius1": {
-                "type": "number",
-                "description": "The radius of the torus"
-            },
-            "Radius2": {
-                "type": "number",
-                "description": "The radius of the torus"
             },
-            "Angle1": {
-                "type": "number",
-                "description": "The angle of the torus"
-            },
-            "Angle2": {
-                "type": "number",
-                "description": "The angle of the torus"
-            },
-            "Angle3": {
-                "type": "number",
-                "description": "The angle of the torus"
+            "Refine": {
+                "type": "boolean",
+                "description": "Refine shape"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -792,14 +669,137 @@
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
+                    "Axis",
+                    "Angle"
+                ],
+                "properties": {
+                    "Position": {
+                        "type": "array",
+                        "description": "Position of the Placement",
+                        "items": {
+                            "type": "number"
+                        }
+                    },
+                    "Axis": {
+                        "type": "array",
+                        "description": "Axis of the Placement",
+                        "items": {
+                            "type": "number"
+                        }
+                    },
+                    "Angle": {
+                        "type": "number",
+                        "description": "Angle of the Placement"
+                    }
+                }
+            }
+        }
+    },
+    "Part::Sphere": {
+        "type": "object",
+        "required": [
+            "Radius",
+            "Angle1",
+            "Angle2",
+            "Angle3",
+            "Placement"
+        ],
+        "additionalProperties": false,
+        "properties": {
+            "Radius": {
+                "type": "number",
+                "description": "The radius of the sphere"
+            },
+            "Angle1": {
+                "type": "number",
+                "description": "The angle of the sphere"
+            },
+            "Angle2": {
+                "type": "number",
+                "description": "The angle of the sphere"
+            },
+            "Angle3": {
+                "type": "number",
+                "description": "The angle of the sphere"
+            },
+            "Placement": {
+                "type": "object",
+                "description": "Placement of the box",
+                "additionalProperties": false,
+                "required": [
+                    "Position",
+                    "Axis",
+                    "Angle"
+                ],
+                "properties": {
+                    "Position": {
+                        "type": "array",
+                        "description": "Position of the Placement",
+                        "items": {
+                            "type": "number"
+                        }
+                    },
+                    "Axis": {
+                        "type": "array",
+                        "description": "Axis of the Placement",
+                        "items": {
+                            "type": "number"
+                        }
+                    },
+                    "Angle": {
+                        "type": "number",
+                        "description": "Angle of the Placement"
+                    }
+                }
+            }
+        }
+    },
+    "Part::Torus": {
+        "type": "object",
+        "required": [
+            "Radius1",
+            "Radius2",
+            "Angle1",
+            "Angle2",
+            "Angle3",
+            "Placement"
+        ],
+        "additionalProperties": false,
+        "properties": {
+            "Radius1": {
+                "type": "number",
+                "description": "The radius of the torus"
+            },
+            "Radius2": {
+                "type": "number",
+                "description": "The radius of the torus"
+            },
+            "Angle1": {
+                "type": "number",
+                "description": "The angle of the torus"
+            },
+            "Angle2": {
+                "type": "number",
+                "description": "The angle of the torus"
+            },
+            "Angle3": {
+                "type": "number",
+                "description": "The angle of the torus"
+            },
+            "Placement": {
+                "type": "object",
+                "description": "Placement of the box",
+                "additionalProperties": false,
+                "required": [
+                    "Position",
                     "Axis",
                     "Angle"
                 ],
                 "properties": {
                     "Position": {
                         "type": "array",
                         "description": "Position of the Placement",
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/fuse.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/fuse.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/geomCircle.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/geomCircle.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/intersection.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/intersection.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/jcad.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/jcad.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/sketch.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/sketch.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/sphere.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/sphere.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/_interface/torus.d.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/_interface/torus.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/annotation/message.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/annotation/message.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/annotation/model.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/annotation/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/annotation/view.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/annotation/view.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/fcplugin/modelfactory.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/fcplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/fcplugin/plugins.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/fcplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/jcadplugin/plugins.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/jcadplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/index.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/model.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/token.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/token.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/view.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/view.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/annotations.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/annotations.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/formbuilder.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/formbuilder.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/leftpanel.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/leftpanel.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/model.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/objectproperties.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/objectproperties.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/objecttree.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/objecttree.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/panelview/rightpanel.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/panelview/rightpanel.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/box.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/box.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/cone.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/cone.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/cut.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/cut.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/cylinder.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/cylinder.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/extrusion.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/extrusion.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/fuse.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/fuse.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/geomCircle.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/geomCircle.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/geomLineSegment.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/geomLineSegment.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/intersection.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/intersection.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/jcad.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/jcad.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/placement.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/placement.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/sketch.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/sketch.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/sphere.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/sphere.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/schema/torus.json` & `jupytercad-0.2.1/packages/jupytercad-extension/src/schema/torus.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/helper.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/helper.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/panzoom.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/panzoom.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/sketchermodel.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/sketchermodel.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/types.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/sketcher/elements/line.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/sketcher/elements/line.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/toolbar/widget.tsx` & `jupytercad-0.2.1/packages/jupytercad-extension/src/toolbar/widget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/worker/actions.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/worker/actions.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/worker/occapi.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/worker/occapi.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/worker/occparser.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/worker/occparser.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/worker/operatorcache.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/worker/operatorcache.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/worker/types.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/worker/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/worker/worker.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/worker/worker.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts` & `jupytercad-0.2.1/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/base.css` & `jupytercad-0.2.1/packages/jupytercad-extension/style/base.css`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/axes.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/axes.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/box.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/box.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/cone.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/cone.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/cut.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/cut.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/cylinder.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/cylinder.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/extrusion.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/extrusion.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/intersection.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/intersection.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/jvcontrol.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/jvcontrol.svg`

 * *Files 0% similar despite different names*

```diff
@@ -59,8 +59,8 @@
 000003a0: 2e36 336c 342c 322e 3333 5631 372e 3137  .63l4,2.33V17.17
 000003b0: 7a20 4d31 322c 3130 2e38 344c 382e 3034  z M12,10.84L8.04
 000003c0: 2c38 2e35 334c 3132 2c36 2e32 356c 332e  ,8.53L12,6.25l3.
 000003d0: 3936 2c32 2e32 384c 3132 2c31 302e 3834  96,2.28L12,10.84
 000003e0: 7a20 4d31 372c 3134 2e38 376c 2d34 2c32  z M17,14.87l-4,2
 000003f0: 2e33 762d 342e 366c 342d 322e 3333 5631  .3v-4.6l4-2.33V1
 00000400: 342e 3837 7a22 2f3e 3c2f 673e 3c2f 673e  4.87z"/></g></g>
-00000410: 3c2f 7376 673e                           </svg>
+00000410: 3c2f 7376 673e 0a                        </svg>.
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/sphere.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/sphere.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/torus.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/torus.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/union.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/union.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/visibility.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/visibility.svg`

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 00000190: 2e35 2d32 2e35 5331 302e 3632 2039 2031  .5-2.5S10.62 9 1
 000001a0: 3220 396d 302d 3263 2d32 2e34 3820 302d  2 9m0-2c-2.48 0-
 000001b0: 342e 3520 322e 3032 2d34 2e35 2034 2e35  4.5 2.02-4.5 4.5
 000001c0: 5339 2e35 3220 3136 2031 3220 3136 7334  S9.52 16 12 16s4
 000001d0: 2e35 2d32 2e30 3220 342e 352d 342e 3553  .5-2.02 4.5-4.5S
 000001e0: 3134 2e34 3820 3720 3132 2037 7a22 2066  14.48 7 12 7z" f
 000001f0: 696c 6c3d 226e 6f6e 6522 202f 3e0a 3c2f  ill="none" />.</
-00000200: 7376 673e                                svg>
+00000200: 7376 673e 0a                             svg>.
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-extension/style/icon/visibilityOff.svg` & `jupytercad-0.2.1/packages/jupytercad-extension/style/icon/visibilityOff.svg`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 00000320: 312e 3233 2d2e 3133 2031 2e37 372d 2e33  1.23-.13 1.77-.3
 00000330: 366c 2e39 382e 3938 632d 2e38 382e 3234  6l.98.98c-.88.24
 00000340: 2d31 2e38 2e33 382d 322e 3735 2e33 382d  -1.8.38-2.75.38-
 00000350: 332e 3739 2030 2d37 2e31 372d 322e 3133  3.79 0-7.17-2.13
 00000360: 2d38 2e38 322d 352e 352e 372d 312e 3433  -8.82-5.5.7-1.43
 00000370: 2031 2e37 322d 322e 3631 2032 2e39 332d   1.72-2.61 2.93-
 00000380: 332e 3533 7a22 2066 696c 6c3d 226e 6f6e  3.53z" fill="non
-00000390: 6522 202f 3e0a 3c2f 7376 673e            e" />.</svg>
+00000390: 6522 202f 3e0a 3c2f 7376 673e 0a         e" />.</svg>.
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-opencascade/build.yml` & `jupytercad-0.2.1/packages/jupytercad-opencascade/build.yml`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-opencascade/build_opencascade.js` & `jupytercad-0.2.1/packages/jupytercad-opencascade/build_opencascade.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-opencascade/package.json` & `jupytercad-0.2.1/packages/jupytercad-opencascade/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -33,9 +33,9 @@
     "scripts": {
         "build": "node build_opencascade.js",
         "build:prod": "node build_opencascade.js",
         "clean": "rimraf ./lib",
         "clean:all": "rimraf ./lib"
     },
     "types": "lib/jupytercad.opencascade.d.ts",
-    "version": "0.2.0-alpha.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupytercad-0.2.0/packages/jupytercad-opencascade/lib/build.yml` & `jupytercad-0.2.1/packages/jupytercad-opencascade/lib/build.yml`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts` & `jupytercad-0.2.1/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js` & `jupytercad-0.2.1/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm` & `jupytercad-0.2.1/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/.gitignore` & `jupytercad-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/LICENSE` & `jupytercad-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/README.md` & `jupytercad-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.0/pyproject.toml` & `jupytercad-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 
 [project]
 name = "jupytercad"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
-    "jupyterlab>=4.0.0",
     "jupyter_server>=2.0.6",
     "jupyter_collaboration>=1.0.0a9,<2",
     "ypywidgets>=0.1.2,<0.2.0",
     "comm>=0.1.2,<0.2.0",
-    "pydantic"
+    "pydantic",
 ]
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
@@ -44,19 +43,23 @@
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.targets.sdist]
-artifacts = ["/jupytercad/labextension", "/jupytercad/notebook/objects/_schema/*.py"]
+artifacts = [
+    "/jupytercad/labextension",
+    "/jupytercad/notebook/objects/_schema/*.py",
+    "/jupytercad/cadapp/",
+]
 exclude = ["/.github", "/binder", "node_modules", "examples", "ui-tests"]
 
 [tool.hatch.build.targets.wheel]
-artifacts = ["/jupytercad/notebook/objects/_schema/*.py"]
+artifacts = ["/jupytercad/notebook/objects/_schema/*.py", "/jupytercad/cadapp/"]
 
 [tool.hatch.build.targets.sdist.force-include]
 "./packages" = "packages"
 
 [tool.hatch.build.targets.wheel.shared-data]
 "install.json" = "share/jupyter/labextensions/@jupytercad/jupytercad-extension/install.json"
 "jupytercad/labextension" = "share/jupyter/labextensions/@jupytercad/jupytercad-extension"
@@ -82,20 +85,18 @@
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
 build_cmd = "install:extension"
 npm = ["jlpm"]
 source_dir = "src"
 build_dir = "jupytercad/labextension"
 
 [tool.jupyter-releaser.options]
-version-cmd = "python scripts/bump-version.py --force"
+version-cmd = "python scripts/bump-version.py"
 
 [tool.jupyter-releaser.hooks]
-before-bump-version = [
-    "python -m pip install hatch 'jupyterlab>=4.0.0b2'",
-]
+before-bump-version = ["python -m pip install hatch 'jupyterlab>=4.0.0'"]
 before-build-npm = [
     "python -m pip install datamodel-code-generator jupyterlab --pre -U",
     "jlpm",
     "jlpm build:prod",
 ]
 before-build-python = ["jlpm clean:all"]
```

### Comparing `jupytercad-0.2.0/PKG-INFO` & `jupytercad-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercad
-Version: 0.2.0
+Version: 0.2.1
 Summary: A JupyterLab extension for 3D modelling.
 Project-URL: Homepage, https://github.com/QuantStack/jupytercad
 Project-URL: Bug Tracker, https://github.com/QuantStack/jupytercad/issues
 Project-URL: Repository, https://github.com/QuantStack/jupytercad.git
 Author: JupyterCad contributors
 License: BSD 3-Clause License
         
@@ -49,15 +49,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: comm<0.2.0,>=0.1.2
 Requires-Dist: jupyter-collaboration<2,>=1.0.0a9
 Requires-Dist: jupyter-server>=2.0.6
-Requires-Dist: jupyterlab>=4.0.0
 Requires-Dist: pydantic
 Requires-Dist: ypywidgets<0.2.0,>=0.1.2
 Description-Content-Type: text/markdown
 
 # JupyterCAD - A JupyterLab extension for 3D geometry modeling.
 
 JupyterCAD is a JupyterLab extension for 3D geometry modeling with collaborative editing support. It is designed to allow multiple people to work on the same file at the same time, and to facilitate discussion and collaboration around the 3D shapes being created.
```

