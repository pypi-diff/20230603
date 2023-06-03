# Comparing `tmp/dlib-19.8.2.tar.gz` & `tmp/dlib-19.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlib-19.8.2.tar", last modified: Fri Jan 19 22:45:31 2018, max compression
+gzip compressed data, was "dist/dlib-19.9.0.tar", last modified: Tue Jan 23 00:41:51 2018, max compression
```

## Comparing `dlib-19.8.2.tar` & `dlib-19.9.0.tar`

### file list

```diff
@@ -1,1725 +1,1725 @@
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/all/
--rw-rw-r--   0 davis     (1001) davis     (1001)     3079 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/all/source.cpp
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/any/
--rw-rw-r--   0 davis     (1001) davis     (1001)     3855 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/any/any.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6057 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/any/any_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5040 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/any/any_decision_function.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6641 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/any/any_decision_function_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    26787 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/any/any_function.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9169 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/any/any_function_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    17219 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/any/any_function_impl.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1751 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/any/any_function_impl2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5246 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/any/any_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7049 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/any/any_trainer_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/appveyor/
--rw-rw-r--   0 davis     (1001) davis     (1001)      392 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/appveyor/dtest.yml
--rw-rw-r--   0 davis     (1001) davis     (1001)      403 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/appveyor/examples.yml
--rw-rw-r--   0 davis     (1001) davis     (1001)      620 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/appveyor/python.yml
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/array/
--rw-rw-r--   0 davis     (1001) davis     (1001)    20506 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array/array_kernel.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11561 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array/array_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      937 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array/array_tools.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1113 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array/array_tools_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/array2d/
--rw-rw-r--   0 davis     (1001) davis     (1001)     1583 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array2d/array2d_generic_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13052 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array2d/array2d_kernel.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8856 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array2d/array2d_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10715 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array2d/serialize_pixel_overloads.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/base64/
--rw-rw-r--   0 davis     (1001) davis     (1001)    12152 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/base64/base64_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2319 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/base64/base64_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3677 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/base64/base64_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/bayes_utils/
--rw-rw-r--   0 davis     (1001) davis     (1001)    58574 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bayes_utils/bayes_utils.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    31986 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bayes_utils/bayes_utils_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/bigint/
--rw-rw-r--   0 davis     (1001) davis     (1001)    45806 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bigint/bigint_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13743 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bigint/bigint_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    53437 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bigint/bigint_kernel_2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    14580 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bigint/bigint_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    17886 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bigint/bigint_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    32081 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bigint/bigint_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/binary_search_tree/
--rw-rw-r--   0 davis     (1001) davis     (1001)    61289 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/binary_search_tree/binary_search_tree_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    54577 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/binary_search_tree/binary_search_tree_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10463 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/binary_search_tree/binary_search_tree_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6742 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/binary_search_tree/binary_search_tree_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/bit_stream/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5098 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bit_stream/bit_stream_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3084 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bit_stream/bit_stream_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5315 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bit_stream/bit_stream_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4748 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bit_stream/bit_stream_kernel_c.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2567 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bit_stream/bit_stream_multi_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2177 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bit_stream/bit_stream_multi_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3115 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bit_stream/bit_stream_multi_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/bits/
--rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bits/c++config.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/bound_function_pointer/
--rw-rw-r--   0 davis     (1001) davis     (1001)    22856 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bound_function_pointer/bound_function_pointer_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13121 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bound_function_pointer/bound_function_pointer_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/bridge/
--rw-rw-r--   0 davis     (1001) davis     (1001)    23609 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bridge/bridge.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13062 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bridge/bridge_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/bsp/
--rw-rw-r--   0 davis     (1001) davis     (1001)    18050 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bsp/bsp.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    30785 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bsp/bsp.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    42983 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bsp/bsp_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/byte_orderer/
--rw-rw-r--   0 davis     (1001) davis     (1001)     4906 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/byte_orderer/byte_orderer_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3974 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/byte_orderer/byte_orderer_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/clustering/
--rw-rw-r--   0 davis     (1001) davis     (1001)     8930 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/clustering/bottom_up_cluster.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4526 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/clustering/bottom_up_cluster_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4556 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/clustering/chinese_whispers.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4018 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/clustering/chinese_whispers_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19209 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/clustering/modularity_clustering.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6193 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/clustering/modularity_clustering_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2776 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/clustering/spectral_cluster.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1690 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/clustering/spectral_cluster_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/cmake_utils/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/cmake_utils/test_for_cpp11/
--rw-rw-r--   0 davis     (1001) davis     (1001)      495 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/test_for_cpp11/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)      951 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/test_for_cpp11/cpp11_test.cpp
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/cmake_utils/test_for_cuda/
--rw-rw-r--   0 davis     (1001) davis     (1001)      559 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/test_for_cuda/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)      537 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/test_for_cuda/cuda_test.cu
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/cmake_utils/test_for_cudnn/
--rw-rw-r--   0 davis     (1001) davis     (1001)      702 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/test_for_cudnn/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)     1063 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/test_for_cudnn/find_cudnn.txt
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/cmake_utils/test_for_neon/
--rw-rw-r--   0 davis     (1001) davis     (1001)      106 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/test_for_neon/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)      154 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/test_for_neon/neon_test.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1252 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/add_global_compiler_switch.cmake
--rw-rw-r--   0 davis     (1001) davis     (1001)      576 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/check_if_neon_available.cmake
--rw-rw-r--   0 davis     (1001) davis     (1001)    14478 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/cmake_find_blas.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)      243 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/dlib.pc.in
--rw-rw-r--   0 davis     (1001) davis     (1001)     1911 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/dlibConfig.cmake.in
--rw-rw-r--   0 davis     (1001) davis     (1001)      219 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/release_build_by_default
--rw-rw-r--   0 davis     (1001) davis     (1001)     6240 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/set_compiler_specific_options.cmake
--rw-rw-r--   0 davis     (1001) davis     (1001)      627 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/tell_visual_studio_to_use_static_runtime.cmake
--rw-rw-r--   0 davis     (1001) davis     (1001)     4636 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake_utils/use_cpp_11.cmake
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/cmd_line_parser/
--rw-rw-r--   0 davis     (1001) davis     (1001)    18812 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_check_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18936 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_check_c.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    26645 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    26390 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6794 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_kernel_c.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6242 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_print_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6702 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmd_line_parser/get_option.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5623 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmd_line_parser/get_option_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/compress_stream/
--rw-rw-r--   0 davis     (1001) davis     (1001)     7267 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/compress_stream/compress_stream_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14574 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/compress_stream/compress_stream_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11013 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/compress_stream/compress_stream_kernel_3.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2853 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/compress_stream/compress_stream_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/conditioning_class/
--rw-rw-r--   0 davis     (1001) davis     (1001)     9281 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14755 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12279 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_3.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16023 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_4.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7951 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5231 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/config_reader/
--rw-rw-r--   0 davis     (1001) davis     (1001)    21709 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/config_reader/config_reader_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14415 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/config_reader/config_reader_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12322 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/config_reader/config_reader_thread_safe_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1369 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/config_reader/config_reader_thread_safe_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/control/
--rw-rw-r--   0 davis     (1001) davis     (1001)     3608 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/control/approximate_linear_models.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7264 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/control/approximate_linear_models_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4947 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/control/lspi.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6106 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/control/lspi_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12295 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/control/mpc.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9822 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/control/mpc_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/cpp_pretty_printer/
--rw-rw-r--   0 davis     (1001) davis     (1001)    20293 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    17299 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2673 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/cpp_tokenizer/
--rw-rw-r--   0 davis     (1001) davis     (1001)    23941 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cpp_tokenizer/cpp_tokenizer_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7263 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cpp_tokenizer/cpp_tokenizer_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3888 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cpp_tokenizer/cpp_tokenizer_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/crc32/
--rw-rw-r--   0 davis     (1001) davis     (1001)     8784 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/crc32/crc32_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3106 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/crc32/crc32_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/data_io/
--rw-rw-r--   0 davis     (1001) davis     (1001)    16628 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io/image_dataset_metadata.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5412 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io/image_dataset_metadata.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9315 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io/libsvm_io.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4348 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io/libsvm_io_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18427 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io/load_image_dataset.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16331 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io/load_image_dataset_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5400 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io/mnist.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)      849 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io/mnist.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1947 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io/mnist_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/dir_nav/
--rw-rw-r--   0 davis     (1001) davis     (1001)     3331 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/dir_nav_extensions.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4611 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/dir_nav_extensions.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6726 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/dir_nav_extensions_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7870 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    18265 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7276 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    18808 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15518 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/posix.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav/windows.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/directed_graph/
--rw-rw-r--   0 davis     (1001) davis     (1001)    25093 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/directed_graph/directed_graph_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12068 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/directed_graph/directed_graph_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/disjoint_subsets/
--rw-rw-r--   0 davis     (1001) davis     (1001)     3755 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/disjoint_subsets/disjoint_subsets.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3064 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/disjoint_subsets/disjoint_subsets_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3854 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/disjoint_subsets/disjoint_subsets_sized.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4248 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/disjoint_subsets/disjoint_subsets_sized_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/dnn/
--rw-rw-r--   0 davis     (1001) davis     (1001)   131170 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/core.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    68464 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/core_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    77232 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cpu_dlib.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13624 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cpu_dlib.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5544 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cublas_dlibapi.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1400 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cublas_dlibapi.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1795 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cuda_data_ptr.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5390 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cuda_data_ptr.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    58284 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cuda_dlib.cu
--rw-rw-r--   0 davis     (1001) davis     (1001)    11866 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cuda_dlib.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1844 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cuda_errors.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12086 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cuda_utils.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    65212 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cudnn_dlibapi.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    16995 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cudnn_dlibapi.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3488 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/curand_dlibapi.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1891 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/curand_dlibapi.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6770 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cusolver_dlibapi.cu
--rw-rw-r--   0 davis     (1001) davis     (1001)     1904 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/cusolver_dlibapi.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8502 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/gpu_data.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8127 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/gpu_data.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10382 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/gpu_data_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    29872 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/input.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18627 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/input_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)   110196 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/layers.h
--rw-rw-r--   0 davis     (1001) davis     (1001)   102864 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/layers_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)   100935 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/loss.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    57257 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/loss_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12377 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/solvers.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7718 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/solvers_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    21462 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/tensor.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    25429 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/tensor_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    23672 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/tensor_tools.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    62779 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/tensor_tools.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    52859 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    35984 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8804 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/utilities.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5157 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/utilities_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4086 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn/validation.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/entropy_decoder/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5833 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4163 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6099 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3841 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7499 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3926 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/entropy_decoder_model/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5031 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7427 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10090 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_3.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19949 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_4.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    24923 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_5.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3667 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_6.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3681 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/entropy_encoder/
--rw-rw-r--   0 davis     (1001) davis     (1001)     6767 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3590 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6586 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3269 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5699 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3373 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/entropy_encoder_model/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5094 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7482 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10507 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_3.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18168 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_4.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    26061 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_5.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3640 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_6.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3845 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2029 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/cblas/
--rw-rw-r--   0 davis     (1001) davis     (1001)     3173 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)      413 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/README
--rw-rw-r--   0 davis     (1001) davis     (1001)    32497 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      499 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_caxpy.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      471 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ccopy.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      558 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cdotc_sub.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      560 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cdotu_sub.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3904 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cgbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2585 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cgemm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3787 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cgemv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1755 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cgerc.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      957 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cgeru.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3178 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_chbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2265 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_chemm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3128 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_chemv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2238 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cher.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3102 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cher2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2476 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cher2k.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2282 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cherk.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3057 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_chpmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2163 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_chpr.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2939 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_chpr2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      416 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cscal.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      418 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_csscal.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      466 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_cswap.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2271 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_csymm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2391 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_csyr2k.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2282 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_csyrk.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3455 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ctbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3464 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ctbsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3267 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ctpmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3277 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ctpsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3330 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ctrmm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3386 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ctrmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3370 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ctrsm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3402 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ctrsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      472 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dasum.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      505 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_daxpy.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      475 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dcopy.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      575 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_ddot.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1997 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dgbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2580 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dgemm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1842 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dgemv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      978 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dger.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      471 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dnrm2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      497 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_drot.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      253 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_drotg.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      376 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_drotm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      304 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_drotmg.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1725 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dsbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      418 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dscal.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      580 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dsdot.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1602 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dspmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1373 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dspr.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1469 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dspr2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      470 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dswap.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2275 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dsymm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1668 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dsymv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1446 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dsyr.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1615 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dsyr2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2414 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dsyr2k.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2287 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dsyrk.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2775 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dtbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2785 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dtbsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2598 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dtpmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2599 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dtpsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3340 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dtrmm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2742 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dtrmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3426 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dtrsm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2728 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dtrsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      475 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dzasum.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      475 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/cblas/cblas_dznrm2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    29053 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_f77.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      497 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_icamax.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      499 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_idamax.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      498 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_isamax.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      499 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_izamax.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      469 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sasum.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      556 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_saxpy.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      473 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_scasum.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      473 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_scnrm2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      473 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_scopy.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      571 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sdot.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      608 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sdsdot.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2004 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sgbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2664 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sgemm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1823 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sgemv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      944 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sger.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      469 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_snrm2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      504 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_srot.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      249 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_srotg.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      490 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_srotm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      299 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_srotmg.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1650 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ssbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      416 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sscal.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1583 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sspmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1373 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sspr.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1470 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sspr2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      468 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_sswap.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2349 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ssymm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1663 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ssymv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1442 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ssyr.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1611 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ssyr2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2489 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ssyr2k.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2365 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ssyrk.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2800 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_stbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2784 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_stbsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2611 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_stpmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2597 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_stpsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3312 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_strmm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2741 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_strmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3340 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_strsm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2726 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_strsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1863 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_xerbla.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      499 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zaxpy.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      471 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zcopy.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      570 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zdotc_sub.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      572 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zdotu_sub.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      420 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zdscal.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3921 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zgbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2582 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zgemm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3751 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zgemv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     1760 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zgerc.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      957 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zgeru.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3188 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zhbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2266 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zhemm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3136 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zhemv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2214 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zher.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3118 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zher2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2476 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zher2k.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2284 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zherk.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3067 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zhpmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2169 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zhpr.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2963 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zhpr2.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      414 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zscal.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      468 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zswap.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2272 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zsymm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2391 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zsyr2k.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2282 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_zsyrk.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3457 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ztbmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3466 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ztbsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3269 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ztpmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3279 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ztpsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3349 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ztrmm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3402 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ztrmv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3371 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ztrsm.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3404 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cblas_ztrsv.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      320 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cdotcsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      320 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/cdotusub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      315 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/dasumsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      329 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/ddotsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      314 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/dnrm2sub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      329 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/dsdotsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      318 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/dzasumsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      318 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/dznrm2sub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      306 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/icamaxsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      315 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/idamaxsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      303 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/isamaxsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      313 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/izamaxsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      290 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/sasumsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      299 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/scasumsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      299 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/scnrm2sub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      311 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/sdotsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      323 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/sdsdotsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      290 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/snrm2sub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      334 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/zdotcsub.f
--rw-rw-r--   0 davis     (1001) davis     (1001)      334 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/cblas/zdotusub.f
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/libjpeg/
--rw-rw-r--   0 davis     (1001) davis     (1001)    19945 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/README
--rw-rw-r--   0 davis     (1001) davis     (1001)     9117 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcapimin.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5877 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcapistd.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    16375 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jccoefct.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    14642 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jccolor.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12341 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcdctmgr.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    28109 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jchuff.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1571 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jchuff.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2345 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcinit.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9156 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcmainct.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    17240 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcmarker.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    19881 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcmaster.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3110 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcomapi.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1258 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jconfig.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    21359 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcparam.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    24958 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcphuff.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12060 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcprepct.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    18773 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jcsample.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12621 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdapimin.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9328 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdapistd.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5115 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdatadst.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7591 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdatasrc.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    25129 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdcoefct.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12737 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdcolor.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7030 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdct.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8291 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jddctmgr.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    20844 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdhuff.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8063 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdhuff.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13496 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdinput.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    20358 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdmainct.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    41100 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdmarker.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    19698 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdmaster.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13793 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdmerge.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    20571 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdphuff.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9651 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdpostct.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    16215 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jdsample.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7797 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jerror.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13936 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jerror.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5486 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jfdctflt.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7573 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jfdctfst.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11047 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jfdctint.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8443 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jidctflt.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13163 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jidctfst.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    14785 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jidctint.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13493 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jidctred.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3250 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jinclude.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    40968 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jmemmgr.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2658 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jmemnobs.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8230 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jmemsys.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12454 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jmorecfg.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15621 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jpegint.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    46189 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jpeglib.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    31123 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jquant1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    48198 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jquant2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5168 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jutils.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)      360 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libjpeg/jversion.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/libpng/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/libpng/arm/
--rw-rw-r--   0 davis     (1001) davis     (1001)     6994 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/arm/arm_init.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     8118 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/arm/filter_neon.S
--rw-rw-r--   0 davis     (1001) davis     (1001)    10923 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/arm/filter_neon_intrinsics.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     4202 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/LICENSE
--rw-rw-r--   0 davis     (1001) davis     (1001)    10485 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/README
--rw-rw-r--   0 davis     (1001) davis     (1001)   148015 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/png.c
--rw-rw-r--   0 davis     (1001) davis     (1001)   149050 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/png.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    22728 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngconf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5403 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngdebug.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    28412 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngerror.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    32795 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngget.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    12346 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pnginfo.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7266 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pnglibconf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8104 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngmem.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    36273 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngpread.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    84534 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngpriv.h
--rw-rw-r--   0 davis     (1001) davis     (1001)   133400 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngread.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     3922 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngrio.c
--rw-rw-r--   0 davis     (1001) davis     (1001)   170860 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngrtran.c
--rw-rw-r--   0 davis     (1001) davis     (1001)   140849 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngrutil.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    46726 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngset.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    20408 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngstruct.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    24936 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngtrans.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     5594 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngwio.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    74233 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngwrite.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    17293 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngwtran.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    88955 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/libpng/pngwutil.c
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/pybind11/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/pybind11/include/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/
--rw-rw-r--   0 davis     (1001) davis     (1001)    24766 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    37956 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3566 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15281 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11446 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1429 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/typeid.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18946 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4326 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    85700 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6616 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      120 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/common.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2001 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/complex.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    29396 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7419 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3865 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2944 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5388 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    65580 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8749 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2031 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/options.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    89681 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    51434 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/pytypes.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13107 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    21614 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/include/pybind11/stl_bind.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/pybind11/tools/
--rw-rw-r--   0 davis     (1001) davis     (1001)     2100 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 davis     (1001) davis     (1001)     2995 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 davis     (1001) davis     (1001)     8112 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/tools/FindPythonLibsNew.cmake
--rwxrwxr-x   0 davis     (1001) davis     (1001)     2528 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/tools/check-style.sh
--rw-rw-r--   0 davis     (1001) davis     (1001)     1098 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/tools/libsize.py
--rw-rw-r--   0 davis     (1001) davis     (1001)    10341 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/tools/mkdoc.py
--rw-rw-r--   0 davis     (1001) davis     (1001)     3952 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/external/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 davis     (1001) davis     (1001)     8388 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 davis     (1001) davis     (1001)     6371 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)     2584 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/CONTRIBUTING.md
--rw-rw-r--   0 davis     (1001) davis     (1001)     1676 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/LICENSE
--rw-rw-r--   0 davis     (1001) davis     (1001)     5807 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/pybind11/README.md
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/external/zlib/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5185 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/README
--rw-rw-r--   0 davis     (1001) davis     (1001)     4968 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/adler32.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2529 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/compress.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    13174 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/crc32.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    30562 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/crc32.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    71476 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/deflate.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    12774 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/deflate.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      678 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/gzclose.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     6944 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/gzguts.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16415 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/gzlib.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    18694 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/gzread.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    16199 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/gzwrite.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    22709 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/infback.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    13455 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/inffast.c
--rw-rw-r--   0 davis     (1001) davis     (1001)      427 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/inffast.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6332 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/inffixed.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    53512 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/inflate.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     6399 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/inflate.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13028 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/inftrees.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     2928 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/inftrees.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    44255 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/trees.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     8472 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/trees.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2003 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/uncompr.c
--rw-rw-r--   0 davis     (1001) davis     (1001)    15508 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/zconf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    87883 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/zlib.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7414 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/zutil.c
--rw-rw-r--   0 davis     (1001) davis     (1001)     6766 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/external/zlib/zutil.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib/filtering/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5048 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/filtering/kalman_filter.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7429 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/filtering/kalman_filter_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6155 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/filtering/rls_filter.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6578 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/filtering/rls_filter_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/general_hash/
--rw-rw-r--   0 davis     (1001) davis     (1001)     2204 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/general_hash/count_bits.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1115 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/general_hash/count_bits_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2387 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/general_hash/general_hash.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3727 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/general_hash/hash.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7940 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/general_hash/hash_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13086 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/general_hash/murmur_hash3.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4840 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/general_hash/murmur_hash3_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    73464 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/general_hash/random_hashing.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2375 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/general_hash/random_hashing_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/geometry/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5053 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/border_enumerator.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3872 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/border_enumerator_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11932 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/drectangle.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18009 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/drectangle_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    31566 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/point_transforms.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    28175 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/point_transforms_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    21828 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/rectangle.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    24095 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/rectangle_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    35531 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/vector.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13001 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry/vector_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/global_optimization/
--rw-rw-r--   0 davis     (1001) davis     (1001)    18877 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/global_optimization/find_max_global.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19998 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/global_optimization/find_max_global_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    33241 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/global_optimization/global_function_search.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6984 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/global_optimization/global_function_search.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    28520 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/global_optimization/global_function_search_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9719 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/global_optimization/upper_bound_function.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9368 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/global_optimization/upper_bound_function_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/graph/
--rw-rw-r--   0 davis     (1001) davis     (1001)    20892 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph/graph_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10052 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph/graph_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/graph_cuts/
--rw-rw-r--   0 davis     (1001) davis     (1001)    33622 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_cuts/find_max_factor_graph_potts.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    28911 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_cuts/find_max_factor_graph_potts_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4968 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_cuts/general_flow_graph.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2651 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_cuts/general_potts_problem.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7672 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_cuts/graph_labeler.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7741 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_cuts/graph_labeler_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19534 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_cuts/min_cut.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18333 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_cuts/min_cut_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/graph_utils/
--rw-rw-r--   0 davis     (1001) davis     (1001)    18886 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/edge_list_graphs.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14529 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/edge_list_graphs_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7604 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/find_k_nearest_neighbors_lsh.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4921 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/find_k_nearest_neighbors_lsh_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3028 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/function_objects.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6590 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/function_objects_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    40677 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/graph_utils.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16972 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/graph_utils_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3041 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/ordered_sample_pair.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3376 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/ordered_sample_pair_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4125 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/sample_pair.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5966 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils/sample_pair_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/gui_core/
--rw-rw-r--   0 davis     (1001) davis     (1001)    79763 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_core/gui_core_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    10069 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_core/gui_core_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    74720 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_core/gui_core_kernel_2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    10094 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_core/gui_core_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    27931 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_core/gui_core_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      200 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_core/windows.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      200 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_core/xlib.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/gui_widgets/
--rw-rw-r--   0 davis     (1001) davis     (1001)    95842 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/base_widgets.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    69822 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/base_widgets.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    77009 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/base_widgets_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4037 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/canvas_drawing.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    35334 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/canvas_drawing.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13193 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/canvas_drawing_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15423 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/drawable.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12851 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/drawable.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    25626 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/drawable_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    25693 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/fonts.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    20296 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/fonts.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    17859 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/fonts_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    23390 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/nativefont.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    31253 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/style.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    24320 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/style.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    28013 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/style_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)   224413 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/widgets.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)   120095 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/widgets.h
--rw-rw-r--   0 davis     (1001) davis     (1001)   117123 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets/widgets_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/hash_map/
--rw-rw-r--   0 davis     (1001) davis     (1001)    11983 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_map/hash_map_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8150 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_map/hash_map_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8252 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_map/hash_map_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/hash_set/
--rw-rw-r--   0 davis     (1001) davis     (1001)     9951 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_set/hash_set_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6553 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_set/hash_set_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5179 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_set/hash_set_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/hash_table/
--rw-rw-r--   0 davis     (1001) davis     (1001)    22306 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_table/hash_table_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16596 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_table/hash_table_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8704 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_table/hash_table_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5713 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_table/hash_table_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/http_client/
--rw-rw-r--   0 davis     (1001) davis     (1001)    24771 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/http_client/http_client.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3855 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/http_client/http_client.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5417 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/http_client/http_client_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/image_keypoint/
--rw-rw-r--   0 davis     (1001) davis     (1001)    11889 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/binned_vector_feature_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10743 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/binned_vector_feature_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6274 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/build_separable_poly_filters.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1373 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/draw_surf_points.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      861 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/draw_surf_points_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11767 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/fine_hog_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9866 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/fine_hog_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14089 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/hashed_feature_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10468 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/hashed_feature_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18879 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/hessian_pyramid.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8743 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/hessian_pyramid_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    20601 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/hog.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13058 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/hog_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10690 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/nearest_neighbor_feature_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8944 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/nearest_neighbor_feature_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    22326 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/poly_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11846 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/poly_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10313 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/surf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6277 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint/surf_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/image_loader/
--rw-rw-r--   0 davis     (1001) davis     (1001)    35819 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/image_loader.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4757 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/image_loader_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5084 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/jpeg_loader.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3171 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/jpeg_loader.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3754 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/jpeg_loader_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10345 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/load_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1341 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/load_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8094 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/png_loader.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7563 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/png_loader.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4535 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_loader/png_loader_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/image_processing/
--rw-rw-r--   0 davis     (1001) davis     (1001)     6798 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/box_overlap_testing.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6579 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/box_overlap_testing_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13963 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/correlation_tracker.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6425 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/correlation_tracker_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3669 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/detection_template_tools.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3291 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/detection_template_tools_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)   219037 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/frontal_face_detector.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      757 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/frontal_face_detector_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5867 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/full_object_detection.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6242 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/full_object_detection_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16060 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/generic_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19561 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/object_detector.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18644 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/object_detector_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12376 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/remove_unobtainable_rectangles.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2445 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/remove_unobtainable_rectangles_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4379 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/render_face_detections.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2458 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/render_face_detections_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    48440 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_fhog_pyramid.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    35510 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_fhog_pyramid_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13802 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10580 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    20932 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image_boxes.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    17212 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image_boxes_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12491 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image_custom.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16669 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image_custom_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    41924 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image_pyramid.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    24364 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image_pyramid_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6593 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image_pyramid_tools.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4754 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/scan_image_pyramid_tools_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7965 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/setup_hashed_features.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8717 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/setup_hashed_features_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    21208 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/shape_predictor.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8732 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/shape_predictor_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    31459 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/shape_predictor_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14149 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing/shape_predictor_trainer_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/image_saver/
--rw-rw-r--   0 davis     (1001) davis     (1001)     8216 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_saver/dng_shared.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    24098 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_saver/image_saver.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4679 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_saver/image_saver_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5647 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_saver/save_jpeg.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2239 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_saver/save_jpeg.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1927 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_saver/save_jpeg_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4443 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_saver/save_png.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5586 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_saver/save_png.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1751 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_saver/save_png_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/image_transforms/
--rw-rw-r--   0 davis     (1001) davis     (1001)    11102 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/assign_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8132 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/assign_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7577 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/colormaps.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5346 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/colormaps_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12038 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/draw.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4911 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/draw_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9783 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/edge_detector.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4342 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/edge_detector_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4318 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/equalize_histogram.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3256 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/equalize_histogram_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    56067 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/fhog.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15436 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/fhog_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13427 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/hough_transform.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5816 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/hough_transform_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    45676 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/image_pyramid.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15382 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/image_pyramid_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6003 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/integral_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5689 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/integral_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    80958 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/interpolation.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    61491 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/interpolation_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5582 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/label_connected_blobs.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7101 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/label_connected_blobs_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11119 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/lbp.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5709 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/lbp_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    29776 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/morphological_operations.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12928 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/morphological_operations_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5642 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/random_color_transform.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3524 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms/random_color_transform_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13653 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/image_transforms/random_cropper.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12387 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/image_transforms/random_cropper_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    28982 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/image_transforms/segment_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6117 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/image_transforms/segment_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    56003 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/image_transforms/spatial_filtering.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    22155 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/image_transforms/spatial_filtering_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11676 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/image_transforms/thresholding.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6042 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/image_transforms/thresholding_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/interfaces/
--rw-rw-r--   0 davis     (1001) davis     (1001)     2889 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/interfaces/cmd_line_parser_option.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3927 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/interfaces/enumerable.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1929 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/interfaces/map_pair.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6862 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/interfaces/remover.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/iosockstream/
--rw-rw-r--   0 davis     (1001) davis     (1001)     4716 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/iosockstream/iosockstream.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6644 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/iosockstream/iosockstream_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/java/
--rw-rw-r--   0 davis     (1001) davis     (1001)      877 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/java/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)    10440 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/java/cmake_swig_jni
--rw-rw-r--   0 davis     (1001) davis     (1001)    24140 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/java/java_array.h
--rwxrwxr-x   0 davis     (1001) davis     (1001)      400 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/java/run_test.sh
--rw-rw-r--   0 davis     (1001) davis     (1001)     4030 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/java/swig_api.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6840 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/java/swig_test.java
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/linker/
--rw-rw-r--   0 davis     (1001) davis     (1001)     9137 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/linker/linker_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4494 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/linker/linker_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5232 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/linker/linker_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/logger/
--rw-rw-r--   0 davis     (1001) davis     (1001)     1007 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/logger/extra_logger_headers.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1164 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/logger/extra_logger_headers.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7209 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/logger/logger_config_file.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4896 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/logger/logger_config_file.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14711 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/logger/logger_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    20586 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/logger/logger_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15742 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/logger/logger_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/lsh/
--rw-rw-r--   0 davis     (1001) davis     (1001)     7611 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lsh/create_random_projection_hash.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6149 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lsh/create_random_projection_hash_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5683 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lsh/hashes.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8836 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lsh/hashes_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3375 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lsh/projection_hash.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3694 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lsh/projection_hash_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/lz77_buffer/
--rw-rw-r--   0 davis     (1001) davis     (1001)     7913 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lz77_buffer/lz77_buffer_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15320 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lz77_buffer/lz77_buffer_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7617 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lz77_buffer/lz77_buffer_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5559 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lz77_buffer/lz77_buffer_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/lzp_buffer/
--rw-rw-r--   0 davis     (1001) davis     (1001)     6212 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lzp_buffer/lzp_buffer_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8804 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lzp_buffer/lzp_buffer_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4190 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lzp_buffer/lzp_buffer_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2822 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lzp_buffer/lzp_buffer_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/manifold_regularization/
--rw-rw-r--   0 davis     (1001) davis     (1001)    11852 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/manifold_regularization/linear_manifold_regularizer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6571 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/manifold_regularization/linear_manifold_regularizer_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/map/
--rw-rw-r--   0 davis     (1001) davis     (1001)    10838 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/map/map_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7646 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/map/map_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7567 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/map/map_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/matlab/
--rw-rw-r--   0 davis     (1001) davis     (1001)      713 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)      670 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/README.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)    27469 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/call_matlab.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4613 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/cmake_mex_wrapper
--rw-rw-r--   0 davis     (1001) davis     (1001)      354 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/example.m
--rw-rw-r--   0 davis     (1001) davis     (1001)     1445 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/example_mex_callback.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1873 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/example_mex_class.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3194 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/example_mex_function.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1257 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/example_mex_struct.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)   216553 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/mex_wrapper.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    16071 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/subprocess_stream.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7917 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matlab/subprocess_stream.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/matrix/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/matrix/lapack/
--rw-rw-r--   0 davis     (1001) davis     (1001)     2413 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/fortran_id.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10711 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/gees.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9125 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/geev.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5616 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/geqrf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14566 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/gesdd.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12944 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/gesvd.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4207 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/getrf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8057 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/ormqr.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5552 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/pbtrf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5522 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/potrf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7181 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/syev.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18408 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/lapack/syevr.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      658 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/cblas_constants.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    69346 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    27630 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    37798 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_assign.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12794 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_assign_fwd.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    73224 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_blas_bindings.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7010 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_cholesky.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2170 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_conj_trans.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9972 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_conv.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5432 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_conv_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    37469 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_data_layout.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1246 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_data_layout_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4761 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_default_mul.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    41069 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_eigenvalue.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8629 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_exp.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7342 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_exp_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8309 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_expressions.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    30761 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_fft.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3890 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_fft_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      775 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_fwd.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2094 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_generic_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    53007 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_la.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    38221 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_la_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10812 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_lu.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    22303 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_mat.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7233 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_mat_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14756 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_math_functions.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    20300 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_math_functions_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    22727 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_op.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12877 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_qr.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2974 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_read_from_istream.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    51643 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_subexp.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19563 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_subexp_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    25739 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_trsm.h
--rw-rw-r--   0 davis     (1001) davis     (1001)   150323 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_utilities.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    61159 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/matrix_utilities_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14963 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/symmetric_matrix_cache.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3168 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix/symmetric_matrix_cache_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/md5/
--rw-rw-r--   0 davis     (1001) davis     (1001)    19273 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/md5/md5_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1177 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/md5/md5_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2243 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/md5/md5_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/member_function_pointer/
--rw-rw-r--   0 davis     (1001) davis     (1001)     3878 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/member_function_pointer/make_mfp.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5776 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/member_function_pointer/make_mfp_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19689 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/member_function_pointer/member_function_pointer_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12121 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/member_function_pointer/member_function_pointer_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/memory_manager/
--rw-rw-r--   0 davis     (1001) davis     (1001)     7695 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager/memory_manager_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7077 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager/memory_manager_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11639 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager/memory_manager_kernel_3.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4706 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager/memory_manager_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/memory_manager_global/
--rw-rw-r--   0 davis     (1001) davis     (1001)     2894 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager_global/memory_manager_global_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6429 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager_global/memory_manager_global_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/memory_manager_stateless/
--rw-rw-r--   0 davis     (1001) davis     (1001)     1996 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager_stateless/memory_manager_stateless_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3176 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager_stateless/memory_manager_stateless_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4866 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager_stateless/memory_manager_stateless_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/misc_api/
--rw-rw-r--   0 davis     (1001) davis     (1001)     4024 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/misc_api/misc_api_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2779 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/misc_api/misc_api_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3035 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/misc_api/misc_api_kernel_2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1928 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/misc_api/misc_api_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4766 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/misc_api/misc_api_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1224 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/misc_api/misc_api_shared.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      200 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/misc_api/posix.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      200 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/misc_api/windows.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/mlp/
--rw-rw-r--   0 davis     (1001) davis     (1001)    12437 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/mlp/mlp_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6833 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/mlp/mlp_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5820 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/mlp/mlp_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/numerical_integration/
--rw-rw-r--   0 davis     (1001) davis     (1001)     2504 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/numerical_integration/integrate_function_adapt_simpson.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1224 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/numerical_integration/integrate_function_adapt_simpson_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/opencv/
--rw-rw-r--   0 davis     (1001) davis     (1001)     6775 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/opencv/cv_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9413 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/opencv/cv_image_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1393 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/opencv/to_open_cv.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1045 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/opencv/to_open_cv_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/optimization/
--rw-rw-r--   0 davis     (1001) davis     (1001)    13085 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/elastic_net.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6517 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/elastic_net_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12747 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/find_max_factor_graph_nmplp.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13713 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/find_max_factor_graph_nmplp_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9830 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/find_max_factor_graph_viterbi.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5639 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/find_max_factor_graph_viterbi_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13314 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/find_max_parse_cky.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15951 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/find_max_parse_cky_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4218 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/find_optimal_parameters.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2346 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/find_optimal_parameters_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9739 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/max_cost_assignment.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2217 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/max_cost_assignment_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9119 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/max_sum_submatrix.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1771 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/max_sum_submatrix_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    26378 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    21519 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)   137881 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_bobyqa.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4809 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_bobyqa_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11153 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_least_squares.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4995 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_least_squares_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    28579 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_line_search.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13276 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_line_search_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15879 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_oca.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13845 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_oca_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10381 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_search_strategies.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12486 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_search_strategies_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14626 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_solve_qp2_using_smo.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5858 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_solve_qp2_using_smo_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14047 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_solve_qp3_using_smo.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5617 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_solve_qp3_using_smo_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    38339 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_solve_qp_using_smo.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13849 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_solve_qp_using_smo_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5302 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_stop_strategies.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5310 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_stop_strategies_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    20806 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_trust_region.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9926 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization/optimization_trust_region_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/pipe/
--rw-rw-r--   0 davis     (1001) davis     (1001)    19293 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/pipe/pipe_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11877 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/pipe/pipe_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/python/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5500 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/python/numpy.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3375 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/python/numpy_image.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      719 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/python/pyassert.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1848 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/python/pybind_utils.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2017 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/python/serialize_pickle.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/quantum_computing/
--rw-rw-r--   0 davis     (1001) davis     (1001)    28059 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/quantum_computing/quantum_computing.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18888 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/quantum_computing/quantum_computing_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/queue/
--rw-rw-r--   0 davis     (1001) davis     (1001)    13613 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/queue/queue_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15807 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/queue/queue_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6215 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/queue/queue_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4917 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/queue/queue_kernel_c.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5044 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/queue/queue_sort_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2158 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/queue/queue_sort_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/rand/
--rw-rw-r--   0 davis     (1001) davis     (1001)     6967 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/rand/mersenne_twister.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8931 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/rand/rand_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5675 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/rand/rand_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/reference_counter/
--rw-rw-r--   0 davis     (1001) davis     (1001)     7404 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/reference_counter/reference_counter_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4202 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/reference_counter/reference_counter_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/sequence/
--rw-rw-r--   0 davis     (1001) davis     (1001)     2523 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence/sequence_compare_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2024 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence/sequence_compare_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    37951 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence/sequence_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19367 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence/sequence_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6151 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence/sequence_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6597 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence/sequence_kernel_c.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4782 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence/sequence_sort_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1551 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence/sequence_sort_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1504 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence/sequence_sort_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/server/
--rw-rw-r--   0 davis     (1001) davis     (1001)    13768 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server/server_http.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6472 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server/server_http.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15608 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server/server_http_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      350 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server/server_iostream.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4060 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server/server_iostream.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3178 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server/server_iostream_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16353 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server/server_kernel.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7756 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server/server_kernel.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12975 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server/server_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/set/
--rw-rw-r--   0 davis     (1001) davis     (1001)     2851 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/set/set_compare_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3089 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/set/set_compare_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8899 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/set/set_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5831 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/set/set_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5232 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/set/set_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/set_utils/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5442 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/set_utils/set_utils.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2616 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/set_utils/set_utils_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/simd/
--rw-rw-r--   0 davis     (1001) davis     (1001)    20525 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/simd/simd4f.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    17714 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/simd/simd4i.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12038 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/simd/simd8f.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10470 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/simd/simd8i.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5706 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/simd/simd_check.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/sliding_buffer/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5911 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/sliding_buffer/circular_buffer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6415 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/sliding_buffer/circular_buffer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5902 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/sliding_buffer/sliding_buffer_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5934 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/sliding_buffer/sliding_buffer_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6488 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/sliding_buffer/sliding_buffer_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/smart_pointers/
--rw-rw-r--   0 davis     (1001) davis     (1001)      412 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/smart_pointers/scoped_ptr.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13813 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/smart_pointers/shared_ptr.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11766 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/smart_pointers/shared_ptr_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13530 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/smart_pointers/shared_ptr_thread_safe.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11900 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/smart_pointers/shared_ptr_thread_safe_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5239 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/smart_pointers/weak_ptr.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5097 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/smart_pointers/weak_ptr_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/sockets/
--rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/posix.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9147 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/sockets_extensions.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3824 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/sockets_extensions.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10379 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/sockets_extensions_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    27924 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/sockets_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    10201 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/sockets_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    30476 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/sockets_kernel_2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    10953 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/sockets_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18613 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/sockets_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets/windows.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/sockstreambuf/
--rw-rw-r--   0 davis     (1001) davis     (1001)     4914 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockstreambuf/sockstreambuf.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4090 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockstreambuf/sockstreambuf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4339 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockstreambuf/sockstreambuf_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4219 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockstreambuf/sockstreambuf_unbuffered.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3210 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockstreambuf/sockstreambuf_unbuffered.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/sqlite/
--rw-rw-r--   0 davis     (1001) davis     (1001)    20007 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sqlite/sqlite.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    17550 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sqlite/sqlite_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4913 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sqlite/sqlite_tools.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5124 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sqlite/sqlite_tools_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/stack/
--rw-rw-r--   0 davis     (1001) davis     (1001)    12380 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/stack/stack_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5383 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/stack/stack_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4854 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/stack/stack_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/static_map/
--rw-rw-r--   0 davis     (1001) davis     (1001)    20163 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_map/static_map_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5755 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_map/static_map_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2712 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_map/static_map_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/static_set/
--rw-rw-r--   0 davis     (1001) davis     (1001)     3103 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_set/static_set_compare_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3111 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_set/static_set_compare_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10739 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_set/static_set_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4434 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_set/static_set_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2452 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_set/static_set_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/statistics/
--rw-rw-r--   0 davis     (1001) davis     (1001)     1805 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/average_precision.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2886 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/average_precision_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6923 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/cca.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9130 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/cca_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18741 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/dpca.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14842 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/dpca_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2413 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/image_feature_sampling.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1707 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/image_feature_sampling_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7942 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/lda.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5197 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/lda_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10733 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/random_subset_selector.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12210 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/random_subset_selector_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11548 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/running_gradient.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9945 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/running_gradient_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11442 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/sammon.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5355 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/sammon_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    54670 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/statistics.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    41834 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/statistics_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    22504 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/vector_normalizer_frobmetric.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12432 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics/vector_normalizer_frobmetric_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/stl_checked/
--rw-rw-r--   0 davis     (1001) davis     (1001)    12299 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/stl_checked/std_vector_c.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13030 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/stl_checked/std_vector_c_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/string/
--rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/string/cassert
--rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/string/iomanip
--rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/string/iosfwd
--rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/string/iostream
--rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/string/locale
--rw-rw-r--   0 davis     (1001) davis     (1001)    29793 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/string/string.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    20951 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/string/string_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/svm/
--rw-rw-r--   0 davis     (1001) davis     (1001)     6761 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/active_learning.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3495 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/active_learning_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7945 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/assignment_function.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13335 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/assignment_function_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6548 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_assignment_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2577 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_assignment_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9114 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_graph_labeling_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6767 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_graph_labeling_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7063 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_multiclass_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4127 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_multiclass_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16232 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_object_detection_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15093 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_object_detection_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4787 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_regression_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3204 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_regression_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4993 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_sequence_labeler.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3378 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_sequence_labeler_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6990 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_sequence_segmenter.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3698 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_sequence_segmenter_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6492 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_track_association_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2859 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/cross_validate_track_association_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16682 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/empirical_kernel_map.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    20532 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/empirical_kernel_map_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16254 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/feature_ranking.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5635 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/feature_ranking_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    27168 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/function.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    34959 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/function_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    21512 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/kcentroid.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12533 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/kcentroid_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    41691 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/kcentroid_overloads.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14833 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/kernel.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    17711 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9336 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/kernel_matrix.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4944 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/kernel_matrix_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    22134 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/kkmeans.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12954 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/kkmeans_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12347 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/krls.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6930 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/krls_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11186 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/krr_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12359 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/krr_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19731 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/linearly_independent_subset_finder.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11704 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/linearly_independent_subset_finder_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1975 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/multiclass_tools.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1585 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/multiclass_tools_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1044 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/null_df.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1754 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/null_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3595 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/null_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2085 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/num_nonnegative_weights.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9686 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/one_vs_all_decision_function.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8577 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/one_vs_all_decision_function_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7261 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/one_vs_all_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5851 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/one_vs_all_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11023 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/one_vs_one_decision_function.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8685 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/one_vs_one_decision_function_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8183 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/one_vs_one_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6010 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/one_vs_one_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    23168 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/pegasos.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    18344 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/pegasos_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14571 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/ranking_tools.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9273 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/ranking_tools_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5015 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/rbf_network.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3869 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/rbf_network_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    23484 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/reduced.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11482 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/reduced_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6819 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/rls.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6308 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/rls_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5249 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/roc_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5362 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/roc_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15504 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/rr_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10073 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/rr_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    38209 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/rvm.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8916 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/rvm_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10433 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sequence_labeler.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15332 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sequence_labeler_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    17579 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sequence_segmenter.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    22695 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sequence_segmenter_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3496 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/simplify_linear_decision_function.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2625 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/simplify_linear_decision_function_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8295 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sort_basis_vectors.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2530 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sort_basis_vectors_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10002 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sparse_kernel.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12063 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sparse_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    37333 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sparse_vector.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    24306 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/sparse_vector_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8341 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_assignment_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10469 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_assignment_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8211 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_graph_labeling_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9680 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_graph_labeling_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13053 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_object_detection_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15931 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_object_detection_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7856 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_sequence_labeling_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8749 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_sequence_labeling_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9051 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_sequence_segmentation_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8637 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_sequence_segmentation_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10887 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_assignment_problem.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3966 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_assignment_problem_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    24753 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_distributed.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14518 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_distributed_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    19772 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_graph_labeling_problem.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11299 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_graph_labeling_problem_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    23030 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_object_detection_problem.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7623 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_object_detection_problem_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    22229 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_problem.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14874 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_problem_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5455 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_problem_threaded.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2539 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_problem_threaded_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9901 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_sequence_labeling_problem.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4487 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_svm_sequence_labeling_problem_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12929 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_track_association_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9812 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/structural_track_association_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    37445 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    25562 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    20837 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_c_ekm_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13305 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_c_ekm_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    24395 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_c_linear_dcd_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14711 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_c_linear_dcd_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    23124 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_c_linear_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13372 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_c_linear_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10608 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_c_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7512 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_c_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14357 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_multiclass_linear_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9887 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_multiclass_linear_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10008 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_nu_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6834 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_nu_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8196 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_one_class_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6429 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_one_class_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15432 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_rank_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11395 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_rank_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8373 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_threaded.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2540 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svm_threaded_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12799 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svr_linear_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9786 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svr_linear_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11793 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svr_trainer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6891 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/svr_trainer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4780 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/track_association_function.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10268 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm/track_association_function_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/sync_extension/
--rw-rw-r--   0 davis     (1001) davis     (1001)     1455 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sync_extension/sync_extension_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6235 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sync_extension/sync_extension_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/test/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/test/blas_bindings/
--rw-rw-r--   0 davis     (1001) davis     (1001)      915 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/blas_bindings/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)    10248 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_dot.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9893 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_gemm.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7694 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_gemv.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6813 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_ger.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8443 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_scal_axpy.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2749 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/blas_bindings/vector.cpp
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/test/examples/
--rw-rw-r--   0 davis     (1001) davis     (1001)      271 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/examples/CMakeLists.txt
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/test/gui/
--rw-rw-r--   0 davis     (1001) davis     (1001)      564 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/gui/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)    21128 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/gui/main.cpp
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/test/tools/
--rw-rw-r--   0 davis     (1001) davis     (1001)      241 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/tools/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)     3788 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)      856 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/WINDOWS_build_and_run_all_unit_tests.bat
--rw-rw-r--   0 davis     (1001) davis     (1001)     5731 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/active_learning.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2847 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/any.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7070 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/any_function.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    18057 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/array.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    17294 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/array2d.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9580 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/assignment_learning.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5196 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/base64.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12395 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/bayes_nets.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12825 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/bigint.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    29027 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/binary_search_tree.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1166 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/binary_search_tree_kernel_1a.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1164 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/binary_search_tree_kernel_2a.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1772 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/binary_search_tree_mm1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1320 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/binary_search_tree_mm2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7642 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/bridge.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    16819 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/bsp.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2569 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/byte_orderer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    15864 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/cca.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1343 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/checkerboard.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    12352 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/clustering.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)      925 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/cmd_line_parser.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    28840 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/cmd_line_parser.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      949 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/cmd_line_parser_wchar_t.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7769 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/compress_stream.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2355 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/conditioning_class.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    29123 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/conditioning_class.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2409 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/conditioning_class_c.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    16761 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/config_reader.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    82171 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/correlation_tracker.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1818 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/crc32.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2789 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/create_iris_datafile.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)      608 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/create_iris_datafile.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7300 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/cublas.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7345 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/data_io.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    18092 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/directed_graph.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13241 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/discriminant_pca.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2624 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/test/disjoint_subsets.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4739 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/disjoint_subsets_sized.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)   118951 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/dnn.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    10732 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/ekm_and_lisf.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3548 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/elastic_net.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    21095 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/empirical_kernel_map.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    15648 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/entropy_coder.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5119 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/entropy_encoder_model.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2986 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/example.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3183 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/example_args.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    26509 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/face.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    38675 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/fft.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    48683 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/fhog.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4620 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/filtering.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    22439 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/find_max_factor_graph_nmplp.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6067 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/find_max_factor_graph_viterbi.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1507 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/find_optimal_parameters.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    28123 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/geometry.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11441 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/global_optimization.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12750 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/graph.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    38050 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/graph_cuts.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13896 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/graph_labeler.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11502 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/hash.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13999 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/hash_map.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11560 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/hash_set.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    19080 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/hash_table.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4957 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/hog_image.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    61126 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/image.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4424 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/iosockstream.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4183 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/is_same_object.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    22980 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/kcentroid.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5499 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/kernel_matrix.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4743 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/kmeans.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9800 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/learning_to_track.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    15380 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/least_squares.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    15875 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/linear_manifold_regularizer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7272 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/lspi.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    18817 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/lz77_buffer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9153 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/main.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4661 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/makefile
--rw-rw-r--   0 davis     (1001) davis     (1001)    14170 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/map.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    48018 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/matrix.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    35908 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/matrix2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    35743 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/matrix3.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    34846 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/matrix4.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5730 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/matrix_chol.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8313 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/matrix_eig.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6989 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/matrix_lu.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6160 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/matrix_qr.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4683 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/max_cost_assignment.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5092 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/max_sum_submatrix.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1772 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/md5.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13766 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/member_function_pointer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3230 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/metaprogramming.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11620 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/mpc.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8948 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/multithreaded_object.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7025 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/numerical_integration.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    41901 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/object_detector.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8456 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/oca.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    10166 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/one_vs_all_trainer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6994 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/one_vs_one_trainer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    26275 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/opt_qp_solver.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    43056 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/optimization.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13256 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/optimization_test_functions.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9096 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/optimization_test_functions.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9376 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/parallel_for.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7597 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/parse.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    19451 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/pipe.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    23069 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/pixel.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3572 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/probabilistic.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    14060 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/pyramid_down.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9980 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/queue.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12108 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/rand.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    15924 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/ranking.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5550 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/read_write_mutex.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3759 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/reference_counter.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6257 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/rls.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4917 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sammon.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    25996 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/scan_image.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7364 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sequence.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    15635 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sequence_labeler.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9458 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sequence_segmenter.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    31555 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/serialize.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    14438 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/set.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12320 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sldf.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11881 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sliding_buffer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13351 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/smart_pointers.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6508 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sockets.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6494 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sockets2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5476 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sockstreambuf.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9132 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/sparse_vector.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8660 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/stack.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8812 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/static_map.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5254 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/static_set.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    29029 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/statistics.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2877 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/std_vector_c.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12139 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/string.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    28392 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/svm.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11864 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/svm_c_linear.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    16623 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/svm_c_linear_dcd.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7138 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/svm_multiclass_linear.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    22607 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/svm_struct.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4985 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/svr_linear_trainer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     7905 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/symmetric_matrix_cache.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4441 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/tester.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5427 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/tester.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14728 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/thread_pool.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4580 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/threads.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11089 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/timer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11267 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/tokenizer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     8958 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/trust_region.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4085 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/tuple.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    13301 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/type_safe_union.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3144 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/test/vectorstream.cpp
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/threads/
--rw-rw-r--   0 davis     (1001) davis     (1001)     1196 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/async.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2878 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/async.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2274 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/async_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4212 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/auto_mutex_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6138 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/auto_mutex_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2886 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/auto_unlock_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3574 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/auto_unlock_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1111 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/create_new_thread_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      844 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/create_new_thread_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6573 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/multithreaded_object_extension.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3959 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/multithreaded_object_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6210 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/multithreaded_object_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    21499 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/parallel_for_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15671 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/parallel_for_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/posix.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5150 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/read_write_mutex_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5459 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/read_write_mutex_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2689 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/rmutex_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3733 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/rmutex_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2019 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/rsignaler_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4115 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/rsignaler_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4688 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/thread_function_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4484 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/thread_function_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9804 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/thread_pool_extension.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    44871 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/thread_pool_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    34586 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/thread_pool_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4119 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/thread_specific_data_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3123 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/thread_specific_data_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7920 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threaded_object_extension.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2652 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threaded_object_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6084 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threaded_object_extension_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      330 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threads_kernel.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1897 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threads_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3867 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threads_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1686 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threads_kernel_2.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4965 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threads_kernel_2.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    11111 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threads_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10990 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threads_kernel_shared.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    10293 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/threads_kernel_shared.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads/windows.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/timeout/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5165 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/timeout/timeout.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6402 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/timeout/timeout_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/timer/
--rw-rw-r--   0 davis     (1001) davis     (1001)     7279 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/timer/timer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9834 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/timer/timer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5823 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/timer/timer_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9943 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/timer/timer_heavy.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/tokenizer/
--rw-rw-r--   0 davis     (1001) davis     (1001)     7944 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/tokenizer/tokenizer_kernel_1.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3977 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/tokenizer/tokenizer_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9424 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/tokenizer/tokenizer_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4802 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/tokenizer/tokenizer_kernel_c.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/travis/
--rwxrwxr-x   0 davis     (1001) davis     (1001)      518 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/travis/build-and-test.sh
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/tuple/
--rw-rw-r--   0 davis     (1001) davis     (1001)    13529 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/tuple/tuple.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9170 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/tuple/tuple_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/type_safe_union/
--rw-rw-r--   0 davis     (1001) davis     (1001)    26449 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/type_safe_union/type_safe_union_kernel.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10590 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/type_safe_union/type_safe_union_kernel_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/unicode/
--rw-rw-r--   0 davis     (1001) davis     (1001)     5555 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/unicode/unicode.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    20729 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/unicode/unicode.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     7046 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/unicode/unicode_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/vectorstream/
--rw-rw-r--   0 davis     (1001) davis     (1001)     2482 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/vectorstream/unserialize.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2066 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/vectorstream/unserialize_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3770 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/vectorstream/vectorstream.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2580 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/vectorstream/vectorstream_abstract.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/dlib/xml_parser/
--rw-rw-r--   0 davis     (1001) davis     (1001)    48236 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/xml_parser/xml_parser_kernel_1.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8839 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/xml_parser/xml_parser_kernel_abstract.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     8273 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/xml_parser/xml_parser_kernel_interfaces.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    37698 2018-01-19 22:45:10.000000 dlib-19.8.2/dlib/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)     1337 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/LICENSE.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)    39033 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/algs.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      310 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/all_console.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)      298 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/all_gui.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)      308 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/any.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      257 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      328 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/array2d.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9110 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/assert.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      233 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/base64.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      259 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bayes_utils.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      825 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bigint.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1274 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/binary_search_tree.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      999 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bit_stream.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      315 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bound_function_pointer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      310 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bridge.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      217 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/bsp.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      267 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/byte_orderer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cassert
--rw-rw-r--   0 davis     (1001) davis     (1001)      404 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/clustering.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       97 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmake
--rw-rw-r--   0 davis     (1001) davis     (1001)     2679 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cmd_line_parser.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4982 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/compress_stream.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2484 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/conditioning_class.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1152 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/config.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1288 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/config.h.in
--rw-rw-r--   0 davis     (1001) davis     (1001)      990 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/config_reader.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6631 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/console_progress_indicator.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      252 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/control.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      907 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cpp_pretty_printer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      941 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cpp_tokenizer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      229 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/crc32.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/cstring
--rw-rw-r--   0 davis     (1001) davis     (1001)      397 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/data_io.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      364 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dir_nav.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      821 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/directed_graph.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      329 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/disjoint_subsets.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      654 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dlib_basic_cpp_build_tutorial.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)     1033 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dlib_include_path_tutorial.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)     1244 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/dnn.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1603 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/enable_if.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      961 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     3796 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_decoder_model.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      950 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5428 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/entropy_encoder_model.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    14334 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/error.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      297 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/filtering.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5975 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/float_details.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/fstream
--rw-rw-r--   0 davis     (1001) davis     (1001)      395 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/geometry.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      416 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/global_optimization.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      741 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      397 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_cuts.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      342 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      328 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/graph_utils_threaded.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      314 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_core.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      330 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/gui_widgets.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      303 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1732 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_map.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1546 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_set.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1644 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/hash_table.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      543 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_io.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      583 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_keypoint.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1024 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_processing.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1108 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/image_transforms.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/iomanip
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/iosfwd
--rw-rw-r--   0 davis     (1001) davis     (1001)      268 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/iosockstream.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/iostream
--rw-rw-r--   0 davis     (1001) davis     (1001)     5658 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/is_kind.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/istream
--rw-rw-r--   0 davis     (1001) davis     (1001)      233 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/linker.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/locale
--rw-rw-r--   0 davis     (1001) davis     (1001)      314 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/logger.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      295 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lsh.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      991 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lz77_buffer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      974 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/lzp_buffer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      417 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/manifold_regularization.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1488 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/map.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      682 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/matrix.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      159 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/md5.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      365 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/member_function_pointer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2069 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      729 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager_global.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2799 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/memory_manager_stateless.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2296 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/metaprogramming.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      366 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/misc_api.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      561 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/mlp.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      933 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/noncopyable.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1608 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/numeric_constants.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      363 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/numerical_integration.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      358 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/opencv.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      889 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/optimization.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/ostream
--rw-rw-r--   0 davis     (1001) davis     (1001)      225 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/pipe.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    53588 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/pixel.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1482 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/platform.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      368 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/python.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      290 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/quantum_computing.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1801 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/queue.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      223 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/rand.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2348 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/ref.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      672 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/reference_counter.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      206 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/revision.h.in
--rw-rw-r--   0 davis     (1001) davis     (1001)     1955 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sequence.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    50637 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/serialize.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      300 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/server.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1671 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/set.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      249 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/set_utils.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      300 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/simd.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      776 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/sliding_buffer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      876 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/smart_pointers.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      955 2018-01-19 22:44:05.000000 dlib-19.8.2/dlib/smart_pointers_thread_safe.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      363 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockets.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      324 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sockstreambuf.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    16126 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sort.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      261 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sparse_vector.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      247 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sqlite.h
--rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sstream
--rw-rw-r--   0 davis     (1001) davis     (1001)      712 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/stack.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2411 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/stack_trace.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     3848 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/stack_trace.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      811 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_map.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1031 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/static_set.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      559 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/statistics.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6971 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/std_allocator.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      269 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/stl_checked.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      237 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/string.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1848 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1228 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/svm_threaded.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      593 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/sync_extension.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      891 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/threads.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2552 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/time_this.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      230 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/timeout.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      250 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/timer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5672 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/timing.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      632 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/tokenizer.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      234 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/tuple.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      291 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/type_safe_union.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     2807 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/uintn.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      242 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/unicode.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4777 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/unordered_pair.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      296 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/vectorstream.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     1327 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/windows_magic.h
--rw-rw-r--   0 davis     (1001) davis     (1001)      326 2018-01-19 22:44:06.000000 dlib-19.8.2/dlib/xml_parser.h
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib.egg-info/
--rw-rw-r--   0 davis     (1001) davis     (1001)     4712 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib.egg-info/PKG-INFO
--rw-rw-r--   0 davis     (1001) davis     (1001)    54358 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib.egg-info/SOURCES.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)        1 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib.egg-info/dependency_links.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)        1 2018-01-19 22:44:25.000000 dlib-19.8.2/dlib.egg-info/not-zip-safe
--rw-rw-r--   0 davis     (1001) davis     (1001)        5 2018-01-19 22:45:30.000000 dlib-19.8.2/dlib.egg-info/top_level.txt
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/python_examples/
--rw-rw-r--   0 davis     (1001) davis     (1001)      788 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/LICENSE_FOR_EXAMPLE_PROGRAMS.txt
--rwxrwxr-x   0 davis     (1001) davis     (1001)     3599 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/cnn_face_detector.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     2753 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/correlation_tracker.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     3102 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/face_alignment.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     5072 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/face_clustering.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     3348 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/face_detector.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     3373 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/face_jitter.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     4329 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/face_landmark_detection.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     5398 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/face_recognition.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     2080 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/find_candidate_object_locations.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     2091 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/global_optimization.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     2501 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/max_cost_assignment.py
--rw-rw-r--   0 davis     (1001) davis     (1001)       41 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/requirements.txt
--rwxrwxr-x   0 davis     (1001) davis     (1001)     8466 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/sequence_segmenter.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     2413 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/svm_binary_classifier.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     7121 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/svm_rank.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)    17274 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/svm_struct.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     7057 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/train_object_detector.py
--rwxrwxr-x   0 davis     (1001) davis     (1001)     5998 2018-01-19 22:44:06.000000 dlib-19.8.2/python_examples/train_shape_predictor.py
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:30.000000 dlib-19.8.2/tools/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/tools/python/
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/tools/python/src/
--rw-rw-r--   0 davis     (1001) davis     (1001)     9962 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/basic.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6123 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/cca.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5956 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/cnn_face_detector.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1586 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/conversion.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     6908 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/correlation_tracker.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11954 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/decision_functions.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2046 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/dlib.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     9876 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/face_recognition.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    12976 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/global_optimization.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     4801 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/gui.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1198 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/image.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)      332 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/indexing.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     5572 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/matrix.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5478 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/numpy_returns.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     2330 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/numpy_returns_stub.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    20097 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/object_detection.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    11031 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/other.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5189 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/rectangles.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    32279 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/sequence_segmenter.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1949 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/serialize_object_detector.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    15097 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/shape_predictor.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)    10020 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/shape_predictor.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    13527 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/simple_object_detector.h
--rw-rw-r--   0 davis     (1001) davis     (1001)    10498 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/simple_object_detector_py.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     9053 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/svm_c_trainer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     6038 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/svm_rank_trainer.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     5461 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/svm_struct.cpp
--rw-rw-r--   0 davis     (1001) davis     (1001)     1165 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/testing_results.h
--rw-rw-r--   0 davis     (1001) davis     (1001)     4706 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/src/vector.cpp
-drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-19 22:45:31.000000 dlib-19.8.2/tools/python/test/
--rw-rw-r--   0 davis     (1001) davis     (1001)       12 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/test/.gitignore
--rw-rw-r--   0 davis     (1001) davis     (1001)     2180 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/test/test_array.py
--rw-rw-r--   0 davis     (1001) davis     (1001)     2579 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/test/test_matrix.py
--rw-rw-r--   0 davis     (1001) davis     (1001)     1003 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/test/test_point.py
--rw-rw-r--   0 davis     (1001) davis     (1001)     2014 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/test/test_range.py
--rw-rw-r--   0 davis     (1001) davis     (1001)      680 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/test/test_rgb_pixel.py
--rw-rw-r--   0 davis     (1001) davis     (1001)     2492 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/test/test_sparse_vector.py
--rw-rw-r--   0 davis     (1001) davis     (1001)     3577 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/test/test_vector.py
--rw-rw-r--   0 davis     (1001) davis     (1001)     3700 2018-01-19 22:44:06.000000 dlib-19.8.2/tools/python/CMakeLists.txt
--rw-rw-r--   0 davis     (1001) davis     (1001)      256 2018-01-19 22:44:05.000000 dlib-19.8.2/MANIFEST.in
--rw-rw-r--   0 davis     (1001) davis     (1001)     2871 2018-01-19 22:44:05.000000 dlib-19.8.2/README.md
--rw-rw-r--   0 davis     (1001) davis     (1001)     9133 2018-01-19 22:44:06.000000 dlib-19.8.2/setup.py
--rw-rw-r--   0 davis     (1001) davis     (1001)     4712 2018-01-19 22:45:31.000000 dlib-19.8.2/PKG-INFO
--rw-rw-r--   0 davis     (1001) davis     (1001)       38 2018-01-19 22:45:31.000000 dlib-19.8.2/setup.cfg
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/all/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3079 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/all/source.cpp
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/any/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3855 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6057 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5040 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any_decision_function.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6641 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any_decision_function_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    26787 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any_function.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9169 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any_function_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17219 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any_function_impl.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1751 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any_function_impl2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5246 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7049 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any/any_trainer_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/appveyor/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      392 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/appveyor/dtest.yml
+-rw-rw-r--   0 davis     (1001) davis     (1001)      403 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/appveyor/examples.yml
+-rw-rw-r--   0 davis     (1001) davis     (1001)      620 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/appveyor/python.yml
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/array/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20506 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array/array_kernel.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11561 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array/array_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      937 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array/array_tools.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1113 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array/array_tools_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/array2d/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1583 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array2d/array2d_generic_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13052 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array2d/array2d_kernel.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8856 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array2d/array2d_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10715 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array2d/serialize_pixel_overloads.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/base64/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12152 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/base64/base64_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2319 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/base64/base64_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3677 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/base64/base64_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/bayes_utils/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    58574 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bayes_utils/bayes_utils.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    31986 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bayes_utils/bayes_utils_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/bigint/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    45806 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bigint/bigint_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13743 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bigint/bigint_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    53437 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bigint/bigint_kernel_2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14580 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bigint/bigint_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17886 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bigint/bigint_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    32081 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bigint/bigint_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/binary_search_tree/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    61289 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/binary_search_tree/binary_search_tree_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    54577 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/binary_search_tree/binary_search_tree_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10463 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/binary_search_tree/binary_search_tree_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6742 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/binary_search_tree/binary_search_tree_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/bit_stream/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5098 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bit_stream/bit_stream_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3084 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bit_stream/bit_stream_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5315 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bit_stream/bit_stream_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4748 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bit_stream/bit_stream_kernel_c.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2567 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bit_stream/bit_stream_multi_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2177 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bit_stream/bit_stream_multi_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3115 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bit_stream/bit_stream_multi_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/bits/
+-rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bits/c++config.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/bound_function_pointer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22856 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bound_function_pointer/bound_function_pointer_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13121 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bound_function_pointer/bound_function_pointer_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/bridge/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    23609 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bridge/bridge.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13062 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bridge/bridge_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/bsp/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18050 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bsp/bsp.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    30785 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bsp/bsp.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    42983 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bsp/bsp_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/byte_orderer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4906 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/byte_orderer/byte_orderer_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3974 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/byte_orderer/byte_orderer_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/clustering/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8930 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/clustering/bottom_up_cluster.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4526 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/clustering/bottom_up_cluster_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4556 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/clustering/chinese_whispers.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4018 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/clustering/chinese_whispers_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19209 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/clustering/modularity_clustering.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6193 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/clustering/modularity_clustering_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2776 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/clustering/spectral_cluster.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1690 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/clustering/spectral_cluster_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/cmake_utils/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/cmake_utils/test_for_cpp11/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      495 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/test_for_cpp11/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)      951 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/test_for_cpp11/cpp11_test.cpp
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/cmake_utils/test_for_cuda/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      559 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/test_for_cuda/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)      537 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/test_for_cuda/cuda_test.cu
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/cmake_utils/test_for_cudnn/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      702 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/test_for_cudnn/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1063 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/test_for_cudnn/find_cudnn.txt
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/cmake_utils/test_for_neon/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      106 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/test_for_neon/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)      154 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/test_for_neon/neon_test.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1252 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/add_global_compiler_switch.cmake
+-rw-rw-r--   0 davis     (1001) davis     (1001)      576 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/check_if_neon_available.cmake
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14478 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/cmake_find_blas.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)      243 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/dlib.pc.in
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1911 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/dlibConfig.cmake.in
+-rw-rw-r--   0 davis     (1001) davis     (1001)      219 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/release_build_by_default
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6240 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/set_compiler_specific_options.cmake
+-rw-rw-r--   0 davis     (1001) davis     (1001)      627 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/tell_visual_studio_to_use_static_runtime.cmake
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4636 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake_utils/use_cpp_11.cmake
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/cmd_line_parser/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18812 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_check_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18936 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_check_c.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    26645 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    26390 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6794 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_kernel_c.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6242 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_print_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6702 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmd_line_parser/get_option.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5623 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmd_line_parser/get_option_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/compress_stream/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7267 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/compress_stream/compress_stream_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14574 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/compress_stream/compress_stream_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11013 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/compress_stream/compress_stream_kernel_3.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2853 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/compress_stream/compress_stream_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/conditioning_class/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9281 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14755 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12279 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_3.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16023 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_4.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7951 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5231 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/config_reader/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21709 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/config_reader/config_reader_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14415 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/config_reader/config_reader_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12322 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/config_reader/config_reader_thread_safe_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1369 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/config_reader/config_reader_thread_safe_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/control/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3608 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/control/approximate_linear_models.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7264 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/control/approximate_linear_models_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4947 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/control/lspi.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6106 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/control/lspi_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12295 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/control/mpc.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9822 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/control/mpc_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/cpp_pretty_printer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20293 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17299 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2673 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/cpp_tokenizer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    23941 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cpp_tokenizer/cpp_tokenizer_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7263 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cpp_tokenizer/cpp_tokenizer_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3888 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cpp_tokenizer/cpp_tokenizer_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/crc32/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8784 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/crc32/crc32_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3106 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/crc32/crc32_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/data_io/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16628 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io/image_dataset_metadata.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5412 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io/image_dataset_metadata.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9315 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io/libsvm_io.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4348 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io/libsvm_io_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18427 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io/load_image_dataset.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16331 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io/load_image_dataset_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5400 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io/mnist.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)      849 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io/mnist.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1947 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io/mnist_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/dir_nav/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3331 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/dir_nav_extensions.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4611 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/dir_nav_extensions.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6726 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/dir_nav_extensions_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7870 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18265 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7276 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18808 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15518 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/posix.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav/windows.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/directed_graph/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    25093 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/directed_graph/directed_graph_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12068 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/directed_graph/directed_graph_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/disjoint_subsets/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3755 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/disjoint_subsets/disjoint_subsets.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3064 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/disjoint_subsets/disjoint_subsets_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3854 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/disjoint_subsets/disjoint_subsets_sized.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4248 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/disjoint_subsets/disjoint_subsets_sized_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/dnn/
+-rw-rw-r--   0 davis     (1001) davis     (1001)   131170 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/core.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    68464 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/core_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    77232 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cpu_dlib.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13624 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cpu_dlib.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5544 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cublas_dlibapi.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1400 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cublas_dlibapi.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1795 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cuda_data_ptr.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5390 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cuda_data_ptr.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    58284 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cuda_dlib.cu
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11866 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cuda_dlib.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1844 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cuda_errors.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12086 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cuda_utils.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    65212 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cudnn_dlibapi.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16995 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cudnn_dlibapi.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3488 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/curand_dlibapi.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1891 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/curand_dlibapi.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6770 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cusolver_dlibapi.cu
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1904 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/cusolver_dlibapi.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8502 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/gpu_data.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8127 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/gpu_data.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10382 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/gpu_data_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    29872 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/input.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18627 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/input_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)   110196 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/layers.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)   102864 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/layers_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)   100935 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/loss.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    57257 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/loss_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12377 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/solvers.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7718 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/solvers_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21462 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/tensor.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    25429 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/tensor_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    23672 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn/tensor_tools.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    62779 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/dnn/tensor_tools.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    52859 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/dnn/trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    35984 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/dnn/trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8804 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/dnn/utilities.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5157 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/dnn/utilities_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4086 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/dnn/validation.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/entropy_decoder/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5833 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4163 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6099 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3841 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7499 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3926 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/entropy_decoder_model/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5031 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7427 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10090 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_3.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19949 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_4.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24923 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_5.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3667 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_6.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3681 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/entropy_encoder/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6767 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3590 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6586 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3269 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5699 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3373 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/entropy_encoder_model/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5094 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7482 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10507 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_3.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18168 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_4.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    26061 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_5.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3640 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_6.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3845 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2029 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/cblas/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3173 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/external/cblas/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)      413 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/external/cblas/README
+-rw-rw-r--   0 davis     (1001) davis     (1001)    32497 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      499 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_caxpy.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      471 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ccopy.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      558 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cdotc_sub.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      560 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cdotu_sub.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3904 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cgbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2585 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cgemm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3787 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cgemv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1755 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cgerc.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      957 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cgeru.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3178 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_chbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2265 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_chemm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3128 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_chemv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2238 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cher.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3102 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cher2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2476 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cher2k.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2282 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cherk.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3057 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_chpmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2163 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_chpr.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2939 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_chpr2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      416 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cscal.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      418 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_csscal.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      466 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_cswap.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2271 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_csymm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2391 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_csyr2k.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2282 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_csyrk.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3455 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ctbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3464 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ctbsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3267 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ctpmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3277 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ctpsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3330 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ctrmm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3386 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ctrmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3370 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ctrsm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3402 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ctrsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      472 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dasum.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      505 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_daxpy.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      475 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dcopy.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      575 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ddot.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1997 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dgbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2580 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dgemm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1842 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dgemv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      978 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dger.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      471 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dnrm2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      497 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_drot.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      253 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_drotg.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      376 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_drotm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      304 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_drotmg.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1725 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dsbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      418 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dscal.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      580 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dsdot.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1602 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dspmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1373 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dspr.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1469 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dspr2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      470 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dswap.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2275 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dsymm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1668 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dsymv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1446 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dsyr.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1615 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dsyr2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2414 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dsyr2k.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2287 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dsyrk.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2775 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dtbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2785 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dtbsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2598 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dtpmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2599 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dtpsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3340 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dtrmm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2742 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dtrmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3426 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dtrsm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2728 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dtrsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      475 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dzasum.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      475 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_dznrm2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    29053 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_f77.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      497 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_icamax.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      499 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_idamax.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      498 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_isamax.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      499 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_izamax.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      469 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sasum.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      556 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_saxpy.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      473 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_scasum.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      473 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_scnrm2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      473 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_scopy.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      571 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sdot.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      608 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sdsdot.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2004 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sgbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2664 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sgemm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1823 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sgemv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      944 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sger.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      469 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_snrm2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      504 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_srot.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      249 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_srotg.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      490 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_srotm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      299 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_srotmg.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1650 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ssbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      416 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sscal.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1583 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sspmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1373 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sspr.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1470 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sspr2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      468 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_sswap.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2349 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ssymm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1663 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ssymv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1442 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ssyr.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1611 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ssyr2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2489 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ssyr2k.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2365 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ssyrk.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2800 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_stbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2784 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_stbsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2611 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_stpmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2597 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_stpsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3312 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_strmm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2741 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_strmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3340 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_strsm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2726 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_strsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1863 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_xerbla.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      499 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zaxpy.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      471 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zcopy.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      570 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zdotc_sub.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      572 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zdotu_sub.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      420 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zdscal.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3921 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zgbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2582 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zgemm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3751 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zgemv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1760 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zgerc.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      957 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zgeru.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3188 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zhbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2266 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zhemm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3136 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zhemv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2214 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zher.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3118 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zher2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2476 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zher2k.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2284 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zherk.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3067 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zhpmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2169 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zhpr.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2963 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zhpr2.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      414 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zscal.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      468 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zswap.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2272 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zsymm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2391 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zsyr2k.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2282 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_zsyrk.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3457 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ztbmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3466 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ztbsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3269 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ztpmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3279 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ztpsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3349 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ztrmm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3402 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ztrmv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3371 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ztrsm.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3404 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cblas_ztrsv.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      320 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cdotcsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      320 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/cdotusub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      315 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/dasumsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      329 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/ddotsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      314 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/dnrm2sub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      329 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/dsdotsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      318 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/dzasumsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      318 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/dznrm2sub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      306 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/icamaxsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      315 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/idamaxsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      303 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/isamaxsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      313 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/izamaxsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      290 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/sasumsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      299 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/scasumsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      299 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/scnrm2sub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      311 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/sdotsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      323 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/sdsdotsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      290 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/snrm2sub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      334 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/zdotcsub.f
+-rw-rw-r--   0 davis     (1001) davis     (1001)      334 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/cblas/zdotusub.f
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/libjpeg/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19945 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/README
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9117 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcapimin.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5877 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcapistd.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16375 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jccoefct.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14642 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jccolor.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12341 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcdctmgr.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28109 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jchuff.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1571 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jchuff.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2345 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcinit.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9156 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcmainct.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17240 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcmarker.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19881 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcmaster.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3110 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcomapi.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1258 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jconfig.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21359 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcparam.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24958 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcphuff.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12060 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcprepct.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18773 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jcsample.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12621 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdapimin.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9328 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdapistd.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5115 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdatadst.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7591 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdatasrc.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    25129 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdcoefct.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12737 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdcolor.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7030 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdct.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8291 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jddctmgr.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20844 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdhuff.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8063 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdhuff.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13496 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdinput.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20358 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdmainct.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    41100 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdmarker.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19698 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdmaster.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13793 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdmerge.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20571 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdphuff.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9651 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdpostct.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16215 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jdsample.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7797 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jerror.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13936 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jerror.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5486 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jfdctflt.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7573 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jfdctfst.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11047 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jfdctint.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8443 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jidctflt.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13163 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jidctfst.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14785 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jidctint.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13493 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jidctred.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3250 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jinclude.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    40968 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jmemmgr.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2658 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jmemnobs.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8230 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jmemsys.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12454 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jmorecfg.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15621 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jpegint.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    46189 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jpeglib.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    31123 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jquant1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    48198 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jquant2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5168 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jutils.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)      360 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libjpeg/jversion.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/libpng/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/libpng/arm/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6994 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/arm/arm_init.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8118 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/arm/filter_neon.S
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10923 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/arm/filter_neon_intrinsics.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4202 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/LICENSE
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10485 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/README
+-rw-rw-r--   0 davis     (1001) davis     (1001)   148015 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/png.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)   149050 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/png.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22728 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngconf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5403 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngdebug.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28412 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngerror.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    32795 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngget.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12346 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pnginfo.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7266 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pnglibconf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8104 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngmem.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    36273 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngpread.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    84534 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngpriv.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)   133400 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngread.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3922 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngrio.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)   170860 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngrtran.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)   140849 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngrutil.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    46726 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngset.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20408 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngstruct.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24936 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngtrans.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5594 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngwio.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    74233 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngwrite.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17293 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngwtran.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    88955 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/libpng/pngwutil.c
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/pybind11/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/pybind11/include/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24766 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    37956 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3566 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15281 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11446 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1429 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18946 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4326 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    85700 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6616 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      120 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2001 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/complex.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    29396 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7419 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3865 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2944 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5388 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    65580 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8749 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2031 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    89681 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    51434 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/pytypes.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13107 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21614 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/include/pybind11/stl_bind.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/pybind11/tools/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2100 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2995 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8112 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/tools/FindPythonLibsNew.cmake
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     2528 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/tools/check-style.sh
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1098 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/tools/libsize.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10341 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/tools/mkdoc.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3952 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8388 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6371 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2584 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/CONTRIBUTING.md
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1676 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/LICENSE
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5807 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/pybind11/README.md
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/external/zlib/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5185 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/README
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4968 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/adler32.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2529 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/compress.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13174 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/crc32.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    30562 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/crc32.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    71476 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/deflate.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12774 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/deflate.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      678 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/gzclose.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6944 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/gzguts.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16415 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/gzlib.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18694 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/gzread.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16199 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/gzwrite.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22709 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/infback.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13455 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/inffast.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)      427 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/inffast.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6332 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/inffixed.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    53512 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/inflate.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6399 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/inflate.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13028 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/inftrees.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2928 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/inftrees.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    44255 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/trees.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8472 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/trees.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2003 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/uncompr.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15508 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/zconf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    87883 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/zlib.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7414 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/zutil.c
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6766 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/external/zlib/zutil.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/filtering/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5048 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/filtering/kalman_filter.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7429 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/filtering/kalman_filter_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6155 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/filtering/rls_filter.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6578 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/filtering/rls_filter_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/general_hash/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2204 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/general_hash/count_bits.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1115 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/general_hash/count_bits_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2387 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/general_hash/general_hash.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3727 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/general_hash/hash.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7940 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/general_hash/hash_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13398 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/general_hash/murmur_hash3.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4840 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/general_hash/murmur_hash3_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    73464 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/general_hash/random_hashing.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2375 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/general_hash/random_hashing_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/geometry/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5053 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/border_enumerator.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3872 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/border_enumerator_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11932 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/drectangle.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18009 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/drectangle_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    31566 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/point_transforms.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28175 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/point_transforms_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21828 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/rectangle.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24095 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/rectangle_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    35531 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/vector.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13001 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry/vector_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/global_optimization/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18877 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/global_optimization/find_max_global.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19998 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/global_optimization/find_max_global_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    33241 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/global_optimization/global_function_search.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6984 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/global_optimization/global_function_search.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28520 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/global_optimization/global_function_search_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9719 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/global_optimization/upper_bound_function.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9368 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/global_optimization/upper_bound_function_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/graph/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20892 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph/graph_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10052 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph/graph_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/graph_cuts/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    33622 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_cuts/find_max_factor_graph_potts.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28911 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_cuts/find_max_factor_graph_potts_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4968 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_cuts/general_flow_graph.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2651 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_cuts/general_potts_problem.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7672 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_cuts/graph_labeler.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7741 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_cuts/graph_labeler_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19534 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_cuts/min_cut.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18333 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_cuts/min_cut_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/graph_utils/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18886 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/edge_list_graphs.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14529 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/edge_list_graphs_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7604 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/find_k_nearest_neighbors_lsh.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4921 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/find_k_nearest_neighbors_lsh_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3028 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/function_objects.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6590 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/function_objects_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    40677 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/graph_utils.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16972 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/graph_utils_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3041 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/ordered_sample_pair.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3376 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/ordered_sample_pair_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4125 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/sample_pair.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5966 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils/sample_pair_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/gui_core/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    79763 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_core/gui_core_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10069 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_core/gui_core_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    74720 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_core/gui_core_kernel_2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10094 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_core/gui_core_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    27931 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_core/gui_core_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      200 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_core/windows.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      200 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_core/xlib.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/gui_widgets/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    95842 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/base_widgets.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    69822 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/base_widgets.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    77009 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/base_widgets_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4037 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/canvas_drawing.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    35334 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/canvas_drawing.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13193 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/canvas_drawing_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15423 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/drawable.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12851 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/drawable.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    25626 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/drawable_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    25693 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/fonts.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20296 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/fonts.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17859 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/fonts_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    23390 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/nativefont.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    31253 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/style.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24320 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/style.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28013 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/style_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)   224413 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/widgets.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)   120095 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/widgets.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)   117123 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets/widgets_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/hash_map/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11983 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_map/hash_map_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8150 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_map/hash_map_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8252 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_map/hash_map_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/hash_set/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9951 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_set/hash_set_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6553 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_set/hash_set_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5179 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_set/hash_set_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/hash_table/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22306 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_table/hash_table_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16596 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_table/hash_table_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8704 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_table/hash_table_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5713 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_table/hash_table_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/http_client/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24771 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/http_client/http_client.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3855 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/http_client/http_client.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5417 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/http_client/http_client_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/image_keypoint/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11889 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/binned_vector_feature_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10743 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/binned_vector_feature_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6274 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/build_separable_poly_filters.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1373 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/draw_surf_points.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      861 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/draw_surf_points_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11767 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/fine_hog_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9866 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/fine_hog_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14089 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/hashed_feature_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10468 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/hashed_feature_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18879 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/hessian_pyramid.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8743 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/hessian_pyramid_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20601 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/hog.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13058 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/hog_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10690 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/nearest_neighbor_feature_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8944 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/nearest_neighbor_feature_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22326 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/poly_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11846 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/poly_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10313 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/surf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6277 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint/surf_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/image_loader/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    35819 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/image_loader.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4757 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/image_loader_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5084 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/jpeg_loader.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3171 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/jpeg_loader.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3754 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/jpeg_loader_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10345 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/load_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1341 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/load_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8094 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/png_loader.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7563 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/png_loader.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4535 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_loader/png_loader_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/image_processing/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6798 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing/box_overlap_testing.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6579 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing/box_overlap_testing_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13963 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing/correlation_tracker.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6425 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing/correlation_tracker_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3669 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing/detection_template_tools.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3291 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing/detection_template_tools_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)   219037 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing/frontal_face_detector.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      757 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing/frontal_face_detector_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5867 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing/full_object_detection.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6242 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/full_object_detection_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16060 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/generic_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19561 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/object_detector.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18644 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/object_detector_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12376 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/remove_unobtainable_rectangles.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2445 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/remove_unobtainable_rectangles_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4379 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/render_face_detections.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2458 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/render_face_detections_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    48440 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_fhog_pyramid.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    35510 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_fhog_pyramid_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13802 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10580 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20932 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image_boxes.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17212 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image_boxes_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12491 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image_custom.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16669 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image_custom_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    41924 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image_pyramid.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24364 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image_pyramid_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6593 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image_pyramid_tools.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4754 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/scan_image_pyramid_tools_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7965 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/setup_hashed_features.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8717 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/setup_hashed_features_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21208 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/shape_predictor.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8732 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/shape_predictor_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    31459 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/shape_predictor_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14149 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_processing/shape_predictor_trainer_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/image_saver/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8216 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_saver/dng_shared.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24098 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_saver/image_saver.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4679 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_saver/image_saver_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5647 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_saver/save_jpeg.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2239 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_saver/save_jpeg.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1927 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_saver/save_jpeg_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4443 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_saver/save_png.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5586 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_saver/save_png.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1751 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_saver/save_png_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/image_transforms/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11102 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/assign_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8132 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/assign_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7577 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/colormaps.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5346 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/colormaps_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12038 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/draw.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4911 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/draw_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9783 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/edge_detector.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4342 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/edge_detector_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4318 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/equalize_histogram.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3256 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/equalize_histogram_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    56067 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/fhog.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15436 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/fhog_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13427 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/hough_transform.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5816 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/hough_transform_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    45676 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/image_pyramid.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15382 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/image_pyramid_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6003 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/integral_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5689 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/integral_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    80958 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/interpolation.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    61491 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/interpolation_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5582 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/label_connected_blobs.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7101 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/label_connected_blobs_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11119 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/lbp.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5709 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/lbp_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    29776 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/morphological_operations.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12928 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/morphological_operations_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5642 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/random_color_transform.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3524 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms/random_color_transform_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13653 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_transforms/random_cropper.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12387 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_transforms/random_cropper_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28982 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_transforms/segment_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6117 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_transforms/segment_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    56003 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_transforms/spatial_filtering.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22155 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_transforms/spatial_filtering_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11676 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_transforms/thresholding.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6042 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_transforms/thresholding_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/interfaces/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2889 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/interfaces/cmd_line_parser_option.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3927 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/interfaces/enumerable.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1929 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/interfaces/map_pair.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6862 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/interfaces/remover.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/iosockstream/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4716 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/iosockstream/iosockstream.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6644 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/iosockstream/iosockstream_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/java/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      877 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/java/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10440 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/java/cmake_swig_jni
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24140 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/java/java_array.h
+-rwxrwxr-x   0 davis     (1001) davis     (1001)      400 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/java/run_test.sh
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4030 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/java/swig_api.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6840 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/java/swig_test.java
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/linker/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9137 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/linker/linker_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4494 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/linker/linker_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5232 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/linker/linker_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/logger/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1007 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/logger/extra_logger_headers.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1164 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/logger/extra_logger_headers.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7209 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/logger/logger_config_file.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4896 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/logger/logger_config_file.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14711 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/logger/logger_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20586 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/logger/logger_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15742 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/logger/logger_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/lsh/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7611 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lsh/create_random_projection_hash.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6149 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lsh/create_random_projection_hash_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5683 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lsh/hashes.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8836 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lsh/hashes_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3375 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lsh/projection_hash.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3694 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lsh/projection_hash_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/lz77_buffer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7913 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lz77_buffer/lz77_buffer_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15320 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lz77_buffer/lz77_buffer_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7617 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lz77_buffer/lz77_buffer_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5559 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lz77_buffer/lz77_buffer_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/lzp_buffer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6212 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lzp_buffer/lzp_buffer_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8804 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lzp_buffer/lzp_buffer_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4190 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lzp_buffer/lzp_buffer_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2822 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lzp_buffer/lzp_buffer_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/manifold_regularization/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11852 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/manifold_regularization/linear_manifold_regularizer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6571 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/manifold_regularization/linear_manifold_regularizer_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/map/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10838 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/map/map_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7646 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/map/map_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7567 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/map/map_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/matlab/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      713 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)      670 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/README.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)    27469 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/call_matlab.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4613 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/cmake_mex_wrapper
+-rw-rw-r--   0 davis     (1001) davis     (1001)      354 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/example.m
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1445 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/example_mex_callback.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1873 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/example_mex_class.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3194 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/example_mex_function.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1257 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/example_mex_struct.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)   216553 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/mex_wrapper.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16071 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/subprocess_stream.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7917 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matlab/subprocess_stream.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/matrix/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/matrix/lapack/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2413 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/fortran_id.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10711 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/gees.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9125 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/geev.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5616 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/geqrf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14566 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/gesdd.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12944 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/gesvd.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4207 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/getrf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8057 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/ormqr.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5552 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/pbtrf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5522 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/potrf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7181 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/syev.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18408 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/lapack/syevr.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      658 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/cblas_constants.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    69346 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    27630 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    37798 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_assign.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12794 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_assign_fwd.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    73224 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_blas_bindings.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7010 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_cholesky.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2170 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_conj_trans.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9972 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_conv.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5432 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_conv_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    37469 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_data_layout.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1246 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_data_layout_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4761 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_default_mul.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    41069 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_eigenvalue.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8629 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_exp.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7342 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_exp_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8309 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_expressions.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    30761 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_fft.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3890 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_fft_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      775 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_fwd.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2094 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_generic_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    53419 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_la.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    38221 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_la_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10812 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_lu.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22303 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_mat.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7233 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_mat_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14756 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_math_functions.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20300 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_math_functions_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22727 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_op.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12877 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_qr.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2974 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_read_from_istream.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    51643 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_subexp.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19563 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_subexp_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    25739 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_trsm.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)   150323 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_utilities.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    61159 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/matrix_utilities_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14963 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/symmetric_matrix_cache.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3168 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix/symmetric_matrix_cache_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/md5/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19273 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/md5/md5_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1177 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/md5/md5_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2243 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/md5/md5_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/member_function_pointer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3878 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/member_function_pointer/make_mfp.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5776 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/member_function_pointer/make_mfp_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19689 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/member_function_pointer/member_function_pointer_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12121 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/member_function_pointer/member_function_pointer_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/memory_manager/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7695 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager/memory_manager_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7077 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager/memory_manager_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11639 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager/memory_manager_kernel_3.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4706 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager/memory_manager_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/memory_manager_global/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2894 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager_global/memory_manager_global_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6429 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager_global/memory_manager_global_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/memory_manager_stateless/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1996 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager_stateless/memory_manager_stateless_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3176 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager_stateless/memory_manager_stateless_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4866 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager_stateless/memory_manager_stateless_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/misc_api/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4024 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/misc_api/misc_api_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2779 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/misc_api/misc_api_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3035 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/misc_api/misc_api_kernel_2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1928 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/misc_api/misc_api_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4766 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/misc_api/misc_api_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1224 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/misc_api/misc_api_shared.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      200 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/misc_api/posix.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      200 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/misc_api/windows.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/mlp/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12437 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/mlp/mlp_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6833 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/mlp/mlp_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5820 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/mlp/mlp_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/numerical_integration/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2504 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/numerical_integration/integrate_function_adapt_simpson.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1224 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/numerical_integration/integrate_function_adapt_simpson_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/opencv/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6775 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/opencv/cv_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9413 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/opencv/cv_image_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1393 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/opencv/to_open_cv.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1045 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/opencv/to_open_cv_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/optimization/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13085 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/elastic_net.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6517 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/elastic_net_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12747 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/find_max_factor_graph_nmplp.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13713 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/find_max_factor_graph_nmplp_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9830 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/find_max_factor_graph_viterbi.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5639 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/find_max_factor_graph_viterbi_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13314 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/find_max_parse_cky.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15951 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/find_max_parse_cky_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4218 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/find_optimal_parameters.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2346 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/find_optimal_parameters_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9739 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/max_cost_assignment.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2217 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/max_cost_assignment_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9119 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/max_sum_submatrix.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1771 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/max_sum_submatrix_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    26378 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21519 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)   137881 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_bobyqa.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4809 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_bobyqa_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11153 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_least_squares.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4995 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_least_squares_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28579 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_line_search.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13276 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_line_search_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15879 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_oca.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13845 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_oca_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10381 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_search_strategies.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12486 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_search_strategies_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14626 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_solve_qp2_using_smo.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5858 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_solve_qp2_using_smo_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14047 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_solve_qp3_using_smo.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5617 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_solve_qp3_using_smo_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    38339 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_solve_qp_using_smo.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13849 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_solve_qp_using_smo_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5302 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_stop_strategies.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5310 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_stop_strategies_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20806 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_trust_region.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9926 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization/optimization_trust_region_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/pipe/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19293 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/pipe/pipe_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11877 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/pipe/pipe_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/python/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5500 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/python/numpy.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3375 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/python/numpy_image.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      719 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/python/pyassert.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1848 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/python/pybind_utils.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2017 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/python/serialize_pickle.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/quantum_computing/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28059 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/quantum_computing/quantum_computing.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18888 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/quantum_computing/quantum_computing_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/queue/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13613 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/queue/queue_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15807 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/queue/queue_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6215 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/queue/queue_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4917 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/queue/queue_kernel_c.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5044 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/queue/queue_sort_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2158 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/queue/queue_sort_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/rand/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6967 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/rand/mersenne_twister.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8931 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/rand/rand_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5675 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/rand/rand_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/reference_counter/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7404 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/reference_counter/reference_counter_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4202 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/reference_counter/reference_counter_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/sequence/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2523 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence/sequence_compare_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2024 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence/sequence_compare_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    37951 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence/sequence_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19367 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence/sequence_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6151 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence/sequence_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6597 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence/sequence_kernel_c.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4782 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence/sequence_sort_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1551 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence/sequence_sort_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1504 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence/sequence_sort_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/server/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13768 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server/server_http.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6472 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server/server_http.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15608 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server/server_http_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      350 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server/server_iostream.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4060 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server/server_iostream.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3178 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server/server_iostream_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16353 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server/server_kernel.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7756 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server/server_kernel.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12975 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server/server_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/set/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2851 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/set/set_compare_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3089 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/set/set_compare_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8899 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/set/set_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5831 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/set/set_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5232 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/set/set_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/set_utils/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5442 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/set_utils/set_utils.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2616 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/set_utils/set_utils_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/simd/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20525 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/simd/simd4f.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17714 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/simd/simd4i.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12038 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/simd/simd8f.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10470 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/simd/simd8i.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5706 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/simd/simd_check.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/sliding_buffer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5911 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sliding_buffer/circular_buffer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6415 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sliding_buffer/circular_buffer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5902 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sliding_buffer/sliding_buffer_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5934 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sliding_buffer/sliding_buffer_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6488 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sliding_buffer/sliding_buffer_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/smart_pointers/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      412 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/smart_pointers/scoped_ptr.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12261 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/smart_pointers/shared_ptr.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10687 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/smart_pointers/shared_ptr_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12189 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/smart_pointers/shared_ptr_thread_safe.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10785 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/smart_pointers/shared_ptr_thread_safe_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5239 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/smart_pointers/weak_ptr.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5097 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/smart_pointers/weak_ptr_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/sockets/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/posix.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9147 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/sockets_extensions.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3824 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/sockets_extensions.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10379 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/sockets_extensions_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    27924 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/sockets_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10201 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/sockets_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    30476 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/sockets_kernel_2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10953 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/sockets_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18613 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/sockets_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets/windows.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/sockstreambuf/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4914 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockstreambuf/sockstreambuf.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4090 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockstreambuf/sockstreambuf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4339 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockstreambuf/sockstreambuf_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4219 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockstreambuf/sockstreambuf_unbuffered.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3210 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockstreambuf/sockstreambuf_unbuffered.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/sqlite/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20007 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sqlite/sqlite.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17550 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sqlite/sqlite_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4913 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sqlite/sqlite_tools.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5124 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sqlite/sqlite_tools_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/stack/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12380 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/stack/stack_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5383 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/stack/stack_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4854 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/stack/stack_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/static_map/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20163 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_map/static_map_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5755 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_map/static_map_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2712 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_map/static_map_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/static_set/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3103 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_set/static_set_compare_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3111 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_set/static_set_compare_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10739 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_set/static_set_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4434 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_set/static_set_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2452 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_set/static_set_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/statistics/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1805 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/average_precision.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2886 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/average_precision_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6923 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/cca.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9130 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/cca_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18741 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/dpca.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14842 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/dpca_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2413 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/image_feature_sampling.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1707 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/image_feature_sampling_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7942 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/lda.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5197 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/lda_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10733 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/random_subset_selector.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12210 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/random_subset_selector_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11548 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/running_gradient.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9945 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/running_gradient_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11442 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/sammon.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5355 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/sammon_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    54670 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/statistics.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    41834 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/statistics_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22504 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/vector_normalizer_frobmetric.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12432 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics/vector_normalizer_frobmetric_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/stl_checked/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12299 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/stl_checked/std_vector_c.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13030 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/stl_checked/std_vector_c_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/string/
+-rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/string/cassert
+-rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/string/iomanip
+-rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/string/iosfwd
+-rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/string/iostream
+-rw-rw-r--   0 davis     (1001) davis     (1001)       45 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/string/locale
+-rw-rw-r--   0 davis     (1001) davis     (1001)    29793 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/string/string.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20951 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/string/string_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/svm/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6761 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/active_learning.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3495 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/active_learning_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7945 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/assignment_function.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13335 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/assignment_function_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6548 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_assignment_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2577 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_assignment_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9114 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_graph_labeling_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6767 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_graph_labeling_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7063 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_multiclass_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4127 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_multiclass_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16232 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_object_detection_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15093 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_object_detection_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4787 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_regression_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3204 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_regression_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4993 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_sequence_labeler.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3378 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_sequence_labeler_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6990 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_sequence_segmenter.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3698 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_sequence_segmenter_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6492 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_track_association_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2859 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/cross_validate_track_association_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16682 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/empirical_kernel_map.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20532 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/empirical_kernel_map_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16254 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/feature_ranking.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5635 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/feature_ranking_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    27168 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/function.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    34959 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/function_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21512 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/kcentroid.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12533 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/kcentroid_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    41691 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/kcentroid_overloads.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14833 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/kernel.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17711 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9336 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/kernel_matrix.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4944 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/kernel_matrix_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22134 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/kkmeans.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12954 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/kkmeans_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12347 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/krls.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6930 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/krls_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11186 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/krr_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12359 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/krr_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19731 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/linearly_independent_subset_finder.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11704 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/linearly_independent_subset_finder_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1975 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/multiclass_tools.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1585 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/multiclass_tools_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1044 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/null_df.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1754 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/null_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3595 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/null_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2085 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/num_nonnegative_weights.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9686 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/one_vs_all_decision_function.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8577 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/one_vs_all_decision_function_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7261 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/one_vs_all_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5851 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/one_vs_all_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11023 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/one_vs_one_decision_function.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8685 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/one_vs_one_decision_function_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8183 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/one_vs_one_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6010 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/one_vs_one_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    23137 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/pegasos.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18344 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/pegasos_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14571 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/ranking_tools.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9273 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/ranking_tools_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5015 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/rbf_network.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3869 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/rbf_network_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    23484 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/reduced.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11482 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/reduced_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6819 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/rls.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6308 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/rls_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5249 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/roc_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5362 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/roc_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15504 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/rr_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10073 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/rr_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    38209 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/rvm.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8916 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/rvm_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10433 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sequence_labeler.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15332 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sequence_labeler_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17579 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sequence_segmenter.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22695 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sequence_segmenter_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3496 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/simplify_linear_decision_function.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2625 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/simplify_linear_decision_function_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8295 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sort_basis_vectors.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2530 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sort_basis_vectors_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10002 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sparse_kernel.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12063 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sparse_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    37333 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sparse_vector.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24306 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/sparse_vector_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8341 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_assignment_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10469 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_assignment_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8211 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_graph_labeling_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9680 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_graph_labeling_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13053 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_object_detection_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15931 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_object_detection_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7856 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_sequence_labeling_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8749 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_sequence_labeling_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9051 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_sequence_segmentation_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8637 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_sequence_segmentation_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10887 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_assignment_problem.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3966 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_assignment_problem_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24753 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_distributed.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14518 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_distributed_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19772 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_graph_labeling_problem.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11299 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_graph_labeling_problem_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    23030 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_object_detection_problem.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7623 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_object_detection_problem_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22229 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_problem.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14874 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_problem_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5455 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_problem_threaded.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2539 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_problem_threaded_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9901 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_sequence_labeling_problem.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4487 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_svm_sequence_labeling_problem_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12929 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_track_association_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9812 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/structural_track_association_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    37445 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm/svm.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    25562 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20837 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_c_ekm_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13305 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_c_ekm_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    24395 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_c_linear_dcd_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14711 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_c_linear_dcd_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    23128 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_c_linear_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13372 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_c_linear_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10608 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_c_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7512 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_c_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14357 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_multiclass_linear_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9887 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_multiclass_linear_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10008 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_nu_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6834 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_nu_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8196 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_one_class_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6429 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_one_class_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15432 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_rank_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11395 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_rank_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8373 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_threaded.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2540 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svm_threaded_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12799 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svr_linear_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9786 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svr_linear_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11793 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svr_trainer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6891 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/svr_trainer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4780 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/track_association_function.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10268 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm/track_association_function_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/sync_extension/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1455 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sync_extension/sync_extension_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6235 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sync_extension/sync_extension_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/test/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/test/blas_bindings/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      915 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/blas_bindings/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10248 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_dot.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9893 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_gemm.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7694 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_gemv.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6813 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_ger.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8443 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_scal_axpy.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2749 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/blas_bindings/vector.cpp
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/test/examples/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      271 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/examples/CMakeLists.txt
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/test/gui/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      564 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/gui/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21128 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/gui/main.cpp
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/test/tools/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      241 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/tools/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3788 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)      856 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/WINDOWS_build_and_run_all_unit_tests.bat
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5731 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/active_learning.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2847 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/any.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7070 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/any_function.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18057 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/array.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17294 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/array2d.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9580 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/assignment_learning.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5196 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/base64.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12395 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/bayes_nets.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12825 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/bigint.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    29027 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/binary_search_tree.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1166 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/binary_search_tree_kernel_1a.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1164 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/binary_search_tree_kernel_2a.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1772 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/binary_search_tree_mm1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1320 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/test/binary_search_tree_mm2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7642 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/bridge.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16819 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/bsp.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2569 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/byte_orderer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    17271 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/cca.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1343 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/checkerboard.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12352 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/clustering.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)      925 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/cmd_line_parser.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28840 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/cmd_line_parser.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      949 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/cmd_line_parser_wchar_t.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7769 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/compress_stream.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2355 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/conditioning_class.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    29123 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/conditioning_class.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2409 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/conditioning_class_c.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16761 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/config_reader.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    82171 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/correlation_tracker.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1818 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/crc32.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2789 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/create_iris_datafile.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)      608 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/create_iris_datafile.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7300 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/cublas.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7345 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/data_io.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18092 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/directed_graph.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13241 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/discriminant_pca.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2624 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/disjoint_subsets.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4739 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/disjoint_subsets_sized.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)   118951 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/dnn.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10732 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/ekm_and_lisf.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3548 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/elastic_net.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21095 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/empirical_kernel_map.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15648 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/entropy_coder.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5119 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/entropy_encoder_model.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2986 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/example.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3183 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/example_args.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    26509 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/face.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    38675 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/fft.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    48683 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/fhog.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4620 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/filtering.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22439 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/find_max_factor_graph_nmplp.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6067 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/find_max_factor_graph_viterbi.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1507 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/find_optimal_parameters.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28123 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/geometry.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11441 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/global_optimization.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12750 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/graph.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    38050 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/graph_cuts.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13896 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/graph_labeler.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11502 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/hash.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13999 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/hash_map.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11560 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/hash_set.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19080 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/hash_table.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4957 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/hog_image.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    61126 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/image.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4424 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/iosockstream.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4183 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/is_same_object.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22980 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/kcentroid.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5499 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/kernel_matrix.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4743 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/kmeans.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9800 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/learning_to_track.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15380 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/least_squares.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15875 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/linear_manifold_regularizer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7272 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/lspi.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    18817 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/lz77_buffer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9153 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/main.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4661 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/makefile
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14170 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/map.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    48056 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/matrix.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    35908 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/matrix2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    35743 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/matrix3.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    34846 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/matrix4.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5730 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/matrix_chol.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8313 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/matrix_eig.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6989 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/matrix_lu.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6160 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/matrix_qr.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4683 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/max_cost_assignment.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5092 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/max_sum_submatrix.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1772 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/md5.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13766 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/member_function_pointer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3230 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/metaprogramming.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11620 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/mpc.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8948 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/multithreaded_object.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7025 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/numerical_integration.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    41901 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/object_detector.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8456 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/oca.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10166 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/one_vs_all_trainer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6994 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/one_vs_one_trainer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    26275 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/opt_qp_solver.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    43056 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/optimization.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13256 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/optimization_test_functions.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9096 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/optimization_test_functions.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9376 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/parallel_for.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7597 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/parse.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    19451 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/pipe.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    23069 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/pixel.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3572 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/probabilistic.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14060 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/pyramid_down.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9980 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/queue.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12108 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/rand.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15924 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/ranking.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5550 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/read_write_mutex.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3759 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/reference_counter.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6257 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/rls.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4917 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sammon.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    25996 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/scan_image.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7364 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sequence.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15635 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sequence_labeler.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9458 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sequence_segmenter.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    31555 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/serialize.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14438 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/set.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12320 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sldf.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11881 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sliding_buffer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13351 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/smart_pointers.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6508 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sockets.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6494 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sockets2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5476 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sockstreambuf.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9132 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/sparse_vector.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8660 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/stack.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8812 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/static_map.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5254 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/static_set.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    29029 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/statistics.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2877 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/std_vector_c.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12139 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/string.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    28392 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/svm.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11864 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/svm_c_linear.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16623 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/svm_c_linear_dcd.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7138 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/svm_multiclass_linear.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    22607 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/svm_struct.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4985 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/svr_linear_trainer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7905 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/symmetric_matrix_cache.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4441 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/tester.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5427 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/tester.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14728 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/thread_pool.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4580 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/threads.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11089 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/timer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11267 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/tokenizer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8958 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/trust_region.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4085 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/tuple.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13301 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/type_safe_union.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3144 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/test/vectorstream.cpp
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/threads/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1196 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/async.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2878 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/async.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2274 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/async_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4212 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/auto_mutex_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6138 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/auto_mutex_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2886 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/auto_unlock_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3574 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/auto_unlock_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1111 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/create_new_thread_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      844 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/create_new_thread_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6573 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/multithreaded_object_extension.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3959 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/multithreaded_object_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6210 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/multithreaded_object_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    21499 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/parallel_for_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15671 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/parallel_for_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/posix.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5150 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/read_write_mutex_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5459 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/read_write_mutex_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2689 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/rmutex_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3733 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/rmutex_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2019 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/rsignaler_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4115 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/rsignaler_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4688 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/thread_function_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4484 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/thread_function_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9804 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/thread_pool_extension.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    44871 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/thread_pool_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    34586 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/thread_pool_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4119 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/thread_specific_data_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3123 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/thread_specific_data_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7920 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threaded_object_extension.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2652 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threaded_object_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6084 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threaded_object_extension_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      330 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threads_kernel.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1897 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threads_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3867 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threads_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1686 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threads_kernel_2.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4965 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threads_kernel_2.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11111 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threads_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10990 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threads_kernel_shared.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10293 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/threads_kernel_shared.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      198 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads/windows.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/timeout/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5165 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/timeout/timeout.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6402 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/timeout/timeout_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/timer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7279 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/timer/timer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9834 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/timer/timer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5823 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/timer/timer_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9943 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/timer/timer_heavy.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/tokenizer/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7944 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/tokenizer/tokenizer_kernel_1.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3977 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/tokenizer/tokenizer_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9424 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/tokenizer/tokenizer_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4802 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/tokenizer/tokenizer_kernel_c.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/travis/
+-rwxrwxr-x   0 davis     (1001) davis     (1001)      628 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/travis/build-and-test.sh
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/tuple/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13529 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/tuple/tuple.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9170 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/tuple/tuple_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/type_safe_union/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    26449 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/type_safe_union/type_safe_union_kernel.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10590 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/type_safe_union/type_safe_union_kernel_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/unicode/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5555 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/unicode/unicode.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20729 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/unicode/unicode.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     7046 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/unicode/unicode_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/vectorstream/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2482 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/vectorstream/unserialize.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2066 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/vectorstream/unserialize_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3770 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/vectorstream/vectorstream.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2580 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/vectorstream/vectorstream_abstract.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib/xml_parser/
+-rw-rw-r--   0 davis     (1001) davis     (1001)    48288 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/xml_parser/xml_parser_kernel_1.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8839 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/xml_parser/xml_parser_kernel_abstract.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     8273 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/xml_parser/xml_parser_kernel_interfaces.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    37698 2018-01-23 00:41:31.000000 dlib-19.9.0/dlib/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1337 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/LICENSE.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)    39033 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/algs.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      310 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/all_console.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)      298 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/all_gui.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)      308 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/any.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      257 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      328 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/array2d.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9110 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/assert.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      233 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/base64.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      259 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bayes_utils.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      825 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bigint.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1274 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/binary_search_tree.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      999 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bit_stream.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      315 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bound_function_pointer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      310 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bridge.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      217 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/bsp.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      267 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/byte_orderer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cassert
+-rw-rw-r--   0 davis     (1001) davis     (1001)      404 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/clustering.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       97 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmake
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2679 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cmd_line_parser.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4982 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/compress_stream.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2484 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/conditioning_class.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1152 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/config.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1288 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/config.h.in
+-rw-rw-r--   0 davis     (1001) davis     (1001)      990 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/config_reader.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6631 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/console_progress_indicator.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      252 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/control.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      907 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cpp_pretty_printer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      941 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cpp_tokenizer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      229 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/crc32.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/cstring
+-rw-rw-r--   0 davis     (1001) davis     (1001)      397 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/data_io.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      364 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dir_nav.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      821 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/directed_graph.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      329 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/disjoint_subsets.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      654 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dlib_basic_cpp_build_tutorial.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1033 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dlib_include_path_tutorial.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1244 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/dnn.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1603 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/enable_if.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      961 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3796 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_decoder_model.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      950 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5428 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/entropy_encoder_model.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    14334 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/error.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      297 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/filtering.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5975 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/float_details.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/fstream
+-rw-rw-r--   0 davis     (1001) davis     (1001)      395 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/geometry.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      416 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/global_optimization.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      741 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      397 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_cuts.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      342 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      328 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/graph_utils_threaded.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      314 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_core.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      330 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/gui_widgets.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      303 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1732 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_map.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1546 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_set.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1644 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/hash_table.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      543 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_io.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      583 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_keypoint.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1024 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/image_processing.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1108 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/image_transforms.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/iomanip
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/iosfwd
+-rw-rw-r--   0 davis     (1001) davis     (1001)      268 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/iosockstream.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/iostream
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5658 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/is_kind.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/istream
+-rw-rw-r--   0 davis     (1001) davis     (1001)      233 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/linker.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/locale
+-rw-rw-r--   0 davis     (1001) davis     (1001)      314 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/logger.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      295 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lsh.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      991 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lz77_buffer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      974 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/lzp_buffer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      417 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/manifold_regularization.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1488 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/map.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      682 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/matrix.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      159 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/md5.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      365 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/member_function_pointer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2069 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      729 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager_global.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2799 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/memory_manager_stateless.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2296 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/metaprogramming.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      366 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/misc_api.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      561 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/mlp.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      933 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/noncopyable.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1608 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/numeric_constants.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      363 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/numerical_integration.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      358 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/opencv.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      889 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/optimization.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/ostream
+-rw-rw-r--   0 davis     (1001) davis     (1001)      225 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/pipe.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    53588 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/pixel.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1482 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/platform.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      368 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/python.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      290 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/quantum_computing.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1801 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/queue.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      223 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/rand.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2348 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/ref.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      672 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/reference_counter.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      206 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/revision.h.in
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1955 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sequence.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    50722 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/serialize.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      300 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/server.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1671 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/set.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      249 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/set_utils.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      300 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/simd.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      776 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sliding_buffer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      876 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/smart_pointers.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      955 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/smart_pointers_thread_safe.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      363 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockets.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      324 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sockstreambuf.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    16126 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sort.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      261 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sparse_vector.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      247 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sqlite.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)       42 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/sstream
+-rw-rw-r--   0 davis     (1001) davis     (1001)      712 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/stack.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2411 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/stack_trace.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3848 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/stack_trace.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      811 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_map.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1031 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/static_set.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      559 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/statistics.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6971 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/std_allocator.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      269 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/stl_checked.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      237 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/string.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1848 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/svm.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1228 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/svm_threaded.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      593 2018-01-23 00:27:20.000000 dlib-19.9.0/dlib/sync_extension.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      891 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/threads.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2552 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/time_this.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      230 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/timeout.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      250 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/timer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5672 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/timing.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      632 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/tokenizer.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      234 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/tuple.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      291 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/type_safe_union.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2807 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/uintn.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      242 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/unicode.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4777 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/unordered_pair.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      296 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/vectorstream.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1327 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/windows_magic.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)      326 2018-01-23 00:27:19.000000 dlib-19.9.0/dlib/xml_parser.h
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib.egg-info/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4712 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib.egg-info/PKG-INFO
+-rw-rw-r--   0 davis     (1001) davis     (1001)    54358 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)        1 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)        1 2018-01-23 00:41:11.000000 dlib-19.9.0/dlib.egg-info/not-zip-safe
+-rw-rw-r--   0 davis     (1001) davis     (1001)        5 2018-01-23 00:41:51.000000 dlib-19.9.0/dlib.egg-info/top_level.txt
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/python_examples/
+-rw-rw-r--   0 davis     (1001) davis     (1001)      788 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/LICENSE_FOR_EXAMPLE_PROGRAMS.txt
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     3563 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/cnn_face_detector.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     2716 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/correlation_tracker.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     3065 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/face_alignment.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     5035 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/face_clustering.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     3311 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/face_detector.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     3336 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/face_jitter.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     4292 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/face_landmark_detection.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     5361 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/face_recognition.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     2043 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/find_candidate_object_locations.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     2054 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/global_optimization.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     2464 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/max_cost_assignment.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)       41 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/requirements.txt
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     8429 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/sequence_segmenter.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     2376 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/svm_binary_classifier.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     7084 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/svm_rank.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)    17237 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/svm_struct.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     7020 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/train_object_detector.py
+-rwxrwxr-x   0 davis     (1001) davis     (1001)     5961 2018-01-23 00:27:19.000000 dlib-19.9.0/python_examples/train_shape_predictor.py
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/tools/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/tools/python/
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/tools/python/src/
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9962 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/basic.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6123 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/cca.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5956 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/cnn_face_detector.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1586 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/conversion.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6908 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/correlation_tracker.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11954 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/decision_functions.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2622 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/dlib.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9876 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/face_recognition.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    12976 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/global_optimization.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4801 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/gui.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1198 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/image.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)      332 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/indexing.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5572 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/matrix.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5478 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/numpy_returns.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2330 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/numpy_returns_stub.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    20097 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/src/object_detection.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    11031 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/other.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5189 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/rectangles.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    32279 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/sequence_segmenter.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1949 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/serialize_object_detector.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    15097 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/shape_predictor.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10020 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/shape_predictor.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    13527 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/simple_object_detector.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)    10498 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/simple_object_detector_py.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9053 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/svm_c_trainer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     6038 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/svm_rank_trainer.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     5461 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/svm_struct.cpp
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1165 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/testing_results.h
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4706 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/src/vector.cpp
+drwxrwxr-x   0 davis     (1001) davis     (1001)        0 2018-01-23 00:41:51.000000 dlib-19.9.0/tools/python/test/
+-rw-rw-r--   0 davis     (1001) davis     (1001)       12 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/test/.gitignore
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2180 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/test/test_array.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2579 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/test/test_matrix.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)     1003 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/test/test_point.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2014 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/test/test_range.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)      680 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/test/test_rgb_pixel.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2492 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/test/test_sparse_vector.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3577 2018-01-23 00:27:20.000000 dlib-19.9.0/tools/python/test/test_vector.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)     3700 2018-01-23 00:27:19.000000 dlib-19.9.0/tools/python/CMakeLists.txt
+-rw-rw-r--   0 davis     (1001) davis     (1001)      256 2018-01-23 00:27:19.000000 dlib-19.9.0/MANIFEST.in
+-rw-rw-r--   0 davis     (1001) davis     (1001)     2871 2018-01-23 00:27:19.000000 dlib-19.9.0/README.md
+-rw-rw-r--   0 davis     (1001) davis     (1001)     9133 2018-01-23 00:27:19.000000 dlib-19.9.0/setup.py
+-rw-rw-r--   0 davis     (1001) davis     (1001)     4712 2018-01-23 00:41:51.000000 dlib-19.9.0/PKG-INFO
+-rw-rw-r--   0 davis     (1001) davis     (1001)       38 2018-01-23 00:41:51.000000 dlib-19.9.0/setup.cfg
```

### Comparing `dlib-19.8.2/dlib/all/source.cpp` & `dlib-19.9.0/dlib/all/source.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any.h` & `dlib-19.9.0/dlib/any/any.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any_abstract.h` & `dlib-19.9.0/dlib/any/any_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any_decision_function.h` & `dlib-19.9.0/dlib/any/any_decision_function.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any_decision_function_abstract.h` & `dlib-19.9.0/dlib/any/any_decision_function_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any_function.h` & `dlib-19.9.0/dlib/any/any_function.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any_function_abstract.h` & `dlib-19.9.0/dlib/any/any_function_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any_function_impl.h` & `dlib-19.9.0/dlib/any/any_function_impl.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any_function_impl2.h` & `dlib-19.9.0/dlib/any/any_function_impl2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any_trainer.h` & `dlib-19.9.0/dlib/any/any_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/any/any_trainer_abstract.h` & `dlib-19.9.0/dlib/any/any_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/appveyor/python.yml` & `dlib-19.9.0/dlib/appveyor/python.yml`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/array/array_kernel.h` & `dlib-19.9.0/dlib/array/array_kernel.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/array/array_kernel_abstract.h` & `dlib-19.9.0/dlib/array/array_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/array/array_tools.h` & `dlib-19.9.0/dlib/array/array_tools.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/array/array_tools_abstract.h` & `dlib-19.9.0/dlib/array/array_tools_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/array2d/array2d_generic_image.h` & `dlib-19.9.0/dlib/array2d/array2d_generic_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/array2d/array2d_kernel.h` & `dlib-19.9.0/dlib/array2d/array2d_kernel.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/array2d/array2d_kernel_abstract.h` & `dlib-19.9.0/dlib/array2d/array2d_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/array2d/serialize_pixel_overloads.h` & `dlib-19.9.0/dlib/array2d/serialize_pixel_overloads.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/base64/base64_kernel_1.cpp` & `dlib-19.9.0/dlib/base64/base64_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/base64/base64_kernel_1.h` & `dlib-19.9.0/dlib/base64/base64_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/base64/base64_kernel_abstract.h` & `dlib-19.9.0/dlib/base64/base64_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bayes_utils/bayes_utils.h` & `dlib-19.9.0/dlib/bayes_utils/bayes_utils.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bayes_utils/bayes_utils_abstract.h` & `dlib-19.9.0/dlib/bayes_utils/bayes_utils_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bigint/bigint_kernel_1.cpp` & `dlib-19.9.0/dlib/bigint/bigint_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bigint/bigint_kernel_1.h` & `dlib-19.9.0/dlib/bigint/bigint_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bigint/bigint_kernel_2.cpp` & `dlib-19.9.0/dlib/bigint/bigint_kernel_2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bigint/bigint_kernel_2.h` & `dlib-19.9.0/dlib/bigint/bigint_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bigint/bigint_kernel_abstract.h` & `dlib-19.9.0/dlib/bigint/bigint_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bigint/bigint_kernel_c.h` & `dlib-19.9.0/dlib/bigint/bigint_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/binary_search_tree/binary_search_tree_kernel_1.h` & `dlib-19.9.0/dlib/binary_search_tree/binary_search_tree_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/binary_search_tree/binary_search_tree_kernel_2.h` & `dlib-19.9.0/dlib/binary_search_tree/binary_search_tree_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/binary_search_tree/binary_search_tree_kernel_abstract.h` & `dlib-19.9.0/dlib/binary_search_tree/binary_search_tree_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/binary_search_tree/binary_search_tree_kernel_c.h` & `dlib-19.9.0/dlib/binary_search_tree/binary_search_tree_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bit_stream/bit_stream_kernel_1.cpp` & `dlib-19.9.0/dlib/bit_stream/bit_stream_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bit_stream/bit_stream_kernel_1.h` & `dlib-19.9.0/dlib/bit_stream/bit_stream_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bit_stream/bit_stream_kernel_abstract.h` & `dlib-19.9.0/dlib/bit_stream/bit_stream_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bit_stream/bit_stream_kernel_c.h` & `dlib-19.9.0/dlib/bit_stream/bit_stream_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bit_stream/bit_stream_multi_1.h` & `dlib-19.9.0/dlib/bit_stream/bit_stream_multi_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bit_stream/bit_stream_multi_abstract.h` & `dlib-19.9.0/dlib/bit_stream/bit_stream_multi_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bit_stream/bit_stream_multi_c.h` & `dlib-19.9.0/dlib/bit_stream/bit_stream_multi_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bound_function_pointer/bound_function_pointer_kernel_1.h` & `dlib-19.9.0/dlib/bound_function_pointer/bound_function_pointer_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bound_function_pointer/bound_function_pointer_kernel_abstract.h` & `dlib-19.9.0/dlib/bound_function_pointer/bound_function_pointer_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bridge/bridge.h` & `dlib-19.9.0/dlib/bridge/bridge.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bridge/bridge_abstract.h` & `dlib-19.9.0/dlib/bridge/bridge_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bsp/bsp.cpp` & `dlib-19.9.0/dlib/bsp/bsp.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bsp/bsp.h` & `dlib-19.9.0/dlib/bsp/bsp.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bsp/bsp_abstract.h` & `dlib-19.9.0/dlib/bsp/bsp_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/byte_orderer/byte_orderer_kernel_1.h` & `dlib-19.9.0/dlib/byte_orderer/byte_orderer_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/byte_orderer/byte_orderer_kernel_abstract.h` & `dlib-19.9.0/dlib/byte_orderer/byte_orderer_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/clustering/bottom_up_cluster.h` & `dlib-19.9.0/dlib/clustering/bottom_up_cluster.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/clustering/bottom_up_cluster_abstract.h` & `dlib-19.9.0/dlib/clustering/bottom_up_cluster_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/clustering/chinese_whispers.h` & `dlib-19.9.0/dlib/clustering/chinese_whispers.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/clustering/chinese_whispers_abstract.h` & `dlib-19.9.0/dlib/clustering/chinese_whispers_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/clustering/modularity_clustering.h` & `dlib-19.9.0/dlib/clustering/modularity_clustering.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/clustering/modularity_clustering_abstract.h` & `dlib-19.9.0/dlib/clustering/modularity_clustering_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/clustering/spectral_cluster.h` & `dlib-19.9.0/dlib/clustering/spectral_cluster.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/clustering/spectral_cluster_abstract.h` & `dlib-19.9.0/dlib/clustering/spectral_cluster_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/test_for_cpp11/cpp11_test.cpp` & `dlib-19.9.0/dlib/cmake_utils/test_for_cpp11/cpp11_test.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/test_for_cuda/CMakeLists.txt` & `dlib-19.9.0/dlib/cmake_utils/test_for_cuda/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/test_for_cuda/cuda_test.cu` & `dlib-19.9.0/dlib/cmake_utils/test_for_cuda/cuda_test.cu`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/test_for_cudnn/CMakeLists.txt` & `dlib-19.9.0/dlib/cmake_utils/test_for_cudnn/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/test_for_cudnn/find_cudnn.txt` & `dlib-19.9.0/dlib/cmake_utils/test_for_cudnn/find_cudnn.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/add_global_compiler_switch.cmake` & `dlib-19.9.0/dlib/cmake_utils/add_global_compiler_switch.cmake`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/check_if_neon_available.cmake` & `dlib-19.9.0/dlib/cmake_utils/check_if_neon_available.cmake`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/cmake_find_blas.txt` & `dlib-19.9.0/dlib/cmake_utils/cmake_find_blas.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/dlibConfig.cmake.in` & `dlib-19.9.0/dlib/cmake_utils/dlibConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/set_compiler_specific_options.cmake` & `dlib-19.9.0/dlib/cmake_utils/set_compiler_specific_options.cmake`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/tell_visual_studio_to_use_static_runtime.cmake` & `dlib-19.9.0/dlib/cmake_utils/tell_visual_studio_to_use_static_runtime.cmake`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmake_utils/use_cpp_11.cmake` & `dlib-19.9.0/dlib/cmake_utils/use_cpp_11.cmake`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_check_1.h` & `dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_check_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_check_c.h` & `dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_check_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_kernel_1.h` & `dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_kernel_abstract.h` & `dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_kernel_c.h` & `dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmd_line_parser/cmd_line_parser_print_1.h` & `dlib-19.9.0/dlib/cmd_line_parser/cmd_line_parser_print_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmd_line_parser/get_option.h` & `dlib-19.9.0/dlib/cmd_line_parser/get_option.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmd_line_parser/get_option_abstract.h` & `dlib-19.9.0/dlib/cmd_line_parser/get_option_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/compress_stream/compress_stream_kernel_1.h` & `dlib-19.9.0/dlib/compress_stream/compress_stream_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/compress_stream/compress_stream_kernel_2.h` & `dlib-19.9.0/dlib/compress_stream/compress_stream_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/compress_stream/compress_stream_kernel_3.h` & `dlib-19.9.0/dlib/compress_stream/compress_stream_kernel_3.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/compress_stream/compress_stream_kernel_abstract.h` & `dlib-19.9.0/dlib/compress_stream/compress_stream_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_1.h` & `dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_2.h` & `dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_3.h` & `dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_3.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_4.h` & `dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_4.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_abstract.h` & `dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/conditioning_class/conditioning_class_kernel_c.h` & `dlib-19.9.0/dlib/conditioning_class/conditioning_class_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/config_reader/config_reader_kernel_1.h` & `dlib-19.9.0/dlib/config_reader/config_reader_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/config_reader/config_reader_kernel_abstract.h` & `dlib-19.9.0/dlib/config_reader/config_reader_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/config_reader/config_reader_thread_safe_1.h` & `dlib-19.9.0/dlib/config_reader/config_reader_thread_safe_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/config_reader/config_reader_thread_safe_abstract.h` & `dlib-19.9.0/dlib/config_reader/config_reader_thread_safe_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/control/approximate_linear_models.h` & `dlib-19.9.0/dlib/control/approximate_linear_models.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/control/approximate_linear_models_abstract.h` & `dlib-19.9.0/dlib/control/approximate_linear_models_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/control/lspi.h` & `dlib-19.9.0/dlib/control/lspi.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/control/lspi_abstract.h` & `dlib-19.9.0/dlib/control/lspi_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/control/mpc.h` & `dlib-19.9.0/dlib/control/mpc.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/control/mpc_abstract.h` & `dlib-19.9.0/dlib/control/mpc_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_1.h` & `dlib-19.9.0/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_2.h` & `dlib-19.9.0/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_abstract.h` & `dlib-19.9.0/dlib/cpp_pretty_printer/cpp_pretty_printer_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cpp_tokenizer/cpp_tokenizer_kernel_1.h` & `dlib-19.9.0/dlib/cpp_tokenizer/cpp_tokenizer_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cpp_tokenizer/cpp_tokenizer_kernel_abstract.h` & `dlib-19.9.0/dlib/cpp_tokenizer/cpp_tokenizer_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cpp_tokenizer/cpp_tokenizer_kernel_c.h` & `dlib-19.9.0/dlib/cpp_tokenizer/cpp_tokenizer_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/crc32/crc32_kernel_1.h` & `dlib-19.9.0/dlib/crc32/crc32_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/crc32/crc32_kernel_abstract.h` & `dlib-19.9.0/dlib/crc32/crc32_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/data_io/image_dataset_metadata.cpp` & `dlib-19.9.0/dlib/data_io/image_dataset_metadata.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/data_io/image_dataset_metadata.h` & `dlib-19.9.0/dlib/data_io/image_dataset_metadata.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/data_io/libsvm_io.h` & `dlib-19.9.0/dlib/data_io/libsvm_io.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/data_io/libsvm_io_abstract.h` & `dlib-19.9.0/dlib/data_io/libsvm_io_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/data_io/load_image_dataset.h` & `dlib-19.9.0/dlib/data_io/load_image_dataset.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/data_io/load_image_dataset_abstract.h` & `dlib-19.9.0/dlib/data_io/load_image_dataset_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/data_io/mnist.cpp` & `dlib-19.9.0/dlib/data_io/mnist.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/data_io/mnist.h` & `dlib-19.9.0/dlib/data_io/mnist.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/data_io/mnist_abstract.h` & `dlib-19.9.0/dlib/data_io/mnist_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dir_nav/dir_nav_extensions.cpp` & `dlib-19.9.0/dlib/dir_nav/dir_nav_extensions.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dir_nav/dir_nav_extensions.h` & `dlib-19.9.0/dlib/dir_nav/dir_nav_extensions.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dir_nav/dir_nav_extensions_abstract.h` & `dlib-19.9.0/dlib/dir_nav/dir_nav_extensions_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_1.cpp` & `dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_1.h` & `dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_2.cpp` & `dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_2.h` & `dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dir_nav/dir_nav_kernel_abstract.h` & `dlib-19.9.0/dlib/dir_nav/dir_nav_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/directed_graph/directed_graph_kernel_1.h` & `dlib-19.9.0/dlib/directed_graph/directed_graph_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/directed_graph/directed_graph_kernel_abstract.h` & `dlib-19.9.0/dlib/directed_graph/directed_graph_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/disjoint_subsets/disjoint_subsets.h` & `dlib-19.9.0/dlib/disjoint_subsets/disjoint_subsets.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/disjoint_subsets/disjoint_subsets_abstract.h` & `dlib-19.9.0/dlib/disjoint_subsets/disjoint_subsets_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/disjoint_subsets/disjoint_subsets_sized.h` & `dlib-19.9.0/dlib/disjoint_subsets/disjoint_subsets_sized.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/disjoint_subsets/disjoint_subsets_sized_abstract.h` & `dlib-19.9.0/dlib/disjoint_subsets/disjoint_subsets_sized_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/core.h` & `dlib-19.9.0/dlib/dnn/core.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/core_abstract.h` & `dlib-19.9.0/dlib/dnn/core_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cpu_dlib.cpp` & `dlib-19.9.0/dlib/dnn/cpu_dlib.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cpu_dlib.h` & `dlib-19.9.0/dlib/dnn/cpu_dlib.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cublas_dlibapi.cpp` & `dlib-19.9.0/dlib/dnn/cublas_dlibapi.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cublas_dlibapi.h` & `dlib-19.9.0/dlib/dnn/cublas_dlibapi.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cuda_data_ptr.cpp` & `dlib-19.9.0/dlib/dnn/cuda_data_ptr.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cuda_data_ptr.h` & `dlib-19.9.0/dlib/dnn/cuda_data_ptr.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cuda_dlib.cu` & `dlib-19.9.0/dlib/dnn/cuda_dlib.cu`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cuda_dlib.h` & `dlib-19.9.0/dlib/dnn/cuda_dlib.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cuda_errors.h` & `dlib-19.9.0/dlib/dnn/cuda_errors.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cuda_utils.h` & `dlib-19.9.0/dlib/dnn/cuda_utils.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cudnn_dlibapi.cpp` & `dlib-19.9.0/dlib/dnn/cudnn_dlibapi.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cudnn_dlibapi.h` & `dlib-19.9.0/dlib/dnn/cudnn_dlibapi.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/curand_dlibapi.cpp` & `dlib-19.9.0/dlib/dnn/curand_dlibapi.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/curand_dlibapi.h` & `dlib-19.9.0/dlib/dnn/curand_dlibapi.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cusolver_dlibapi.cu` & `dlib-19.9.0/dlib/dnn/cusolver_dlibapi.cu`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/cusolver_dlibapi.h` & `dlib-19.9.0/dlib/dnn/cusolver_dlibapi.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/gpu_data.cpp` & `dlib-19.9.0/dlib/dnn/gpu_data.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/gpu_data.h` & `dlib-19.9.0/dlib/dnn/gpu_data.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/gpu_data_abstract.h` & `dlib-19.9.0/dlib/dnn/gpu_data_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/input.h` & `dlib-19.9.0/dlib/dnn/input.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/input_abstract.h` & `dlib-19.9.0/dlib/dnn/input_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/layers.h` & `dlib-19.9.0/dlib/dnn/layers.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/layers_abstract.h` & `dlib-19.9.0/dlib/dnn/layers_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/loss.h` & `dlib-19.9.0/dlib/dnn/loss.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/loss_abstract.h` & `dlib-19.9.0/dlib/dnn/loss_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/solvers.h` & `dlib-19.9.0/dlib/dnn/solvers.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/solvers_abstract.h` & `dlib-19.9.0/dlib/dnn/solvers_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/tensor.h` & `dlib-19.9.0/dlib/dnn/tensor.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/tensor_abstract.h` & `dlib-19.9.0/dlib/dnn/tensor_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/tensor_tools.cpp` & `dlib-19.9.0/dlib/dnn/tensor_tools.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/tensor_tools.h` & `dlib-19.9.0/dlib/dnn/tensor_tools.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/trainer.h` & `dlib-19.9.0/dlib/dnn/trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/trainer_abstract.h` & `dlib-19.9.0/dlib/dnn/trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/utilities.h` & `dlib-19.9.0/dlib/dnn/utilities.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/utilities_abstract.h` & `dlib-19.9.0/dlib/dnn/utilities_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn/validation.h` & `dlib-19.9.0/dlib/dnn/validation.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_1.cpp` & `dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_1.h` & `dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_2.cpp` & `dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_2.h` & `dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_abstract.h` & `dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder/entropy_decoder_kernel_c.h` & `dlib-19.9.0/dlib/entropy_decoder/entropy_decoder_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_1.h` & `dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_2.h` & `dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_3.h` & `dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_3.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_4.h` & `dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_4.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_5.h` & `dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_5.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_6.h` & `dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_6.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder_model/entropy_decoder_model_kernel_abstract.h` & `dlib-19.9.0/dlib/entropy_decoder_model/entropy_decoder_model_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_1.cpp` & `dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_1.h` & `dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_2.cpp` & `dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_2.h` & `dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_abstract.h` & `dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder/entropy_encoder_kernel_c.h` & `dlib-19.9.0/dlib/entropy_encoder/entropy_encoder_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_1.h` & `dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_2.h` & `dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_3.h` & `dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_3.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_4.h` & `dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_4.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_5.h` & `dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_5.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_6.h` & `dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_6.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_abstract.h` & `dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder_model/entropy_encoder_model_kernel_c.h` & `dlib-19.9.0/dlib/entropy_encoder_model/entropy_encoder_model_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/CMakeLists.txt` & `dlib-19.9.0/dlib/external/cblas/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas.h` & `dlib-19.9.0/dlib/external/cblas/cblas.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cdotc_sub.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cdotc_sub.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cdotu_sub.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cdotu_sub.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cgbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cgbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cgemm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cgemm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cgemv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cgemv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cgerc.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cgerc.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cgeru.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cgeru.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_chbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_chbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_chemm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_chemm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_chemv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_chemv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cher.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cher.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cher2.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cher2.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cher2k.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cher2k.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_cherk.c` & `dlib-19.9.0/dlib/external/cblas/cblas_cherk.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_chpmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_chpmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_chpr.c` & `dlib-19.9.0/dlib/external/cblas/cblas_chpr.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_chpr2.c` & `dlib-19.9.0/dlib/external/cblas/cblas_chpr2.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_csymm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_csymm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_csyr2k.c` & `dlib-19.9.0/dlib/external/cblas/cblas_csyr2k.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_csyrk.c` & `dlib-19.9.0/dlib/external/cblas/cblas_csyrk.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ctbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ctbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ctbsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ctbsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ctpmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ctpmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ctpsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ctpsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ctrmm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ctrmm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ctrmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ctrmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ctrsm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ctrsm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ctrsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ctrsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ddot.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ddot.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dgbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dgbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dgemm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dgemm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dgemv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dgemv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dger.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dger.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dsbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dsbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dsdot.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dsdot.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dspmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dspmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dspr.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dspr.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dspr2.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dspr2.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dsymm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dsymm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dsymv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dsymv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dsyr.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dsyr.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dsyr2.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dsyr2.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dsyr2k.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dsyr2k.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dsyrk.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dsyrk.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dtbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dtbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dtbsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dtbsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dtpmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dtpmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dtpsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dtpsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dtrmm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dtrmm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dtrmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dtrmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dtrsm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dtrsm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_dtrsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_dtrsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_f77.h` & `dlib-19.9.0/dlib/external/cblas/cblas_f77.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_saxpy.c` & `dlib-19.9.0/dlib/external/cblas/cblas_saxpy.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_sdot.c` & `dlib-19.9.0/dlib/external/cblas/cblas_sdot.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_sdsdot.c` & `dlib-19.9.0/dlib/external/cblas/cblas_sdsdot.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_sgbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_sgbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_sgemm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_sgemm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_sgemv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_sgemv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_sger.c` & `dlib-19.9.0/dlib/external/cblas/cblas_sger.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ssbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ssbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_sspmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_sspmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_sspr.c` & `dlib-19.9.0/dlib/external/cblas/cblas_sspr.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_sspr2.c` & `dlib-19.9.0/dlib/external/cblas/cblas_sspr2.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ssymm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ssymm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ssymv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ssymv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ssyr.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ssyr.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ssyr2.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ssyr2.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ssyr2k.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ssyr2k.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ssyrk.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ssyrk.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_stbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_stbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_stbsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_stbsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_stpmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_stpmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_stpsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_stpsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_strmm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_strmm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_strmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_strmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_strsm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_strsm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_strsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_strsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_xerbla.c` & `dlib-19.9.0/dlib/external/cblas/cblas_xerbla.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zdotc_sub.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zdotc_sub.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zdotu_sub.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zdotu_sub.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zgbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zgbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zgemm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zgemm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zgemv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zgemv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zgerc.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zgerc.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zgeru.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zgeru.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zhbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zhbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zhemm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zhemm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zhemv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zhemv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zher.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zher.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zher2.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zher2.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zher2k.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zher2k.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zherk.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zherk.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zhpmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zhpmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zhpr.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zhpr.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zhpr2.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zhpr2.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zsymm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zsymm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zsyr2k.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zsyr2k.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_zsyrk.c` & `dlib-19.9.0/dlib/external/cblas/cblas_zsyrk.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ztbmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ztbmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ztbsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ztbsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ztpmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ztpmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ztpsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ztpsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ztrmm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ztrmm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ztrmv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ztrmv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ztrsm.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ztrsm.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/cblas/cblas_ztrsv.c` & `dlib-19.9.0/dlib/external/cblas/cblas_ztrsv.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/README` & `dlib-19.9.0/dlib/external/libjpeg/README`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcapimin.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcapimin.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcapistd.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcapistd.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jccoefct.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jccoefct.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jccolor.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jccolor.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcdctmgr.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcdctmgr.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jchuff.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jchuff.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jchuff.h` & `dlib-19.9.0/dlib/external/libjpeg/jchuff.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcinit.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcinit.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcmainct.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcmainct.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcmarker.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcmarker.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcmaster.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcmaster.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcomapi.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcomapi.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jconfig.h` & `dlib-19.9.0/dlib/external/libjpeg/jconfig.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcparam.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcparam.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcphuff.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcphuff.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcprepct.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcprepct.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jcsample.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jcsample.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdapimin.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdapimin.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdapistd.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdapistd.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdatadst.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdatadst.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdatasrc.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdatasrc.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdcoefct.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdcoefct.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdcolor.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdcolor.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdct.h` & `dlib-19.9.0/dlib/external/libjpeg/jdct.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jddctmgr.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jddctmgr.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdhuff.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdhuff.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdhuff.h` & `dlib-19.9.0/dlib/external/libjpeg/jdhuff.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdinput.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdinput.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdmainct.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdmainct.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdmarker.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdmarker.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdmaster.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdmaster.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdmerge.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdmerge.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdphuff.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdphuff.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdpostct.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdpostct.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jdsample.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jdsample.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jerror.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jerror.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jerror.h` & `dlib-19.9.0/dlib/external/libjpeg/jerror.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jfdctflt.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jfdctflt.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jfdctfst.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jfdctfst.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jfdctint.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jfdctint.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jidctflt.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jidctflt.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jidctfst.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jidctfst.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jidctint.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jidctint.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jidctred.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jidctred.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jinclude.h` & `dlib-19.9.0/dlib/external/libjpeg/jinclude.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jmemmgr.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jmemmgr.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jmemnobs.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jmemnobs.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jmemsys.h` & `dlib-19.9.0/dlib/external/libjpeg/jmemsys.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jmorecfg.h` & `dlib-19.9.0/dlib/external/libjpeg/jmorecfg.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jpegint.h` & `dlib-19.9.0/dlib/external/libjpeg/jpegint.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jpeglib.h` & `dlib-19.9.0/dlib/external/libjpeg/jpeglib.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jquant1.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jquant1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jquant2.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jquant2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libjpeg/jutils.cpp` & `dlib-19.9.0/dlib/external/libjpeg/jutils.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/arm/arm_init.c` & `dlib-19.9.0/dlib/external/libpng/arm/arm_init.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/arm/filter_neon.S` & `dlib-19.9.0/dlib/external/libpng/arm/filter_neon.S`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/arm/filter_neon_intrinsics.c` & `dlib-19.9.0/dlib/external/libpng/arm/filter_neon_intrinsics.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/LICENSE` & `dlib-19.9.0/dlib/external/libpng/LICENSE`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/README` & `dlib-19.9.0/dlib/external/libpng/README`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/png.c` & `dlib-19.9.0/dlib/external/libpng/png.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/png.h` & `dlib-19.9.0/dlib/external/libpng/png.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngconf.h` & `dlib-19.9.0/dlib/external/libpng/pngconf.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngdebug.h` & `dlib-19.9.0/dlib/external/libpng/pngdebug.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngerror.c` & `dlib-19.9.0/dlib/external/libpng/pngerror.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngget.c` & `dlib-19.9.0/dlib/external/libpng/pngget.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pnginfo.h` & `dlib-19.9.0/dlib/external/libpng/pnginfo.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pnglibconf.h` & `dlib-19.9.0/dlib/external/libpng/pnglibconf.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngmem.c` & `dlib-19.9.0/dlib/external/libpng/pngmem.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngpread.c` & `dlib-19.9.0/dlib/external/libpng/pngpread.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngpriv.h` & `dlib-19.9.0/dlib/external/libpng/pngpriv.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngread.c` & `dlib-19.9.0/dlib/external/libpng/pngread.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngrio.c` & `dlib-19.9.0/dlib/external/libpng/pngrio.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngrtran.c` & `dlib-19.9.0/dlib/external/libpng/pngrtran.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngrutil.c` & `dlib-19.9.0/dlib/external/libpng/pngrutil.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngset.c` & `dlib-19.9.0/dlib/external/libpng/pngset.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngstruct.h` & `dlib-19.9.0/dlib/external/libpng/pngstruct.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngtrans.c` & `dlib-19.9.0/dlib/external/libpng/pngtrans.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngwio.c` & `dlib-19.9.0/dlib/external/libpng/pngwio.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngwrite.c` & `dlib-19.9.0/dlib/external/libpng/pngwrite.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngwtran.c` & `dlib-19.9.0/dlib/external/libpng/pngwtran.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/libpng/pngwutil.c` & `dlib-19.9.0/dlib/external/libpng/pngwutil.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/class.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/common.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/descr.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/init.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/internals.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/detail/typeid.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/attr.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/buffer_info.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/cast.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/chrono.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/complex.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/eigen.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/embed.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/eval.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/functional.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/iostream.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/numpy.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/operators.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/options.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/pybind11.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/pytypes.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/stl.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/include/pybind11/stl_bind.h` & `dlib-19.9.0/dlib/external/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/tools/FindCatch.cmake` & `dlib-19.9.0/dlib/external/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/tools/FindEigen3.cmake` & `dlib-19.9.0/dlib/external/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/tools/FindPythonLibsNew.cmake` & `dlib-19.9.0/dlib/external/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/tools/check-style.sh` & `dlib-19.9.0/dlib/external/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/tools/libsize.py` & `dlib-19.9.0/dlib/external/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/tools/mkdoc.py` & `dlib-19.9.0/dlib/external/pybind11/tools/mkdoc.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/tools/pybind11Config.cmake.in` & `dlib-19.9.0/dlib/external/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/tools/pybind11Tools.cmake` & `dlib-19.9.0/dlib/external/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/CMakeLists.txt` & `dlib-19.9.0/dlib/external/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/CONTRIBUTING.md` & `dlib-19.9.0/dlib/external/pybind11/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/LICENSE` & `dlib-19.9.0/dlib/external/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/pybind11/README.md` & `dlib-19.9.0/dlib/external/pybind11/README.md`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/README` & `dlib-19.9.0/dlib/external/zlib/README`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/adler32.c` & `dlib-19.9.0/dlib/external/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/compress.c` & `dlib-19.9.0/dlib/external/zlib/compress.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/crc32.c` & `dlib-19.9.0/dlib/external/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/crc32.h` & `dlib-19.9.0/dlib/external/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/deflate.c` & `dlib-19.9.0/dlib/external/zlib/deflate.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/deflate.h` & `dlib-19.9.0/dlib/external/zlib/deflate.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/gzclose.c` & `dlib-19.9.0/dlib/external/zlib/gzclose.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/gzguts.h` & `dlib-19.9.0/dlib/external/zlib/gzguts.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/gzlib.c` & `dlib-19.9.0/dlib/external/zlib/gzlib.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/gzread.c` & `dlib-19.9.0/dlib/external/zlib/gzread.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/gzwrite.c` & `dlib-19.9.0/dlib/external/zlib/gzwrite.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/infback.c` & `dlib-19.9.0/dlib/external/zlib/infback.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/inffast.c` & `dlib-19.9.0/dlib/external/zlib/inffast.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/inffixed.h` & `dlib-19.9.0/dlib/external/zlib/inffixed.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/inflate.c` & `dlib-19.9.0/dlib/external/zlib/inflate.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/inflate.h` & `dlib-19.9.0/dlib/external/zlib/inflate.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/inftrees.c` & `dlib-19.9.0/dlib/external/zlib/inftrees.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/inftrees.h` & `dlib-19.9.0/dlib/external/zlib/inftrees.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/trees.c` & `dlib-19.9.0/dlib/external/zlib/trees.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/trees.h` & `dlib-19.9.0/dlib/external/zlib/trees.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/uncompr.c` & `dlib-19.9.0/dlib/external/zlib/uncompr.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/zconf.h` & `dlib-19.9.0/dlib/external/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/zlib.h` & `dlib-19.9.0/dlib/external/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/zutil.c` & `dlib-19.9.0/dlib/external/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/external/zlib/zutil.h` & `dlib-19.9.0/dlib/external/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/filtering/kalman_filter.h` & `dlib-19.9.0/dlib/filtering/kalman_filter.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/filtering/kalman_filter_abstract.h` & `dlib-19.9.0/dlib/filtering/kalman_filter_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/filtering/rls_filter.h` & `dlib-19.9.0/dlib/filtering/rls_filter.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/filtering/rls_filter_abstract.h` & `dlib-19.9.0/dlib/filtering/rls_filter_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/general_hash/count_bits.h` & `dlib-19.9.0/dlib/general_hash/count_bits.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/general_hash/count_bits_abstract.h` & `dlib-19.9.0/dlib/general_hash/count_bits_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/general_hash/general_hash.h` & `dlib-19.9.0/dlib/general_hash/general_hash.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/general_hash/hash.h` & `dlib-19.9.0/dlib/general_hash/hash.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/general_hash/hash_abstract.h` & `dlib-19.9.0/dlib/general_hash/hash_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/general_hash/murmur_hash3.h` & `dlib-19.9.0/dlib/general_hash/murmur_hash3.h`

 * *Files 10% similar despite different names*

