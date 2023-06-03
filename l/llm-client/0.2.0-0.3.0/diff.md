# Comparing `tmp/llm_client-0.2.0.tar.gz` & `tmp/llm_client-0.3.0.tar.gz`

## Comparing `llm_client-0.2.0.tar` & `llm_client-0.3.0.tar`

### file list

```diff
@@ -1,227 +1,233 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 llm_client-0.2.0/.DS_Store
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 llm_client-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/base_llm_client.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/consts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_api_client/__init__.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_api_client/ai21_client.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_api_client/aleph_alpha_client.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_api_client/anthropic_client.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_api_client/base_llm_api_client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_api_client/huggingface_client.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_api_client/llm_api_client_factory.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_api_client/openai_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_client/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/llm_client/local_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/sync/__init__.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 llm_client-0.2.0/llm_client/sync/sync_llm_api_client_factory.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/pyvenv.cfg
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/activate
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/activate.csh
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/activate.fish
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/activate_this.py
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/convert-caffe2-to-onnx
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/convert-onnx-to-caffe2
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/deactivate.nu
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/docutils
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/f2py
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/f2py3
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/f2py3.11
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/httpx
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/huggingface-cli
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/isympy
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/keyring
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/markdown-it
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/normalizer
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/openai
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/pip
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/pip3
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/pip3.11
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/pkginfo
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/publish.py
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/py.test
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/pygmentize
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/pyproject-build
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2html.py
--rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2html5.py
--rwxr-xr-x   0        0        0      846 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2latex.py
--rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2man.py
--rwxr-xr-x   0        0        0      835 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2odt.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2s5.py
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rst2xml.py
--rwxr-xr-x   0        0        0      723 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/torchrun
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/tqdm
--rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/transformers-cli
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/twine
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/wheel
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/wheel-3.11
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/wheel3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/bin/wheel3.11
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/LICENSE.txt
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/README.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/README.txt
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/README.txt
--rw-r--r--   0        0        0  1346746 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/basic/README.txt
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/README.txt
--rw-r--r--   0        0        0   100224 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2
--rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_edge_colormap.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_node_colormap.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_simple_path.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/README.txt
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_expected_degree_sequence.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_karate_club.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py
--rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz
--rw-r--r--   0        0        0    33695 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/subclass/README.txt
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 llm_client-0.2.0/new_venv/share/man/man1/isympy.1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/conftest.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/test_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/ai21_client/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/ai21_client/conftest.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/ai21_client/test_ai21.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/anthropic_client/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/anthropic_client/conftest.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/huggingface_client/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/huggingface_client/conftest.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/huggingface_client/test_huggingface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/openai_client/__init__.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/openai_client/conftest.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_api_client/openai_client/test_openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_client/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_client/local_client/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_client/local_client/conftest.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/llm_client/local_client/test_local_client.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/resources/ai21/text_completion.json
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/resources/ai21/tokenize.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/resources/huggingface/text_completion.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/resources/openai/chat_completion.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/resources/openai/text_completion.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/sync/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/sync/test_sync_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.2.0/tests/test_utils/load_json_resource.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/pyvenv.cfg
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/activate
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/activate.csh
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/activate.fish
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/activate_this.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/deactivate.nu
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/normalizer
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/pip
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/pip3
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/pip3.11
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/py.test
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/wheel
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/wheel-3.11
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/wheel3
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_ai21/bin/wheel3.11
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/pyvenv.cfg
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/activate
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/activate.csh
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/activate.fish
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/activate_this.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/deactivate.nu
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/f2py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/f2py3
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/f2py3.11
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/huggingface-cli
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/normalizer
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/pip
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/pip3
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/pip3.11
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/py.test
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/tqdm
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/transformers-cli
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/wheel
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/wheel-3.11
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/wheel3
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.2.0/venv_local/bin/wheel3.11
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.2.0/LICENSE
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 llm_client-0.2.0/README.md
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 llm_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9219 2020-02-02 00:00:00.000000 llm_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 llm_client-0.3.0/.DS_Store
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 llm_client-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/base_llm_client.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/consts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_api_client/__init__.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_api_client/ai21_client.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_api_client/aleph_alpha_client.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_api_client/anthropic_client.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_api_client/base_llm_api_client.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_api_client/huggingface_client.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_api_client/llm_api_client_factory.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_api_client/openai_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_client/__init__.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/llm_client/local_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/sync/__init__.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 llm_client-0.3.0/llm_client/sync/sync_llm_api_client_factory.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/pyvenv.cfg
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/activate
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/activate.csh
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/activate.fish
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/activate_this.py
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/convert-caffe2-to-onnx
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/convert-onnx-to-caffe2
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/docutils
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/f2py
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/f2py3
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/f2py3.11
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/httpx
+-rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/huggingface-cli
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/isympy
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/keyring
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/markdown-it
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/normalizer
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/openai
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pip
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pip3
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pip3.11
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pkginfo
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/publish.py
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/py.test
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pygmentize
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pyproject-build
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pyrsa-decrypt
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pyrsa-encrypt
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pyrsa-keygen
+-rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pyrsa-priv2pub
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pyrsa-sign
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pyrsa-verify
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2html.py
+-rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      846 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2man.py
+-rwxr-xr-x   0        0        0      835 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2odt.py
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      723 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/torchrun
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/tqdm
+-rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/transformers-cli
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/twine
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/wheel
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/wheel3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/bin/wheel3.11
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/LICENSE.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/README.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/README.txt
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/README.txt
+-rw-r--r--   0        0        0  1346746 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/basic/README.txt
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/README.txt
+-rw-r--r--   0        0        0   100224 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2
+-rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_edge_colormap.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_node_colormap.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_simple_path.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/README.txt
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_expected_degree_sequence.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_karate_club.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py
+-rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz
+-rw-r--r--   0        0        0    33695 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/subclass/README.txt
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 llm_client-0.3.0/new_venv/share/man/man1/isympy.1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/conftest.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/test_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/ai21_client/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/ai21_client/conftest.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/ai21_client/test_ai21.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/anthropic_client/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/anthropic_client/conftest.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/huggingface_client/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/huggingface_client/conftest.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/huggingface_client/test_huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/openai_client/__init__.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/openai_client/conftest.py
+-rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_api_client/openai_client/test_openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_client/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_client/local_client/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_client/local_client/conftest.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/llm_client/local_client/test_local_client.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/resources/ai21/text_completion.json
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/resources/ai21/tokenize.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/resources/huggingface/text_completion.json
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/resources/openai/chat_completion.json
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/resources/openai/text_completion.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/sync/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/sync/test_sync_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.3.0/tests/test_utils/load_json_resource.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/pyvenv.cfg
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/activate
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/activate.csh
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/activate.fish
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/activate_this.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/normalizer
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/pip
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/pip3
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/pip3.11
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/py.test
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/wheel
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/wheel3
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_ai21/bin/wheel3.11
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/pyvenv.cfg
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/activate
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/activate.csh
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/activate.fish
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/activate_this.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/f2py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/f2py3
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/f2py3.11
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/huggingface-cli
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/normalizer
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/pip
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/pip3
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/pip3.11
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/py.test
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/tqdm
+-rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/transformers-cli
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/wheel
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/wheel3
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.3.0/venv_local/bin/wheel3.11
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 llm_client-0.3.0/README.md
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 llm_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 llm_client-0.3.0/PKG-INFO
```

