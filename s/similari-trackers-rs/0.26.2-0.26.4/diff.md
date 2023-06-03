# Comparing `tmp/similari_trackers_rs-0.26.2.tar.gz` & `tmp/similari_trackers_rs-0.26.4.tar.gz`

## Comparing `similari_trackers_rs-0.26.2.tar` & `similari_trackers_rs-0.26.4.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 similari_trackers_rs-0.26.2/Cargo.toml
--rw-r--r--   0     1001      123      274 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.cargo/config
--rw-r--r--   0     1001      123       62 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.dockerignore
--rw-r--r--   0     1001      123     2085 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-python-3_10.yml
--rw-r--r--   0     1001      123     2085 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-python-3_11.yml
--rw-r--r--   0     1001      123     2083 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-python-3_8.yml
--rw-r--r--   0     1001      123     2083 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-python-3_9.yml
--rw-r--r--   0     1001      123     2081 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-rust-1_67.yml
--rw-r--r--   0     1001      123     2806 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.github/workflows/maturin.yml
--rw-r--r--   0     1001      123      346 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.github/workflows/rust.yml
--rw-r--r--   0     1001      123       48 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/.gitignore
--rw-r--r--   0     1001      123    29869 2023-05-13 07:54:07.000000 similari_trackers_rs-0.26.2/Cargo.lock
--rw-r--r--   0     1001      123    11384 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/LICENSE
--rw-r--r--   0     1001      123    14799 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/README.md
--rw-r--r--   0     1001      123     5748 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/assets/benchmarks/benchmarks.md
--rw-r--r--   0     1001      123    14603 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/assets/documentation/python/api.md
--rw-r--r--   0     1001      123     2418 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/batch_sort_iou_tracker.rs
--rw-r--r--   0     1001      123     2307 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/batch_sort_maha_tracker.rs
--rw-r--r--   0     1001      123     1344 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/bbox_own_areas.rs
--rw-r--r--   0     1001      123     5023 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/feature_tracker.rs
--rw-r--r--   0     1001      123      841 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/kalman_2d_point.rs
--rw-r--r--   0     1001      123      952 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/kalman_bbox.rs
--rw-r--r--   0     1001      123      986 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/nms.rs
--rw-r--r--   0     1001      123     1182 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/nms_oriented.rs
--rw-r--r--   0     1001      123     2084 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/simple_search.rs
--rw-r--r--   0     1001      123     2209 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/simple_sort_iou_tracker.rs
--rw-r--r--   0     1001      123     2379 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/simple_sort_iou_tracker_oriented.rs
--rw-r--r--   0     1001      123     2123 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/simple_sort_maha_tracker.rs
--rw-r--r--   0     1001      123     2271 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/simple_sort_maha_tracker_oriented.rs
--rw-r--r--   0     1001      123     4354 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/simple_visual_sort_tracker.rs
--rw-r--r--   0     1001      123     2052 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/benches/track_search.rs
--rw-r--r--   0     1001      123       71 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/build.rs
--rw-r--r--   0     1001      123      392 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/docker/common/install-basic-deps.sh
--rw-r--r--   0     1001      123      641 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/docker/python_3.10/Dockerfile
--rw-r--r--   0     1001      123      641 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/docker/python_3.11/Dockerfile
--rw-r--r--   0     1001      123      638 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/docker/python_3.8/Dockerfile
--rw-r--r--   0     1001      123      640 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/docker/python_3.9/Dockerfile
--rw-r--r--   0     1001      123      702 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/docker/rust_1.67/Dockerfile
--rw-r--r--   0     1001      123     1737 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/examples/batch_sort_iou_tracker.rs
--rw-r--r--   0     1001      123     5285 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/examples/incremental_track_build.rs
--rw-r--r--   0     1001      123     3086 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/examples/middleware_sort_tracker.rs
--rw-r--r--   0     1001      123     2427 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/examples/simple.rs
--rw-r--r--   0     1001      123     1385 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/examples/simple_sort_iou_tracker.rs
--rw-r--r--   0     1001      123     1280 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/examples/simple_sort_iou_tracker_oriented.rs
--rw-r--r--   0     1001      123     1256 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/examples/simple_sort_maha_tracker.rs
--rw-r--r--   0     1001      123     1136 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/examples/simple_sort_maha_tracker_oriented.rs
--rw-r--r--   0     1001      123    16013 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/examples/track_merging.rs
--rw-r--r--   0     1001      123      469 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/pyproject.toml
--rw-r--r--   0     1001      123      850 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/bb.py
--rw-r--r--   0     1001      123     2539 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/bug_visual_sort.py
--rw-r--r--   0     1001      123    25550 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_1.json
--rw-r--r--   0     1001      123    25569 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_2.json
--rw-r--r--   0     1001      123    25393 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/in/in-1.json
--rw-r--r--   0     1001      123    25550 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/in/in-2.json
--rw-r--r--   0     1001      123     5744 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/bugfixes/github-84.py
--rw-r--r--   0     1001      123      650 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/clipping_intersection.py
--rw-r--r--   0     1001      123      369 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/kalman_2d_point.py
--rw-r--r--   0     1001      123      508 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/kalman_2d_vec.py
--rw-r--r--   0     1001      123      916 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/kalman_bbox.py
--rw-r--r--   0     1001      123     1391 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/Dockerfile
--rw-r--r--   0     1001      123     2564 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/README.md
--rw-r--r--   0     1001      123        0 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/__init__.py
--rw-r--r--   0     1001      123     2879 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/__main__.py
--rw-r--r--   0     1001      123     3639 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/config.py
--rw-r--r--   0     1001      123     1923 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/config.yml
--rw-r--r--   0     1001      123     1940 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/confs/original-sort-config.yml
--rw-r--r--   0     1001      123     1506 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/confs/similari-maha-sort-config.yml
--rw-r--r--   0     1001      123     1437 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/evaluator.py
--rw-r--r--   0     1001      123       38 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/requirements.txt
--rw-r--r--   0     1001      123     4126 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/trackers.py
--rw-r--r--   0     1001      123     1116 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/motchallenge/utils.py
--rw-r--r--   0     1001      123      576 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/nms.py
--rw-r--r--   0     1001      123     1156 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/sort/batch_sort_iou.py
--rw-r--r--   0     1001      123     1406 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/sort/batch_sort_iou_bench.py
--rw-r--r--   0     1001      123      665 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/sort/sort_idle.py
--rw-r--r--   0     1001      123      797 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/sort/sort_iou.py
--rw-r--r--   0     1001      123      987 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/sort/sort_iou_bench.py
--rw-r--r--   0     1001      123     1071 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/sort/sort_iou_rotated.py
--rw-r--r--   0     1001      123     1009 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/sort/sort_iou_scene_id.py
--rw-r--r--   0     1001      123      806 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/sort/sort_maha.py
--rw-r--r--   0     1001      123     5068 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/visual_sort/batch_visual_sort.py
--rw-r--r--   0     1001      123     3363 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/visual_sort/visual_sort.py
--rw-r--r--   0     1001      123     1574 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/python/visual_sort.py
--rw-r--r--   0     1001      123     2297 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/distance.rs
--rw-r--r--   0     1001      123     2452 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/examples/iou.rs
--rw-r--r--   0     1001      123     7222 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/examples.rs
--rw-r--r--   0     1001      123     5348 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/lib.rs
--rw-r--r--   0     1001      123      836 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/prelude.rs
--rw-r--r--   0     1001      123     6390 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/builder.rs
--rw-r--r--   0     1001      123      221 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/notify.rs
--rw-r--r--   0     1001      123     2732 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/store/builder.rs
--rw-r--r--   0     1001      123    19590 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/store/store_tests.rs
--rw-r--r--   0     1001      123     9338 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/store/track_distance.rs
--rw-r--r--   0     1001      123    25504 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/store.rs
--rw-r--r--   0     1001      123     2649 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/utils.rs
--rw-r--r--   0     1001      123     3928 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/voting/best.rs
--rw-r--r--   0     1001      123     8799 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/voting/topn.rs
--rw-r--r--   0     1001      123      759 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track/voting.rs
--rw-r--r--   0     1001      123    42240 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/track.rs
--rw-r--r--   0     1001      123     3425 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/batch.rs
--rw-r--r--   0     1001      123     3825 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/epoch_db.rs
--rw-r--r--   0     1001      123      944 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/kalman_prediction.rs
--rw-r--r--   0     1001      123    16922 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/sort/batch_api.rs
--rw-r--r--   0     1001      123     6729 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/sort/metric.rs
--rw-r--r--   0     1001      123    19512 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/sort/simple_api.rs
--rw-r--r--   0     1001      123      787 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/sort/sort_py.rs
--rw-r--r--   0     1001      123     4986 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/sort/voting.rs
--rw-r--r--   0     1001      123    13720 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/sort.rs
--rw-r--r--   0     1001      123     3374 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/spatio_temporal_constraints.rs
--rw-r--r--   0     1001      123     3783 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/tracker_api.rs
--rw-r--r--   0     1001      123    20356 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort/batch_api.rs
--rw-r--r--   0     1001      123     8106 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort/metric/builder.rs
--rw-r--r--   0     1001      123    36076 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort/metric.rs
--rw-r--r--   0     1001      123     3904 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort/observation_attributes.rs
--rw-r--r--   0     1001      123    14760 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort/options.rs
--rw-r--r--   0     1001      123    30552 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort/simple_api.rs
--rw-r--r--   0     1001      123     8182 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort/track_attributes.rs
--rw-r--r--   0     1001      123     2640 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort/visual_sort_py.rs
--rw-r--r--   0     1001      123     7537 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort/voting.rs
--rw-r--r--   0     1001      123     2614 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers/visual_sort.rs
--rw-r--r--   0     1001      123      643 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/trackers.rs
--rw-r--r--   0     1001      123    18919 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/bbox.rs
--rw-r--r--   0     1001      123     2613 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/clipping/bbox_own_areas.rs
--rw-r--r--   0     1001      123     1803 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/clipping/clipping_py.rs
--rw-r--r--   0     1001      123     3347 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/clipping.rs
--rw-r--r--   0     1001      123    11445 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/kalman/kalman_2d_box.rs
--rw-r--r--   0     1001      123    10152 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/kalman/kalman_2d_point.rs
--rw-r--r--   0     1001      123     5029 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/kalman/kalman_2d_point_vec.rs
--rw-r--r--   0     1001      123     2435 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/kalman.rs
--rw-r--r--   0     1001      123     2104 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/nms/nms_py.rs
--rw-r--r--   0     1001      123     5115 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/nms.rs
--rw-r--r--   0     1001      123       30 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/point.rs
--rw-r--r--   0     1001      123      612 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils/primitive.rs
--rw-r--r--   0     1001      123      466 2023-05-13 07:52:42.000000 similari_trackers_rs-0.26.2/src/utils.rs
--rw-r--r--   0        0        0    15582 1970-01-01 00:00:00.000000 similari_trackers_rs-0.26.2/PKG-INFO
+-rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 similari_trackers_rs-0.26.4/Cargo.toml
+-rw-r--r--   0     1001      123      274 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.cargo/config
+-rw-r--r--   0     1001      123       62 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.dockerignore
+-rw-r--r--   0     1001      123     2086 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_10.yml
+-rw-r--r--   0     1001      123     2086 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_11.yml
+-rw-r--r--   0     1001      123     2084 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_8.yml
+-rw-r--r--   0     1001      123     2084 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_9.yml
+-rw-r--r--   0     1001      123     2082 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-rust-1_67.yml
+-rw-r--r--   0     1001      123     2206 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      123      346 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/rust.yml
+-rw-r--r--   0     1001      123       48 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.gitignore
+-rw-r--r--   0     1001      123    29851 2023-06-03 08:29:31.000000 similari_trackers_rs-0.26.4/Cargo.lock
+-rw-r--r--   0     1001      123    11384 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/LICENSE
+-rw-r--r--   0     1001      123    15407 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/README.md
+-rw-r--r--   0     1001      123     5748 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/assets/benchmarks/benchmarks.md
+-rw-r--r--   0     1001      123    14603 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/assets/documentation/python/api.md
+-rw-r--r--   0     1001      123     2418 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/batch_sort_iou_tracker.rs
+-rw-r--r--   0     1001      123     2307 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/batch_sort_maha_tracker.rs
+-rw-r--r--   0     1001      123     1344 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/bbox_own_areas.rs
+-rw-r--r--   0     1001      123     5023 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/feature_tracker.rs
+-rw-r--r--   0     1001      123      841 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/kalman_2d_point.rs
+-rw-r--r--   0     1001      123      952 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/kalman_bbox.rs
+-rw-r--r--   0     1001      123      986 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/nms.rs
+-rw-r--r--   0     1001      123     1182 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/nms_oriented.rs
+-rw-r--r--   0     1001      123     2084 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_search.rs
+-rw-r--r--   0     1001      123     2209 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_sort_iou_tracker.rs
+-rw-r--r--   0     1001      123     2379 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_sort_iou_tracker_oriented.rs
+-rw-r--r--   0     1001      123     2123 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_sort_maha_tracker.rs
+-rw-r--r--   0     1001      123     2271 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_sort_maha_tracker_oriented.rs
+-rw-r--r--   0     1001      123     4354 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_visual_sort_tracker.rs
+-rw-r--r--   0     1001      123     2052 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/track_search.rs
+-rw-r--r--   0     1001      123       71 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/build.rs
+-rw-r--r--   0     1001      123      392 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/common/install-basic-deps.sh
+-rw-r--r--   0     1001      123      641 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/python_3.10/Dockerfile
+-rw-r--r--   0     1001      123      641 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/python_3.11/Dockerfile
+-rw-r--r--   0     1001      123      638 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/python_3.8/Dockerfile
+-rw-r--r--   0     1001      123      640 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/python_3.9/Dockerfile
+-rw-r--r--   0     1001      123      634 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/rust_1.67/Dockerfile
+-rw-r--r--   0     1001      123     1737 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/batch_sort_iou_tracker.rs
+-rw-r--r--   0     1001      123     5285 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/incremental_track_build.rs
+-rw-r--r--   0     1001      123     3086 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/middleware_sort_tracker.rs
+-rw-r--r--   0     1001      123     2427 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple.rs
+-rw-r--r--   0     1001      123     1385 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple_sort_iou_tracker.rs
+-rw-r--r--   0     1001      123     1280 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple_sort_iou_tracker_oriented.rs
+-rw-r--r--   0     1001      123     1256 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple_sort_maha_tracker.rs
+-rw-r--r--   0     1001      123     1136 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple_sort_maha_tracker_oriented.rs
+-rw-r--r--   0     1001      123    16013 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/track_merging.rs
+-rw-r--r--   0     1001      123      469 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/pyproject.toml
+-rw-r--r--   0     1001      123      850 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bb.py
+-rw-r--r--   0     1001      123     2539 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/bug_visual_sort.py
+-rw-r--r--   0     1001      123    25550 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_1.json
+-rw-r--r--   0     1001      123    25569 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_2.json
+-rw-r--r--   0     1001      123    25393 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/in-1.json
+-rw-r--r--   0     1001      123    25550 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/in-2.json
+-rw-r--r--   0     1001      123     5744 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/github-84.py
+-rw-r--r--   0     1001      123      650 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/clipping_intersection.py
+-rw-r--r--   0     1001      123      369 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/kalman_2d_point.py
+-rw-r--r--   0     1001      123      508 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/kalman_2d_vec.py
+-rw-r--r--   0     1001      123      916 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/kalman_bbox.py
+-rw-r--r--   0     1001      123     1391 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/Dockerfile
+-rw-r--r--   0     1001      123     2564 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/README.md
+-rw-r--r--   0     1001      123        0 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/__init__.py
+-rw-r--r--   0     1001      123     2879 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/__main__.py
+-rw-r--r--   0     1001      123     3639 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/config.py
+-rw-r--r--   0     1001      123     1923 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/config.yml
+-rw-r--r--   0     1001      123     1940 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/confs/original-sort-config.yml
+-rw-r--r--   0     1001      123     1506 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/confs/similari-maha-sort-config.yml
+-rw-r--r--   0     1001      123     1437 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/evaluator.py
+-rw-r--r--   0     1001      123       38 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/requirements.txt
+-rw-r--r--   0     1001      123     4126 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/trackers.py
+-rw-r--r--   0     1001      123     1116 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/utils.py
+-rw-r--r--   0     1001      123      576 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/nms.py
+-rw-r--r--   0     1001      123     1156 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/batch_sort_iou.py
+-rw-r--r--   0     1001      123     1406 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/batch_sort_iou_bench.py
+-rw-r--r--   0     1001      123      665 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_idle.py
+-rw-r--r--   0     1001      123      797 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_iou.py
+-rw-r--r--   0     1001      123      987 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_iou_bench.py
+-rw-r--r--   0     1001      123     1071 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_iou_rotated.py
+-rw-r--r--   0     1001      123     1009 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_iou_scene_id.py
+-rw-r--r--   0     1001      123      806 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_maha.py
+-rw-r--r--   0     1001      123     5068 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/visual_sort/batch_visual_sort.py
+-rw-r--r--   0     1001      123     3363 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/visual_sort/visual_sort.py
+-rw-r--r--   0     1001      123     1574 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/visual_sort.py
+-rw-r--r--   0     1001      123     2297 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/distance.rs
+-rw-r--r--   0     1001      123     2452 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/examples/iou.rs
+-rw-r--r--   0     1001      123     7222 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/examples.rs
+-rw-r--r--   0     1001      123     5508 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/lib.rs
+-rw-r--r--   0     1001      123      836 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/prelude.rs
+-rw-r--r--   0     1001      123     6390 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/builder.rs
+-rw-r--r--   0     1001      123      221 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/notify.rs
+-rw-r--r--   0     1001      123     2732 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/store/builder.rs
+-rw-r--r--   0     1001      123    19590 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/store/store_tests.rs
+-rw-r--r--   0     1001      123     9338 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/store/track_distance.rs
+-rw-r--r--   0     1001      123    25504 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/store.rs
+-rw-r--r--   0     1001      123     2649 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/utils.rs
+-rw-r--r--   0     1001      123     3928 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/voting/best.rs
+-rw-r--r--   0     1001      123     8799 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/voting/topn.rs
+-rw-r--r--   0     1001      123      759 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/voting.rs
+-rw-r--r--   0     1001      123    42240 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track.rs
+-rw-r--r--   0     1001      123     3425 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/batch.rs
+-rw-r--r--   0     1001      123     3825 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/epoch_db.rs
+-rw-r--r--   0     1001      123      944 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/kalman_prediction.rs
+-rw-r--r--   0     1001      123    16922 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/batch_api.rs
+-rw-r--r--   0     1001      123     6729 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/metric.rs
+-rw-r--r--   0     1001      123    19512 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/simple_api.rs
+-rw-r--r--   0     1001      123      787 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/sort_py.rs
+-rw-r--r--   0     1001      123     4986 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/voting.rs
+-rw-r--r--   0     1001      123    13720 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort.rs
+-rw-r--r--   0     1001      123     3374 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/spatio_temporal_constraints.rs
+-rw-r--r--   0     1001      123     3783 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/tracker_api.rs
+-rw-r--r--   0     1001      123    20356 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/batch_api.rs
+-rw-r--r--   0     1001      123     8106 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/metric/builder.rs
+-rw-r--r--   0     1001      123    36076 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/metric.rs
+-rw-r--r--   0     1001      123     3904 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/observation_attributes.rs
+-rw-r--r--   0     1001      123    14760 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/options.rs
+-rw-r--r--   0     1001      123    30552 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/simple_api.rs
+-rw-r--r--   0     1001      123     8182 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/track_attributes.rs
+-rw-r--r--   0     1001      123     2640 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/visual_sort_py.rs
+-rw-r--r--   0     1001      123     7537 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/voting.rs
+-rw-r--r--   0     1001      123     2614 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort.rs
+-rw-r--r--   0     1001      123      643 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers.rs
+-rw-r--r--   0     1001      123    18919 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/bbox.rs
+-rw-r--r--   0     1001      123     2613 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/clipping/bbox_own_areas.rs
+-rw-r--r--   0     1001      123     1803 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/clipping/clipping_py.rs
+-rw-r--r--   0     1001      123     3347 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/clipping.rs
+-rw-r--r--   0     1001      123    11445 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_box.rs
+-rw-r--r--   0     1001      123    10152 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_point.rs
+-rw-r--r--   0     1001      123     5029 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_point_vec.rs
+-rw-r--r--   0     1001      123     2435 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/kalman.rs
+-rw-r--r--   0     1001      123     2104 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/nms/nms_py.rs
+-rw-r--r--   0     1001      123     5115 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/nms.rs
+-rw-r--r--   0     1001      123       30 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/point.rs
+-rw-r--r--   0     1001      123      612 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/primitive.rs
+-rw-r--r--   0     1001      123      466 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils.rs
+-rw-r--r--   0        0        0    16190 1970-01-01 00:00:00.000000 similari_trackers_rs-0.26.4/PKG-INFO
```

### Comparing `similari_trackers_rs-0.26.2/Cargo.toml` & `similari_trackers_rs-0.26.4/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [package]
-name = "similari"
+name = "similari-trackers-rs"
 authors = ["Ivan Kudriavtsev <ivan.a.kudryavtsev@gmail.com>"]
 description = "Machine learning framework for building object trackers and similarity search engines"
 homepage = "https://github.com/insight-platform/Similari"
 repository = "https://github.com/insight-platform/Similari"
 readme = "README.md"
 keywords = ["machine-learning", "similarity", "tracking", "SORT", "DeepSORT"]
 categories = ["algorithms", "data-structures", "computer-vision", "science"]