```diff
@@ -210,15 +210,17 @@
         const uint8 * tail = (const uint8*)(data + nblocks*4);
 
         uint32 k1 = 0;
 
         switch(len & 3)
         {
             case 3: k1 ^= tail[2] << 16;
+                    // fall through
             case 2: k1 ^= tail[1] << 8;
+                    // fall through
             case 1: k1 ^= tail[0];
                     k1 *= c1; k1 = DLIB_ROTL32(k1,15); k1 *= c2; h1 ^= k1;
         };
 
         //----------
         // finalization
 
@@ -380,32 +382,32 @@
         const uint8 * tail = (const uint8*)(data + nblocks*16);
 
         uint64 k1 = 0;
         uint64 k2 = 0;
 
         switch(len & 15)
         {
-            case 15: k2 ^= uint64(tail[14]) << 48;
-            case 14: k2 ^= uint64(tail[13]) << 40;
-            case 13: k2 ^= uint64(tail[12]) << 32;
-            case 12: k2 ^= uint64(tail[11]) << 24;
-            case 11: k2 ^= uint64(tail[10]) << 16;
-            case 10: k2 ^= uint64(tail[ 9]) << 8;
+            case 15: k2 ^= uint64(tail[14]) << 48; // fall through
+            case 14: k2 ^= uint64(tail[13]) << 40; // fall through
+            case 13: k2 ^= uint64(tail[12]) << 32; // fall through
+            case 12: k2 ^= uint64(tail[11]) << 24; // fall through
+            case 11: k2 ^= uint64(tail[10]) << 16; // fall through
+            case 10: k2 ^= uint64(tail[ 9]) << 8; // fall through
             case  9: k2 ^= uint64(tail[ 8]) << 0;
-                     k2 *= c2; k2  = DLIB_ROTL64(k2,33); k2 *= c1; h2 ^= k2;
+                     k2 *= c2; k2  = DLIB_ROTL64(k2,33); k2 *= c1; h2 ^= k2; // fall through
 
-            case  8: k1 ^= uint64(tail[ 7]) << 56;
-            case  7: k1 ^= uint64(tail[ 6]) << 48;
-            case  6: k1 ^= uint64(tail[ 5]) << 40;
-            case  5: k1 ^= uint64(tail[ 4]) << 32;
-            case  4: k1 ^= uint64(tail[ 3]) << 24;
-            case  3: k1 ^= uint64(tail[ 2]) << 16;
-            case  2: k1 ^= uint64(tail[ 1]) << 8;
+            case  8: k1 ^= uint64(tail[ 7]) << 56; // fall through
+            case  7: k1 ^= uint64(tail[ 6]) << 48; // fall through
+            case  6: k1 ^= uint64(tail[ 5]) << 40; // fall through
+            case  5: k1 ^= uint64(tail[ 4]) << 32; // fall through
+            case  4: k1 ^= uint64(tail[ 3]) << 24; // fall through
+            case  3: k1 ^= uint64(tail[ 2]) << 16; // fall through
+            case  2: k1 ^= uint64(tail[ 1]) << 8; // fall through
             case  1: k1 ^= uint64(tail[ 0]) << 0;
-                     k1 *= c1; k1  = DLIB_ROTL64(k1,31); k1 *= c2; h1 ^= k1;
+                     k1 *= c1; k1  = DLIB_ROTL64(k1,31); k1 *= c2; h1 ^= k1; // fall through
         };
 
         //----------
         // finalization
 
         h1 ^= len; h2 ^= len;
```