### Comparing `llm_client-0.2.0/.DS_Store` & `llm_client-0.3.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/.github/workflows/test.yml` & `llm_client-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/llm_client/__init__.py` & `llm_client-0.3.0/llm_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 from llm_client.base_llm_client import BaseLLMClient
 
 # load api clients
 try:
     from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
     from llm_client.llm_api_client.llm_api_client_factory import LLMAPIClientFactory, LLMAPIClientType
```

### Comparing `llm_client-0.2.0/llm_client/llm_api_client/ai21_client.py` & `llm_client-0.3.0/llm_client/llm_api_client/ai21_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 class AI21Client(BaseLLMAPIClient):
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         if self._base_url is None:
             self._base_url = BASE_URL
         self._headers[AUTH_HEADER] = BEARER_TOKEN + self._api_key
 
-    async def text_completion(self, prompt: str, model: str | None = None, **kwargs) -> list[str]:
+    async def text_completion(self, prompt: str, model: str | None = None, max_tokens : int = 16, temperature : float = 0.7, **kwargs) -> list[str]:
         model = model or self._default_model
         kwargs[PROMPT_KEY] = prompt
+        kwargs["maxTokens"] = kwargs.pop("maxTokens", max_tokens)
+        kwargs["temperature"] = temperature
         response = await self._session.post(self._base_url + model + "/" + COMPLETE_PATH,
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
         completions = response_json[COMPLETIONS_KEY]
         return [completion[DATA_KEY][TEXT_KEY] for completion in completions]
```

### Comparing `llm_client-0.2.0/llm_client/llm_api_client/aleph_alpha_client.py` & `llm_client-0.3.0/llm_client/llm_api_client/aleph_alpha_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,31 @@
 class AlephAlphaClient(BaseLLMAPIClient):
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         if self._base_url is None:
             self._base_url = BASE_URL
         self._headers[AUTH_HEADER] = BEARER_TOKEN + self._api_key
 
-    async def text_completion(self, prompt: str, model: str | None = None, max_tokens: int | None = None, **kwargs) ->\
+    async def text_completion(self, prompt: str, model: str | None = None, max_tokens : int | None= None, temperature : float = 0 , **kwargs) ->\
             list[str]:
+        self._set_model_in_kwargs(kwargs, model)
         if max_tokens is None:
             raise ValueError("max_tokens must be specified")
-        self._set_model_in_kwargs(kwargs, model)
         kwargs[PROMPT_KEY] = prompt
-        kwargs[MAX_TOKENS_KEY] = max_tokens
+        kwargs["maximum_tokens"] = kwargs.pop("maximum_tokens", max_tokens)
+        kwargs["temperature"]  = temperature
         response = await self._session.post(self._base_url + COMPLETE_PATH,
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
         completions = response_json[COMPLETIONS_KEY]
         return [completion[TEXT_KEY] for completion in completions]
 
-    async def embedding(self, text: str, model: str | None = None, representation: str = REPRESENTATION_DEFAULT_VALUE,
+    async def embedding(self, text: str, model: str | None = None,representation: str = REPRESENTATION_DEFAULT_VALUE,
                         **kwargs) -> list[float]:
         self._set_model_in_kwargs(kwargs, model)
         kwargs[REPRESENTATION_KEY] = representation
         kwargs[PROMPT_KEY] = text
         response = await self._session.post(self._base_url + EMBEDDING_PATH,
                                             json=kwargs,
                                             headers=self._headers,
```

### Comparing `llm_client-0.2.0/llm_client/llm_api_client/anthropic_client.py` & `llm_client-0.3.0/llm_client/llm_api_client/anthropic_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from anthropic import count_tokens
 
 from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
 from llm_client.consts import PROMPT_KEY
 
-
 COMPLETE_PATH = "complete"
 BASE_URL = "https://api.anthropic.com/v1/"
 COMPLETIONS_KEY = "completion"
 AUTH_HEADER = "x-api-key"
 ACCEPT_HEADER = "Accept"
 ACCEPT_VALUE = "application/json"
 MAX_TOKENS_KEY = "max_tokens_to_sample"
@@ -17,21 +16,23 @@
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         if self._base_url is None:
             self._base_url = BASE_URL
         self._headers[ACCEPT_HEADER] = ACCEPT_VALUE
         self._headers[AUTH_HEADER] = self._api_key
 
-    async def text_completion(self, prompt: str, model: str | None = None, max_tokens: int | None = None, **kwargs) ->\
+    async def text_completion(self, prompt: str, model: str | None = None, max_tokens: int | None = None, temperature: float = 1,
+                              **kwargs) -> \
             list[str]:
-        if max_tokens is None:
-            raise ValueError("max_tokens must be specified")
+        if max_tokens is None and kwargs.get(MAX_TOKENS_KEY) is None:
+            raise ValueError(f"max_tokens or {MAX_TOKENS_KEY} must be specified")
         self._set_model_in_kwargs(kwargs, model)
         kwargs[PROMPT_KEY] = prompt
-        kwargs[MAX_TOKENS_KEY] = max_tokens
+        kwargs[MAX_TOKENS_KEY] = kwargs.pop(MAX_TOKENS_KEY, max_tokens)
+        kwargs["temperature"] = temperature
         response = await self._session.post(self._base_url + COMPLETE_PATH,
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
         return [response_json[COMPLETIONS_KEY]]
```

### Comparing `llm_client-0.2.0/llm_client/llm_api_client/base_llm_api_client.py` & `llm_client-0.3.0/llm_client/llm_api_client/base_llm_api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         self._api_key: str = config.api_key
         self._session: ClientSession = config.session
         self._base_url: str = config.base_url
         self._default_model: str = config.default_model
         self._headers: dict[str, str] = config.headers
 
     @abstractmethod
-    async def text_completion(self, prompt: str, model: str | None = None, **kwargs) -> list[str]:
+    async def text_completion(self, prompt: str, model: str | None = None, max_tokens: int | None = None,
+                              temperature: float | None = None, **kwargs) -> list[str]:
         raise NotImplementedError()
 
     async def embedding(self, text: str, model: str | None = None, **kwargs) -> list[float]:
         raise NotImplementedError()
 
     def _set_model_in_kwargs(self, kwargs, model: str | None) -> None:
         if model is not None:
```

### Comparing `llm_client-0.2.0/llm_client/llm_api_client/huggingface_client.py` & `llm_client-0.3.0/llm_client/llm_api_client/huggingface_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,28 +8,33 @@
 TEXT_KEY = "generated_text"
 AUTH_HEADER = "Authorization"
 BEARER_TOKEN = "Bearer "
 DEFAULT_MODEL = "oasst-sft-4-pythia-12b-epoch-3.5"
 CONST_SLASH = '/'
 EMPTY_STR = ''
 NEWLINE = '\n'
+TEMPERATURE_KEY = "temperature"
+TOKENS_KEY = "max_length"
 
 
 class HuggingFaceClient(BaseLLMAPIClient):
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         if self._base_url is None:
             self._base_url = BASE_URL
         if self._default_model is None:
             self._default_model = DEFAULT_MODEL
         self._headers[AUTH_HEADER] = BEARER_TOKEN + self._api_key
 
-    async def text_completion(self, prompt: str, model: str | None = None, **kwargs) -> list[str]:
+    async def text_completion(self, prompt: str, max_tokens: int | None = None, temperature: float = 1.0,
+                              model: str | None = None, **kwargs) -> list[str]:
         model = model or self._default_model
         kwargs[INPUT_KEY] = prompt
+        kwargs[TEMPERATURE_KEY] = temperature
+        kwargs[TOKENS_KEY] = kwargs.pop(TOKENS_KEY, max_tokens)
         response = await self._session.post(self._base_url + model + CONST_SLASH,
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
         if isinstance(response_json, list):
             completions = response_json[COMPLETIONS_KEY][TEXT_KEY]
```

### Comparing `llm_client-0.2.0/llm_client/llm_api_client/llm_api_client_factory.py` & `llm_client-0.3.0/llm_client/llm_api_client/llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/llm_client/llm_api_client/openai_client.py` & `llm_client-0.3.0/llm_client/llm_api_client/openai_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,23 +31,29 @@
 class OpenAIClient(BaseLLMAPIClient):
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         openai.api_key = self._api_key
         openai.aiosession.set(self._session)
         self._client = openai
 
-    async def text_completion(self, prompt: str, model: str | None = None, **kwargs) -> list[str]:
+    async def text_completion(self, prompt: str, model: str | None = None,temperature: float = 0,
+        max_tokens: int = 16 , **kwargs) -> list[str]:
         self._set_model_in_kwargs(kwargs, model)
         kwargs[PROMPT_KEY] = prompt
+        kwargs["temperature"] = temperature
+        kwargs["max_tokens"] = max_tokens
         completions = await self._client.Completion.acreate(headers=self._headers, **kwargs)
         return [choice.text for choice in completions.choices]
 
-    async def chat_completion(self, messages: list[ChatMessage], model: str | None = None, **kwargs) -> list[str]:
+    async def chat_completion(self, messages: list[ChatMessage],  temperature: float = 0,
+        max_tokens: int = 16 ,model: str | None = None, **kwargs) -> list[str]:
         self._set_model_in_kwargs(kwargs, model)
         kwargs["messages"] = [message.to_dict() for message in messages]
+        kwargs["temperature"] = temperature
+        kwargs["max_tokens"] = max_tokens
         completions = await self._client.ChatCompletion.acreate(headers=self._headers, **kwargs)
         return [choice.message.content for choice in completions.choices]
 
     async def embedding(self, text: str, model: str | None = None, **kwargs) -> list[float]:
         self._set_model_in_kwargs(kwargs, model)
         kwargs[INPUT_KEY] = text
         embeddings = await openai.Embedding.acreate(**kwargs)
```

### Comparing `llm_client-0.2.0/llm_client/llm_client/local_client.py` & `llm_client-0.3.0/llm_client/llm_client/local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/llm_client/sync/sync_llm_api_client_factory.py` & `llm_client-0.3.0/llm_client/sync/sync_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/activate` & `llm_client-0.3.0/new_venv/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/activate.csh` & `llm_client-0.3.0/new_venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/activate.fish` & `llm_client-0.3.0/new_venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/activate.nu` & `llm_client-0.3.0/new_venv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/activate.ps1` & `llm_client-0.3.0/new_venv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/activate_this.py` & `llm_client-0.3.0/new_venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/deactivate.nu` & `llm_client-0.3.0/new_venv/bin/deactivate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/publish.py` & `llm_client-0.3.0/new_venv/bin/publish.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2html.py` & `llm_client-0.3.0/new_venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2html4.py` & `llm_client-0.3.0/new_venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2html5.py` & `llm_client-0.3.0/new_venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2latex.py` & `llm_client-0.3.0/new_venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2man.py` & `llm_client-0.3.0/new_venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2odt.py` & `llm_client-0.3.0/new_venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2odt_prepstyles.py` & `llm_client-0.3.0/new_venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2pseudoxml.py` & `llm_client-0.3.0/new_venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2s5.py` & `llm_client-0.3.0/new_venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2xetex.py` & `llm_client-0.3.0/new_venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rst2xml.py` & `llm_client-0.3.0/new_venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/bin/rstpep2html.py` & `llm_client-0.3.0/new_venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/LICENSE.txt` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py` & `llm_client-0.3.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/new_venv/share/man/man1/isympy.1` & `llm_client-0.3.0/new_venv/share/man/man1/isympy.1`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/tests/llm_api_client/test_llm_api_client_factory.py` & `llm_client-0.3.0/tests/llm_api_client/test_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/tests/llm_api_client/ai21_client/conftest.py` & `llm_client-0.3.0/tests/llm_api_client/ai21_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/tests/llm_api_client/ai21_client/test_ai21.py` & `llm_client-0.3.0/tests/llm_api_client/ai21_client/test_ai21.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
     actual = await llm_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == [
         ' things!\n\nI love entertaining, entertaining and decorating my home, entertaining clients, entertaining '
         'friends, entertaining family...you get the point! One of my favorite things to do is plan parties']
     mock_aioresponse.assert_called_once_with(url, method='POST',
-                                             headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'prompt': 'These are a few of my favorite'},
+                                             headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key },
+                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 16, "temperature" : 0.7 },
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__return_multiple_completions(mock_aioresponse, llm_client, url):
     payload = load_json_resource("ai21/text_completion.json")
     payload["completions"].append({DATA_KEY: {TEXT_KEY: "second completion"}})
@@ -45,15 +45,15 @@
     assert actual == [
         ' things!\n\nI love entertaining, entertaining and decorating my home, entertaining clients, entertaining '
         'friends, entertaining family...you get the point! One of my favorite things to do is plan parties',
         "second completion"
     ]
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'prompt': 'These are a few of my favorite'},
+                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 16, "temperature" : 0.7 },
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__override_model(mock_aioresponse, llm_client):
     new_model_name = "gpt3"
     url = build_url(new_model_name)
@@ -65,15 +65,15 @@
     actual = await llm_client.text_completion(prompt="These are a few of my favorite", model=new_model_name)
 
     assert actual == [
         ' things!\n\nI love entertaining, entertaining and decorating my home, entertaining clients, entertaining '
         'friends, entertaining family...you get the point! One of my favorite things to do is plan parties']
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'prompt': 'These are a few of my favorite'},
+                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 16, "temperature" : 0.7 },
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_kwargs(mock_aioresponse, llm_client, url):
     mock_aioresponse.post(
         url,
@@ -83,15 +83,15 @@
     actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10)
 
     assert actual == [
         ' things!\n\nI love entertaining, entertaining and decorating my home, entertaining clients, entertaining '
         'friends, entertaining family...you get the point! One of my favorite things to do is plan parties']
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'prompt': 'These are a few of my favorite', 'max_tokens': 10},
+                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 10, "temperature" : 0.7 },
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_get_tokens_count__sanity(mock_aioresponse, llm_client, url):
     mock_aioresponse.post(
         BASE_URL + TOKENIZE_PATH,
```

### Comparing `llm_client-0.2.0/tests/llm_api_client/anthropic_client/conftest.py` & `llm_client-0.3.0/tests/llm_api_client/anthropic_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py` & `llm_client-0.3.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10)
 
     assert actual == ["completion text"]
     mock_aioresponse.assert_called_once_with(complete_url, method='POST',
                                              headers={AUTH_HEADER: llm_client._api_key,
                                                       ACCEPT_HEADER: ACCEPT_VALUE},
                                              json={PROMPT_KEY: 'These are a few of my favorite',
-                                                   MAX_TOKENS_KEY: 10,
+                                                   MAX_TOKENS_KEY: 10, "temperature": 1,
                                                    MODEL_KEY: llm_client._default_model},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__without_max_tokens_raise_value_error(mock_aioresponse, llm_client):
     with pytest.raises(ValueError):
@@ -54,15 +54,15 @@
                                               max_tokens=10)
 
     assert actual == ["completion text"]
     mock_aioresponse.assert_called_once_with(complete_url, method='POST',
                                              headers={AUTH_HEADER: llm_client._api_key,
                                                       ACCEPT_HEADER: ACCEPT_VALUE},
                                              json={PROMPT_KEY: 'These are a few of my favorite',
-                                                   MAX_TOKENS_KEY: 10,
+                                                   MAX_TOKENS_KEY: 10, "temperature": 1,
                                                    MODEL_KEY: new_model_name},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_kwargs(mock_aioresponse, llm_client, complete_url):
     mock_aioresponse.post(
```

### Comparing `llm_client-0.2.0/tests/llm_api_client/huggingface_client/conftest.py` & `llm_client-0.3.0/tests/llm_api_client/huggingface_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/tests/llm_api_client/huggingface_client/test_huggingface.py` & `llm_client-0.3.0/tests/llm_api_client/huggingface_client/test_huggingface.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     )
 
     actual = await llm_client.text_completion(prompt="who is kobe bryant")
 
     assert actual == ['Kobe Bryant is a retired professional basketball player who played for the Los Angeles Lakers of']
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'inputs': 'who is kobe bryant'},
+                                             json={'inputs': 'who is kobe bryant',"max_length": None, "temperature": 1.0},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_kwargs(mock_aioresponse, llm_client, url):
     mock_aioresponse.post(
         url,
@@ -40,15 +40,15 @@
     )
 
     actual = await llm_client.text_completion(prompt="who is kobe bryant",max_tokens = 10)
 
     assert actual == ['Kobe Bryant is a retired professional basketball player who played for the Los Angeles Lakers of']
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'inputs': 'who is kobe bryant','max_tokens' : 10},
+                                             json={'inputs': 'who is kobe bryant',"max_length": 10, "temperature": 1.0},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 def test_get_tokens_count__sanity(mock_aioresponse, llm_client, url):
     actual = llm_client.get_tokens_count(text="is queen elisabeth alive?")
     assert actual == 7