-version = "0.26.2"
+version = "0.26.4"
 edition = "2021"
 license="Apache-2.0"
 rust-version = "1.66"
 
 [lib]
 crate-type = ["cdylib", "lib"]
+name = "similari"
 
 [dependencies]
 itertools = "0.10"
 anyhow = "1.0"
 thiserror = "1.0"
 once_cell = "1.17"
 num_cpus = "1.15"
```

### Comparing `similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-python-3_10.yml` & `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_11.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Docker Python 3.10
+name: Docker Python 3.11
 
 # This workflow uses actions that are not certified by GitHub.
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
 on:
@@ -17,15 +17,15 @@
   # github.repository as <account>/<repo>
   IMAGE_NAME: ${{ github.repository }}
 
 
 jobs:
   build:
 
-    runs-on: ubuntu-22.04
+    runs-on: ubuntu-latest
     permissions:
       contents: read
       packages: write
       # This is used to complete the identity challenge
       # with sigstore/fulcio when running outside of PRs.
       id-token: write
 
@@ -59,11 +59,11 @@
           images: ${{ env.REGISTRY }}/${{ env.IMAGE_NAME }}
 
       - name: Build Python API with Maturin (Rust base image)
         id: build-and-push
         uses: docker/build-push-action@ad44023a93711e3deb337508980b4b5e9bcdc5dc
         with:
           context: .