### Comparing `dlib-19.8.2/dlib/general_hash/murmur_hash3_abstract.h` & `dlib-19.9.0/dlib/general_hash/murmur_hash3_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/general_hash/random_hashing.h` & `dlib-19.9.0/dlib/general_hash/random_hashing.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/general_hash/random_hashing_abstract.h` & `dlib-19.9.0/dlib/general_hash/random_hashing_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/border_enumerator.h` & `dlib-19.9.0/dlib/geometry/border_enumerator.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/border_enumerator_abstract.h` & `dlib-19.9.0/dlib/geometry/border_enumerator_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/drectangle.h` & `dlib-19.9.0/dlib/geometry/drectangle.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/drectangle_abstract.h` & `dlib-19.9.0/dlib/geometry/drectangle_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/point_transforms.h` & `dlib-19.9.0/dlib/geometry/point_transforms.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/point_transforms_abstract.h` & `dlib-19.9.0/dlib/geometry/point_transforms_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/rectangle.h` & `dlib-19.9.0/dlib/geometry/rectangle.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/rectangle_abstract.h` & `dlib-19.9.0/dlib/geometry/rectangle_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/vector.h` & `dlib-19.9.0/dlib/geometry/vector.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/geometry/vector_abstract.h` & `dlib-19.9.0/dlib/geometry/vector_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/global_optimization/find_max_global.h` & `dlib-19.9.0/dlib/global_optimization/find_max_global.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/global_optimization/find_max_global_abstract.h` & `dlib-19.9.0/dlib/global_optimization/find_max_global_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/global_optimization/global_function_search.cpp` & `dlib-19.9.0/dlib/global_optimization/global_function_search.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/global_optimization/global_function_search.h` & `dlib-19.9.0/dlib/global_optimization/global_function_search.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/global_optimization/global_function_search_abstract.h` & `dlib-19.9.0/dlib/global_optimization/global_function_search_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/global_optimization/upper_bound_function.h` & `dlib-19.9.0/dlib/global_optimization/upper_bound_function.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/global_optimization/upper_bound_function_abstract.h` & `dlib-19.9.0/dlib/global_optimization/upper_bound_function_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph/graph_kernel_1.h` & `dlib-19.9.0/dlib/graph/graph_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph/graph_kernel_abstract.h` & `dlib-19.9.0/dlib/graph/graph_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_cuts/find_max_factor_graph_potts.h` & `dlib-19.9.0/dlib/graph_cuts/find_max_factor_graph_potts.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_cuts/find_max_factor_graph_potts_abstract.h` & `dlib-19.9.0/dlib/graph_cuts/find_max_factor_graph_potts_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_cuts/general_flow_graph.h` & `dlib-19.9.0/dlib/graph_cuts/general_flow_graph.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_cuts/general_potts_problem.h` & `dlib-19.9.0/dlib/graph_cuts/general_potts_problem.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_cuts/graph_labeler.h` & `dlib-19.9.0/dlib/graph_cuts/graph_labeler.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_cuts/graph_labeler_abstract.h` & `dlib-19.9.0/dlib/graph_cuts/graph_labeler_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_cuts/min_cut.h` & `dlib-19.9.0/dlib/graph_cuts/min_cut.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_cuts/min_cut_abstract.h` & `dlib-19.9.0/dlib/graph_cuts/min_cut_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/edge_list_graphs.h` & `dlib-19.9.0/dlib/graph_utils/edge_list_graphs.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/edge_list_graphs_abstract.h` & `dlib-19.9.0/dlib/graph_utils/edge_list_graphs_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/find_k_nearest_neighbors_lsh.h` & `dlib-19.9.0/dlib/graph_utils/find_k_nearest_neighbors_lsh.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/find_k_nearest_neighbors_lsh_abstract.h` & `dlib-19.9.0/dlib/graph_utils/find_k_nearest_neighbors_lsh_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/function_objects.h` & `dlib-19.9.0/dlib/graph_utils/function_objects.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/function_objects_abstract.h` & `dlib-19.9.0/dlib/graph_utils/function_objects_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/graph_utils.h` & `dlib-19.9.0/dlib/graph_utils/graph_utils.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/graph_utils_abstract.h` & `dlib-19.9.0/dlib/graph_utils/graph_utils_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/ordered_sample_pair.h` & `dlib-19.9.0/dlib/graph_utils/ordered_sample_pair.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/ordered_sample_pair_abstract.h` & `dlib-19.9.0/dlib/graph_utils/ordered_sample_pair_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/sample_pair.h` & `dlib-19.9.0/dlib/graph_utils/sample_pair.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph_utils/sample_pair_abstract.h` & `dlib-19.9.0/dlib/graph_utils/sample_pair_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_core/gui_core_kernel_1.cpp` & `dlib-19.9.0/dlib/gui_core/gui_core_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_core/gui_core_kernel_1.h` & `dlib-19.9.0/dlib/gui_core/gui_core_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_core/gui_core_kernel_2.cpp` & `dlib-19.9.0/dlib/gui_core/gui_core_kernel_2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_core/gui_core_kernel_2.h` & `dlib-19.9.0/dlib/gui_core/gui_core_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_core/gui_core_kernel_abstract.h` & `dlib-19.9.0/dlib/gui_core/gui_core_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/base_widgets.cpp` & `dlib-19.9.0/dlib/gui_widgets/base_widgets.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/base_widgets.h` & `dlib-19.9.0/dlib/gui_widgets/base_widgets.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/base_widgets_abstract.h` & `dlib-19.9.0/dlib/gui_widgets/base_widgets_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/canvas_drawing.cpp` & `dlib-19.9.0/dlib/gui_widgets/canvas_drawing.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/canvas_drawing.h` & `dlib-19.9.0/dlib/gui_widgets/canvas_drawing.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/canvas_drawing_abstract.h` & `dlib-19.9.0/dlib/gui_widgets/canvas_drawing_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/drawable.cpp` & `dlib-19.9.0/dlib/gui_widgets/drawable.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/drawable.h` & `dlib-19.9.0/dlib/gui_widgets/drawable.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/drawable_abstract.h` & `dlib-19.9.0/dlib/gui_widgets/drawable_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/fonts.cpp` & `dlib-19.9.0/dlib/gui_widgets/fonts.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/fonts.h` & `dlib-19.9.0/dlib/gui_widgets/fonts.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/fonts_abstract.h` & `dlib-19.9.0/dlib/gui_widgets/fonts_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/nativefont.h` & `dlib-19.9.0/dlib/gui_widgets/nativefont.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/style.cpp` & `dlib-19.9.0/dlib/gui_widgets/style.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/style.h` & `dlib-19.9.0/dlib/gui_widgets/style.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/style_abstract.h` & `dlib-19.9.0/dlib/gui_widgets/style_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/widgets.cpp` & `dlib-19.9.0/dlib/gui_widgets/widgets.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/widgets.h` & `dlib-19.9.0/dlib/gui_widgets/widgets.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/gui_widgets/widgets_abstract.h` & `dlib-19.9.0/dlib/gui_widgets/widgets_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_map/hash_map_kernel_1.h` & `dlib-19.9.0/dlib/hash_map/hash_map_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_map/hash_map_kernel_abstract.h` & `dlib-19.9.0/dlib/hash_map/hash_map_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_map/hash_map_kernel_c.h` & `dlib-19.9.0/dlib/hash_map/hash_map_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_set/hash_set_kernel_1.h` & `dlib-19.9.0/dlib/hash_set/hash_set_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_set/hash_set_kernel_abstract.h` & `dlib-19.9.0/dlib/hash_set/hash_set_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_set/hash_set_kernel_c.h` & `dlib-19.9.0/dlib/hash_set/hash_set_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_table/hash_table_kernel_1.h` & `dlib-19.9.0/dlib/hash_table/hash_table_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_table/hash_table_kernel_2.h` & `dlib-19.9.0/dlib/hash_table/hash_table_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_table/hash_table_kernel_abstract.h` & `dlib-19.9.0/dlib/hash_table/hash_table_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_table/hash_table_kernel_c.h` & `dlib-19.9.0/dlib/hash_table/hash_table_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/http_client/http_client.cpp` & `dlib-19.9.0/dlib/http_client/http_client.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/http_client/http_client.h` & `dlib-19.9.0/dlib/http_client/http_client.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/http_client/http_client_abstract.h` & `dlib-19.9.0/dlib/http_client/http_client_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/binned_vector_feature_image.h` & `dlib-19.9.0/dlib/image_keypoint/binned_vector_feature_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/binned_vector_feature_image_abstract.h` & `dlib-19.9.0/dlib/image_keypoint/binned_vector_feature_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/build_separable_poly_filters.h` & `dlib-19.9.0/dlib/image_keypoint/build_separable_poly_filters.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/draw_surf_points.h` & `dlib-19.9.0/dlib/image_keypoint/draw_surf_points.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/draw_surf_points_abstract.h` & `dlib-19.9.0/dlib/image_keypoint/draw_surf_points_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/fine_hog_image.h` & `dlib-19.9.0/dlib/image_keypoint/fine_hog_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/fine_hog_image_abstract.h` & `dlib-19.9.0/dlib/image_keypoint/fine_hog_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/hashed_feature_image.h` & `dlib-19.9.0/dlib/image_keypoint/hashed_feature_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/hashed_feature_image_abstract.h` & `dlib-19.9.0/dlib/image_keypoint/hashed_feature_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/hessian_pyramid.h` & `dlib-19.9.0/dlib/image_keypoint/hessian_pyramid.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/hessian_pyramid_abstract.h` & `dlib-19.9.0/dlib/image_keypoint/hessian_pyramid_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/hog.h` & `dlib-19.9.0/dlib/image_keypoint/hog.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/hog_abstract.h` & `dlib-19.9.0/dlib/image_keypoint/hog_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/nearest_neighbor_feature_image.h` & `dlib-19.9.0/dlib/image_keypoint/nearest_neighbor_feature_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/nearest_neighbor_feature_image_abstract.h` & `dlib-19.9.0/dlib/image_keypoint/nearest_neighbor_feature_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/poly_image.h` & `dlib-19.9.0/dlib/image_keypoint/poly_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/poly_image_abstract.h` & `dlib-19.9.0/dlib/image_keypoint/poly_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/surf.h` & `dlib-19.9.0/dlib/image_keypoint/surf.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint/surf_abstract.h` & `dlib-19.9.0/dlib/image_keypoint/surf_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/image_loader.h` & `dlib-19.9.0/dlib/image_loader/image_loader.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/image_loader_abstract.h` & `dlib-19.9.0/dlib/image_loader/image_loader_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/jpeg_loader.cpp` & `dlib-19.9.0/dlib/image_loader/jpeg_loader.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/jpeg_loader.h` & `dlib-19.9.0/dlib/image_loader/jpeg_loader.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/jpeg_loader_abstract.h` & `dlib-19.9.0/dlib/image_loader/jpeg_loader_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/load_image.h` & `dlib-19.9.0/dlib/image_loader/load_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/load_image_abstract.h` & `dlib-19.9.0/dlib/image_loader/load_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/png_loader.cpp` & `dlib-19.9.0/dlib/image_loader/png_loader.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/png_loader.h` & `dlib-19.9.0/dlib/image_loader/png_loader.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_loader/png_loader_abstract.h` & `dlib-19.9.0/dlib/image_loader/png_loader_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/box_overlap_testing.h` & `dlib-19.9.0/dlib/image_processing/box_overlap_testing.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/box_overlap_testing_abstract.h` & `dlib-19.9.0/dlib/image_processing/box_overlap_testing_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/correlation_tracker.h` & `dlib-19.9.0/dlib/image_processing/correlation_tracker.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/correlation_tracker_abstract.h` & `dlib-19.9.0/dlib/image_processing/correlation_tracker_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/detection_template_tools.h` & `dlib-19.9.0/dlib/image_processing/detection_template_tools.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/detection_template_tools_abstract.h` & `dlib-19.9.0/dlib/image_processing/detection_template_tools_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/frontal_face_detector.h` & `dlib-19.9.0/dlib/image_processing/frontal_face_detector.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/frontal_face_detector_abstract.h` & `dlib-19.9.0/dlib/image_processing/frontal_face_detector_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/full_object_detection.h` & `dlib-19.9.0/dlib/image_processing/full_object_detection.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/full_object_detection_abstract.h` & `dlib-19.9.0/dlib/image_processing/full_object_detection_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/generic_image.h` & `dlib-19.9.0/dlib/image_processing/generic_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/object_detector.h` & `dlib-19.9.0/dlib/image_processing/object_detector.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/object_detector_abstract.h` & `dlib-19.9.0/dlib/image_processing/object_detector_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/remove_unobtainable_rectangles.h` & `dlib-19.9.0/dlib/image_processing/remove_unobtainable_rectangles.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/remove_unobtainable_rectangles_abstract.h` & `dlib-19.9.0/dlib/image_processing/remove_unobtainable_rectangles_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/render_face_detections.h` & `dlib-19.9.0/dlib/image_processing/render_face_detections.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/render_face_detections_abstract.h` & `dlib-19.9.0/dlib/image_processing/render_face_detections_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_fhog_pyramid.h` & `dlib-19.9.0/dlib/image_processing/scan_fhog_pyramid.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_fhog_pyramid_abstract.h` & `dlib-19.9.0/dlib/image_processing/scan_fhog_pyramid_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image.h` & `dlib-19.9.0/dlib/image_processing/scan_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image_abstract.h` & `dlib-19.9.0/dlib/image_processing/scan_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image_boxes.h` & `dlib-19.9.0/dlib/image_processing/scan_image_boxes.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image_boxes_abstract.h` & `dlib-19.9.0/dlib/image_processing/scan_image_boxes_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image_custom.h` & `dlib-19.9.0/dlib/image_processing/scan_image_custom.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image_custom_abstract.h` & `dlib-19.9.0/dlib/image_processing/scan_image_custom_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image_pyramid.h` & `dlib-19.9.0/dlib/image_processing/scan_image_pyramid.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image_pyramid_abstract.h` & `dlib-19.9.0/dlib/image_processing/scan_image_pyramid_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image_pyramid_tools.h` & `dlib-19.9.0/dlib/image_processing/scan_image_pyramid_tools.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/scan_image_pyramid_tools_abstract.h` & `dlib-19.9.0/dlib/image_processing/scan_image_pyramid_tools_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/setup_hashed_features.h` & `dlib-19.9.0/dlib/image_processing/setup_hashed_features.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/setup_hashed_features_abstract.h` & `dlib-19.9.0/dlib/image_processing/setup_hashed_features_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/shape_predictor.h` & `dlib-19.9.0/dlib/image_processing/shape_predictor.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/shape_predictor_abstract.h` & `dlib-19.9.0/dlib/image_processing/shape_predictor_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/shape_predictor_trainer.h` & `dlib-19.9.0/dlib/image_processing/shape_predictor_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing/shape_predictor_trainer_abstract.h` & `dlib-19.9.0/dlib/image_processing/shape_predictor_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_saver/dng_shared.h` & `dlib-19.9.0/dlib/image_saver/dng_shared.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_saver/image_saver.h` & `dlib-19.9.0/dlib/image_saver/image_saver.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_saver/image_saver_abstract.h` & `dlib-19.9.0/dlib/image_saver/image_saver_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_saver/save_jpeg.cpp` & `dlib-19.9.0/dlib/image_saver/save_jpeg.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_saver/save_jpeg.h` & `dlib-19.9.0/dlib/image_saver/save_jpeg.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_saver/save_jpeg_abstract.h` & `dlib-19.9.0/dlib/image_saver/save_jpeg_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_saver/save_png.cpp` & `dlib-19.9.0/dlib/image_saver/save_png.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_saver/save_png.h` & `dlib-19.9.0/dlib/image_saver/save_png.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_saver/save_png_abstract.h` & `dlib-19.9.0/dlib/image_saver/save_png_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/assign_image.h` & `dlib-19.9.0/dlib/image_transforms/assign_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/assign_image_abstract.h` & `dlib-19.9.0/dlib/image_transforms/assign_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/colormaps.h` & `dlib-19.9.0/dlib/image_transforms/colormaps.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/colormaps_abstract.h` & `dlib-19.9.0/dlib/image_transforms/colormaps_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/draw.h` & `dlib-19.9.0/dlib/image_transforms/draw.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/draw_abstract.h` & `dlib-19.9.0/dlib/image_transforms/draw_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/edge_detector.h` & `dlib-19.9.0/dlib/image_transforms/edge_detector.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/edge_detector_abstract.h` & `dlib-19.9.0/dlib/image_transforms/edge_detector_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/equalize_histogram.h` & `dlib-19.9.0/dlib/image_transforms/equalize_histogram.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/equalize_histogram_abstract.h` & `dlib-19.9.0/dlib/image_transforms/equalize_histogram_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/fhog.h` & `dlib-19.9.0/dlib/image_transforms/fhog.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/fhog_abstract.h` & `dlib-19.9.0/dlib/image_transforms/fhog_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/hough_transform.h` & `dlib-19.9.0/dlib/image_transforms/hough_transform.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/hough_transform_abstract.h` & `dlib-19.9.0/dlib/image_transforms/hough_transform_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/image_pyramid.h` & `dlib-19.9.0/dlib/image_transforms/image_pyramid.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/image_pyramid_abstract.h` & `dlib-19.9.0/dlib/image_transforms/image_pyramid_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/integral_image.h` & `dlib-19.9.0/dlib/image_transforms/integral_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/integral_image_abstract.h` & `dlib-19.9.0/dlib/image_transforms/integral_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/interpolation.h` & `dlib-19.9.0/dlib/image_transforms/interpolation.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/interpolation_abstract.h` & `dlib-19.9.0/dlib/image_transforms/interpolation_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/label_connected_blobs.h` & `dlib-19.9.0/dlib/image_transforms/label_connected_blobs.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/label_connected_blobs_abstract.h` & `dlib-19.9.0/dlib/image_transforms/label_connected_blobs_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/lbp.h` & `dlib-19.9.0/dlib/image_transforms/lbp.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/lbp_abstract.h` & `dlib-19.9.0/dlib/image_transforms/lbp_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/morphological_operations.h` & `dlib-19.9.0/dlib/image_transforms/morphological_operations.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/morphological_operations_abstract.h` & `dlib-19.9.0/dlib/image_transforms/morphological_operations_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/random_color_transform.h` & `dlib-19.9.0/dlib/image_transforms/random_color_transform.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/random_color_transform_abstract.h` & `dlib-19.9.0/dlib/image_transforms/random_color_transform_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/random_cropper.h` & `dlib-19.9.0/dlib/image_transforms/random_cropper.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/random_cropper_abstract.h` & `dlib-19.9.0/dlib/image_transforms/random_cropper_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/segment_image.h` & `dlib-19.9.0/dlib/image_transforms/segment_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/segment_image_abstract.h` & `dlib-19.9.0/dlib/image_transforms/segment_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/spatial_filtering.h` & `dlib-19.9.0/dlib/image_transforms/spatial_filtering.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/spatial_filtering_abstract.h` & `dlib-19.9.0/dlib/image_transforms/spatial_filtering_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/thresholding.h` & `dlib-19.9.0/dlib/image_transforms/thresholding.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms/thresholding_abstract.h` & `dlib-19.9.0/dlib/image_transforms/thresholding_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/interfaces/cmd_line_parser_option.h` & `dlib-19.9.0/dlib/interfaces/cmd_line_parser_option.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/interfaces/enumerable.h` & `dlib-19.9.0/dlib/interfaces/enumerable.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/interfaces/map_pair.h` & `dlib-19.9.0/dlib/interfaces/map_pair.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/interfaces/remover.h` & `dlib-19.9.0/dlib/interfaces/remover.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/iosockstream/iosockstream.h` & `dlib-19.9.0/dlib/iosockstream/iosockstream.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/iosockstream/iosockstream_abstract.h` & `dlib-19.9.0/dlib/iosockstream/iosockstream_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/java/CMakeLists.txt` & `dlib-19.9.0/dlib/java/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/java/cmake_swig_jni` & `dlib-19.9.0/dlib/java/cmake_swig_jni`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/java/java_array.h` & `dlib-19.9.0/dlib/java/java_array.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/java/swig_api.h` & `dlib-19.9.0/dlib/java/swig_api.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/java/swig_test.java` & `dlib-19.9.0/dlib/java/swig_test.java`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/linker/linker_kernel_1.cpp` & `dlib-19.9.0/dlib/linker/linker_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/linker/linker_kernel_1.h` & `dlib-19.9.0/dlib/linker/linker_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/linker/linker_kernel_abstract.h` & `dlib-19.9.0/dlib/linker/linker_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/logger/extra_logger_headers.cpp` & `dlib-19.9.0/dlib/logger/extra_logger_headers.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/logger/extra_logger_headers.h` & `dlib-19.9.0/dlib/logger/extra_logger_headers.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/logger/logger_config_file.cpp` & `dlib-19.9.0/dlib/logger/logger_config_file.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/logger/logger_config_file.h` & `dlib-19.9.0/dlib/logger/logger_config_file.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/logger/logger_kernel_1.cpp` & `dlib-19.9.0/dlib/logger/logger_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/logger/logger_kernel_1.h` & `dlib-19.9.0/dlib/logger/logger_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/logger/logger_kernel_abstract.h` & `dlib-19.9.0/dlib/logger/logger_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lsh/create_random_projection_hash.h` & `dlib-19.9.0/dlib/lsh/create_random_projection_hash.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lsh/create_random_projection_hash_abstract.h` & `dlib-19.9.0/dlib/lsh/create_random_projection_hash_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lsh/hashes.h` & `dlib-19.9.0/dlib/lsh/hashes.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lsh/hashes_abstract.h` & `dlib-19.9.0/dlib/lsh/hashes_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lsh/projection_hash.h` & `dlib-19.9.0/dlib/lsh/projection_hash.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lsh/projection_hash_abstract.h` & `dlib-19.9.0/dlib/lsh/projection_hash_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lz77_buffer/lz77_buffer_kernel_1.h` & `dlib-19.9.0/dlib/lz77_buffer/lz77_buffer_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lz77_buffer/lz77_buffer_kernel_2.h` & `dlib-19.9.0/dlib/lz77_buffer/lz77_buffer_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lz77_buffer/lz77_buffer_kernel_abstract.h` & `dlib-19.9.0/dlib/lz77_buffer/lz77_buffer_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lz77_buffer/lz77_buffer_kernel_c.h` & `dlib-19.9.0/dlib/lz77_buffer/lz77_buffer_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lzp_buffer/lzp_buffer_kernel_1.h` & `dlib-19.9.0/dlib/lzp_buffer/lzp_buffer_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lzp_buffer/lzp_buffer_kernel_2.h` & `dlib-19.9.0/dlib/lzp_buffer/lzp_buffer_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lzp_buffer/lzp_buffer_kernel_abstract.h` & `dlib-19.9.0/dlib/lzp_buffer/lzp_buffer_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lzp_buffer/lzp_buffer_kernel_c.h` & `dlib-19.9.0/dlib/lzp_buffer/lzp_buffer_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/manifold_regularization/linear_manifold_regularizer.h` & `dlib-19.9.0/dlib/manifold_regularization/linear_manifold_regularizer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/manifold_regularization/linear_manifold_regularizer_abstract.h` & `dlib-19.9.0/dlib/manifold_regularization/linear_manifold_regularizer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/map/map_kernel_1.h` & `dlib-19.9.0/dlib/map/map_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/map/map_kernel_abstract.h` & `dlib-19.9.0/dlib/map/map_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/map/map_kernel_c.h` & `dlib-19.9.0/dlib/map/map_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/CMakeLists.txt` & `dlib-19.9.0/dlib/matlab/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/README.txt` & `dlib-19.9.0/dlib/matlab/README.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/call_matlab.h` & `dlib-19.9.0/dlib/matlab/call_matlab.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/cmake_mex_wrapper` & `dlib-19.9.0/dlib/matlab/cmake_mex_wrapper`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/example_mex_callback.cpp` & `dlib-19.9.0/dlib/matlab/example_mex_callback.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/example_mex_class.cpp` & `dlib-19.9.0/dlib/matlab/example_mex_class.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/example_mex_function.cpp` & `dlib-19.9.0/dlib/matlab/example_mex_function.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/example_mex_struct.cpp` & `dlib-19.9.0/dlib/matlab/example_mex_struct.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/mex_wrapper.cpp` & `dlib-19.9.0/dlib/matlab/mex_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/subprocess_stream.cpp` & `dlib-19.9.0/dlib/matlab/subprocess_stream.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matlab/subprocess_stream.h` & `dlib-19.9.0/dlib/matlab/subprocess_stream.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/fortran_id.h` & `dlib-19.9.0/dlib/matrix/lapack/fortran_id.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/gees.h` & `dlib-19.9.0/dlib/matrix/lapack/gees.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/geev.h` & `dlib-19.9.0/dlib/matrix/lapack/geev.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/geqrf.h` & `dlib-19.9.0/dlib/matrix/lapack/geqrf.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/gesdd.h` & `dlib-19.9.0/dlib/matrix/lapack/gesdd.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/gesvd.h` & `dlib-19.9.0/dlib/matrix/lapack/gesvd.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/getrf.h` & `dlib-19.9.0/dlib/matrix/lapack/getrf.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/ormqr.h` & `dlib-19.9.0/dlib/matrix/lapack/ormqr.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/pbtrf.h` & `dlib-19.9.0/dlib/matrix/lapack/pbtrf.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/potrf.h` & `dlib-19.9.0/dlib/matrix/lapack/potrf.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/syev.h` & `dlib-19.9.0/dlib/matrix/lapack/syev.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/lapack/syevr.h` & `dlib-19.9.0/dlib/matrix/lapack/syevr.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/cblas_constants.h` & `dlib-19.9.0/dlib/matrix/cblas_constants.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix.h` & `dlib-19.9.0/dlib/matrix/matrix.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_assign.h` & `dlib-19.9.0/dlib/matrix/matrix_assign.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_assign_fwd.h` & `dlib-19.9.0/dlib/matrix/matrix_assign_fwd.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_blas_bindings.h` & `dlib-19.9.0/dlib/matrix/matrix_blas_bindings.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_cholesky.h` & `dlib-19.9.0/dlib/matrix/matrix_cholesky.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_conj_trans.h` & `dlib-19.9.0/dlib/matrix/matrix_conj_trans.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_conv.h` & `dlib-19.9.0/dlib/matrix/matrix_conv.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_conv_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_conv_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_data_layout.h` & `dlib-19.9.0/dlib/matrix/matrix_data_layout.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_data_layout_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_data_layout_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_default_mul.h` & `dlib-19.9.0/dlib/matrix/matrix_default_mul.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_eigenvalue.h` & `dlib-19.9.0/dlib/matrix/matrix_eigenvalue.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_exp.h` & `dlib-19.9.0/dlib/matrix/matrix_exp.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_exp_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_exp_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_expressions.h` & `dlib-19.9.0/dlib/matrix/matrix_expressions.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_fft.h` & `dlib-19.9.0/dlib/matrix/matrix_fft.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_fft_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_fft_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_fwd.h` & `dlib-19.9.0/dlib/matrix/matrix_fwd.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_generic_image.h` & `dlib-19.9.0/dlib/matrix/matrix_generic_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_la.h` & `dlib-19.9.0/dlib/matrix/matrix_la.h`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 #ifdef DLIB_USE_LAPACK
 #include "lapack/potrf.h"
 #include "lapack/pbtrf.h"
 #include "lapack/gesdd.h"
 #include "lapack/gesvd.h"
 #endif
 