```

### Comparing `llm_client-0.2.0/tests/llm_api_client/openai_client/conftest.py` & `llm_client-0.3.0/tests/llm_api_client/openai_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/tests/llm_api_client/openai_client/test_openai.py` & `llm_client-0.3.0/tests/llm_api_client/openai_client/test_openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,59 +33,59 @@
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        headers={})
+        headers={},temperature=0,max_tokens=16)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__return_multiple_completions(openai_mock, open_ai_client, model_name):
     open_ai_object = OpenAIObject.construct_from(load_json_resource("openai/text_completion.json"))
     open_ai_object.choices.append(OpenAIObject.construct_from({"text": "second completion"}))
     openai_mock.Completion.acreate = AsyncMock(return_value=open_ai_object)
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == ["\n\nThis is indeed a test", "second completion"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        headers={})
+        headers={},temperature=0,max_tokens=16)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__override_model(openai_mock, open_ai_client, model_name):
     new_model_name = "gpt3"
     openai_mock.Completion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite", model=new_model_name)
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=new_model_name,
         prompt="These are a few of my favorite",
-        headers={})
+        headers={},temperature=0,max_tokens=16)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_kwargs(openai_mock, open_ai_client, model_name):
     openai_mock.Completion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite", max_tokens=10)
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        max_tokens=10,
+        temperature=0,max_tokens=10,
         headers={})
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_headers(openai_mock, model_name):
     openai_mock.Completion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