-          file: docker/python_3.10/Dockerfile
+          file: docker/python_3.11/Dockerfile
           push: false
           tags: ${{ steps.meta.outputs.tags }}
           labels: ${{ steps.meta.outputs.labels }}
```

### Comparing `similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-python-3_11.yml` & `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_8.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Docker Python 3.11
+name: Docker Python 3.8
 
 # This workflow uses actions that are not certified by GitHub.
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
 on:
@@ -17,15 +17,15 @@
   # github.repository as <account>/<repo>
   IMAGE_NAME: ${{ github.repository }}
 
 
 jobs:
   build:
 
-    runs-on: ubuntu-22.04
+    runs-on: ubuntu-latest
     permissions:
       contents: read
       packages: write
       # This is used to complete the identity challenge
       # with sigstore/fulcio when running outside of PRs.
       id-token: write
 
@@ -59,11 +59,11 @@
           images: ${{ env.REGISTRY }}/${{ env.IMAGE_NAME }}
 
       - name: Build Python API with Maturin (Rust base image)
         id: build-and-push
         uses: docker/build-push-action@ad44023a93711e3deb337508980b4b5e9bcdc5dc
         with:
           context: .
-          file: docker/python_3.11/Dockerfile
+          file: docker/python_3.8/Dockerfile
           push: false
           tags: ${{ steps.meta.outputs.tags }}
           labels: ${{ steps.meta.outputs.labels }}