+#include "../threads.h"
+
 #include <iostream>
 
 namespace dlib
 {
 
 // ----------------------------------------------------------------------------------------
 // ----------------------------------------------------------------------------------------
@@ -640,61 +642,67 @@
               singular values.  In these cases, using a q of 1 or 2 is good.
     !*/
     {
         DLIB_ASSERT(A.size() >= l, "Invalid inputs were given to this function.");
         Q.set_size(A.size(), l);
 
         // Compute Q = A*gaussian_randm()
-        for (long r = 0; r < Q.nr(); ++r)
+        parallel_for(0, Q.nr(), [&](long r)
         {
             for (long c = 0; c < Q.nc(); ++c)
             {
                 Q(r,c) = dot(A[r], gaussian_randm(std::numeric_limits<long>::max(), 1, c));
             }
-        }
+        });
 
         orthogonalize(Q);
 
         // Do some extra iterations of the power method to make sure we get Q into the 
         // span of the most important singular vectors of A.
         if (q != 0)
         {
+            dlib::mutex mut;
             const unsigned long n = max_index_plus_one(A);
             for (unsigned long itr = 0; itr < q; ++itr)
             {
-                matrix<T,0,0,MM,L> Z(n, l);
+                matrix<T,0,0,MM> Z;
                 // Compute Z = trans(A)*Q
-                Z = 0;
-                for (unsigned long m = 0; m < A.size(); ++m)
+                parallel_for_blocked(0, A.size(), [&](long begin, long end)
                 {
-                    for (unsigned long r = 0; r < l; ++r)
+                    matrix<T,0,0,MM> Zlocal(n,l);
+                    Zlocal = 0;
+                    for (long m = begin; m < end; ++m)
                     {
-                        typename sparse_vector_type::const_iterator i;
-                        for (i = A[m].begin(); i != A[m].end(); ++i)
+                        for (unsigned long r = 0; r < l; ++r)
                         {
-                            const unsigned long c = i->first;
-                            const T val = i->second;
+                            for (auto& i : A[m])
+                            {
+                                const auto c = i.first;
+                                const auto val = i.second;
 
-                            Z(c,r) += Q(m,r)*val;
+                                Zlocal(c,r) += Q(m,r)*val;
+                            }
                         }
                     }
-                }
+                    auto_mutex lock(mut);
+                    Z += Zlocal;
+                },1);
 
                 Q.set_size(0,0); // free RAM
                 orthogonalize(Z);
 
                 // Compute Q = A*Z
                 Q.set_size(A.size(), l);
-                for (long r = 0; r < Q.nr(); ++r)
+                parallel_for(0, Q.nr(), [&](long r)
                 {
                     for (long c = 0; c < Q.nc(); ++c)
                     {
                         Q(r,c) = dot(A[r], colm(Z,c));
                     }
-                }
+                });
 
                 Z.set_size(0,0); // free RAM
                 orthogonalize(Q);
             }
         }
     }
 