@@ -94,74 +94,74 @@
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        headers={"header_name": "header_value"})
+        headers={"header_name": "header_value"},temperature=0,max_tokens=16)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__sanity(openai_mock, open_ai_client, model_name):
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")])
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={})
+        headers={},temperature=0,max_tokens=16)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__return_multiple_completions(openai_mock, open_ai_client, model_name):
     open_ai_object = OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json"))
     open_ai_object.choices.append(OpenAIObject.construct_from({"message": {"content": "second completion"}}))
     openai_mock.ChatCompletion.acreate = AsyncMock(return_value=open_ai_object)
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")])
 
     assert actual == ["\n\nHello there, how may I assist you today?", "second completion"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={})
+        headers={},temperature=0,max_tokens=16)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__override_model(openai_mock, open_ai_client, model_name):
     new_model_name = "gpt3"
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")], model=new_model_name)
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=new_model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={})
+        headers={},temperature=0,max_tokens=16)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__with_kwargs(openai_mock, open_ai_client, model_name):
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")], max_tokens=10)
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
         max_tokens=10,
-        headers={})
+        headers={},temperature=0)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__with_headers(openai_mock, model_name):
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
     open_ai_client = OpenAIClient(LLMAPIClientConfig("fake_api_key", MagicMock(ClientSession), default_model=model_name,
@@ -169,15 +169,15 @@
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")])
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={"header_name": "header_value"})
+        headers={"header_name": "header_value"},temperature=0,max_tokens=16)
 
 
 @pytest.mark.asyncio
 async def test_get_tokens_count__sanity(model_name, open_ai_client, tiktoken_mock):
     tokeniser_mock = tiktoken_mock.encoding_for_model.return_value
     tokeniser_mock.encode.return_value = [123, 456]
     text = "This is a test"