```

### Comparing `similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-python-3_8.yml` & `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_10.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Docker Python 3.8
+name: Docker Python 3.10
 
 # This workflow uses actions that are not certified by GitHub.
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
 on:
@@ -17,15 +17,15 @@
   # github.repository as <account>/<repo>
   IMAGE_NAME: ${{ github.repository }}
 
 
 jobs:
   build:
 
-    runs-on: ubuntu-22.04
+    runs-on: ubuntu-latest
     permissions:
       contents: read
       packages: write
       # This is used to complete the identity challenge
       # with sigstore/fulcio when running outside of PRs.
       id-token: write
 
@@ -59,11 +59,11 @@
           images: ${{ env.REGISTRY }}/${{ env.IMAGE_NAME }}
 
       - name: Build Python API with Maturin (Rust base image)
         id: build-and-push
         uses: docker/build-push-action@ad44023a93711e3deb337508980b4b5e9bcdc5dc
         with:
           context: .
-          file: docker/python_3.8/Dockerfile
+          file: docker/python_3.10/Dockerfile
           push: false
           tags: ${{ steps.meta.outputs.tags }}
           labels: ${{ steps.meta.outputs.labels }}
```

### Comparing `similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-python-3_9.yml` & `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_9.yml`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   # github.repository as <account>/<repo>
   IMAGE_NAME: ${{ github.repository }}
 
 
 jobs:
   build:
 
-    runs-on: ubuntu-22.04
+    runs-on: ubuntu-latest
     permissions:
       contents: read
       packages: write
       # This is used to complete the identity challenge
       # with sigstore/fulcio when running outside of PRs.
       id-token: write
```