@@ -732,30 +740,36 @@
         matrix<T,0,0,MM,L> Q;
         find_matrix_range(A, k, Q, q);
 
         // Compute trans(B) = trans(Q)*A.   The reason we store B transposed
         // is so that when we take its SVD later using svd3() it doesn't consume
         // a whole lot of RAM.  That is, we make sure the square matrix coming out
         // of svd3() has size lxl rather than the potentially much larger nxn.
-        matrix<T,0,0,MM,L> B(n,k);
-        B = 0;
-        for (unsigned long m = 0; m < A.size(); ++m)
+        matrix<T,0,0,MM> B;
+        dlib::mutex mut;
+        parallel_for_blocked(0, A.size(), [&](long begin, long end)
         {
-            for (unsigned long r = 0; r < k; ++r)
+            matrix<T,0,0,MM> Blocal(n,k);
+            Blocal = 0;
+            for (long m = begin; m < end; ++m)
             {
-                typename sparse_vector_type::const_iterator i;
-                for (i = A[m].begin(); i != A[m].end(); ++i)
+                for (unsigned long r = 0; r < k; ++r)
                 {
-                    const unsigned long c = i->first;
-                    const T val = i->second;
+                    for (auto& i : A[m])
+                    {
+                        const auto c = i.first;
+                        const auto val = i.second;
 
-                    B(c,r) += Q(m,r)*val;
+                        Blocal(c,r) += Q(m,r)*val;
+                    }
                 }
             }
-        }
+            auto_mutex lock(mut);
+            B += Blocal;
+        },1);
 
         svd3(B, v,w,u);
         u = Q*u;
     }
 
 // ----------------------------------------------------------------------------------------
 // ----------------------------------------------------------------------------------------