```

### Comparing `llm_client-0.2.0/tests/llm_client/local_client/conftest.py` & `llm_client-0.3.0/tests/llm_client/local_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/tests/llm_client/local_client/test_local_client.py` & `llm_client-0.3.0/tests/llm_client/local_client/test_local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/tests/resources/ai21/text_completion.json` & `llm_client-0.3.0/tests/resources/ai21/text_completion.json`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/tests/sync/test_sync_llm_api_client_factory.py` & `llm_client-0.3.0/tests/sync/test_sync_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_ai21/bin/activate` & `llm_client-0.3.0/venv_ai21/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_ai21/bin/activate.csh` & `llm_client-0.3.0/venv_ai21/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_ai21/bin/activate.fish` & `llm_client-0.3.0/venv_ai21/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_ai21/bin/activate.nu` & `llm_client-0.3.0/venv_ai21/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_ai21/bin/activate.ps1` & `llm_client-0.3.0/venv_ai21/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_ai21/bin/activate_this.py` & `llm_client-0.3.0/venv_ai21/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_ai21/bin/deactivate.nu` & `llm_client-0.3.0/venv_ai21/bin/deactivate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_local/bin/activate` & `llm_client-0.3.0/venv_local/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_local/bin/activate.csh` & `llm_client-0.3.0/venv_local/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_local/bin/activate.fish` & `llm_client-0.3.0/venv_local/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_local/bin/activate.nu` & `llm_client-0.3.0/venv_local/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_local/bin/activate.ps1` & `llm_client-0.3.0/venv_local/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_local/bin/activate_this.py` & `llm_client-0.3.0/venv_local/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/venv_local/bin/deactivate.nu` & `llm_client-0.3.0/venv_local/bin/deactivate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/.gitignore` & `llm_client-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/LICENSE` & `llm_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/README.md` & `llm_client-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # LLM-Client-SDK
 [![Test](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml)
 [![License: MIT](https://img.shields.io/github/license/uripeled2/llm-client-sdk.svg)](https://opensource.org/licenses/MIT)
 
 LLM-Client-SDK is an SDK for communicating with generative AI large language models
-(We currently support - OpenAI, AI21, HuggingfaceHub, Aleph Alpha, Anthropic
+(We currently support - OpenAI, AI21, HuggingfaceHub, Aleph Alpha, Anthropic,
 Local models with transformers - and many more soon).
 
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
 more details below in Usage section.
 
 ## Base Interface
-The package expose two simple interface for communicating with LLMs (In the future we 
-will expend the interface to support more tasks like embeddings, list models, edits, etc.
+The package exposes two simple interfaces for communicating with LLMs (In the future, we 
+will expand the interface to support more tasks like embeddings, list models, edits, etc.
 and we will add a standardized for LLMs param like max_tokens, temperature, etc.):
 ```python
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any
 from aiohttp import ClientSession
 