### Comparing `similari_trackers_rs-0.26.2/.github/workflows/docker-maturin-rust-1_67.yml` & `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-rust-1_67.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   # github.repository as <account>/<repo>
   IMAGE_NAME: ${{ github.repository }}
 
 
 jobs:
   build:
 
-    runs-on: ubuntu-22.04
+    runs-on: ubuntu-latest
     permissions:
       contents: read
       packages: write
       # This is used to complete the identity challenge
       # with sigstore/fulcio when running outside of PRs.
       id-token: write
```

### Comparing `similari_trackers_rs-0.26.2/.github/workflows/maturin.yml` & `similari_trackers_rs-0.26.4/.github/workflows/maturin.yml`

 * *Files 7% similar despite different names*

```diff
@@ -38,37 +38,14 @@
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
-  windows:
-    runs-on: windows-latest
-    strategy:
-      matrix:
-        target: [x64]
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'
-          architecture: ${{ matrix.target }}
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
-
   macos:
     runs-on: macos-latest
     strategy:
       matrix:
         target: [x86_64, aarch64]
     steps:
       - uses: actions/checkout@v3
@@ -102,15 +79,15 @@
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos, sdist]
+    needs: [linux, macos, sdist]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
```

### Comparing `similari_trackers_rs-0.26.2/Cargo.lock` & `similari_trackers_rs-0.26.4/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -336,17 +336,17 @@
 checksum = "276ec31bcb4a9ee45f58bec6f9ec700ae4cf4f4f8f2fa7e06cb406bd5ffdd770"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
@@ -380,42 +380,39 @@
 name = "libc"
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.7"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "matrixmultiply"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
@@ -513,17 +510,17 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -548,17 +545,17 @@
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "pathfinding"
-version = "4.2.1"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c4eef7dd95d1ad58de5954f7368116d2663ccc01e0e03e50b724fef7eb2161c"
+checksum = "dfc597cf0c06c15bcca90fba95ee81b3a80a934403562001d0ed7d8626f7c6ae"
 dependencies = [
  "fixedbitset",
  "indexmap",
  "integer-sqrt",
  "num-traits",
  "rustc-hash",
  "thiserror",
@@ -568,17 +565,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -637,17 +634,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -713,28 +710,28 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "robust"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5864e7ef1a6b7bcf1d6ca3f655e65e724ed3b52546a0d0a663c991522f552ea"
 
@@ -812,15 +809,15 @@
 name = "serde_derive"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "simba"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
@@ -829,16 +826,16 @@
  "num-complex",
  "num-traits",
  "paste",
  "wide",
 ]
 
 [[package]]