```

### Comparing `dlib-19.8.2/dlib/matrix/matrix_la_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_la_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_lu.h` & `dlib-19.9.0/dlib/matrix/matrix_lu.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_mat.h` & `dlib-19.9.0/dlib/matrix/matrix_mat.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_mat_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_mat_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_math_functions.h` & `dlib-19.9.0/dlib/matrix/matrix_math_functions.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_math_functions_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_math_functions_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_op.h` & `dlib-19.9.0/dlib/matrix/matrix_op.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_qr.h` & `dlib-19.9.0/dlib/matrix/matrix_qr.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_read_from_istream.h` & `dlib-19.9.0/dlib/matrix/matrix_read_from_istream.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_subexp.h` & `dlib-19.9.0/dlib/matrix/matrix_subexp.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_subexp_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_subexp_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_trsm.h` & `dlib-19.9.0/dlib/matrix/matrix_trsm.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_utilities.h` & `dlib-19.9.0/dlib/matrix/matrix_utilities.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/matrix_utilities_abstract.h` & `dlib-19.9.0/dlib/matrix/matrix_utilities_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/symmetric_matrix_cache.h` & `dlib-19.9.0/dlib/matrix/symmetric_matrix_cache.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix/symmetric_matrix_cache_abstract.h` & `dlib-19.9.0/dlib/matrix/symmetric_matrix_cache_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/md5/md5_kernel_1.cpp` & `dlib-19.9.0/dlib/md5/md5_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/md5/md5_kernel_1.h` & `dlib-19.9.0/dlib/md5/md5_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/md5/md5_kernel_abstract.h` & `dlib-19.9.0/dlib/md5/md5_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/member_function_pointer/make_mfp.h` & `dlib-19.9.0/dlib/member_function_pointer/make_mfp.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/member_function_pointer/make_mfp_abstract.h` & `dlib-19.9.0/dlib/member_function_pointer/make_mfp_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/member_function_pointer/member_function_pointer_kernel_1.h` & `dlib-19.9.0/dlib/member_function_pointer/member_function_pointer_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/member_function_pointer/member_function_pointer_kernel_abstract.h` & `dlib-19.9.0/dlib/member_function_pointer/member_function_pointer_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager/memory_manager_kernel_1.h` & `dlib-19.9.0/dlib/memory_manager/memory_manager_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager/memory_manager_kernel_2.h` & `dlib-19.9.0/dlib/memory_manager/memory_manager_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager/memory_manager_kernel_3.h` & `dlib-19.9.0/dlib/memory_manager/memory_manager_kernel_3.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager/memory_manager_kernel_abstract.h` & `dlib-19.9.0/dlib/memory_manager/memory_manager_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager_global/memory_manager_global_kernel_1.h` & `dlib-19.9.0/dlib/memory_manager_global/memory_manager_global_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager_global/memory_manager_global_kernel_abstract.h` & `dlib-19.9.0/dlib/memory_manager_global/memory_manager_global_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager_stateless/memory_manager_stateless_kernel_1.h` & `dlib-19.9.0/dlib/memory_manager_stateless/memory_manager_stateless_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager_stateless/memory_manager_stateless_kernel_2.h` & `dlib-19.9.0/dlib/memory_manager_stateless/memory_manager_stateless_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager_stateless/memory_manager_stateless_kernel_abstract.h` & `dlib-19.9.0/dlib/memory_manager_stateless/memory_manager_stateless_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/misc_api/misc_api_kernel_1.cpp` & `dlib-19.9.0/dlib/misc_api/misc_api_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/misc_api/misc_api_kernel_1.h` & `dlib-19.9.0/dlib/misc_api/misc_api_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/misc_api/misc_api_kernel_2.cpp` & `dlib-19.9.0/dlib/misc_api/misc_api_kernel_2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/misc_api/misc_api_kernel_2.h` & `dlib-19.9.0/dlib/misc_api/misc_api_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/misc_api/misc_api_kernel_abstract.h` & `dlib-19.9.0/dlib/misc_api/misc_api_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/misc_api/misc_api_shared.h` & `dlib-19.9.0/dlib/misc_api/misc_api_shared.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/mlp/mlp_kernel_1.h` & `dlib-19.9.0/dlib/mlp/mlp_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/mlp/mlp_kernel_abstract.h` & `dlib-19.9.0/dlib/mlp/mlp_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/mlp/mlp_kernel_c.h` & `dlib-19.9.0/dlib/mlp/mlp_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/numerical_integration/integrate_function_adapt_simpson.h` & `dlib-19.9.0/dlib/numerical_integration/integrate_function_adapt_simpson.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/numerical_integration/integrate_function_adapt_simpson_abstract.h` & `dlib-19.9.0/dlib/numerical_integration/integrate_function_adapt_simpson_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/opencv/cv_image.h` & `dlib-19.9.0/dlib/opencv/cv_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/opencv/cv_image_abstract.h` & `dlib-19.9.0/dlib/opencv/cv_image_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/opencv/to_open_cv.h` & `dlib-19.9.0/dlib/opencv/to_open_cv.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/opencv/to_open_cv_abstract.h` & `dlib-19.9.0/dlib/opencv/to_open_cv_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/elastic_net.h` & `dlib-19.9.0/dlib/optimization/elastic_net.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/elastic_net_abstract.h` & `dlib-19.9.0/dlib/optimization/elastic_net_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/find_max_factor_graph_nmplp.h` & `dlib-19.9.0/dlib/optimization/find_max_factor_graph_nmplp.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/find_max_factor_graph_nmplp_abstract.h` & `dlib-19.9.0/dlib/optimization/find_max_factor_graph_nmplp_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/find_max_factor_graph_viterbi.h` & `dlib-19.9.0/dlib/optimization/find_max_factor_graph_viterbi.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/find_max_factor_graph_viterbi_abstract.h` & `dlib-19.9.0/dlib/optimization/find_max_factor_graph_viterbi_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/find_max_parse_cky.h` & `dlib-19.9.0/dlib/optimization/find_max_parse_cky.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/find_max_parse_cky_abstract.h` & `dlib-19.9.0/dlib/optimization/find_max_parse_cky_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/find_optimal_parameters.h` & `dlib-19.9.0/dlib/optimization/find_optimal_parameters.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/find_optimal_parameters_abstract.h` & `dlib-19.9.0/dlib/optimization/find_optimal_parameters_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/max_cost_assignment.h` & `dlib-19.9.0/dlib/optimization/max_cost_assignment.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/max_cost_assignment_abstract.h` & `dlib-19.9.0/dlib/optimization/max_cost_assignment_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/max_sum_submatrix.h` & `dlib-19.9.0/dlib/optimization/max_sum_submatrix.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/max_sum_submatrix_abstract.h` & `dlib-19.9.0/dlib/optimization/max_sum_submatrix_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization.h` & `dlib-19.9.0/dlib/optimization/optimization.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_bobyqa.h` & `dlib-19.9.0/dlib/optimization/optimization_bobyqa.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_bobyqa_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_bobyqa_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_least_squares.h` & `dlib-19.9.0/dlib/optimization/optimization_least_squares.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_least_squares_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_least_squares_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_line_search.h` & `dlib-19.9.0/dlib/optimization/optimization_line_search.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_line_search_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_line_search_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_oca.h` & `dlib-19.9.0/dlib/optimization/optimization_oca.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_oca_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_oca_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_search_strategies.h` & `dlib-19.9.0/dlib/optimization/optimization_search_strategies.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_search_strategies_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_search_strategies_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_solve_qp2_using_smo.h` & `dlib-19.9.0/dlib/optimization/optimization_solve_qp2_using_smo.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_solve_qp2_using_smo_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_solve_qp2_using_smo_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_solve_qp3_using_smo.h` & `dlib-19.9.0/dlib/optimization/optimization_solve_qp3_using_smo.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_solve_qp3_using_smo_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_solve_qp3_using_smo_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_solve_qp_using_smo.h` & `dlib-19.9.0/dlib/optimization/optimization_solve_qp_using_smo.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_solve_qp_using_smo_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_solve_qp_using_smo_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_stop_strategies.h` & `dlib-19.9.0/dlib/optimization/optimization_stop_strategies.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_stop_strategies_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_stop_strategies_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_trust_region.h` & `dlib-19.9.0/dlib/optimization/optimization_trust_region.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization/optimization_trust_region_abstract.h` & `dlib-19.9.0/dlib/optimization/optimization_trust_region_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/pipe/pipe_kernel_1.h` & `dlib-19.9.0/dlib/pipe/pipe_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/pipe/pipe_kernel_abstract.h` & `dlib-19.9.0/dlib/pipe/pipe_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/python/numpy.h` & `dlib-19.9.0/dlib/python/numpy.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/python/numpy_image.h` & `dlib-19.9.0/dlib/python/numpy_image.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/python/pyassert.h` & `dlib-19.9.0/dlib/python/pyassert.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/python/pybind_utils.h` & `dlib-19.9.0/dlib/python/pybind_utils.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/python/serialize_pickle.h` & `dlib-19.9.0/dlib/python/serialize_pickle.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/quantum_computing/quantum_computing.h` & `dlib-19.9.0/dlib/quantum_computing/quantum_computing.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/quantum_computing/quantum_computing_abstract.h` & `dlib-19.9.0/dlib/quantum_computing/quantum_computing_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/queue/queue_kernel_1.h` & `dlib-19.9.0/dlib/queue/queue_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/queue/queue_kernel_2.h` & `dlib-19.9.0/dlib/queue/queue_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/queue/queue_kernel_abstract.h` & `dlib-19.9.0/dlib/queue/queue_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/queue/queue_kernel_c.h` & `dlib-19.9.0/dlib/queue/queue_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/queue/queue_sort_1.h` & `dlib-19.9.0/dlib/queue/queue_sort_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/queue/queue_sort_abstract.h` & `dlib-19.9.0/dlib/queue/queue_sort_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/rand/mersenne_twister.h` & `dlib-19.9.0/dlib/rand/mersenne_twister.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/rand/rand_kernel_1.h` & `dlib-19.9.0/dlib/rand/rand_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/rand/rand_kernel_abstract.h` & `dlib-19.9.0/dlib/rand/rand_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/reference_counter/reference_counter_kernel_1.h` & `dlib-19.9.0/dlib/reference_counter/reference_counter_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/reference_counter/reference_counter_kernel_abstract.h` & `dlib-19.9.0/dlib/reference_counter/reference_counter_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence/sequence_compare_1.h` & `dlib-19.9.0/dlib/sequence/sequence_compare_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence/sequence_compare_abstract.h` & `dlib-19.9.0/dlib/sequence/sequence_compare_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence/sequence_kernel_1.h` & `dlib-19.9.0/dlib/sequence/sequence_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence/sequence_kernel_2.h` & `dlib-19.9.0/dlib/sequence/sequence_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence/sequence_kernel_abstract.h` & `dlib-19.9.0/dlib/sequence/sequence_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence/sequence_kernel_c.h` & `dlib-19.9.0/dlib/sequence/sequence_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence/sequence_sort_1.h` & `dlib-19.9.0/dlib/sequence/sequence_sort_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence/sequence_sort_2.h` & `dlib-19.9.0/dlib/sequence/sequence_sort_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence/sequence_sort_abstract.h` & `dlib-19.9.0/dlib/sequence/sequence_sort_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/server/server_http.cpp` & `dlib-19.9.0/dlib/server/server_http.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/server/server_http.h` & `dlib-19.9.0/dlib/server/server_http.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/server/server_http_abstract.h` & `dlib-19.9.0/dlib/server/server_http_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/server/server_iostream.h` & `dlib-19.9.0/dlib/server/server_iostream.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/server/server_iostream_abstract.h` & `dlib-19.9.0/dlib/server/server_iostream_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/server/server_kernel.cpp` & `dlib-19.9.0/dlib/server/server_kernel.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/server/server_kernel.h` & `dlib-19.9.0/dlib/server/server_kernel.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/server/server_kernel_abstract.h` & `dlib-19.9.0/dlib/server/server_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/set/set_compare_1.h` & `dlib-19.9.0/dlib/set/set_compare_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/set/set_compare_abstract.h` & `dlib-19.9.0/dlib/set/set_compare_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/set/set_kernel_1.h` & `dlib-19.9.0/dlib/set/set_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/set/set_kernel_abstract.h` & `dlib-19.9.0/dlib/set/set_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/set/set_kernel_c.h` & `dlib-19.9.0/dlib/set/set_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/set_utils/set_utils.h` & `dlib-19.9.0/dlib/set_utils/set_utils.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/set_utils/set_utils_abstract.h` & `dlib-19.9.0/dlib/set_utils/set_utils_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/simd/simd4f.h` & `dlib-19.9.0/dlib/simd/simd4f.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/simd/simd4i.h` & `dlib-19.9.0/dlib/simd/simd4i.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/simd/simd8f.h` & `dlib-19.9.0/dlib/simd/simd8f.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/simd/simd8i.h` & `dlib-19.9.0/dlib/simd/simd8i.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/simd/simd_check.h` & `dlib-19.9.0/dlib/simd/simd_check.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sliding_buffer/circular_buffer.h` & `dlib-19.9.0/dlib/sliding_buffer/circular_buffer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sliding_buffer/circular_buffer_abstract.h` & `dlib-19.9.0/dlib/sliding_buffer/circular_buffer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sliding_buffer/sliding_buffer_kernel_1.h` & `dlib-19.9.0/dlib/sliding_buffer/sliding_buffer_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sliding_buffer/sliding_buffer_kernel_abstract.h` & `dlib-19.9.0/dlib/sliding_buffer/sliding_buffer_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sliding_buffer/sliding_buffer_kernel_c.h` & `dlib-19.9.0/dlib/sliding_buffer/sliding_buffer_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/smart_pointers/shared_ptr.h` & `dlib-19.9.0/dlib/smart_pointers/shared_ptr.h`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,14 @@
 #include <algorithm>
 #include <memory>
 #include <typeinfo>
 #include <string>       // for the exceptions
 #include "../algs.h"
 #include "shared_ptr_abstract.h"
 
-// Don't warn about the use of std::auto_ptr in this file.  There is a pragma at the end of
-// this file that re-enables the warning.
-#if (defined(__GNUC__) && ((__GNUC__ >= 4 && __GNUC_MINOR__ >= 6) || (__GNUC__ > 4))) || \
-    (defined(__clang__) && ((__clang_major__ >= 3 && __clang_minor__ >= 4)))
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wdeprecated-declarations"
-#endif
-
 namespace dlib 
 {
 
 // ----------------------------------------------------------------------------------------
 
     class bad_weak_ptr: public std::exception {};
 
@@ -297,29 +289,14 @@
                 throw bad_weak_ptr();
 
             data = r.data;
             shared_node = r.weak_node->shared_node;
             shared_node->ref_count += 1;
         }
 
-        template<typename Y>
-        explicit shared_ptr(
-            std::auto_ptr<Y>& r
-        )
-        {
-            DLIB_ASSERT(r.get() != 0,
-                "\tshared_ptr::shared_ptr(auto_ptr r)"
-                << "\n\tr.get() can't be null"
-                << "\n\tthis: " << this
-                );
-            shared_node = new shared_ptr_node;
-            shared_node->del = new default_deleter;
-            data = r.release();
-        }
-
         shared_ptr& operator= (
             const shared_ptr& r
         )
         {
             shared_ptr(r).swap(*this);
             return *this;
         }
@@ -329,32 +306,14 @@
             const shared_ptr<Y>& r
         )
         {
             shared_ptr(r).swap(*this);
             return *this;
         }
 
-        template<typename Y> 
-        shared_ptr& operator= (
-            std::auto_ptr<Y>& r
-        )
-        {
-            DLIB_ASSERT(r.get() != 0,
-                "\tshared_ptr::operator=(auto_ptr r)"
-                << "\n\tr.get() can't be null"
-                << "\n\tthis: " << this
-                );
-
-            reset();
-            shared_node = new shared_ptr_node;
-            shared_node->del = new default_deleter;
-            data = r.release();
-            return *this;
-        }
-
         void reset()
         {
             shared_ptr().swap(*this);
         }
 
         template<typename Y> 
         void reset(Y* p)
@@ -524,14 +483,10 @@
         return p.template _get_deleter<D>();
     }
 
 // ----------------------------------------------------------------------------------------
 
 }
 
-#if (defined(__GNUC__) && ((__GNUC__ >= 4 && __GNUC_MINOR__ >= 6) || (__GNUC__ > 4))) || \
-    (defined(__clang__) && ((__clang_major__ >= 3 && __clang_minor__ >= 4)))
-#pragma GCC diagnostic pop
-#endif
 
 #endif // DLIB_SHARED_PTr_
```

### Comparing `dlib-19.8.2/dlib/smart_pointers/shared_ptr_abstract.h` & `dlib-19.9.0/dlib/smart_pointers/shared_ptr_abstract.h`

 * *Files 4% similar despite different names*

```diff
@@ -132,32 +132,14 @@
                 - If r is empty, constructs an empty shared_ptr object; otherwise, constructs 
                   a shared_ptr object that shares ownership with r.
             throws
                 - bad_weak_ptr
                   this exception is thrown if r.expired() == true
         !*/
 
-        template<typename Y>
-        explicit shared_ptr(
-            std::auto_ptr<Y>& r
-        );
-        /*!
-            requires
-                - p.get() != 0
-                - p.release() is convertible to a T* type pointer
-                - p.release() can be deleted by calling "delete p.release();" and doing so will not throw exceptions
-            ensures
-                - #get() == p.release()
-                - #use_count() == 1
-                - #r.get() == 0
-                - #*this object owns the pointer p.release()
-            throws
-                - std::bad_alloc
-        !*/
-
         ~shared_ptr(
         );
         /*!
             ensures
                 - if (use_count() > 1)
                     - this object destroys itself but otherwise has no effect (i.e. 
                       the pointer get() is still valid and shared between the remaining
@@ -186,28 +168,14 @@
             requires
                 - Y* is convertible to T* 
             ensures
                 - equivalent to shared_ptr(r).swap(*this).
                 - returns #*this
         !*/
 
-        template<typename Y> 
-        shared_ptr& operator= (
-            std::auto_ptr<Y>& r
-        );
-        /*!
-            requires
-                - p.get() != 0
-                - p.release() is convertible to a T* type pointer
-                - p.release() can be deleted by calling "delete p.release();" and doing so will not throw exceptions
-            ensures
-                - equivalent to shared_ptr(r).swap(*this).
-                - returns #*this
-        !*/
-
         void reset(
         );
         /*!
             ensures
                 - equivalent to shared_ptr().swap(*this)
         !*/
```

### Comparing `dlib-19.8.2/dlib/smart_pointers/shared_ptr_thread_safe.h` & `dlib-19.9.0/dlib/smart_pointers/shared_ptr_thread_safe.h`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,14 @@
 #include <memory>
 #include <typeinfo>
 #include <string>       // for the exceptions
 #include "../algs.h"
 #include "shared_ptr_thread_safe_abstract.h"
 #include "../threads/threads_kernel.h"
 