@@ -42,15 +42,16 @@
 
 
 class BaseLLMAPIClient(BaseLLMClient, ABC):
     def __init__(self, config: LLMAPIClientConfig):
         ...
 
     @abstractmethod
-    async def text_completion(self, prompt: str, model: str | None = None, **kwargs) -> list[str]:
+    async def text_completion(self, prompt: str, model: str | None = None, max_tokens: int | None = None,
+                              temperature: float | None = None, **kwargs) -> list[str]:
         raise NotImplementedError()
 
     async def embedding(self, text: str, model: str | None = None, **kwargs) -> list[float]:
         raise NotImplementedError()
 ```
 
 ## Requirements
@@ -126,26 +127,26 @@
 
 async def main():
     async with LLMAPIClientFactory() as llm_api_client_factory:
         llm_client = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI,
                                                                api_key=OPENAI_API_KEY)
 
         await llm_client.text_completion(prompt="This is indeed a test")
-        await llm_client.text_completion(prompt="This is indeed a test", max_length=50)
+        await llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 
         
 # Or if you don't want to use async
 from llm_client import SyncLLMAPIClientFactory
 
 with SyncLLMAPIClientFactory() as llm_api_client_factory:
     llm_client = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI,
                                                            api_key=OPENAI_API_KEY)
 
     llm_client.text_completion(prompt="This is indeed a test")
-    llm_client.text_completion(prompt="This is indeed a test", max_length=50)
+    llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 ```
 Local model
 ```python
 import os
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoTokenizer
 from llm_client import LocalClientConfig, LocalClient
 
@@ -154,15 +155,15 @@
         model = AutoModelForCausalLM.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
     except ValueError:
         model = AutoModelForSeq2SeqLM.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
     tokenizer = AutoTokenizer.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
     llm_client = LocalClient(LocalClientConfig(model, tokenizer, os.environ["TENSORS_TYPE"], os.environ["DEVICE"]))
 
     await llm_client.text_completion(prompt="This is indeed a test")
-    await llm_client.text_completion(prompt="This is indeed a test", max_length=50)
+    await llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 
 
 # Or if you don't want to use async
 import async_to_sync
 
 try:
     model = AutoModelForCausalLM.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
@@ -170,15 +171,15 @@
     model = AutoModelForSeq2SeqLM.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
 tokenizer = AutoTokenizer.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
 llm_client = LocalClient(LocalClientConfig(model, tokenizer, os.environ["TENSORS_TYPE"], os.environ["DEVICE"]))
 
 llm_client = async_to_sync.methods(llm_client)
 
 llm_client.text_completion(prompt="This is indeed a test")
-llm_client.text_completion(prompt="This is indeed a test", max_length=50)
+llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 ```
 
 ## Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open issue or a pull request.
 
 ### Todo