-name = "similari"
-version = "0.26.2"
+name = "similari-trackers-rs"
+version = "0.26.4"
 dependencies = [
  "anyhow",
  "crossbeam",
  "env_logger",
  "geo",
  "itertools",
  "log",
@@ -885,17 +882,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -926,15 +923,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
@@ -946,17 +943,17 @@
 checksum = "ca0b28b9a6ce66d47e3c5666aa738c5ec5223fcdd4c263f3edc98ab6fef618b3"
 dependencies = [
  "wide",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -964,17 +961,17 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wide"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b689b6c49d6549434bf944e6b0f39238cf63693cb7a147e9d887507fffa3b223"
+checksum = "5cd0496a71f3cc6bc4bf0ed91346426a5099e93d89807e663162dc5a1069ff65"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
```

### Comparing `similari_trackers_rs-0.26.2/LICENSE` & `similari_trackers_rs-0.26.4/LICENSE`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/README.md` & `similari_trackers_rs-0.26.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Similari
 
+Newer versions (renamed):
+
+[![Rust](https://img.shields.io/crates/v/similari-trackers-rs.svg)](https://crates.io/crates/similari-trackers-rs)
+[![Rust](https://img.shields.io/crates/d/similari-trackers-rs.svg)](https://crates.io/crates/similari-trackers-rs)
+[![Rust](https://img.shields.io/github/license/insight-platform/Similari.svg)](https://img.shields.io/github/license/insight-platform/Similari.svg)
+
+[![PyPI version](https://badge.fury.io/py/similari-trackers-rs.svg)](https://pypi.org/project/similari-trackers-rs/)
+
+Older versions:
+
+[![Rust](https://img.shields.io/crates/v/similari.svg)](https://crates.io/crates/similari)
 [![Rust](https://img.shields.io/crates/d/similari.svg)](https://crates.io/crates/similari)
-[![Rust](https://img.shields.io/crates/v/similari.svg)](https://img.shields.io/crates/v/similari.svg)
-[![Rust](https://github.com/insight-platform/Similari/actions/workflows/rust.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/rust.yml)
 [![Rust](https://img.shields.io/github/license/insight-platform/Similari.svg)](https://img.shields.io/github/license/insight-platform/Similari.svg)
 
+Build status:
+
+[![Rust](https://github.com/insight-platform/Similari/actions/workflows/rust.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/rust.yml)
 [![Docker Rust 1.67](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-rust-1_67.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-rust-1_67.yml)
 [![Docker Python 3.8](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_8.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_8.yml)
 [![Docker Python 3.9](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_9.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_9.yml)
 [![Docker Python 3.10](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_10.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_10.yml)
 [![Docker Python 3.11](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_11.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_11.yml)
 
 :star: Star us on GitHub — it motivates us a lot!
@@ -194,49 +206,49 @@
 
 #### Rust 1.67 Base Image
 
 If you use other rust libraries you may find it beneficial to build with base Rust 
 container (and Python 3.8):  
 
 ```
-docker build -t similari_py -f docker/rust_1.67/Dockerfile .
+docker build -t similari-trackers-rs -f docker/rust_1.67/Dockerfile .
 
 # optional: copy and install to host system
-docker run --rm -it -v $(pwd)/distfiles:/tmp similari_py cp -R /opt/dist /tmp
+docker run --rm -it -v $(pwd)/distfiles:/tmp similari-trackers-rs cp -R /opt/dist /tmp
 pip3 install --force-reinstall distfiles/dist/*.whl
 ```
 
 #### Python 3.8 Base Image
 
 Python 3.8 is still a very frequently used. Here is how to build Similari with it:
 
 ```
-docker build -t similari_py -f docker/python_3.8/Dockerfile .
+docker build -t similari-trackers-rs -f docker/python_3.8/Dockerfile .
 
 # optional: copy and install to host system
-docker run --rm -it -v $(pwd)/distfiles:/tmp similari_py cp -R /opt/dist /tmp
+docker run --rm -it -v $(pwd)/distfiles:/tmp similari-trackers-rs cp -R /opt/dist /tmp
 pip3 install --force-reinstall distfiles/dist/*.whl
 ```
 
 #### Python 3.10 Base Image
 
 If you use the most recent Python environment, you can build with base Python container:
 
 ```
-docker build -t similari_py -f docker/python_3.10/Dockerfile .
+docker build -t similari-trackers-rs -f docker/python_3.10/Dockerfile .
 
 # optional: copy and install to host system
-docker run --rm -it -v $(pwd)/distfiles:/tmp similari_py cp -R /opt/dist /tmp
+docker run --rm -it -v $(pwd)/distfiles:/tmp similari-trackers-rs cp -R /opt/dist /tmp
 pip3 install --force-reinstall distfiles/dist/*.whl
 ```
 
 **NOTE**: If you are getting the `pip3` error like:
 
 ```
-ERROR: similari_py-0.22.5-cp38-cp38-manylinux_2_28_x86_64.whl is not a supported wheel on this platform.
+ERROR: similari-trackers-rs-0.26.4-cp38-cp38-manylinux_2_28_x86_64.whl is not a supported wheel on this platform.
 ```
 
 It means that the Python version in the host system doesn't match to the one that is in the image used
 to build the wheel.
 
 ### Build Python API in Host System
 
@@ -252,15 +264,15 @@
 
 1. Install build-essential tools `apt install build-essential -y`.
 
 2. Install Python3 (>= 3.8) and the development files (`python3-dev`).
 
 3. Install Maturin:
 ```
-pip3 install --upgrade maturin~=0.13
+pip3 install --upgrade maturin~=0.15
 ```
 
 4. **Not in VENV**. Build the python module: 
 
 ```
 RUSTFLAGS=" -C target-cpu=native -C opt-level=3" maturin build --release --out dist
 pip3 install --force-reinstall dist/*.whl
```

### Comparing `similari_trackers_rs-0.26.2/assets/benchmarks/benchmarks.md` & `similari_trackers_rs-0.26.4/assets/benchmarks/benchmarks.md`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/assets/documentation/python/api.md` & `similari_trackers_rs-0.26.4/assets/documentation/python/api.md`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/batch_sort_iou_tracker.rs` & `similari_trackers_rs-0.26.4/benches/batch_sort_iou_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/batch_sort_maha_tracker.rs` & `similari_trackers_rs-0.26.4/benches/batch_sort_maha_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/bbox_own_areas.rs` & `similari_trackers_rs-0.26.4/benches/bbox_own_areas.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/feature_tracker.rs` & `similari_trackers_rs-0.26.4/benches/feature_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/kalman_2d_point.rs` & `similari_trackers_rs-0.26.4/benches/kalman_2d_point.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/kalman_bbox.rs` & `similari_trackers_rs-0.26.4/benches/kalman_bbox.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/nms.rs` & `similari_trackers_rs-0.26.4/benches/nms.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/nms_oriented.rs` & `similari_trackers_rs-0.26.4/benches/nms_oriented.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/simple_search.rs` & `similari_trackers_rs-0.26.4/benches/simple_search.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/simple_sort_iou_tracker.rs` & `similari_trackers_rs-0.26.4/benches/simple_sort_iou_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/simple_sort_iou_tracker_oriented.rs` & `similari_trackers_rs-0.26.4/benches/simple_sort_iou_tracker_oriented.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/simple_sort_maha_tracker.rs` & `similari_trackers_rs-0.26.4/benches/simple_sort_maha_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/simple_sort_maha_tracker_oriented.rs` & `similari_trackers_rs-0.26.4/benches/simple_sort_maha_tracker_oriented.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/simple_visual_sort_tracker.rs` & `similari_trackers_rs-0.26.4/benches/simple_visual_sort_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/benches/track_search.rs` & `similari_trackers_rs-0.26.4/benches/track_search.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/docker/python_3.10/Dockerfile` & `similari_trackers_rs-0.26.4/docker/python_3.10/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/docker/python_3.11/Dockerfile` & `similari_trackers_rs-0.26.4/docker/python_3.11/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/docker/python_3.8/Dockerfile` & `similari_trackers_rs-0.26.4/docker/python_3.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/docker/python_3.9/Dockerfile` & `similari_trackers_rs-0.26.4/docker/python_3.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/docker/rust_1.67/Dockerfile` & `similari_trackers_rs-0.26.4/docker/rust_1.67/Dockerfile`

 * *Files 22% similar despite different names*

```diff
@@ -16,13 +16,12 @@
 RUN cargo chef cook --release --recipe-path recipe.json
 COPY .cargo/config /root/.cargo/
 COPY . .
 
 ENV RUSTFLAGS=" -C target-cpu=native -C opt-level=3"
 
 RUN cargo build --release
-#RUN maturin build --release --out dist
-#RUN pip3 install dist/*.whl
+
```

### Comparing `similari_trackers_rs-0.26.2/examples/batch_sort_iou_tracker.rs` & `similari_trackers_rs-0.26.4/examples/batch_sort_iou_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/examples/incremental_track_build.rs` & `similari_trackers_rs-0.26.4/examples/incremental_track_build.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/examples/middleware_sort_tracker.rs` & `similari_trackers_rs-0.26.4/examples/middleware_sort_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/examples/simple.rs` & `similari_trackers_rs-0.26.4/examples/simple.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/examples/simple_sort_iou_tracker.rs` & `similari_trackers_rs-0.26.4/examples/simple_sort_iou_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/examples/simple_sort_iou_tracker_oriented.rs` & `similari_trackers_rs-0.26.4/examples/simple_sort_iou_tracker_oriented.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/examples/simple_sort_maha_tracker.rs` & `similari_trackers_rs-0.26.4/examples/simple_sort_maha_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/examples/simple_sort_maha_tracker_oriented.rs` & `similari_trackers_rs-0.26.4/examples/simple_sort_maha_tracker_oriented.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/examples/track_merging.rs` & `similari_trackers_rs-0.26.4/examples/track_merging.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/bb.py` & `similari_trackers_rs-0.26.4/python/bb.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/bug_visual_sort.py` & `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/bug_visual_sort.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_1.json` & `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_1.json`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_2.json` & `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_2.json`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/in/in-1.json` & `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/in-1.json`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/bugfixes/bug_vs_1/in/in-2.json` & `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/in-2.json`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/bugfixes/github-84.py` & `similari_trackers_rs-0.26.4/python/bugfixes/github-84.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/clipping_intersection.py` & `similari_trackers_rs-0.26.4/python/clipping_intersection.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/kalman_bbox.py` & `similari_trackers_rs-0.26.4/python/kalman_bbox.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/Dockerfile` & `similari_trackers_rs-0.26.4/python/motchallenge/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/README.md` & `similari_trackers_rs-0.26.4/python/motchallenge/README.md`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/__main__.py` & `similari_trackers_rs-0.26.4/python/motchallenge/__main__.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/config.py` & `similari_trackers_rs-0.26.4/python/motchallenge/config.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/config.yml` & `similari_trackers_rs-0.26.4/python/motchallenge/config.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/confs/original-sort-config.yml` & `similari_trackers_rs-0.26.4/python/motchallenge/confs/original-sort-config.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/confs/similari-maha-sort-config.yml` & `similari_trackers_rs-0.26.4/python/motchallenge/confs/similari-maha-sort-config.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/evaluator.py` & `similari_trackers_rs-0.26.4/python/motchallenge/evaluator.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/trackers.py` & `similari_trackers_rs-0.26.4/python/motchallenge/trackers.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/motchallenge/utils.py` & `similari_trackers_rs-0.26.4/python/motchallenge/utils.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/nms.py` & `similari_trackers_rs-0.26.4/python/nms.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/sort/batch_sort_iou.py` & `similari_trackers_rs-0.26.4/python/sort/batch_sort_iou.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/sort/batch_sort_iou_bench.py` & `similari_trackers_rs-0.26.4/python/sort/batch_sort_iou_bench.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/sort/sort_idle.py` & `similari_trackers_rs-0.26.4/python/sort/sort_idle.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/sort/sort_iou.py` & `similari_trackers_rs-0.26.4/python/sort/sort_iou.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/sort/sort_iou_bench.py` & `similari_trackers_rs-0.26.4/python/sort/sort_iou_bench.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/sort/sort_iou_rotated.py` & `similari_trackers_rs-0.26.4/python/sort/sort_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/sort/sort_iou_scene_id.py` & `similari_trackers_rs-0.26.4/python/sort/sort_iou_scene_id.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/sort/sort_maha.py` & `similari_trackers_rs-0.26.4/python/sort/sort_maha.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/visual_sort/batch_visual_sort.py` & `similari_trackers_rs-0.26.4/python/visual_sort/batch_visual_sort.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/visual_sort/visual_sort.py` & `similari_trackers_rs-0.26.4/python/visual_sort/visual_sort.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/python/visual_sort.py` & `similari_trackers_rs-0.26.4/python/visual_sort.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/distance.rs` & `similari_trackers_rs-0.26.4/src/distance.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/examples/iou.rs` & `similari_trackers_rs-0.26.4/src/examples/iou.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/examples.rs` & `similari_trackers_rs-0.26.4/src/examples.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/lib.rs` & `similari_trackers_rs-0.26.4/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,19 @@
     use crate::utils::kalman::kalman_2d_point::python::{
         PyPoint2DKalmanFilter, PyPoint2DKalmanFilterState,
     };
     use crate::utils::kalman::kalman_2d_point_vec::python::PyVec2DKalmanFilter;
     use crate::utils::nms::nms_py::nms_py;
     use pyo3::prelude::*;
 
+    #[pyfunction]
+    pub fn version() -> String {
+        env!("CARGO_PKG_VERSION").to_string()
+    }
+
     #[pymodule]
     #[pyo3(name = "similari")]
     fn similari(_py: Python, m: &PyModule) -> PyResult<()> {
         let _ = env_logger::try_init();
 
         m.add_class::<BoundingBox>()?;
         m.add_class::<Universal2DBox>()?;
@@ -142,13 +147,14 @@
 
         m.add_class::<PySortPredictionBatchRequest>()?;
         m.add_class::<BatchSort>()?;
 
         m.add_class::<PyVisualSortPredictionBatchRequest>()?;
         m.add_class::<BatchVisualSort>()?;
 
+        m.add_function(wrap_pyfunction!(version, m)?)?;
         m.add_function(wrap_pyfunction!(nms_py, m)?)?;
         m.add_function(wrap_pyfunction!(sutherland_hodgman_clip_py, m)?)?;
         m.add_function(wrap_pyfunction!(intersection_area_py, m)?)?;
         Ok(())
     }
 }
```

### Comparing `similari_trackers_rs-0.26.2/src/prelude.rs` & `similari_trackers_rs-0.26.4/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track/builder.rs` & `similari_trackers_rs-0.26.4/src/track/builder.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track/store/builder.rs` & `similari_trackers_rs-0.26.4/src/track/store/builder.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track/store/store_tests.rs` & `similari_trackers_rs-0.26.4/src/track/store/store_tests.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track/store/track_distance.rs` & `similari_trackers_rs-0.26.4/src/track/store/track_distance.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track/store.rs` & `similari_trackers_rs-0.26.4/src/track/store.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track/utils.rs` & `similari_trackers_rs-0.26.4/src/track/utils.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track/voting/best.rs` & `similari_trackers_rs-0.26.4/src/track/voting/best.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track/voting/topn.rs` & `similari_trackers_rs-0.26.4/src/track/voting/topn.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track/voting.rs` & `similari_trackers_rs-0.26.4/src/track/voting.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/track.rs` & `similari_trackers_rs-0.26.4/src/track.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/batch.rs` & `similari_trackers_rs-0.26.4/src/trackers/batch.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/epoch_db.rs` & `similari_trackers_rs-0.26.4/src/trackers/epoch_db.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/kalman_prediction.rs` & `similari_trackers_rs-0.26.4/src/trackers/kalman_prediction.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/sort/batch_api.rs` & `similari_trackers_rs-0.26.4/src/trackers/sort/batch_api.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/sort/metric.rs` & `similari_trackers_rs-0.26.4/src/trackers/sort/metric.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/sort/simple_api.rs` & `similari_trackers_rs-0.26.4/src/trackers/sort/simple_api.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/sort/sort_py.rs` & `similari_trackers_rs-0.26.4/src/trackers/sort/sort_py.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/sort/voting.rs` & `similari_trackers_rs-0.26.4/src/trackers/sort/voting.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/sort.rs` & `similari_trackers_rs-0.26.4/src/trackers/sort.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/spatio_temporal_constraints.rs` & `similari_trackers_rs-0.26.4/src/trackers/spatio_temporal_constraints.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/tracker_api.rs` & `similari_trackers_rs-0.26.4/src/trackers/tracker_api.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort/batch_api.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort/batch_api.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort/metric/builder.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort/metric/builder.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort/metric.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort/metric.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort/observation_attributes.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort/observation_attributes.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort/options.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort/options.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort/simple_api.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort/simple_api.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort/track_attributes.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort/track_attributes.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort/visual_sort_py.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort/visual_sort_py.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort/voting.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort/voting.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers/visual_sort.rs` & `similari_trackers_rs-0.26.4/src/trackers/visual_sort.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/trackers.rs` & `similari_trackers_rs-0.26.4/src/trackers.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/bbox.rs` & `similari_trackers_rs-0.26.4/src/utils/bbox.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/clipping/bbox_own_areas.rs` & `similari_trackers_rs-0.26.4/src/utils/clipping/bbox_own_areas.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/clipping/clipping_py.rs` & `similari_trackers_rs-0.26.4/src/utils/clipping/clipping_py.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/clipping.rs` & `similari_trackers_rs-0.26.4/src/utils/clipping.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/kalman/kalman_2d_box.rs` & `similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_box.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/kalman/kalman_2d_point.rs` & `similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_point.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/kalman/kalman_2d_point_vec.rs` & `similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_point_vec.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/kalman.rs` & `similari_trackers_rs-0.26.4/src/utils/kalman.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/nms/nms_py.rs` & `similari_trackers_rs-0.26.4/src/utils/nms/nms_py.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/nms.rs` & `similari_trackers_rs-0.26.4/src/utils/nms.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/src/utils/primitive.rs` & `similari_trackers_rs-0.26.4/src/utils/primitive.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.2/PKG-INFO` & `similari_trackers_rs-0.26.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similari-trackers-rs
-Version: 0.26.2
+Version: 0.26.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Machine learning framework for building object trackers and similarity search engines
 Keywords: machine-learning,similarity,tracking,SORT,DeepSORT
 Home-Page: https://github.com/insight-platform/Similari
@@ -13,19 +13,31 @@
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/insight-platform/Similari
 
 # Similari
 
+Newer versions (renamed):
+
+[![Rust](https://img.shields.io/crates/v/similari-trackers-rs.svg)](https://crates.io/crates/similari-trackers-rs)
+[![Rust](https://img.shields.io/crates/d/similari-trackers-rs.svg)](https://crates.io/crates/similari-trackers-rs)
+[![Rust](https://img.shields.io/github/license/insight-platform/Similari.svg)](https://img.shields.io/github/license/insight-platform/Similari.svg)
+
+[![PyPI version](https://badge.fury.io/py/similari-trackers-rs.svg)](https://pypi.org/project/similari-trackers-rs/)
+
+Older versions:
+
+[![Rust](https://img.shields.io/crates/v/similari.svg)](https://crates.io/crates/similari)
 [![Rust](https://img.shields.io/crates/d/similari.svg)](https://crates.io/crates/similari)
-[![Rust](https://img.shields.io/crates/v/similari.svg)](https://img.shields.io/crates/v/similari.svg)
-[![Rust](https://github.com/insight-platform/Similari/actions/workflows/rust.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/rust.yml)
 [![Rust](https://img.shields.io/github/license/insight-platform/Similari.svg)](https://img.shields.io/github/license/insight-platform/Similari.svg)
 
+Build status:
+
+[![Rust](https://github.com/insight-platform/Similari/actions/workflows/rust.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/rust.yml)
 [![Docker Rust 1.67](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-rust-1_67.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-rust-1_67.yml)
 [![Docker Python 3.8](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_8.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_8.yml)
 [![Docker Python 3.9](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_9.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_9.yml)
 [![Docker Python 3.10](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_10.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_10.yml)
 [![Docker Python 3.11](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_11.yml/badge.svg?branch=main)](https://github.com/insight-platform/Similari/actions/workflows/docker-maturin-python-3_11.yml)
 
 :star: Star us on GitHub — it motivates us a lot!
@@ -211,49 +223,49 @@
 
 #### Rust 1.67 Base Image
 
 If you use other rust libraries you may find it beneficial to build with base Rust 
 container (and Python 3.8):  
 
 ```
-docker build -t similari_py -f docker/rust_1.67/Dockerfile .
+docker build -t similari-trackers-rs -f docker/rust_1.67/Dockerfile .
 
 # optional: copy and install to host system
-docker run --rm -it -v $(pwd)/distfiles:/tmp similari_py cp -R /opt/dist /tmp
+docker run --rm -it -v $(pwd)/distfiles:/tmp similari-trackers-rs cp -R /opt/dist /tmp
 pip3 install --force-reinstall distfiles/dist/*.whl
 ```
 
 #### Python 3.8 Base Image
 
 Python 3.8 is still a very frequently used. Here is how to build Similari with it:
 
 ```
-docker build -t similari_py -f docker/python_3.8/Dockerfile .
+docker build -t similari-trackers-rs -f docker/python_3.8/Dockerfile .
 
 # optional: copy and install to host system
-docker run --rm -it -v $(pwd)/distfiles:/tmp similari_py cp -R /opt/dist /tmp
+docker run --rm -it -v $(pwd)/distfiles:/tmp similari-trackers-rs cp -R /opt/dist /tmp
 pip3 install --force-reinstall distfiles/dist/*.whl
 ```
 
 #### Python 3.10 Base Image
 
 If you use the most recent Python environment, you can build with base Python container:
 
 ```
-docker build -t similari_py -f docker/python_3.10/Dockerfile .
+docker build -t similari-trackers-rs -f docker/python_3.10/Dockerfile .
 
 # optional: copy and install to host system
-docker run --rm -it -v $(pwd)/distfiles:/tmp similari_py cp -R /opt/dist /tmp
+docker run --rm -it -v $(pwd)/distfiles:/tmp similari-trackers-rs cp -R /opt/dist /tmp
 pip3 install --force-reinstall distfiles/dist/*.whl
 ```
 
 **NOTE**: If you are getting the `pip3` error like:
 
 ```
-ERROR: similari_py-0.22.5-cp38-cp38-manylinux_2_28_x86_64.whl is not a supported wheel on this platform.
+ERROR: similari-trackers-rs-0.26.4-cp38-cp38-manylinux_2_28_x86_64.whl is not a supported wheel on this platform.
 ```
 
 It means that the Python version in the host system doesn't match to the one that is in the image used
 to build the wheel.
 
 ### Build Python API in Host System
 
@@ -269,15 +281,15 @@
 
 1. Install build-essential tools `apt install build-essential -y`.
 
 2. Install Python3 (>= 3.8) and the development files (`python3-dev`).
 
 3. Install Maturin:
 ```
-pip3 install --upgrade maturin~=0.13
+pip3 install --upgrade maturin~=0.15
 ```
 
 4. **Not in VENV**. Build the python module: 
 
 ```
 RUSTFLAGS=" -C target-cpu=native -C opt-level=3" maturin build --release --out dist
 pip3 install --force-reinstall dist/*.whl
```