-// Don't warn about the use of std::auto_ptr in this file.  There is a pragma at the end of
-// this file that re-enables the warning.
-#if defined(__GNUC__) && ((__GNUC__ >= 4 && __GNUC_MINOR__ >= 6) || (__GNUC__ > 4))
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wdeprecated-declarations"
-#endif
-
 
 namespace dlib 
 {
 
 // ----------------------------------------------------------------------------------------
 
     struct shared_ptr_thread_safe_deleter
@@ -260,28 +253,14 @@
             if (shared_node)
             {
                 auto_mutex M(shared_node->m);
                 shared_node->ref_count += 1;
             }
         }
 
-        template<typename Y>
-        explicit shared_ptr_thread_safe(
-            std::auto_ptr<Y>& r
-        )
-        {
-            DLIB_ASSERT(r.get() != 0,
-                "\tshared_ptr::shared_ptr_thread_safe(auto_ptr r)"
-                << "\n\tr.get() can't be null"
-                << "\n\tthis: " << this
-                );
-            shared_node = new shared_ptr_thread_safe_node;
-            data = r.release();
-        }
-
         shared_ptr_thread_safe& operator= (
             const shared_ptr_thread_safe& r
         )
         {
             shared_ptr_thread_safe(r).swap(*this);
             return *this;
         }
@@ -291,31 +270,14 @@
             const shared_ptr_thread_safe<Y>& r
         )
         {
             shared_ptr_thread_safe(r).swap(*this);
             return *this;
         }
 
-        template<typename Y> 
-        shared_ptr_thread_safe& operator= (
-            std::auto_ptr<Y>& r
-        )
-        {
-            DLIB_ASSERT(r.get() != 0,
-                "\tshared_ptr::operator=(auto_ptr r)"
-                << "\n\tr.get() can't be null"
-                << "\n\tthis: " << this
-                );
-
-            reset();
-            shared_node = new shared_ptr_thread_safe_node;
-            data = r.release();
-            return *this;
-        }
-
         void reset()
         {
             shared_ptr_thread_safe().swap(*this);
         }
 
         template<typename Y> 
         void reset(Y* p)
@@ -490,15 +452,11 @@
     D* get_deleter(const shared_ptr_thread_safe<T>& p)
     {
         return p.template _get_deleter<D>();
     }
 
 // ----------------------------------------------------------------------------------------
 
-#if defined(__GNUC__) && ((__GNUC__ >= 4 && __GNUC_MINOR__ >= 6) || (__GNUC__ > 4))
-#pragma GCC diagnostic pop
-#endif
-
 }
 
 #endif // DLIB_SHARED_THREAD_SAFE_PTr_
```

### Comparing `dlib-19.8.2/dlib/smart_pointers/shared_ptr_thread_safe_abstract.h` & `dlib-19.9.0/dlib/smart_pointers/shared_ptr_thread_safe_abstract.h`

 * *Files 4% similar despite different names*

```diff
@@ -110,32 +110,14 @@
             ensures
                 - #get() == #r.get()
                 - #use_count() == #r.use_count()
                 - If r is empty, constructs an empty shared_ptr_thread_safe object; otherwise, constructs 
                   a shared_ptr_thread_safe object that shares ownership with r.
         !*/
 
-        template<typename Y>
-        explicit shared_ptr_thread_safe(
-            std::auto_ptr<Y>& r
-        );
-        /*!
-            requires
-                - p.get() != 0
-                - p.release() is convertible to a T* type pointer
-                - p.release() can be deleted by calling "delete p.release();" and doing so will not throw exceptions
-            ensures
-                - #get() == p.release()
-                - #use_count() == 1
-                - #r.get() == 0
-                - #*this object owns the pointer p.release()
-            throws
-                - std::bad_alloc
-        !*/
-
         ~shared_ptr_thread_safe(
         );
         /*!
             ensures
                 - if (use_count() > 1)
                     - this object destroys itself but otherwise has no effect (i.e. 
                       the pointer get() is still valid and shared between the remaining
@@ -164,28 +146,14 @@
             requires
                 - Y* is convertible to T* 
             ensures
                 - equivalent to shared_ptr_thread_safe(r).swap(*this).
                 - returns #*this
         !*/
 
-        template<typename Y> 
-        shared_ptr_thread_safe& operator= (
-            std::auto_ptr<Y>& r
-        );
-        /*!
-            requires
-                - p.get() != 0
-                - p.release() is convertible to a T* type pointer
-                - p.release() can be deleted by calling "delete p.release();" and doing so will not throw exceptions
-            ensures
-                - equivalent to shared_ptr_thread_safe(r).swap(*this).
-                - returns #*this
-        !*/
-
         void reset(
         );
         /*!
             ensures
                 - equivalent to shared_ptr_thread_safe().swap(*this)
         !*/
```

### Comparing `dlib-19.8.2/dlib/smart_pointers/weak_ptr.h` & `dlib-19.9.0/dlib/smart_pointers/weak_ptr.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/smart_pointers/weak_ptr_abstract.h` & `dlib-19.9.0/dlib/smart_pointers/weak_ptr_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockets/sockets_extensions.cpp` & `dlib-19.9.0/dlib/sockets/sockets_extensions.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockets/sockets_extensions.h` & `dlib-19.9.0/dlib/sockets/sockets_extensions.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockets/sockets_extensions_abstract.h` & `dlib-19.9.0/dlib/sockets/sockets_extensions_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockets/sockets_kernel_1.cpp` & `dlib-19.9.0/dlib/sockets/sockets_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockets/sockets_kernel_1.h` & `dlib-19.9.0/dlib/sockets/sockets_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockets/sockets_kernel_2.cpp` & `dlib-19.9.0/dlib/sockets/sockets_kernel_2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockets/sockets_kernel_2.h` & `dlib-19.9.0/dlib/sockets/sockets_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockets/sockets_kernel_abstract.h` & `dlib-19.9.0/dlib/sockets/sockets_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockstreambuf/sockstreambuf.cpp` & `dlib-19.9.0/dlib/sockstreambuf/sockstreambuf.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockstreambuf/sockstreambuf.h` & `dlib-19.9.0/dlib/sockstreambuf/sockstreambuf.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockstreambuf/sockstreambuf_abstract.h` & `dlib-19.9.0/dlib/sockstreambuf/sockstreambuf_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockstreambuf/sockstreambuf_unbuffered.cpp` & `dlib-19.9.0/dlib/sockstreambuf/sockstreambuf_unbuffered.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sockstreambuf/sockstreambuf_unbuffered.h` & `dlib-19.9.0/dlib/sockstreambuf/sockstreambuf_unbuffered.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sqlite/sqlite.h` & `dlib-19.9.0/dlib/sqlite/sqlite.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sqlite/sqlite_abstract.h` & `dlib-19.9.0/dlib/sqlite/sqlite_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sqlite/sqlite_tools.h` & `dlib-19.9.0/dlib/sqlite/sqlite_tools.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sqlite/sqlite_tools_abstract.h` & `dlib-19.9.0/dlib/sqlite/sqlite_tools_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/stack/stack_kernel_1.h` & `dlib-19.9.0/dlib/stack/stack_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/stack/stack_kernel_abstract.h` & `dlib-19.9.0/dlib/stack/stack_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/stack/stack_kernel_c.h` & `dlib-19.9.0/dlib/stack/stack_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_map/static_map_kernel_1.h` & `dlib-19.9.0/dlib/static_map/static_map_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_map/static_map_kernel_abstract.h` & `dlib-19.9.0/dlib/static_map/static_map_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_map/static_map_kernel_c.h` & `dlib-19.9.0/dlib/static_map/static_map_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_set/static_set_compare_1.h` & `dlib-19.9.0/dlib/static_set/static_set_compare_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_set/static_set_compare_abstract.h` & `dlib-19.9.0/dlib/static_set/static_set_compare_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_set/static_set_kernel_1.h` & `dlib-19.9.0/dlib/static_set/static_set_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_set/static_set_kernel_abstract.h` & `dlib-19.9.0/dlib/static_set/static_set_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_set/static_set_kernel_c.h` & `dlib-19.9.0/dlib/static_set/static_set_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/average_precision.h` & `dlib-19.9.0/dlib/statistics/average_precision.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/average_precision_abstract.h` & `dlib-19.9.0/dlib/statistics/average_precision_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/cca.h` & `dlib-19.9.0/dlib/statistics/cca.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/cca_abstract.h` & `dlib-19.9.0/dlib/statistics/cca_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/dpca.h` & `dlib-19.9.0/dlib/statistics/dpca.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/dpca_abstract.h` & `dlib-19.9.0/dlib/statistics/dpca_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/image_feature_sampling.h` & `dlib-19.9.0/dlib/statistics/image_feature_sampling.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/image_feature_sampling_abstract.h` & `dlib-19.9.0/dlib/statistics/image_feature_sampling_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/lda.h` & `dlib-19.9.0/dlib/statistics/lda.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/lda_abstract.h` & `dlib-19.9.0/dlib/statistics/lda_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/random_subset_selector.h` & `dlib-19.9.0/dlib/statistics/random_subset_selector.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/random_subset_selector_abstract.h` & `dlib-19.9.0/dlib/statistics/random_subset_selector_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/running_gradient.h` & `dlib-19.9.0/dlib/statistics/running_gradient.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/running_gradient_abstract.h` & `dlib-19.9.0/dlib/statistics/running_gradient_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/sammon.h` & `dlib-19.9.0/dlib/statistics/sammon.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/sammon_abstract.h` & `dlib-19.9.0/dlib/statistics/sammon_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/statistics.h` & `dlib-19.9.0/dlib/statistics/statistics.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/statistics_abstract.h` & `dlib-19.9.0/dlib/statistics/statistics_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/vector_normalizer_frobmetric.h` & `dlib-19.9.0/dlib/statistics/vector_normalizer_frobmetric.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics/vector_normalizer_frobmetric_abstract.h` & `dlib-19.9.0/dlib/statistics/vector_normalizer_frobmetric_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/stl_checked/std_vector_c.h` & `dlib-19.9.0/dlib/stl_checked/std_vector_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/stl_checked/std_vector_c_abstract.h` & `dlib-19.9.0/dlib/stl_checked/std_vector_c_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/string/string.h` & `dlib-19.9.0/dlib/string/string.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/string/string_abstract.h` & `dlib-19.9.0/dlib/string/string_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/active_learning.h` & `dlib-19.9.0/dlib/svm/active_learning.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/active_learning_abstract.h` & `dlib-19.9.0/dlib/svm/active_learning_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/assignment_function.h` & `dlib-19.9.0/dlib/svm/assignment_function.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/assignment_function_abstract.h` & `dlib-19.9.0/dlib/svm/assignment_function_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_assignment_trainer.h` & `dlib-19.9.0/dlib/svm/cross_validate_assignment_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_assignment_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/cross_validate_assignment_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_graph_labeling_trainer.h` & `dlib-19.9.0/dlib/svm/cross_validate_graph_labeling_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_graph_labeling_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/cross_validate_graph_labeling_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_multiclass_trainer.h` & `dlib-19.9.0/dlib/svm/cross_validate_multiclass_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_multiclass_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/cross_validate_multiclass_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_object_detection_trainer.h` & `dlib-19.9.0/dlib/svm/cross_validate_object_detection_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_object_detection_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/cross_validate_object_detection_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_regression_trainer.h` & `dlib-19.9.0/dlib/svm/cross_validate_regression_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_regression_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/cross_validate_regression_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_sequence_labeler.h` & `dlib-19.9.0/dlib/svm/cross_validate_sequence_labeler.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_sequence_labeler_abstract.h` & `dlib-19.9.0/dlib/svm/cross_validate_sequence_labeler_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_sequence_segmenter.h` & `dlib-19.9.0/dlib/svm/cross_validate_sequence_segmenter.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_sequence_segmenter_abstract.h` & `dlib-19.9.0/dlib/svm/cross_validate_sequence_segmenter_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_track_association_trainer.h` & `dlib-19.9.0/dlib/svm/cross_validate_track_association_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/cross_validate_track_association_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/cross_validate_track_association_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/empirical_kernel_map.h` & `dlib-19.9.0/dlib/svm/empirical_kernel_map.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/empirical_kernel_map_abstract.h` & `dlib-19.9.0/dlib/svm/empirical_kernel_map_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/feature_ranking.h` & `dlib-19.9.0/dlib/svm/feature_ranking.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/feature_ranking_abstract.h` & `dlib-19.9.0/dlib/svm/feature_ranking_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/function.h` & `dlib-19.9.0/dlib/svm/function.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/function_abstract.h` & `dlib-19.9.0/dlib/svm/function_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/kcentroid.h` & `dlib-19.9.0/dlib/svm/kcentroid.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/kcentroid_abstract.h` & `dlib-19.9.0/dlib/svm/kcentroid_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/kcentroid_overloads.h` & `dlib-19.9.0/dlib/svm/kcentroid_overloads.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/kernel.h` & `dlib-19.9.0/dlib/svm/kernel.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/kernel_abstract.h` & `dlib-19.9.0/dlib/svm/kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/kernel_matrix.h` & `dlib-19.9.0/dlib/svm/kernel_matrix.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/kernel_matrix_abstract.h` & `dlib-19.9.0/dlib/svm/kernel_matrix_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/kkmeans.h` & `dlib-19.9.0/dlib/svm/kkmeans.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/kkmeans_abstract.h` & `dlib-19.9.0/dlib/svm/kkmeans_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/krls.h` & `dlib-19.9.0/dlib/svm/krls.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/krls_abstract.h` & `dlib-19.9.0/dlib/svm/krls_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/krr_trainer.h` & `dlib-19.9.0/dlib/svm/krr_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/krr_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/krr_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/linearly_independent_subset_finder.h` & `dlib-19.9.0/dlib/svm/linearly_independent_subset_finder.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/linearly_independent_subset_finder_abstract.h` & `dlib-19.9.0/dlib/svm/linearly_independent_subset_finder_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/multiclass_tools.h` & `dlib-19.9.0/dlib/svm/multiclass_tools.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/multiclass_tools_abstract.h` & `dlib-19.9.0/dlib/svm/multiclass_tools_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/null_df.h` & `dlib-19.9.0/dlib/svm/null_df.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/null_trainer.h` & `dlib-19.9.0/dlib/svm/null_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/null_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/null_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/num_nonnegative_weights.h` & `dlib-19.9.0/dlib/svm/num_nonnegative_weights.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/one_vs_all_decision_function.h` & `dlib-19.9.0/dlib/svm/one_vs_all_decision_function.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/one_vs_all_decision_function_abstract.h` & `dlib-19.9.0/dlib/svm/one_vs_all_decision_function_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/one_vs_all_trainer.h` & `dlib-19.9.0/dlib/svm/one_vs_all_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/one_vs_all_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/one_vs_all_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/one_vs_one_decision_function.h` & `dlib-19.9.0/dlib/svm/one_vs_one_decision_function.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/one_vs_one_decision_function_abstract.h` & `dlib-19.9.0/dlib/svm/one_vs_one_decision_function_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/one_vs_one_trainer.h` & `dlib-19.9.0/dlib/svm/one_vs_one_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/one_vs_one_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/one_vs_one_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/pegasos.h` & `dlib-19.9.0/dlib/svm/pegasos.h`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         {
         public:
             typedef typename K::scalar_type scalar_type;
             typedef long sample_type;
             //typedef typename K::sample_type sample_type;
             typedef typename K::mem_manager_type mem_manager_type;
 
-            caching_kernel () : samples(0), counter(0), counter_threshold(0) {}
+            caching_kernel () {}
 
             caching_kernel (
                 const K& kern,
                 const sample_vector_type& samps,
                 long cache_size_
             ) : real_kernel(kern), samples(&samps), counter(0)  
             {
@@ -454,20 +454,20 @@
             {
                 matrix<scalar_type> kernel;  
 
                 std::vector<long> sample_location; // where in the cache a sample is.  -1 means not in cache
                 std::vector<std::pair<long,long> > frequency_of_use;  
             };
 
-            const sample_vector_type* samples;
+            const sample_vector_type* samples = 0;
 
             std::shared_ptr<cache_type> cache;
-            mutable unsigned long counter;
-            unsigned long counter_threshold;
-            long cache_size;
+            mutable unsigned long counter = 0;
+            unsigned long counter_threshold = 0;
+            long cache_size = 0;
         };
 
     // ------------------------------------------------------------------------------------
 
     public:
         typedef typename trainer_type::kernel_type kernel_type;
         typedef typename trainer_type::scalar_type scalar_type;
```

### Comparing `dlib-19.8.2/dlib/svm/pegasos_abstract.h` & `dlib-19.9.0/dlib/svm/pegasos_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/ranking_tools.h` & `dlib-19.9.0/dlib/svm/ranking_tools.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/ranking_tools_abstract.h` & `dlib-19.9.0/dlib/svm/ranking_tools_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/rbf_network.h` & `dlib-19.9.0/dlib/svm/rbf_network.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/rbf_network_abstract.h` & `dlib-19.9.0/dlib/svm/rbf_network_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/reduced.h` & `dlib-19.9.0/dlib/svm/reduced.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/reduced_abstract.h` & `dlib-19.9.0/dlib/svm/reduced_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/rls.h` & `dlib-19.9.0/dlib/svm/rls.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/rls_abstract.h` & `dlib-19.9.0/dlib/svm/rls_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/roc_trainer.h` & `dlib-19.9.0/dlib/svm/roc_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/roc_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/roc_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/rr_trainer.h` & `dlib-19.9.0/dlib/svm/rr_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/rr_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/rr_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/rvm.h` & `dlib-19.9.0/dlib/svm/rvm.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/rvm_abstract.h` & `dlib-19.9.0/dlib/svm/rvm_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sequence_labeler.h` & `dlib-19.9.0/dlib/svm/sequence_labeler.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sequence_labeler_abstract.h` & `dlib-19.9.0/dlib/svm/sequence_labeler_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sequence_segmenter.h` & `dlib-19.9.0/dlib/svm/sequence_segmenter.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sequence_segmenter_abstract.h` & `dlib-19.9.0/dlib/svm/sequence_segmenter_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/simplify_linear_decision_function.h` & `dlib-19.9.0/dlib/svm/simplify_linear_decision_function.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/simplify_linear_decision_function_abstract.h` & `dlib-19.9.0/dlib/svm/simplify_linear_decision_function_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sort_basis_vectors.h` & `dlib-19.9.0/dlib/svm/sort_basis_vectors.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sort_basis_vectors_abstract.h` & `dlib-19.9.0/dlib/svm/sort_basis_vectors_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sparse_kernel.h` & `dlib-19.9.0/dlib/svm/sparse_kernel.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sparse_kernel_abstract.h` & `dlib-19.9.0/dlib/svm/sparse_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sparse_vector.h` & `dlib-19.9.0/dlib/svm/sparse_vector.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/sparse_vector_abstract.h` & `dlib-19.9.0/dlib/svm/sparse_vector_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_assignment_trainer.h` & `dlib-19.9.0/dlib/svm/structural_assignment_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_assignment_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/structural_assignment_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_graph_labeling_trainer.h` & `dlib-19.9.0/dlib/svm/structural_graph_labeling_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_graph_labeling_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/structural_graph_labeling_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_object_detection_trainer.h` & `dlib-19.9.0/dlib/svm/structural_object_detection_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_object_detection_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/structural_object_detection_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_sequence_labeling_trainer.h` & `dlib-19.9.0/dlib/svm/structural_sequence_labeling_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_sequence_labeling_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/structural_sequence_labeling_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_sequence_segmentation_trainer.h` & `dlib-19.9.0/dlib/svm/structural_sequence_segmentation_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_sequence_segmentation_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/structural_sequence_segmentation_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_assignment_problem.h` & `dlib-19.9.0/dlib/svm/structural_svm_assignment_problem.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_assignment_problem_abstract.h` & `dlib-19.9.0/dlib/svm/structural_svm_assignment_problem_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_distributed.h` & `dlib-19.9.0/dlib/svm/structural_svm_distributed.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_distributed_abstract.h` & `dlib-19.9.0/dlib/svm/structural_svm_distributed_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_graph_labeling_problem.h` & `dlib-19.9.0/dlib/svm/structural_svm_graph_labeling_problem.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_graph_labeling_problem_abstract.h` & `dlib-19.9.0/dlib/svm/structural_svm_graph_labeling_problem_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_object_detection_problem.h` & `dlib-19.9.0/dlib/svm/structural_svm_object_detection_problem.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_object_detection_problem_abstract.h` & `dlib-19.9.0/dlib/svm/structural_svm_object_detection_problem_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_problem.h` & `dlib-19.9.0/dlib/svm/structural_svm_problem.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_problem_abstract.h` & `dlib-19.9.0/dlib/svm/structural_svm_problem_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_problem_threaded.h` & `dlib-19.9.0/dlib/svm/structural_svm_problem_threaded.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_problem_threaded_abstract.h` & `dlib-19.9.0/dlib/svm/structural_svm_problem_threaded_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_sequence_labeling_problem.h` & `dlib-19.9.0/dlib/svm/structural_svm_sequence_labeling_problem.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_svm_sequence_labeling_problem_abstract.h` & `dlib-19.9.0/dlib/svm/structural_svm_sequence_labeling_problem_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_track_association_trainer.h` & `dlib-19.9.0/dlib/svm/structural_track_association_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/structural_track_association_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/structural_track_association_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm.h` & `dlib-19.9.0/dlib/svm/svm.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_abstract.h` & `dlib-19.9.0/dlib/svm/svm_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_c_ekm_trainer.h` & `dlib-19.9.0/dlib/svm/svm_c_ekm_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_c_ekm_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svm_c_ekm_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_c_linear_dcd_trainer.h` & `dlib-19.9.0/dlib/svm/svm_c_linear_dcd_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_c_linear_dcd_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svm_c_linear_dcd_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_c_linear_trainer.h` & `dlib-19.9.0/dlib/svm/svm_c_linear_trainer.h`

 * *Files 1% similar despite different names*

```diff
@@ -688,15 +688,15 @@
         oca solver;
         scalar_type eps;
         bool verbose;
         unsigned long max_iterations;
         bool learn_nonnegative_weights;
         bool last_weight_1;
         matrix<scalar_type,0,1> prior;
-        scalar_type prior_b;
+        scalar_type prior_b = 0;
     }; 
 
 // ----------------------------------------------------------------------------------------
 
 }
 
 // ----------------------------------------------------------------------------------------
```

### Comparing `dlib-19.8.2/dlib/svm/svm_c_linear_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svm_c_linear_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_c_trainer.h` & `dlib-19.9.0/dlib/svm/svm_c_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_c_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svm_c_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_multiclass_linear_trainer.h` & `dlib-19.9.0/dlib/svm/svm_multiclass_linear_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_multiclass_linear_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svm_multiclass_linear_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_nu_trainer.h` & `dlib-19.9.0/dlib/svm/svm_nu_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_nu_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svm_nu_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_one_class_trainer.h` & `dlib-19.9.0/dlib/svm/svm_one_class_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_one_class_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svm_one_class_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_rank_trainer.h` & `dlib-19.9.0/dlib/svm/svm_rank_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_rank_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svm_rank_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_threaded.h` & `dlib-19.9.0/dlib/svm/svm_threaded.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svm_threaded_abstract.h` & `dlib-19.9.0/dlib/svm/svm_threaded_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svr_linear_trainer.h` & `dlib-19.9.0/dlib/svm/svr_linear_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svr_linear_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svr_linear_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svr_trainer.h` & `dlib-19.9.0/dlib/svm/svr_trainer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/svr_trainer_abstract.h` & `dlib-19.9.0/dlib/svm/svr_trainer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/track_association_function.h` & `dlib-19.9.0/dlib/svm/track_association_function.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm/track_association_function_abstract.h` & `dlib-19.9.0/dlib/svm/track_association_function_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sync_extension/sync_extension_kernel_1.h` & `dlib-19.9.0/dlib/sync_extension/sync_extension_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sync_extension/sync_extension_kernel_abstract.h` & `dlib-19.9.0/dlib/sync_extension/sync_extension_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/blas_bindings/CMakeLists.txt` & `dlib-19.9.0/dlib/test/blas_bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_dot.cpp` & `dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_dot.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_gemm.cpp` & `dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_gemm.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_gemv.cpp` & `dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_gemv.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_ger.cpp` & `dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_ger.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/blas_bindings/blas_bindings_scal_axpy.cpp` & `dlib-19.9.0/dlib/test/blas_bindings/blas_bindings_scal_axpy.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/blas_bindings/vector.cpp` & `dlib-19.9.0/dlib/test/blas_bindings/vector.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/gui/CMakeLists.txt` & `dlib-19.9.0/dlib/test/gui/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/gui/main.cpp` & `dlib-19.9.0/dlib/test/gui/main.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/CMakeLists.txt` & `dlib-19.9.0/dlib/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/WINDOWS_build_and_run_all_unit_tests.bat` & `dlib-19.9.0/dlib/test/WINDOWS_build_and_run_all_unit_tests.bat`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/active_learning.cpp` & `dlib-19.9.0/dlib/test/active_learning.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/any.cpp` & `dlib-19.9.0/dlib/test/any.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/any_function.cpp` & `dlib-19.9.0/dlib/test/any_function.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/array.cpp` & `dlib-19.9.0/dlib/test/array.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/array2d.cpp` & `dlib-19.9.0/dlib/test/array2d.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/assignment_learning.cpp` & `dlib-19.9.0/dlib/test/assignment_learning.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/base64.cpp` & `dlib-19.9.0/dlib/test/base64.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/bayes_nets.cpp` & `dlib-19.9.0/dlib/test/bayes_nets.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/bigint.cpp` & `dlib-19.9.0/dlib/test/bigint.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/binary_search_tree.h` & `dlib-19.9.0/dlib/test/binary_search_tree.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/binary_search_tree_kernel_1a.cpp` & `dlib-19.9.0/dlib/test/binary_search_tree_kernel_1a.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/binary_search_tree_kernel_2a.cpp` & `dlib-19.9.0/dlib/test/binary_search_tree_kernel_2a.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/binary_search_tree_mm1.cpp` & `dlib-19.9.0/dlib/test/binary_search_tree_mm1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/binary_search_tree_mm2.cpp` & `dlib-19.9.0/dlib/test/binary_search_tree_mm2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/bridge.cpp` & `dlib-19.9.0/dlib/test/bridge.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/bsp.cpp` & `dlib-19.9.0/dlib/test/bsp.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/byte_orderer.cpp` & `dlib-19.9.0/dlib/test/byte_orderer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/cca.cpp` & `dlib-19.9.0/dlib/test/cca.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 // Copyright (C) 2013  Davis E. King (davis@dlib.net)
 // License: Boost Software License   See LICENSE.txt for the full license.
 
 #include <dlib/statistics.h>
 #include <dlib/sparse_vector.h>
+#include <dlib/timing.h>
 #include <map>
 
 #include "tester.h"
 
 namespace  
 {
     using namespace test;
@@ -370,26 +371,80 @@
         test_svd_fast(1, 2, 2);
         test_svd_fast(1, 1, 2);
         test_svd_fast(1, 2, 1);
     }
 
 // ----------------------------------------------------------------------------------------
 