@@ -191,15 +192,18 @@
 - [x] Add support for more functions via LLMs 
   - [x] embeddings
   - [ ] list models
   - [ ] edits
   - [ ] more
 - [ ] Add contributing guidelines
 - [ ] Create an easy way to run multiple LLMs in parallel with the same prompts
-- [ ] Convert common models parameter (e.g. temperature, max_tokens, etc.)
+- [x] Convert common models parameter
+  - [x] temperature 
+  - [x] max_tokens
+  - [ ] more
 
 ### Development
 To install the package in development mode, run the following command:
 ```console
 $ pip install -e ".[all,test]"
 ```
 To run the tests, run the following command:
```

### Comparing `llm_client-0.2.0/pyproject.toml` & `llm_client-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_client-0.2.0/PKG-INFO` & `llm_client-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: SDK for using LLM
 Project-URL: Homepage, https://github.com/uripeled2/llm-client-sdk
 Author-email: Uri Peled <uripeled2@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -39,25 +39,25 @@
 Description-Content-Type: text/markdown
 
 # LLM-Client-SDK
 [![Test](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml)
 [![License: MIT](https://img.shields.io/github/license/uripeled2/llm-client-sdk.svg)](https://opensource.org/licenses/MIT)
 
 LLM-Client-SDK is an SDK for communicating with generative AI large language models
-(We currently support - OpenAI, AI21, HuggingfaceHub, Aleph Alpha, Anthropic
+(We currently support - OpenAI, AI21, HuggingfaceHub, Aleph Alpha, Anthropic,
 Local models with transformers - and many more soon).
 
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
 more details below in Usage section.
 
 ## Base Interface
-The package expose two simple interface for communicating with LLMs (In the future we 
-will expend the interface to support more tasks like embeddings, list models, edits, etc.
+The package exposes two simple interfaces for communicating with LLMs (In the future, we 
+will expand the interface to support more tasks like embeddings, list models, edits, etc.
 and we will add a standardized for LLMs param like max_tokens, temperature, etc.):
 ```python
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any
 from aiohttp import ClientSession
 
@@ -82,15 +82,16 @@
 
 
 class BaseLLMAPIClient(BaseLLMClient, ABC):
     def __init__(self, config: LLMAPIClientConfig):
         ...
 
     @abstractmethod
-    async def text_completion(self, prompt: str, model: str | None = None, **kwargs) -> list[str]:
+    async def text_completion(self, prompt: str, model: str | None = None, max_tokens: int | None = None,
+                              temperature: float | None = None, **kwargs) -> list[str]:
         raise NotImplementedError()
 
     async def embedding(self, text: str, model: str | None = None, **kwargs) -> list[float]:
         raise NotImplementedError()
 ```
 
 ## Requirements
@@ -166,26 +167,26 @@
 
 async def main():
     async with LLMAPIClientFactory() as llm_api_client_factory:
         llm_client = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI,
                                                                api_key=OPENAI_API_KEY)
 
         await llm_client.text_completion(prompt="This is indeed a test")
-        await llm_client.text_completion(prompt="This is indeed a test", max_length=50)
+        await llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 
         
 # Or if you don't want to use async
 from llm_client import SyncLLMAPIClientFactory
 
 with SyncLLMAPIClientFactory() as llm_api_client_factory:
     llm_client = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI,
                                                            api_key=OPENAI_API_KEY)
 
     llm_client.text_completion(prompt="This is indeed a test")
-    llm_client.text_completion(prompt="This is indeed a test", max_length=50)
+    llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 ```
 Local model
 ```python
 import os
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoTokenizer
 from llm_client import LocalClientConfig, LocalClient
 
@@ -194,15 +195,15 @@
         model = AutoModelForCausalLM.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
     except ValueError:
         model = AutoModelForSeq2SeqLM.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
     tokenizer = AutoTokenizer.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
     llm_client = LocalClient(LocalClientConfig(model, tokenizer, os.environ["TENSORS_TYPE"], os.environ["DEVICE"]))
 
     await llm_client.text_completion(prompt="This is indeed a test")
-    await llm_client.text_completion(prompt="This is indeed a test", max_length=50)
+    await llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 
 
 # Or if you don't want to use async
 import async_to_sync
 
 try:
     model = AutoModelForCausalLM.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
@@ -210,15 +211,15 @@
     model = AutoModelForSeq2SeqLM.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
 tokenizer = AutoTokenizer.from_pretrained(os.environ["MODEL_NAME_OR_PATH"])
 llm_client = LocalClient(LocalClientConfig(model, tokenizer, os.environ["TENSORS_TYPE"], os.environ["DEVICE"]))
 
 llm_client = async_to_sync.methods(llm_client)
 
 llm_client.text_completion(prompt="This is indeed a test")
-llm_client.text_completion(prompt="This is indeed a test", max_length=50)
+llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 ```
 
 ## Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open issue or a pull request.
 
 ### Todo
@@ -231,15 +232,18 @@
 - [x] Add support for more functions via LLMs 
   - [x] embeddings
   - [ ] list models
   - [ ] edits
   - [ ] more
 - [ ] Add contributing guidelines
 - [ ] Create an easy way to run multiple LLMs in parallel with the same prompts
-- [ ] Convert common models parameter (e.g. temperature, max_tokens, etc.)
+- [x] Convert common models parameter
+  - [x] temperature 
+  - [x] max_tokens
+  - [ ] more
 
 ### Development
 To install the package in development mode, run the following command:
 ```console
 $ pip install -e ".[all,test]"
 ```
 To run the tests, run the following command:
```