+    /*
+    typedef std::vector<std::pair<unsigned int, float>> sv;
+    sv rand_sparse_vector()
+    {
+        static dlib::rand rnd;
+        sv v;
+        for (int i = 0; i < 50; ++i)
+            v.push_back(make_pair(rnd.get_integer(400000), rnd.get_random_gaussian()*100));
+
+        make_sparse_vector_inplace(v);
+        return v;
+    }
+
+    sv rand_basis_combo(const std::vector<sv>& basis)
+    {
+        static dlib::rand rnd;
+        sv result;
+
+        for (int i = 0; i < 5; ++i)
+        {
+            sv temp = basis[rnd.get_integer(basis.size())];
+            scale_by(temp, rnd.get_random_gaussian());
+            result = add(result,temp);
+        }
+        return result;
+    }
+
+    void big_sparse_speed_test()
+    {
+        cout << "making A" << endl;
+        std::vector<sv> basis;
+        for (int i = 0; i < 100; ++i)
+            basis.emplace_back(rand_sparse_vector());
+
+        std::vector<sv> A;
+        for (int i = 0; i < 500000; ++i)
+            A.emplace_back(rand_basis_combo(basis));
+
+        cout << "done making A" << endl;
+
+        matrix<float> u,v;
+        matrix<float,0,1> w;
+        {
+        timing::block aosijdf(0,"call it");
+        svd_fast(A, u,w,v, 100, 5);
+        }
+
+        timing::print();
+    }
+    */
+
+// ----------------------------------------------------------------------------------------
+
     class test_cca : public tester
     {
     public:
         test_cca (
         ) :
             tester ("test_cca",
                 "Runs tests on the cca() and svd_fast() routines.")
         {}
 
         void perform_test (
         )
         {
+            //big_sparse_speed_test();
             for (int i = 0; i < 200; ++i)
             {
                 test_cca1();
                 test_cca2();
                 test_cca3();
             }
             test_svd_fast();
```

### Comparing `dlib-19.8.2/dlib/test/checkerboard.h` & `dlib-19.9.0/dlib/test/checkerboard.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/clustering.cpp` & `dlib-19.9.0/dlib/test/clustering.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/cmd_line_parser.cpp` & `dlib-19.9.0/dlib/test/cmd_line_parser.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/cmd_line_parser.h` & `dlib-19.9.0/dlib/test/cmd_line_parser.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/cmd_line_parser_wchar_t.cpp` & `dlib-19.9.0/dlib/test/cmd_line_parser_wchar_t.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/compress_stream.cpp` & `dlib-19.9.0/dlib/test/compress_stream.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/conditioning_class.cpp` & `dlib-19.9.0/dlib/test/conditioning_class.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/conditioning_class.h` & `dlib-19.9.0/dlib/test/conditioning_class.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/conditioning_class_c.cpp` & `dlib-19.9.0/dlib/test/conditioning_class_c.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/config_reader.cpp` & `dlib-19.9.0/dlib/test/config_reader.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/correlation_tracker.cpp` & `dlib-19.9.0/dlib/test/correlation_tracker.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/crc32.cpp` & `dlib-19.9.0/dlib/test/crc32.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/create_iris_datafile.cpp` & `dlib-19.9.0/dlib/test/create_iris_datafile.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/create_iris_datafile.h` & `dlib-19.9.0/dlib/test/create_iris_datafile.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/cublas.cpp` & `dlib-19.9.0/dlib/test/cublas.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/data_io.cpp` & `dlib-19.9.0/dlib/test/data_io.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/directed_graph.cpp` & `dlib-19.9.0/dlib/test/directed_graph.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/discriminant_pca.cpp` & `dlib-19.9.0/dlib/test/discriminant_pca.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/disjoint_subsets.cpp` & `dlib-19.9.0/dlib/test/disjoint_subsets.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/disjoint_subsets_sized.cpp` & `dlib-19.9.0/dlib/test/disjoint_subsets_sized.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/dnn.cpp` & `dlib-19.9.0/dlib/test/dnn.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/ekm_and_lisf.cpp` & `dlib-19.9.0/dlib/test/ekm_and_lisf.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/elastic_net.cpp` & `dlib-19.9.0/dlib/test/elastic_net.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/empirical_kernel_map.cpp` & `dlib-19.9.0/dlib/test/empirical_kernel_map.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/entropy_coder.cpp` & `dlib-19.9.0/dlib/test/entropy_coder.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/entropy_encoder_model.cpp` & `dlib-19.9.0/dlib/test/entropy_encoder_model.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/example.cpp` & `dlib-19.9.0/dlib/test/example.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/example_args.cpp` & `dlib-19.9.0/dlib/test/example_args.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/face.cpp` & `dlib-19.9.0/dlib/test/face.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/fft.cpp` & `dlib-19.9.0/dlib/test/fft.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/fhog.cpp` & `dlib-19.9.0/dlib/test/fhog.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/filtering.cpp` & `dlib-19.9.0/dlib/test/filtering.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/find_max_factor_graph_nmplp.cpp` & `dlib-19.9.0/dlib/test/find_max_factor_graph_nmplp.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/find_max_factor_graph_viterbi.cpp` & `dlib-19.9.0/dlib/test/find_max_factor_graph_viterbi.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/find_optimal_parameters.cpp` & `dlib-19.9.0/dlib/test/find_optimal_parameters.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/geometry.cpp` & `dlib-19.9.0/dlib/test/geometry.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/global_optimization.cpp` & `dlib-19.9.0/dlib/test/global_optimization.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/graph.cpp` & `dlib-19.9.0/dlib/test/graph.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/graph_cuts.cpp` & `dlib-19.9.0/dlib/test/graph_cuts.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/graph_labeler.cpp` & `dlib-19.9.0/dlib/test/graph_labeler.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/hash.cpp` & `dlib-19.9.0/dlib/test/hash.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/hash_map.cpp` & `dlib-19.9.0/dlib/test/hash_map.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/hash_set.cpp` & `dlib-19.9.0/dlib/test/hash_set.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/hash_table.cpp` & `dlib-19.9.0/dlib/test/hash_table.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/hog_image.cpp` & `dlib-19.9.0/dlib/test/hog_image.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/image.cpp` & `dlib-19.9.0/dlib/test/image.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/iosockstream.cpp` & `dlib-19.9.0/dlib/test/iosockstream.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/is_same_object.cpp` & `dlib-19.9.0/dlib/test/is_same_object.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/kcentroid.cpp` & `dlib-19.9.0/dlib/test/kcentroid.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/kernel_matrix.cpp` & `dlib-19.9.0/dlib/test/kernel_matrix.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/kmeans.cpp` & `dlib-19.9.0/dlib/test/kmeans.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/learning_to_track.cpp` & `dlib-19.9.0/dlib/test/learning_to_track.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/least_squares.cpp` & `dlib-19.9.0/dlib/test/least_squares.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/linear_manifold_regularizer.cpp` & `dlib-19.9.0/dlib/test/linear_manifold_regularizer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/lspi.cpp` & `dlib-19.9.0/dlib/test/lspi.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/lz77_buffer.cpp` & `dlib-19.9.0/dlib/test/lz77_buffer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/main.cpp` & `dlib-19.9.0/dlib/test/main.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/makefile` & `dlib-19.9.0/dlib/test/makefile`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/map.cpp` & `dlib-19.9.0/dlib/test/map.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/matrix.cpp` & `dlib-19.9.0/dlib/test/matrix.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1467,32 +1467,32 @@
         {
             matrix<double,0,0,default_memory_manager,column_major_layout> a(3,3);
             matrix<double,0,0,default_memory_manager,column_major_layout> m = randm(3,3);
             matrix<double,0,0,default_memory_manager,column_major_layout> b = randm(3,1);
 
             a = 0;
             set_colm(a,0) = m*b;
-            DLIB_TEST(colm(a,0) == m*b);
+            DLIB_TEST(equal(colm(a,0) , m*b));
             a = 0;
             set_rowm(a,0) = trans(m*b);
-            DLIB_TEST(rowm(a,0) == trans(m*b));
-            DLIB_TEST(rowm(a,0) != m*b);
+            DLIB_TEST(equal(rowm(a,0) , trans(m*b)));
+            DLIB_TEST(!equal(rowm(a,0) , m*b));
         }
         {
             matrix<double> a(3,3);
             matrix<double> m = randm(3,3);
             matrix<double> b = randm(3,1);
 
             a = 0;
             set_colm(a,0) = m*b;
-            DLIB_TEST(colm(a,0) == m*b);
+            DLIB_TEST(equal(colm(a,0) , m*b));
             a = 0;
             set_rowm(a,0) = trans(m*b);
-            DLIB_TEST(rowm(a,0) == trans(m*b));
-            DLIB_TEST(rowm(a,0) != m*b);
+            DLIB_TEST(equal(rowm(a,0) , trans(m*b)));
+            DLIB_TEST(!equal(rowm(a,0) , m*b));
         }
     }
```

### Comparing `dlib-19.8.2/dlib/test/matrix2.cpp` & `dlib-19.9.0/dlib/test/matrix2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/matrix3.cpp` & `dlib-19.9.0/dlib/test/matrix3.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/matrix4.cpp` & `dlib-19.9.0/dlib/test/matrix4.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/matrix_chol.cpp` & `dlib-19.9.0/dlib/test/matrix_chol.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/matrix_eig.cpp` & `dlib-19.9.0/dlib/test/matrix_eig.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/matrix_lu.cpp` & `dlib-19.9.0/dlib/test/matrix_lu.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/matrix_qr.cpp` & `dlib-19.9.0/dlib/test/matrix_qr.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/max_cost_assignment.cpp` & `dlib-19.9.0/dlib/test/max_cost_assignment.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/max_sum_submatrix.cpp` & `dlib-19.9.0/dlib/test/max_sum_submatrix.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/md5.cpp` & `dlib-19.9.0/dlib/test/md5.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/member_function_pointer.cpp` & `dlib-19.9.0/dlib/test/member_function_pointer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/metaprogramming.cpp` & `dlib-19.9.0/dlib/test/metaprogramming.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/mpc.cpp` & `dlib-19.9.0/dlib/test/mpc.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/multithreaded_object.cpp` & `dlib-19.9.0/dlib/test/multithreaded_object.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/numerical_integration.cpp` & `dlib-19.9.0/dlib/test/numerical_integration.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/object_detector.cpp` & `dlib-19.9.0/dlib/test/object_detector.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/oca.cpp` & `dlib-19.9.0/dlib/test/oca.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/one_vs_all_trainer.cpp` & `dlib-19.9.0/dlib/test/one_vs_all_trainer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/one_vs_one_trainer.cpp` & `dlib-19.9.0/dlib/test/one_vs_one_trainer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/opt_qp_solver.cpp` & `dlib-19.9.0/dlib/test/opt_qp_solver.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/optimization.cpp` & `dlib-19.9.0/dlib/test/optimization.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/optimization_test_functions.cpp` & `dlib-19.9.0/dlib/test/optimization_test_functions.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/optimization_test_functions.h` & `dlib-19.9.0/dlib/test/optimization_test_functions.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/parallel_for.cpp` & `dlib-19.9.0/dlib/test/parallel_for.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/parse.cpp` & `dlib-19.9.0/dlib/test/parse.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/pipe.cpp` & `dlib-19.9.0/dlib/test/pipe.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/pixel.cpp` & `dlib-19.9.0/dlib/test/pixel.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/probabilistic.cpp` & `dlib-19.9.0/dlib/test/probabilistic.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/pyramid_down.cpp` & `dlib-19.9.0/dlib/test/pyramid_down.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/queue.cpp` & `dlib-19.9.0/dlib/test/queue.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/rand.cpp` & `dlib-19.9.0/dlib/test/rand.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/ranking.cpp` & `dlib-19.9.0/dlib/test/ranking.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/read_write_mutex.cpp` & `dlib-19.9.0/dlib/test/read_write_mutex.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/reference_counter.cpp` & `dlib-19.9.0/dlib/test/reference_counter.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/rls.cpp` & `dlib-19.9.0/dlib/test/rls.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sammon.cpp` & `dlib-19.9.0/dlib/test/sammon.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/scan_image.cpp` & `dlib-19.9.0/dlib/test/scan_image.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sequence.cpp` & `dlib-19.9.0/dlib/test/sequence.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sequence_labeler.cpp` & `dlib-19.9.0/dlib/test/sequence_labeler.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sequence_segmenter.cpp` & `dlib-19.9.0/dlib/test/sequence_segmenter.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/serialize.cpp` & `dlib-19.9.0/dlib/test/serialize.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/set.cpp` & `dlib-19.9.0/dlib/test/set.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sldf.cpp` & `dlib-19.9.0/dlib/test/sldf.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sliding_buffer.cpp` & `dlib-19.9.0/dlib/test/sliding_buffer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/smart_pointers.cpp` & `dlib-19.9.0/dlib/test/smart_pointers.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sockets.cpp` & `dlib-19.9.0/dlib/test/sockets.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sockets2.cpp` & `dlib-19.9.0/dlib/test/sockets2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sockstreambuf.cpp` & `dlib-19.9.0/dlib/test/sockstreambuf.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/sparse_vector.cpp` & `dlib-19.9.0/dlib/test/sparse_vector.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/stack.cpp` & `dlib-19.9.0/dlib/test/stack.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/static_map.cpp` & `dlib-19.9.0/dlib/test/static_map.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/static_set.cpp` & `dlib-19.9.0/dlib/test/static_set.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/statistics.cpp` & `dlib-19.9.0/dlib/test/statistics.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/std_vector_c.cpp` & `dlib-19.9.0/dlib/test/std_vector_c.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/string.cpp` & `dlib-19.9.0/dlib/test/string.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/svm.cpp` & `dlib-19.9.0/dlib/test/svm.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/svm_c_linear.cpp` & `dlib-19.9.0/dlib/test/svm_c_linear.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/svm_c_linear_dcd.cpp` & `dlib-19.9.0/dlib/test/svm_c_linear_dcd.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/svm_multiclass_linear.cpp` & `dlib-19.9.0/dlib/test/svm_multiclass_linear.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/svm_struct.cpp` & `dlib-19.9.0/dlib/test/svm_struct.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/svr_linear_trainer.cpp` & `dlib-19.9.0/dlib/test/svr_linear_trainer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/symmetric_matrix_cache.cpp` & `dlib-19.9.0/dlib/test/symmetric_matrix_cache.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/tester.cpp` & `dlib-19.9.0/dlib/test/tester.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/tester.h` & `dlib-19.9.0/dlib/test/tester.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/thread_pool.cpp` & `dlib-19.9.0/dlib/test/thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/threads.cpp` & `dlib-19.9.0/dlib/test/threads.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/timer.cpp` & `dlib-19.9.0/dlib/test/timer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/tokenizer.cpp` & `dlib-19.9.0/dlib/test/tokenizer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/trust_region.cpp` & `dlib-19.9.0/dlib/test/trust_region.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/tuple.cpp` & `dlib-19.9.0/dlib/test/tuple.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/type_safe_union.cpp` & `dlib-19.9.0/dlib/test/type_safe_union.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/test/vectorstream.cpp` & `dlib-19.9.0/dlib/test/vectorstream.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/async.cpp` & `dlib-19.9.0/dlib/threads/async.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/async.h` & `dlib-19.9.0/dlib/threads/async.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/async_abstract.h` & `dlib-19.9.0/dlib/threads/async_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/auto_mutex_extension.h` & `dlib-19.9.0/dlib/threads/auto_mutex_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/auto_mutex_extension_abstract.h` & `dlib-19.9.0/dlib/threads/auto_mutex_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/auto_unlock_extension.h` & `dlib-19.9.0/dlib/threads/auto_unlock_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/auto_unlock_extension_abstract.h` & `dlib-19.9.0/dlib/threads/auto_unlock_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/create_new_thread_extension.h` & `dlib-19.9.0/dlib/threads/create_new_thread_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/create_new_thread_extension_abstract.h` & `dlib-19.9.0/dlib/threads/create_new_thread_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/multithreaded_object_extension.cpp` & `dlib-19.9.0/dlib/threads/multithreaded_object_extension.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/multithreaded_object_extension.h` & `dlib-19.9.0/dlib/threads/multithreaded_object_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/multithreaded_object_extension_abstract.h` & `dlib-19.9.0/dlib/threads/multithreaded_object_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/parallel_for_extension.h` & `dlib-19.9.0/dlib/threads/parallel_for_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/parallel_for_extension_abstract.h` & `dlib-19.9.0/dlib/threads/parallel_for_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/read_write_mutex_extension.h` & `dlib-19.9.0/dlib/threads/read_write_mutex_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/read_write_mutex_extension_abstract.h` & `dlib-19.9.0/dlib/threads/read_write_mutex_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/rmutex_extension.h` & `dlib-19.9.0/dlib/threads/rmutex_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/rmutex_extension_abstract.h` & `dlib-19.9.0/dlib/threads/rmutex_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/rsignaler_extension.h` & `dlib-19.9.0/dlib/threads/rsignaler_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/rsignaler_extension_abstract.h` & `dlib-19.9.0/dlib/threads/rsignaler_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/thread_function_extension.h` & `dlib-19.9.0/dlib/threads/thread_function_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/thread_function_extension_abstract.h` & `dlib-19.9.0/dlib/threads/thread_function_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/thread_pool_extension.cpp` & `dlib-19.9.0/dlib/threads/thread_pool_extension.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/thread_pool_extension.h` & `dlib-19.9.0/dlib/threads/thread_pool_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/thread_pool_extension_abstract.h` & `dlib-19.9.0/dlib/threads/thread_pool_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/thread_specific_data_extension.h` & `dlib-19.9.0/dlib/threads/thread_specific_data_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/thread_specific_data_extension_abstract.h` & `dlib-19.9.0/dlib/threads/thread_specific_data_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threaded_object_extension.cpp` & `dlib-19.9.0/dlib/threads/threaded_object_extension.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threaded_object_extension.h` & `dlib-19.9.0/dlib/threads/threaded_object_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threaded_object_extension_abstract.h` & `dlib-19.9.0/dlib/threads/threaded_object_extension_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threads_kernel_1.cpp` & `dlib-19.9.0/dlib/threads/threads_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threads_kernel_1.h` & `dlib-19.9.0/dlib/threads/threads_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threads_kernel_2.cpp` & `dlib-19.9.0/dlib/threads/threads_kernel_2.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threads_kernel_2.h` & `dlib-19.9.0/dlib/threads/threads_kernel_2.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threads_kernel_abstract.h` & `dlib-19.9.0/dlib/threads/threads_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threads_kernel_shared.cpp` & `dlib-19.9.0/dlib/threads/threads_kernel_shared.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads/threads_kernel_shared.h` & `dlib-19.9.0/dlib/threads/threads_kernel_shared.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/timeout/timeout.h` & `dlib-19.9.0/dlib/timeout/timeout.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/timeout/timeout_abstract.h` & `dlib-19.9.0/dlib/timeout/timeout_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/timer/timer.cpp` & `dlib-19.9.0/dlib/timer/timer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/timer/timer.h` & `dlib-19.9.0/dlib/timer/timer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/timer/timer_abstract.h` & `dlib-19.9.0/dlib/timer/timer_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/timer/timer_heavy.h` & `dlib-19.9.0/dlib/timer/timer_heavy.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/tokenizer/tokenizer_kernel_1.cpp` & `dlib-19.9.0/dlib/tokenizer/tokenizer_kernel_1.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/tokenizer/tokenizer_kernel_1.h` & `dlib-19.9.0/dlib/tokenizer/tokenizer_kernel_1.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/tokenizer/tokenizer_kernel_abstract.h` & `dlib-19.9.0/dlib/tokenizer/tokenizer_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/tokenizer/tokenizer_kernel_c.h` & `dlib-19.9.0/dlib/tokenizer/tokenizer_kernel_c.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/tuple/tuple.h` & `dlib-19.9.0/dlib/tuple/tuple.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/tuple/tuple_abstract.h` & `dlib-19.9.0/dlib/tuple/tuple_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/type_safe_union/type_safe_union_kernel.h` & `dlib-19.9.0/dlib/type_safe_union/type_safe_union_kernel.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/type_safe_union/type_safe_union_kernel_abstract.h` & `dlib-19.9.0/dlib/type_safe_union/type_safe_union_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/unicode/unicode.cpp` & `dlib-19.9.0/dlib/unicode/unicode.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/unicode/unicode.h` & `dlib-19.9.0/dlib/unicode/unicode.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/unicode/unicode_abstract.h` & `dlib-19.9.0/dlib/unicode/unicode_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/vectorstream/unserialize.h` & `dlib-19.9.0/dlib/vectorstream/unserialize.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/vectorstream/unserialize_abstract.h` & `dlib-19.9.0/dlib/vectorstream/unserialize_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/vectorstream/vectorstream.h` & `dlib-19.9.0/dlib/vectorstream/vectorstream.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/vectorstream/vectorstream_abstract.h` & `dlib-19.9.0/dlib/vectorstream/vectorstream_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/xml_parser/xml_parser_kernel_1.h` & `dlib-19.9.0/dlib/xml_parser/xml_parser_kernel_1.h`

 * *Files 0% similar despite different names*

```diff
@@ -353,14 +353,15 @@
                 bool is_empty = false;  // this becomes true when this token is an empty_element
 
                 switch (token_kind)
                 {
 
 
                 case empty_element: is_empty = true;
+                                    // fall through
                 case element_start:
                     {
                         seen_root_tag = true;
 
                         int status = parse_element(token_text,name,atts);
                         // if there was no error parsing the element
                         if (status == 0)
```

### Comparing `dlib-19.8.2/dlib/xml_parser/xml_parser_kernel_abstract.h` & `dlib-19.9.0/dlib/xml_parser/xml_parser_kernel_abstract.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/xml_parser/xml_parser_kernel_interfaces.h` & `dlib-19.9.0/dlib/xml_parser/xml_parser_kernel_interfaces.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/CMakeLists.txt` & `dlib-19.9.0/dlib/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 # default to a Release build (except if CMAKE_BUILD_TYPE is set)
 include(cmake_utils/release_build_by_default)
 include(cmake_utils/use_cpp_11.cmake)
 
 
 set(CPACK_PACKAGE_VERSION_MAJOR "19")
-set(CPACK_PACKAGE_VERSION_MINOR "8")
-set(CPACK_PACKAGE_VERSION_PATCH "2")
+set(CPACK_PACKAGE_VERSION_MINOR "9")
+set(CPACK_PACKAGE_VERSION_PATCH "0")
 set(VERSION ${CPACK_PACKAGE_VERSION_MAJOR}.${CPACK_PACKAGE_VERSION_MINOR}.${CPACK_PACKAGE_VERSION_PATCH})
 # Set DLIB_VERSION in the including CMake file so they can use it to do whatever they want. 
 get_directory_property(has_parent PARENT_DIRECTORY)
 if(has_parent)
    set(DLIB_VERSION ${VERSION} PARENT_SCOPE)
    if (NOT DEFINED DLIB_IN_PROJECT_BUILD)
       set(DLIB_IN_PROJECT_BUILD true)
```

### Comparing `dlib-19.8.2/dlib/LICENSE.txt` & `dlib-19.9.0/dlib/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/algs.h` & `dlib-19.9.0/dlib/algs.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/assert.h` & `dlib-19.9.0/dlib/assert.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bigint.h` & `dlib-19.9.0/dlib/bigint.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/binary_search_tree.h` & `dlib-19.9.0/dlib/binary_search_tree.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/bit_stream.h` & `dlib-19.9.0/dlib/bit_stream.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cmd_line_parser.h` & `dlib-19.9.0/dlib/cmd_line_parser.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/compress_stream.h` & `dlib-19.9.0/dlib/compress_stream.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/conditioning_class.h` & `dlib-19.9.0/dlib/conditioning_class.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/config.h` & `dlib-19.9.0/dlib/config.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/config.h.in` & `dlib-19.9.0/dlib/config.h.in`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/config_reader.h` & `dlib-19.9.0/dlib/config_reader.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/console_progress_indicator.h` & `dlib-19.9.0/dlib/console_progress_indicator.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cpp_pretty_printer.h` & `dlib-19.9.0/dlib/cpp_pretty_printer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/cpp_tokenizer.h` & `dlib-19.9.0/dlib/cpp_tokenizer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/directed_graph.h` & `dlib-19.9.0/dlib/directed_graph.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dlib_basic_cpp_build_tutorial.txt` & `dlib-19.9.0/dlib/dlib_basic_cpp_build_tutorial.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dlib_include_path_tutorial.txt` & `dlib-19.9.0/dlib/dlib_include_path_tutorial.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/dnn.h` & `dlib-19.9.0/dlib/dnn.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/enable_if.h` & `dlib-19.9.0/dlib/enable_if.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder.h` & `dlib-19.9.0/dlib/entropy_decoder.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_decoder_model.h` & `dlib-19.9.0/dlib/entropy_decoder_model.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder.h` & `dlib-19.9.0/dlib/entropy_encoder.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/entropy_encoder_model.h` & `dlib-19.9.0/dlib/entropy_encoder_model.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/error.h` & `dlib-19.9.0/dlib/error.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/float_details.h` & `dlib-19.9.0/dlib/float_details.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/graph.h` & `dlib-19.9.0/dlib/graph.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_map.h` & `dlib-19.9.0/dlib/hash_map.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_set.h` & `dlib-19.9.0/dlib/hash_set.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/hash_table.h` & `dlib-19.9.0/dlib/hash_table.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_io.h` & `dlib-19.9.0/dlib/image_io.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_keypoint.h` & `dlib-19.9.0/dlib/image_keypoint.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_processing.h` & `dlib-19.9.0/dlib/image_processing.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/image_transforms.h` & `dlib-19.9.0/dlib/image_transforms.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/is_kind.h` & `dlib-19.9.0/dlib/is_kind.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lz77_buffer.h` & `dlib-19.9.0/dlib/lz77_buffer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/lzp_buffer.h` & `dlib-19.9.0/dlib/lzp_buffer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/map.h` & `dlib-19.9.0/dlib/map.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/matrix.h` & `dlib-19.9.0/dlib/matrix.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager.h` & `dlib-19.9.0/dlib/memory_manager.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager_global.h` & `dlib-19.9.0/dlib/memory_manager_global.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/memory_manager_stateless.h` & `dlib-19.9.0/dlib/memory_manager_stateless.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/metaprogramming.h` & `dlib-19.9.0/dlib/metaprogramming.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/mlp.h` & `dlib-19.9.0/dlib/mlp.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/noncopyable.h` & `dlib-19.9.0/dlib/noncopyable.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/numeric_constants.h` & `dlib-19.9.0/dlib/numeric_constants.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/optimization.h` & `dlib-19.9.0/dlib/optimization.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/pixel.h` & `dlib-19.9.0/dlib/pixel.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/platform.h` & `dlib-19.9.0/dlib/platform.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/queue.h` & `dlib-19.9.0/dlib/queue.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/ref.h` & `dlib-19.9.0/dlib/ref.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/reference_counter.h` & `dlib-19.9.0/dlib/reference_counter.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sequence.h` & `dlib-19.9.0/dlib/sequence.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/serialize.h` & `dlib-19.9.0/dlib/serialize.h`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
             if (size&0x80)
                 is_negative = true;
             else
                 is_negative = false;
             size &= 0x0F;
             
             // check if the serialized object is too big
-            if (size > sizeof(T))
+            if (size > (unsigned long)tmin<sizeof(T),8>::value || size == 0)
             {
                 return true;
             }
 
             if (sbuf->sgetn(reinterpret_cast<char*>(&buf),size) != size)
             {
                 in.setstate(std::ios::badbit);
@@ -387,15 +387,15 @@
             }
 
 
             // mask out the 3 reserved bits
             size &= 0x8F;
 
             // check if an error occurred 
-            if (size > sizeof(T)) 
+            if (size > (unsigned long)tmin<sizeof(T),8>::value || size == 0)
                 return true;
            
 
             if (sbuf->sgetn(reinterpret_cast<char*>(&buf),size) != size)
             {
                 in.setstate(std::ios::badbit);
                 return true;
```

### Comparing `dlib-19.8.2/dlib/set.h` & `dlib-19.9.0/dlib/set.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sliding_buffer.h` & `dlib-19.9.0/dlib/sliding_buffer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/smart_pointers.h` & `dlib-19.9.0/dlib/smart_pointers.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/smart_pointers_thread_safe.h` & `dlib-19.9.0/dlib/smart_pointers_thread_safe.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sort.h` & `dlib-19.9.0/dlib/sort.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/stack.h` & `dlib-19.9.0/dlib/stack.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/stack_trace.cpp` & `dlib-19.9.0/dlib/stack_trace.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/stack_trace.h` & `dlib-19.9.0/dlib/stack_trace.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_map.h` & `dlib-19.9.0/dlib/static_map.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/static_set.h` & `dlib-19.9.0/dlib/static_set.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/statistics.h` & `dlib-19.9.0/dlib/statistics.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/std_allocator.h` & `dlib-19.9.0/dlib/std_allocator.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm.h` & `dlib-19.9.0/dlib/svm.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/svm_threaded.h` & `dlib-19.9.0/dlib/svm_threaded.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/sync_extension.h` & `dlib-19.9.0/dlib/sync_extension.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/threads.h` & `dlib-19.9.0/dlib/threads.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/time_this.h` & `dlib-19.9.0/dlib/time_this.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/timing.h` & `dlib-19.9.0/dlib/timing.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/tokenizer.h` & `dlib-19.9.0/dlib/tokenizer.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/uintn.h` & `dlib-19.9.0/dlib/uintn.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/unordered_pair.h` & `dlib-19.9.0/dlib/unordered_pair.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib/windows_magic.h` & `dlib-19.9.0/dlib/windows_magic.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/dlib.egg-info/PKG-INFO` & `dlib-19.9.0/dlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dlib
-Version: 19.8.2
+Version: 19.9.0
 Summary: A toolkit for making real world machine learning and data analysis applications
 Home-page: https://github.com/davisking/dlib
 Author: Davis King
 Author-email: davis@dlib.net
 License: Boost Software License
 Description: # dlib C++ library [![Travis Status](https://travis-ci.org/davisking/dlib.svg?branch=master)](https://travis-ci.org/davisking/dlib)
```

### Comparing `dlib-19.8.2/dlib.egg-info/SOURCES.txt` & `dlib-19.9.0/dlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/python_examples/LICENSE_FOR_EXAMPLE_PROGRAMS.txt` & `dlib-19.9.0/python_examples/LICENSE_FOR_EXAMPLE_PROGRAMS.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/python_examples/cnn_face_detector.py` & `dlib-19.9.0/python_examples/cnn_face_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS --yes DLIB_USE_CUDA
 #   if you have a CPU that supports AVX instructions, you have an Nvidia GPU
 #   and you have CUDA installed since this makes things run *much* faster.
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires scikit-image which can be installed
 #   via the command:
 #       pip install scikit-image
 #   Or downloaded from http://scikit-image.org/download.html.
 
 import sys
@@ -78,8 +78,8 @@
 
     rects = dlib.rectangles()
     rects.extend([d.rect for d in dets])
 
     win.clear_overlay()
     win.set_image(img)
     win.add_overlay(rects)
-    dlib.hit_enter_to_continue()
+    dlib.hit_enter_to_continue()
```

### Comparing `dlib-19.8.2/python_examples/correlation_tracker.py` & `dlib-19.9.0/python_examples/correlation_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires scikit-image which can be installed
 #   via the command:
 #       pip install scikit-image
 #   Or downloaded from http://scikit-image.org/download.html. 
 
 import os
```

### Comparing `dlib-19.8.2/python_examples/face_alignment.py` & `dlib-19.9.0/python_examples/face_alignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  This code will also use CUDA if you have CUDA and cuDNN
 #   installed.
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires OpenCV and Numpy which can be installed
 #   via the command:
 #       pip install opencv-python numpy
 #   Or downloaded from http://opencv.org/releases.html
 
 import sys
```

### Comparing `dlib-19.8.2/python_examples/face_clustering.py` & `dlib-19.9.0/python_examples/face_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  This code will also use CUDA if you have CUDA and cuDNN
 #   installed.
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires scikit-image which can be installed
 #   via the command:
 #       pip install scikit-image
 #   Or downloaded from http://scikit-image.org/download.html. 
 
 import sys
```

### Comparing `dlib-19.8.2/python_examples/face_detector.py` & `dlib-19.9.0/python_examples/face_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires scikit-image which can be installed
 #   via the command:
 #       pip install scikit-image
 #   Or downloaded from http://scikit-image.org/download.html. 
 
 import sys
```

### Comparing `dlib-19.8.2/python_examples/face_jitter.py` & `dlib-19.9.0/python_examples/face_jitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  This code will also use CUDA if you have CUDA and cuDNN
 #   installed.
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires OpenCV and Numpy which can be installed
 #   via the command:
 #       pip install opencv-python numpy
 #
 #   The image file used in this example is in the public domain:
 #   https://commons.wikimedia.org/wiki/File:Tom_Cruise_avp_2014_4.jpg
```

### Comparing `dlib-19.8.2/python_examples/face_landmark_detection.py` & `dlib-19.9.0/python_examples/face_landmark_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires scikit-image which can be installed
 #   via the command:
 #       pip install scikit-image
 #   Or downloaded from http://scikit-image.org/download.html. 
 
 import sys
```

### Comparing `dlib-19.8.2/python_examples/face_recognition.py` & `dlib-19.9.0/python_examples/face_recognition.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  This code will also use CUDA if you have CUDA and cuDNN
 #   installed.
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires scikit-image which can be installed
 #   via the command:
 #       pip install scikit-image
 #   Or downloaded from http://scikit-image.org/download.html. 
 
 import sys
```

### Comparing `dlib-19.8.2/python_examples/find_candidate_object_locations.py` & `dlib-19.9.0/python_examples/find_candidate_object_locations.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires scikit-image which can be installed
 #   via the command:
 #       pip install scikit-image
 #   Or downloaded from http://scikit-image.org/download.html.
```

### Comparing `dlib-19.8.2/python_examples/global_optimization.py` & `dlib-19.9.0/python_examples/global_optimization.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 #       pip install dlib
 #
 #   Alternatively, if you want to compile dlib yourself then go into the dlib
 #   root folder and run:
 #       python setup.py install
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 
 import dlib
 from math import sin,cos,pi,exp,sqrt
 
 # This is a standard test function for these kinds of optimization problems.
 # It has a bunch of local minima, with the global minimum resulting in
```

### Comparing `dlib-19.8.2/python_examples/max_cost_assignment.py` & `dlib-19.9.0/python_examples/max_cost_assignment.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 
 import dlib
 
 # Let's imagine you need to assign N people to N jobs.  Additionally, each
 # person will make your company a certain amount of money at each job, but each
 # person has different skills so they are better at some jobs and worse at
```

### Comparing `dlib-19.8.2/python_examples/sequence_segmenter.py` & `dlib-19.9.0/python_examples/sequence_segmenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 import sys
 import dlib
 
 
 # The sequence segmentation models we work with in this example are chain
 # structured conditional random field style models.  Therefore, central to a
```

### Comparing `dlib-19.8.2/python_examples/svm_binary_classifier.py` & `dlib-19.9.0/python_examples/svm_binary_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 
 import dlib
 try:
     import cPickle as pickle
 except ImportError:
     import pickle
```

### Comparing `dlib-19.8.2/python_examples/svm_rank.py` & `dlib-19.9.0/python_examples/svm_rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 
 import dlib
 
 
 # Now let's make some testing data.  To make it really simple, let's suppose
 # that we are ranking 2D vectors and that vectors with positive values in the
```

### Comparing `dlib-19.8.2/python_examples/svm_struct.py` & `dlib-19.9.0/python_examples/svm_struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 
 import dlib
 
 
 def main():
     # In this example, we have three types of samples: class 0, 1, or 2.  That
```

### Comparing `dlib-19.8.2/python_examples/train_object_detector.py` & `dlib-19.9.0/python_examples/train_object_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires scikit-image which can be installed
 #   via the command:
 #       pip install scikit-image
 #   Or downloaded from http://scikit-image.org/download.html. 
 
 import os
```

### Comparing `dlib-19.8.2/python_examples/train_shape_predictor.py` & `dlib-19.9.0/python_examples/train_shape_predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 #       python setup.py install
 #   or
 #       python setup.py install --yes USE_AVX_INSTRUCTIONS
 #   if you have a CPU that supports AVX instructions, since this makes some
 #   things run faster.  
 #
 #   Compiling dlib should work on any operating system so long as you have
-#   CMake and boost-python installed.  On Ubuntu, this can be done easily by
-#   running the command:
-#       sudo apt-get install libboost-python-dev cmake
+#   CMake installed.  On Ubuntu, this can be done easily by running the
+#   command:
+#       sudo apt-get install cmake
 #
 #   Also note that this example requires scikit-image which can be installed
 #   via the command:
 #       pip install scikit-image
 #   Or downloaded from http://scikit-image.org/download.html. 
 
 import os
```

### Comparing `dlib-19.8.2/tools/python/src/basic.cpp` & `dlib-19.9.0/tools/python/src/basic.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/cca.cpp` & `dlib-19.9.0/tools/python/src/cca.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/cnn_face_detector.cpp` & `dlib-19.9.0/tools/python/src/cnn_face_detector.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/conversion.h` & `dlib-19.9.0/tools/python/src/conversion.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/correlation_tracker.cpp` & `dlib-19.9.0/tools/python/src/correlation_tracker.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/decision_functions.cpp` & `dlib-19.9.0/tools/python/src/decision_functions.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/face_recognition.cpp` & `dlib-19.9.0/tools/python/src/face_recognition.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/global_optimization.cpp` & `dlib-19.9.0/tools/python/src/global_optimization.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/gui.cpp` & `dlib-19.9.0/tools/python/src/gui.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/image.cpp` & `dlib-19.9.0/tools/python/src/image.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/matrix.cpp` & `dlib-19.9.0/tools/python/src/matrix.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/numpy_returns.cpp` & `dlib-19.9.0/tools/python/src/numpy_returns.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/numpy_returns_stub.cpp` & `dlib-19.9.0/tools/python/src/numpy_returns_stub.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/object_detection.cpp` & `dlib-19.9.0/tools/python/src/object_detection.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/other.cpp` & `dlib-19.9.0/tools/python/src/other.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/rectangles.cpp` & `dlib-19.9.0/tools/python/src/rectangles.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/sequence_segmenter.cpp` & `dlib-19.9.0/tools/python/src/sequence_segmenter.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/serialize_object_detector.h` & `dlib-19.9.0/tools/python/src/serialize_object_detector.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/shape_predictor.cpp` & `dlib-19.9.0/tools/python/src/shape_predictor.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/shape_predictor.h` & `dlib-19.9.0/tools/python/src/shape_predictor.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/simple_object_detector.h` & `dlib-19.9.0/tools/python/src/simple_object_detector.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/simple_object_detector_py.h` & `dlib-19.9.0/tools/python/src/simple_object_detector_py.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/svm_c_trainer.cpp` & `dlib-19.9.0/tools/python/src/svm_c_trainer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/svm_rank_trainer.cpp` & `dlib-19.9.0/tools/python/src/svm_rank_trainer.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/svm_struct.cpp` & `dlib-19.9.0/tools/python/src/svm_struct.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/testing_results.h` & `dlib-19.9.0/tools/python/src/testing_results.h`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/src/vector.cpp` & `dlib-19.9.0/tools/python/src/vector.cpp`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/test/test_array.py` & `dlib-19.9.0/tools/python/test/test_array.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/test/test_matrix.py` & `dlib-19.9.0/tools/python/test/test_matrix.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/test/test_point.py` & `dlib-19.9.0/tools/python/test/test_point.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/test/test_range.py` & `dlib-19.9.0/tools/python/test/test_range.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/test/test_rgb_pixel.py` & `dlib-19.9.0/tools/python/test/test_rgb_pixel.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/test/test_sparse_vector.py` & `dlib-19.9.0/tools/python/test/test_sparse_vector.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/test/test_vector.py` & `dlib-19.9.0/tools/python/test/test_vector.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/tools/python/CMakeLists.txt` & `dlib-19.9.0/tools/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/README.md` & `dlib-19.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/setup.py` & `dlib-19.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `dlib-19.8.2/PKG-INFO` & `dlib-19.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dlib
-Version: 19.8.2
+Version: 19.9.0
 Summary: A toolkit for making real world machine learning and data analysis applications
 Home-page: https://github.com/davisking/dlib
 Author: Davis King
 Author-email: davis@dlib.net
 License: Boost Software License
 Description: # dlib C++ library [![Travis Status](https://travis-ci.org/davisking/dlib.svg?branch=master)](https://travis-ci.org/davisking/dlib)
```

