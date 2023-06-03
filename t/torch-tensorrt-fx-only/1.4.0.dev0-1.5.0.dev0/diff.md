# Comparing `tmp/torch_tensorrt_fx_only-1.4.0.dev0-py3-none-any.whl.zip` & `tmp/torch_tensorrt_fx_only-1.5.0.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,60 +1,72 @@
-Zip file size: 138047 bytes, number of entries: 58
--rw-rw-rw-  2.0 fat      553 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/__init__.py
--rw-rw-rw-  2.0 fat      831 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converter_registry.py
--rw-rw-rw-  2.0 fat     9883 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/diagnostics.py
--rw-rw-rw-  2.0 fat    14884 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/fx2trt.py
--rw-rw-rw-  2.0 fat     7501 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/input_tensor_spec.py
--rw-rw-rw-  2.0 fat    12922 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/lower.py
--rw-rw-rw-  2.0 fat     4861 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/lower_setting.py
--rw-rw-rw-  2.0 fat     6021 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/observer.py
--rw-rw-rw-  2.0 fat     9987 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/trt_module.py
--rw-rw-rw-  2.0 fat      785 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/types.py
--rw-rw-rw-  2.0 fat     2688 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/utils.py
--rw-rw-rw-  2.0 fat      798 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/__init__.py
--rw-rw-rw-  2.0 fat   128855 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/acc_ops_converters.py
--rw-rw-rw-  2.0 fat     2221 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/activation.py
--rw-rw-rw-  2.0 fat     1211 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/adaptive_avgpool.py
--rw-rw-rw-  2.0 fat     2521 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/add.py
--rw-rw-rw-  2.0 fat    13705 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/aten_ops_converters.py
--rw-rw-rw-  2.0 fat     1824 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/batchnorm.py
--rw-rw-rw-  2.0 fat    31945 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/converter_utils.py
--rw-rw-rw-  2.0 fat     6703 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/convolution.py
--rw-rw-rw-  2.0 fat     2914 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/linear.py
--rw-rw-rw-  2.0 fat     1496 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/maxpool.py
--rw-rw-rw-  2.0 fat     1562 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/mul.py
--rw-rw-rw-  2.0 fat     2162 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/quantization.py
--rw-rw-rw-  2.0 fat     1547 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/converters/transformation.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/passes/__init__.py
--rw-rw-rw-  2.0 fat     2044 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/passes/graph_opts.py
--rw-rw-rw-  2.0 fat    23744 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/passes/lower_basic_pass.py
--rw-rw-rw-  2.0 fat    19757 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/passes/lower_basic_pass_aten.py
--rw-rw-rw-  2.0 fat    12014 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/passes/lower_pass_manager_builder.py
--rw-rw-rw-  2.0 fat     9875 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/passes/pass_utils.py
--rw-rw-rw-  2.0 fat     4961 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/passes/remove_duplicate_output_args.py
--rw-rw-rw-  2.0 fat       49 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/__init__.py
--rw-rw-rw-  2.0 fat    15697 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/common_fx2trt.py
--rw-rw-rw-  2.0 fat     7067 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/engine_layer_visualize.py
--rw-rw-rw-  2.0 fat     2423 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/graph_util.py
--rw-rw-rw-  2.0 fat     3939 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/model_packager.py
--rw-rw-rw-  2.0 fat     1777 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/node_profiler.py
--rw-rw-rw-  2.0 fat     1163 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/tensor_prop.py
--rw-rw-rw-  2.0 fat     1451 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/timing_cache_utils.py
--rw-rw-rw-  2.0 fat     3780 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/trt_minimizer.py
--rw-rw-rw-  2.0 fat     2052 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/trt_profiler_sorted.py
--rw-rw-rw-  2.0 fat     5518 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tools/trt_splitter.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/acc_tracer/__init__.py
--rw-rw-rw-  2.0 fat    19889 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/acc_tracer/acc_normalizer.py
--rw-rw-rw-  2.0 fat     1573 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/acc_tracer/acc_op_properties.py
--rw-rw-rw-  2.0 fat   105950 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/acc_tracer/acc_ops.py
--rw-rw-rw-  2.0 fat     5557 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/acc_tracer/acc_shape_prop.py
--rw-rw-rw-  2.0 fat    28268 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/acc_tracer/acc_tracer.py
--rw-rw-rw-  2.0 fat     7148 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/acc_tracer/acc_utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/dispatch_tracer/__init__.py
--rw-rw-rw-  2.0 fat     5341 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/dispatch_tracer/aten_tracer.py
--rw-rw-rw-  2.0 fat     7785 b- defN 23-Apr-08 05:48 torch_tensorrt/fx/tracer/dispatch_tracer/tracer.py
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-08 06:12 torch_tensorrt_fx_only-1.4.0.dev0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13818 b- defN 23-Apr-08 06:12 torch_tensorrt_fx_only-1.4.0.dev0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-08 06:12 torch_tensorrt_fx_only-1.4.0.dev0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Apr-08 06:12 torch_tensorrt_fx_only-1.4.0.dev0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     5715 b- defN 23-Apr-08 06:12 torch_tensorrt_fx_only-1.4.0.dev0.dist-info/RECORD
-58 files, 588852 bytes uncompressed, 128679 bytes compressed:  78.1%
+Zip file size: 167299 bytes, number of entries: 70
+-rw-rw-rw-  2.0 fat       78 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/__init__.py
+-rw-rw-rw-  2.0 fat      459 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/__init__.py
+-rw-rw-rw-  2.0 fat    14997 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/fx2trt.py
+-rw-rw-rw-  2.0 fat     7093 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/input_tensor_spec.py
+-rw-rw-rw-  2.0 fat    14366 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/lower.py
+-rw-rw-rw-  2.0 fat     4407 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/lower_setting.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/passes/__init__.py
+-rw-rw-rw-  2.0 fat    13108 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/passes/lower_pass_manager_builder.py
+-rw-rw-rw-  2.0 fat    10929 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/passes/pass_utils.py
+-rw-rw-rw-  2.0 fat       49 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/tools/__init__.py
+-rw-rw-rw-  2.0 fat    15762 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/tools/common_fx2trt.py
+-rw-rw-rw-  2.0 fat     3622 b- defN 23-May-20 15:45 torch_tensorrt/dynamo/fx_ts_compat/tools/trt_minimizer.py
+-rw-rw-rw-  2.0 fat      553 b- defN 23-May-20 15:45 torch_tensorrt/fx/__init__.py
+-rw-rw-rw-  2.0 fat      831 b- defN 23-May-20 15:45 torch_tensorrt/fx/converter_registry.py
+-rw-rw-rw-  2.0 fat    10067 b- defN 23-May-20 15:45 torch_tensorrt/fx/diagnostics.py
+-rw-rw-rw-  2.0 fat    15161 b- defN 23-May-20 15:45 torch_tensorrt/fx/fx2trt.py
+-rw-rw-rw-  2.0 fat     9575 b- defN 23-May-20 15:45 torch_tensorrt/fx/input_tensor_spec.py
+-rw-rw-rw-  2.0 fat    13066 b- defN 23-May-20 15:45 torch_tensorrt/fx/lower.py
+-rw-rw-rw-  2.0 fat     4861 b- defN 23-May-20 15:45 torch_tensorrt/fx/lower_setting.py
+-rw-rw-rw-  2.0 fat     6021 b- defN 23-May-20 15:45 torch_tensorrt/fx/observer.py
+-rw-rw-rw-  2.0 fat     9987 b- defN 23-May-20 15:45 torch_tensorrt/fx/trt_module.py
+-rw-rw-rw-  2.0 fat      785 b- defN 23-May-20 15:45 torch_tensorrt/fx/types.py
+-rw-rw-rw-  2.0 fat     4401 b- defN 23-May-20 15:45 torch_tensorrt/fx/utils.py
+-rw-rw-rw-  2.0 fat      798 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/__init__.py
+-rw-rw-rw-  2.0 fat   129037 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/acc_ops_converters.py
+-rw-rw-rw-  2.0 fat     2221 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/activation.py
+-rw-rw-rw-  2.0 fat     1211 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/adaptive_avgpool.py
+-rw-rw-rw-  2.0 fat     2521 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/add.py
+-rw-rw-rw-  2.0 fat    14228 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/aten_ops_converters.py
+-rw-rw-rw-  2.0 fat     1824 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/batchnorm.py
+-rw-rw-rw-  2.0 fat    31945 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/converter_utils.py
+-rw-rw-rw-  2.0 fat     6703 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/convolution.py
+-rw-rw-rw-  2.0 fat     2914 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/linear.py
+-rw-rw-rw-  2.0 fat     1496 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/maxpool.py
+-rw-rw-rw-  2.0 fat     1562 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/mul.py
+-rw-rw-rw-  2.0 fat     2162 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/quantization.py
+-rw-rw-rw-  2.0 fat     1547 b- defN 23-May-20 15:45 torch_tensorrt/fx/converters/transformation.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-20 15:45 torch_tensorrt/fx/passes/__init__.py
+-rw-rw-rw-  2.0 fat     2044 b- defN 23-May-20 15:45 torch_tensorrt/fx/passes/graph_opts.py
+-rw-rw-rw-  2.0 fat    25182 b- defN 23-May-20 15:45 torch_tensorrt/fx/passes/lower_basic_pass.py
+-rw-rw-rw-  2.0 fat    19757 b- defN 23-May-20 15:45 torch_tensorrt/fx/passes/lower_basic_pass_aten.py
+-rw-rw-rw-  2.0 fat    12274 b- defN 23-May-20 15:45 torch_tensorrt/fx/passes/lower_pass_manager_builder.py
+-rw-rw-rw-  2.0 fat    19519 b- defN 23-May-20 15:45 torch_tensorrt/fx/passes/pass_utils.py
+-rw-rw-rw-  2.0 fat     4961 b- defN 23-May-20 15:45 torch_tensorrt/fx/passes/remove_duplicate_output_args.py
+-rw-rw-rw-  2.0 fat       49 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/__init__.py
+-rw-rw-rw-  2.0 fat    15853 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/common_fx2trt.py
+-rw-rw-rw-  2.0 fat     7067 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/engine_layer_visualize.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/graph_util.py
+-rw-rw-rw-  2.0 fat     4703 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/model_packager.py
+-rw-rw-rw-  2.0 fat     1777 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/node_profiler.py
+-rw-rw-rw-  2.0 fat     1163 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/tensor_prop.py
+-rw-rw-rw-  2.0 fat     1451 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/timing_cache_utils.py
+-rw-rw-rw-  2.0 fat     3780 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/trt_minimizer.py
+-rw-rw-rw-  2.0 fat     2052 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/trt_profiler_sorted.py
+-rw-rw-rw-  2.0 fat     5592 b- defN 23-May-20 15:45 torch_tensorrt/fx/tools/trt_splitter.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/acc_tracer/__init__.py
+-rw-rw-rw-  2.0 fat    20455 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/acc_tracer/acc_normalizer.py
+-rw-rw-rw-  2.0 fat     1573 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/acc_tracer/acc_op_properties.py
+-rw-rw-rw-  2.0 fat   113034 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/acc_tracer/acc_ops.py
+-rw-rw-rw-  2.0 fat     5557 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/acc_tracer/acc_shape_prop.py
+-rw-rw-rw-  2.0 fat    28756 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/acc_tracer/acc_tracer.py
+-rw-rw-rw-  2.0 fat     7430 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/acc_tracer/acc_utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/dispatch_tracer/__init__.py
+-rw-rw-rw-  2.0 fat     5262 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/dispatch_tracer/aten_tracer.py
+-rw-rw-rw-  2.0 fat     7785 b- defN 23-May-20 15:45 torch_tensorrt/fx/tracer/dispatch_tracer/tracer.py
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-20 15:57 torch_tensorrt_fx_only-1.5.0.dev0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13822 b- defN 23-May-20 15:57 torch_tensorrt_fx_only-1.5.0.dev0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 15:57 torch_tensorrt_fx_only-1.5.0.dev0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-20 15:57 torch_tensorrt_fx_only-1.5.0.dev0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     7015 b- defN 23-May-20 15:57 torch_tensorrt_fx_only-1.5.0.dev0.dist-info/RECORD
+70 files, 700800 bytes uncompressed, 155785 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -1,7 +1,43 @@
+Filename: torch_tensorrt/dynamo/__init__.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/__init__.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/fx2trt.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/input_tensor_spec.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/lower.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/lower_setting.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/passes/__init__.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/passes/lower_pass_manager_builder.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/passes/pass_utils.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/tools/__init__.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/tools/common_fx2trt.py
+Comment: 
+
+Filename: torch_tensorrt/dynamo/fx_ts_compat/tools/trt_minimizer.py
+Comment: 
+
 Filename: torch_tensorrt/fx/__init__.py
 Comment: 
 
 Filename: torch_tensorrt/fx/converter_registry.py
 Comment: 
 
 Filename: torch_tensorrt/fx/diagnostics.py
@@ -153,23 +189,23 @@
 
 Filename: torch_tensorrt/fx/tracer/dispatch_tracer/aten_tracer.py
 Comment: 
 
 Filename: torch_tensorrt/fx/tracer/dispatch_tracer/tracer.py
 Comment: 
 
-Filename: torch_tensorrt_fx_only-1.4.0.dev0.dist-info/LICENSE
+Filename: torch_tensorrt_fx_only-1.5.0.dev0.dist-info/LICENSE
 Comment: 
 
-Filename: torch_tensorrt_fx_only-1.4.0.dev0.dist-info/METADATA
+Filename: torch_tensorrt_fx_only-1.5.0.dev0.dist-info/METADATA
 Comment: 
 
-Filename: torch_tensorrt_fx_only-1.4.0.dev0.dist-info/WHEEL
+Filename: torch_tensorrt_fx_only-1.5.0.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: torch_tensorrt_fx_only-1.4.0.dev0.dist-info/top_level.txt
+Filename: torch_tensorrt_fx_only-1.5.0.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: torch_tensorrt_fx_only-1.4.0.dev0.dist-info/RECORD
+Filename: torch_tensorrt_fx_only-1.5.0.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torch_tensorrt/fx/diagnostics.py

```diff
@@ -83,20 +83,22 @@
 class DiagnosticsWriter:
 
     # the root dir in which the diagnostics will be written
     _root_dir: str
 
     def __init__(self):
         self._root_dir = tempfile.mkdtemp(prefix="fx2trt.")
+        self._data = ""
         _LOGGER.info(f"Initializing DiagnosticsWriter with root_dir: {self._root_dir}")
 
     def write(self, file_name: str, data: WriteObj):
         """
         TODO: Can be disabled by regex on file_name
         """
+        self._data = data
         # Only write if we are inside a collect_when() context.
         if not _IS_IN_COLLECT_CONTEXT.get(False):
             return
 
         try:
             res, err = _res_or_err(data)
             if err:
@@ -113,14 +115,17 @@
             # Log the error and swallow the exception, as this should not
             # propagated into business logic
             _LOGGER.warning(f"Error writing diagnostics: {e}")
 
     def root_dir(self) -> str:
         return self._root_dir
 
+    def data(self) -> WriteObj:
+        return self._data
+
     def _write(self, file_name: str, to_write: bytes):
         # ms granularity - no naming collash, otherwise file will be
         # overwritten.
         ts = int(time.time() * 1000)
         file_name = f"{file_name}.{ts}"
         fn = os.path.join(self.root_dir(), file_name)
         with open(fn, "wb") as f:
@@ -267,14 +272,17 @@
         try:
             zip_path = shutil.make_archive(fp, "zip", self._write.root_dir())
             self._last_zip_path_for_test = zip_path
             return zip_path
         finally:
             os.remove(fp)
 
+    def data(self) -> WriteObj:
+        return self._write.data()
+
 
 def _res_or_err(data: WriteObj) -> t.Tuple[TWrite, str]:
     if isinstance(data, (str, bytes)):
         return data, ""
     if not callable(data):
         raise TypeError(
             f"data must be a callable that returns actual data to"
```

## torch_tensorrt/fx/fx2trt.py

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import warnings
 from datetime import datetime
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Sequence
 
 import numpy
 
 # @manual=//deeplearning/trt/python:py_tensorrt
@@ -207,14 +208,19 @@
         )
         build_engine_start_time = datetime.now()
 
         self.builder.max_batch_size = max_batch_size
         builder_config = self.builder.create_builder_config()
         builder_config.max_workspace_size = max_workspace_size
 
+        # Speed up TRT build time in the test environment
+        if trt.__version__ >= "8.6" and os.environ.get("TRT_TEST_ENV", "0") == "1":
+            _LOGGER.info("Set TRT optimization level to 0")
+            builder_config.builder_optimization_level = 0
+
         cache = None
         if timing_cache:
             cache_file = numpy.array(timing_cache)
             cache = builder_config.create_timing_cache(cache_file.tobytes())
         else:
             cache = builder_config.create_timing_cache(b"")
         builder_config.set_timing_cache(cache, False)
```

## torch_tensorrt/fx/input_tensor_spec.py

```diff
@@ -1,8 +1,8 @@
-from typing import Iterable, List, NamedTuple, Optional, Sequence, Tuple
+from typing import Any, Iterable, List, NamedTuple, Optional, Sequence, Tuple
 
 import torch
 
 from .types import Shape, ShapeRange
 from .utils import get_dynamic_dims
 
 
@@ -14,22 +14,29 @@
     ):
         return InputTensorSpec.from_tensors(inputs)
 
     # If we don't have additional inputs, we assume the first dimension
     # is the dynamic batch dimension. Otherwise, we use the additional
     # inputs to determine the batch dimension.
     if additional_inputs is None:
+        batch_dims = None
+        if not isinstance(inputs, torch.Tensor) and len(inputs) > 1:
+            bs = inputs[0].size(0)
+            batch_dims = None
+            if not all(x.size(0) == bs for x in inputs):
+                batch_dims = InputTensorSpec.find_batch_size_dim(inputs)
         return InputTensorSpec.from_tensors_with_dynamic_batch_size(
             inputs,
             (
                 0,
                 lower_setting.max_batch_size,
                 lower_setting.max_batch_size,
             ),
             lower_setting.opt_profile_replica,
+            batch_dims,
         )
     else:
         batch_dims = []
 
         for i, j in zip(inputs, additional_inputs):
             found_batch_dim = False
 
@@ -143,33 +150,77 @@
                 and allow user to specify the batch dims using this arg. Default we treat
                 dim 0 as the batch dim.
 
         Returns:
             A list of InputTensorSpec named tuples with dynamic ranges.
         """
         if batch_dims is None:
-            batch_dims = [0] * len(tensors)
+            batch_dims = cls.find_batch_size_dim(tensors)
 
         input_specs = []
         batch_size = tensors[0].size(batch_dims[0])
 
         for i, tensor in enumerate(tensors):
             batch_dim = batch_dims[i]
-            assert batch_size == tensor.size(
-                batch_dim
-            ), f"The {i}th tensor (shape: {tensor.shape}) doesn't have the correct batch size: {batch_size}."
-            shape = list(tensor.shape)
-            shape[batch_dim] = -1
-            shape_ranges: List[ShapeRange] = [tuple(tuple(shape[0:batch_dim] + [bs] + shape[batch_dim + 1 :]) for bs in batch_size_range)] * opt_profile_replica  # type: ignore[list-item]
-            input_specs.append(
-                cls(tuple(shape), tensor.dtype, tensor.device, shape_ranges)
-            )
+            if batch_dim == -1:
+                input_specs.append(cls.from_tensor(tensor))
+            else:
+                shape = list(tensor.shape)
+                assert batch_size == tensor.size(
+                    batch_dim
+                ), f"The {i}th tensor (shape: {tensor.shape}) doesn't have the correct batch size: {batch_size}."
+                shape[batch_dim] = -1
+                shape_ranges: List[ShapeRange] = [tuple(tuple(shape[0:batch_dim] + [bs] + shape[batch_dim + 1 :]) for bs in batch_size_range)] * opt_profile_replica  # type: ignore[list-item]
+                input_specs.append(
+                    cls(tuple(shape), tensor.dtype, tensor.device, shape_ranges)
+                )
 
         return input_specs
 
+    @classmethod
+    # pyre-ignore [2]: Parameter `sample_input` must have a type other than `Any`
+    def find_batch_size_dim(cls, inputs: Any) -> []:
+        if isinstance(inputs, torch.Tensor) or len(inputs) <= 1:
+            return [0]
+        shapes = [i.shape for i in inputs]
+        frequency_map = {}
+        first_dims = set()
+        for shape in shapes:
+            if len(shape) < 2:
+                # By pass for rank-1 tensors. MRS model has rank-1 tensor carry no batch_size info
+                continue
+            # Dedup shape value for single tensor
+            first_dims.add(shape[0])
+            shape = set(shape)
+            for i in shape:
+                frequency_map[i] = frequency_map.get(i, 0) + 1
+
+        if len(first_dims) == 1:
+            # first dim is the same in every input: we use it as batch_size
+            batch_size = first_dims.pop()
+        elif frequency_map:
+            # first dims are different: we use the most frequent dim as batch_size
+            sorted_frequency = sorted(frequency_map.items(), key=lambda x: -x[1])
+            batch_size = sorted_frequency[0][0]
+        else:
+            # no dims to sort: no batch_size
+            batch_size = -1
+
+        bs_dim = []
+        for i in inputs:
+            # Default batch size dim = -1, indicate no batch_size
+            dim = -1
+            for index, val in enumerate(i.shape):
+                if val == batch_size:
+                    dim = index
+                    break
+            bs_dim.append(dim)
+
+        return bs_dim
+
     def to_random_tensor(self, id=1):
         shape = tuple(self.shape)
         if len(get_dynamic_dims(shape)):
             # id=0 -> min shape
             # id=1 -> optimal shape
             # id=2 -> max shape
             shape = tuple(self.shape_ranges[0][id])
```

## torch_tensorrt/fx/lower.py

```diff
@@ -37,14 +37,16 @@
     verbose_log=False,
     timing_cache_prefix="",
     save_timing_cache=False,
     cuda_graph_batch_size=-1,
     dynamic_batch=True,
     is_aten=False,
     use_experimental_fx_rt=False,
+    correctness_atol=1e-1,
+    correctness_rtol=1e-1,
 ) -> nn.Module:
     """
     Takes in original module, input and lowering setting, run lowering workflow to turn module
     into lowered module, or so called TRTModule.
 
     Args:
         module: Original module for lowering.
@@ -77,14 +79,16 @@
         verbose_log=verbose_log,
         timing_cache_prefix=timing_cache_prefix,
         save_timing_cache=save_timing_cache,
         cuda_graph_batch_size=cuda_graph_batch_size,
         dynamic_batch=dynamic_batch,
         is_aten=is_aten,
         use_experimental_rt=use_experimental_fx_rt,
+        correctness_atol=correctness_atol,
+        correctness_rtol=correctness_rtol,
     )
     lowerer = Lowerer.create(lower_setting=lower_setting)
     return lowerer(module, input)
 
 
 @dc.dataclass
 class LowerTrtInterpreter:
```

## torch_tensorrt/fx/utils.py

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
-from typing import List
+from typing import List, Optional, Callable
+from packaging import version
 
 # @manual=//deeplearning/trt/python:py_tensorrt
 import tensorrt as trt
 import torch
 from functorch import make_fx
 from functorch.experimental import functionalize
 from torch_tensorrt.fx.passes.lower_basic_pass import (
@@ -14,14 +15,28 @@
 from .types import Shape, TRTDataType
 
 
 class LowerPrecision(Enum):
     FP32 = "fp32"
     FP16 = "fp16"
     INT8 = "int8"
+    BF16 = "bf16"
+
+    @staticmethod
+    def from_str(label: str) -> Optional["LowerPrecision"]:
+        if label in ("fp32", "float32", "float", "torch.float32"):
+            return LowerPrecision.FP32
+        elif label in ("fp16", "float16", "half", "torch.half", "torch.float16"):
+            return LowerPrecision.FP16
+        elif label in ("int8"):
+            return LowerPrecision.INT8
+        elif label in ("bf16", "bfloat16", "torch.bfloat16"):
+            return LowerPrecision.BF16
+        else:
+            return None
 
 
 def torch_dtype_to_trt(dtype: torch.dtype) -> TRTDataType:
     """
     Convert PyTorch data types to TensorRT data types.
 
     Args:
@@ -100,7 +115,40 @@
     mod = make_fx(functionalize(f))(*inputs)
 
     # Remove const operation. For ex, nn.Linear has transpose operation on weight
     mod.graph.eliminate_dead_code()
     mod = run_const_fold(mod)
     mod = replace_op_with_indices(mod)
     return mod
+
+
+def req_torch_version(min_torch_version: str = "2.dev"):
+    """
+    Create a decorator which verifies the Torch version installed
+    against a specified version range
+
+    Args:
+        min_torch_version (str): The minimum required Torch version
+        for the decorated function to work properly
+
+    Returns:
+        A decorator which raises a descriptive error message if
+        an unsupported Torch version is used
+    """
+
+    def nested_decorator(f: Callable):
+        def function_wrapper(*args, **kwargs):
+            # Parse minimum and current Torch versions
+            min_version = version.parse(min_torch_version)
+            current_version = version.parse(torch.__version__)
+
+            if current_version < min_version:
+                raise AssertionError(
+                    f"Expected Torch version {min_torch_version} or greater, "
+                    + f"when calling {f}. Detected version {torch.__version__}"
+                )
+            else:
+                return f(*args, **kwargs)
+
+        return function_wrapper
+
+    return nested_decorator
```

## torch_tensorrt/fx/converters/acc_ops_converters.py

```diff
@@ -112,15 +112,15 @@
         assert input_val.shape[1] != -1, "Channel dim can't be dynamic for convolution."
 
     # for now we'll assume bias is constant Tensor or None,
     # and bias being ITensor is not supported in TensorRT api
     # right now
     if kwargs["bias"] is not None and not isinstance(kwargs["bias"], torch.Tensor):
         raise RuntimeError(
-            f"linear {name} has bias of type {type(kwargs['bias'])}, Expect Optional[Tenosr]"
+            f"linear {name} has bias of type {type(kwargs['bias'])}, Expect Optional[Tensor]"
         )
     bias = to_numpy(kwargs["bias"])  # type: ignore[arg-type]
     if bias is not None:
         bias = bias[None]
     weight = kwargs["weight"]
 
     if network.has_explicit_precision or isinstance(weight, TRTTensor):
@@ -142,15 +142,15 @@
             bias=bias,
         )
 
         layer.set_input(1, weight)
     else:
         if not isinstance(kwargs["weight"], torch.Tensor):
             raise RuntimeError(
-                f"linear {name} has weight of type {type(kwargs['weight'])}, Expect Optional[Tenosr]"
+                f"linear {name} has weight of type {type(kwargs['weight'])}, Expect Optional[Tensor]"
             )
         weight = to_numpy(weight)
         weight = np.expand_dims(weight, -1)
         layer = network.add_convolution_nd(
             input=input_val,
             num_output_maps=weight.shape[0],
             kernel_shape=weight.shape[2:],
@@ -198,19 +198,19 @@
         assert input_val.shape[1] != -1, "Channel dim can't be dynamic for convolution."
 
     # for now we'll assume bias is constant Tensor or None,
     # and bias being ITensor is not supported in TensorRT api
     # right now
     if kwargs["bias"] is not None and not isinstance(kwargs["bias"], torch.Tensor):
         raise RuntimeError(
-            f"linear {name} has bias of type {type(kwargs['bias'])}, Expect Optional[Tenosr]"
+            f"linear {name} has bias of type {type(kwargs['bias'])}, Expect Optional[Tensor]"
         )
     bias = to_numpy(kwargs["bias"])  # type: ignore[arg-type]
 
-    if network.has_explicit_precision:
+    if network.has_explicit_precision or isinstance(kwargs["weight"], TRTTensor):
         weight = get_trt_tensor(network, kwargs["weight"], f"{name}_weight")
         weight_shape = tuple(kwargs["weight"].shape)  # type: ignore[union-attr]
         # will need to use uninitialized weight and set it later to support
         # ITensor weights
         dummy_weight = trt.Weights()
         layer = network.add_convolution_nd(
             input=input_val,
@@ -220,15 +220,15 @@
             bias=bias,
         )
 
         layer.set_input(1, weight)
     else:
         if not isinstance(kwargs["weight"], torch.Tensor):
             raise RuntimeError(
-                f"linear {name} has weight of type {type(kwargs['weight'])}, Expect Optional[Tenosr]"
+                f"linear {name} has weight of type {type(kwargs['weight'])}, Expect Optional[Tensor]"
             )
         weight = to_numpy(kwargs["weight"])
         layer = network.add_convolution_nd(
             input=input_val,
             num_output_maps=weight.shape[0],
             kernel_shape=weight.shape[2:],
             kernel=weight,
@@ -272,15 +272,15 @@
     # right now
     if kwargs["bias"] is not None and not isinstance(kwargs["bias"], torch.Tensor):
         raise RuntimeError(
             f"ConvTranspose {name} has bias of type {type(kwargs['bias'])}, Expect Optional[Tensor]"
         )
     bias = to_numpy(kwargs["bias"])  # type: ignore[arg-type]
 
-    if network.has_explicit_precision:
+    if network.has_explicit_precision or isinstance(kwargs["weight"], TRTTensor):
         weight = get_trt_tensor(network, kwargs["weight"], f"{name}_weight")
         weight_shape = tuple(kwargs["weight"].shape)  # type: ignore[union-attr]
         # will need to use uninitialized weight and set it later to support
         # ITensor weights
         dummy_weight = trt.Weights()
 
         # nn.ConvTranspose2d/3d weight size is (in_channels, out_channels/groups, kernel_0, kernel_1, [kernel_2])
@@ -687,18 +687,21 @@
     gamma = kwargs["weight"].detach().cpu().float().numpy()
     gamma_field = trt.PluginField("gamma", gamma, trt.PluginFieldType.FLOAT32)
     beta = kwargs["bias"].detach().cpu().float().numpy()
     beta_field = trt.PluginField("beta", beta, trt.PluginFieldType.FLOAT32)
     eps_field = trt.PluginField(
         "eps", np.array([kwargs["eps"]], dtype=np.float32), trt.PluginFieldType.FLOAT32
     )
+    normalized_shape = kwargs["normalized_shape"]
     try:
-        normalized_shape = np.array(kwargs["normalized_shape"], dtype=np.int32)
+        normalized_shape = np.array(normalized_shape, dtype=np.int32)
     except TypeError:
-        _LOGGER.error("Unable to convert normalized_shape to a field, fall back to []")
+        _LOGGER.error(
+            f"Unable to convert normalized_shape with value {normalized_shape} to a field, fall back to []"
+        )
         normalized_shape = np.array([], dtype=np.int32)
 
     normalized_shape_filed = trt.PluginField(
         "normalized_shape", normalized_shape, trt.PluginFieldType.INT32
     )
     field_collection = trt.PluginFieldCollection(
         [gamma_field, beta_field, eps_field, normalized_shape_filed]
```

## torch_tensorrt/fx/converters/aten_ops_converters.py

```diff
@@ -37,42 +37,55 @@
     kwargs_new = {
         "input": args[0],
         "other": args[1],
     }
     return acc_ops_converters.acc_ops_add(network, target, None, kwargs_new, name)
 
 
-@tensorrt_converter(torch.ops.aten.mean.dim)
 @tensorrt_converter(torch.ops.aten._adaptive_avg_pool3d.default)
 @tensorrt_converter(torch.ops.aten._adaptive_avg_pool2d.default)
 def aten_ops_adaptive_avg_poolnd(
     network: TRTNetwork,
     target: Target,
     args: Tuple[Argument, ...],
     kwargs: Dict[str, Argument],
     name: str,
 ) -> Union[TRTTensor, Sequence[TRTTensor]]:
-    if target == torch.ops.aten.mean.dim:
-
-        if list(args[1]) != [-1, -2]:
-            raise RuntimeError(f"We do not support {target} has dim={args[1]}")
-        else:
-            output_size = [1, 1]
-    else:
-        output_size = args[1]
-
     kwargs_new = {
         "input": args[0],
-        "output_size": output_size,
+        "output_size": args[1],
     }
     return acc_ops_converters.acc_ops_adaptive_avg_poolnd(
         network, target, None, kwargs_new, name
     )
 
 
+@tensorrt_converter(torch.ops.aten.mean.default)
+@tensorrt_converter(torch.ops.aten.mean.dim)
+def aten_ops_mean(
+    network: TRTNetwork,
+    target: Target,
+    args: Tuple[Argument, ...],
+    kwargs: Dict[str, Argument],
+    name: str,
+) -> TRTTensor:
+    # Default invocation of aten.mean only uses first argument and
+    # averages over all elements (all dimensions)
+    # aten.mean.dim invocation allows specification of dimensions to average
+    # over, as well at the option to keep the dimension or not
+    kwargs_new = {
+        "input": args[0],
+        "dim": args[1] if len(args) >= 2 else list(range(len(args[0].shape))),
+        "keepdim": args[2] if len(args) >= 3 else False,
+    }
+    return add_reduce_layer(
+        network, target, args, kwargs_new, trt.ReduceOperation.AVG, name
+    )
+
+
 @tensorrt_converter(torch.ops.aten.batch_norm)
 def aten_ops_batch_norm(
     network: TRTNetwork,
     target: Target,
     args: Tuple[Argument, ...],
     kwargs: Dict[str, Argument],
     name: str,
```

## torch_tensorrt/fx/passes/lower_basic_pass.py

```diff
@@ -50,27 +50,31 @@
                     n.replace_all_uses_with(new_node)
                     module.graph.erase_node(n)
     module.recompile()
     return module
 
 
 def run_const_fold(traced_mod: torch.fx.GraphModule) -> torch.fx.GraphModule:
-    # Now we do constant folding on traced module. We want to skip pattern like
-    # weights -> quant -> dequant -> op during constant folding when the model is
-    # a quantized int8 model.
-    def skip_folding_quant_dequant(node: torch.fx.Node):
+    def skip_folding_ops(node: torch.fx.Node):
+        # dtype op
+        if node.target == acc_ops.dtype:
+            return True
+        # Now we do constant folding on traced module. We want to skip pattern like
+        # weights -> quant -> dequant -> op during constant folding when the model is
+        # a quantized int8 model.
+        # quant_dequant
         if node.target != acc_ops.quantize_per_tensor:
             return False
         # If quantize_per_node -> dequantize, then skip folding.
         for user in node.users:
             if user.target == acc_ops.dequantize:
                 return True
         return False
 
-    const_split_mod = split_const_subgraphs(traced_mod, skip_folding_quant_dequant)
+    const_split_mod = split_const_subgraphs(traced_mod, skip_folding_ops)
     const_split_mod.run_folding()
     return const_split_mod
 
 
 def replace_op_with_indices(module: torch.fx.GraphModule) -> torch.fx.GraphModule:
     for n in module.graph.nodes:
         if n.op == "call_function" and n.target in (
@@ -626,7 +630,39 @@
                     "min": MIN_FP16,
                     "max": MAX_FP16,
                 }
                 node.kwargs = new_kwargs
 
     mod.recompile()
     return mod
+
+
+@log_before_after
+@validate_inference(atol=1e-3, rtol=1e-2)
+def remove_dtype_and_to_pattern(
+    mod: torch.fx.GraphModule, input: Input
+) -> torch.fx.GraphModule:
+    """
+    Remove this pattern since it is unnecessary to cast to dtype
+        %dtype : [#users=1] = call_function[target=torch_tensorrt.fx.tracer.acc_tracer.acc_ops.dtype](args = (), kwargs = {input: %_attention_layers_0__uva})
+        %to_18 : [#users=2] = call_function[target=torch_tensorrt.fx.tracer.acc_tracer.acc_ops.to_dtype](args = (), kwargs = {input: %x})
+    """
+    for node in mod.graph.nodes:
+        if node.op == "call_function" and node.target == acc_ops.dtype:
+            # find its first user
+            next_node = next(iter(node.users))
+            # acc_op or pt op is treated differently
+            input = (
+                next_node.kwargs["input"]
+                if "input" in next_node.kwargs
+                else next_node.args[0]
+            )
+            if len(node.users) == 1 and (
+                next_node.target == acc_ops.to_dtype or next_node.target == "to"
+            ):
+                next_node.replace_all_uses_with(input)
+                mod.graph.erase_node(next_node)
+                mod.graph.erase_node(node)
+
+    mod.graph.eliminate_dead_code()
+    mod.recompile()
+    return mod
```

## torch_tensorrt/fx/passes/lower_pass_manager_builder.py

```diff
@@ -4,14 +4,15 @@
 from typing import Any, Callable, Optional, Sequence
 
 import torch
 from torch import nn
 from torch.fx.passes.pass_manager import inplace_wrapper, PassManager
 from torch.fx.passes.shape_prop import ShapeProp
 from torch.fx.passes.splitter_base import generate_inputs_for_submodules, SplitResult
+from torch_tensorrt.fx.passes.pass_utils import apply_bfloat_float_conversion
 from torch_tensorrt.fx.utils import LowerPrecision
 
 from ..input_tensor_spec import generate_input_specs
 
 from ..lower_setting import LowerSetting
 from ..observer import Observer
 from ..passes.remove_duplicate_output_args import remove_duplicate_output_args
@@ -225,18 +226,17 @@
             else:
                 additional_submodule_inputs = None
 
             for submod_name, submod_inputs in split_result.submodule_inputs.items():
                 submod = getattr(split_result.split_module, submod_name)
 
                 LOWER_SPLIT_PRE_OBSERVER.observe(submod_name, submod, submod_inputs)
-
                 # Only acc submodules will be lowered.
                 if not submod_name.startswith(split_result.non_acc_submodule_prefix):
-                    _LOGGER.info(f"Now lowering submodule {submod_name}")
+                    _LOGGER.info(f"ACC submodule graph: {submod.graph}")
                     lowering_start_time = datetime.datetime.now()
 
                     self.lower_setting.additional_inputs = (
                         additional_submodule_inputs[submod_name]
                         if additional_submodule_inputs
                         else None,
                     )
@@ -247,14 +247,17 @@
                     setattr(split_result.split_module, submod_name, lowered_module)
                     LOWER_SPLIT_POST_OBSERVER.observe(
                         submod_name, lowered_module, submod_inputs
                     )
                     _LOGGER.info(
                         f"Lowering submodule {submod_name} elapsed time {datetime.datetime.now() - lowering_start_time}"
                     )
+                else:
+                    _LOGGER.info(f"GPU submodule graph: {submod.graph}")
+                    apply_bfloat_float_conversion(submod, submod_inputs, submod_name)
 
             return split_result.split_module
 
         return PassManager.build_from_passlist([lower_func])
 
     def _default_replace_mutable_op_pass(self) -> PassManager:
         return PassManager.build_from_passlist([replace_mutable_op])
```

## torch_tensorrt/fx/passes/pass_utils.py

```diff
@@ -1,29 +1,39 @@
+import contextlib
 import io
+import json
 import logging
 import tempfile
 from datetime import datetime
 from functools import wraps
+from traceback import TracebackException
 from typing import Any, Callable, List, Optional
 
 import torch
+import torch_tensorrt.fx.diagnostics as diagnostics
 from torch import fx
+from torch.fx.node import Node
 from torch.fx.passes.shape_prop import ShapeProp
 
 # Create an alias for module input type to avoid littering pyre-ignore for Any
 # throughout the file.
 Input = Any
 _LOGGER: logging.Logger = logging.getLogger(__name__)
 
 PassFunc = Callable[[fx.GraphModule, Input], fx.GraphModule]
 
 RELAX_ACCURACY_FAILURE: bool = False
 FINAL_CHECK_ATOL_MULTIPLIER: float = 10
 FINAL_CHECK_RTOL_MULTIPLIER: float = 10
 
+# A global override of the alternative batch size used in validate_variable_batch_sizes
+ALTERNATIVE_BATCH_SIZE_OVERRIDE: Optional[int] = None
+# If exception during validate_variable_batch_sizes should be thrown
+ALTERNATIVE_BATCH_SIZE_EXCEPTION_SHOULD_THROW: bool = False
+
 
 class RelaxAccuracyCheckMode:
     """
     Basically a context manager that controls a global variable that controls
     the accuracy check mode. Use it like
     with RelaxAccuracyCheckMode(True):
         fx2trt()
@@ -79,14 +89,54 @@
             FINAL_CHECK_RTOL_MULTIPLIER,
         ) = self._old_mode
         _LOGGER.info(
             f"Restored old relaxed accuracy check mode: {RELAX_ACCURACY_FAILURE=}, {FINAL_CHECK_ATOL_MULTIPLIER=}, {FINAL_CHECK_RTOL_MULTIPLIER=}"
         )
 
 
+@contextlib.contextmanager
+def override_alternative_batch_size(alternative_batch_size: int = -1):
+    """
+    A context manager to override alternative_batch_size
+
+    Example:
+
+    >>> # disables run_alternative_batch_size verification
+    >>> with override_alternative_batch_size(-1):
+    >>>     fx2ait()
+    """
+
+    global ALTERNATIVE_BATCH_SIZE_OVERRIDE
+    old_value = ALTERNATIVE_BATCH_SIZE_OVERRIDE
+    ALTERNATIVE_BATCH_SIZE_OVERRIDE = alternative_batch_size
+    _LOGGER.info(f"Override {ALTERNATIVE_BATCH_SIZE_OVERRIDE=} ({old_value=})")
+    try:
+        yield
+    finally:
+        ALTERNATIVE_BATCH_SIZE_OVERRIDE = old_value
+        _LOGGER.info(f"Restored old value: {ALTERNATIVE_BATCH_SIZE_OVERRIDE=})")
+
+
+@contextlib.contextmanager
+def override_alternative_batch_size_exception_should_throw(
+    exception_should_throw: bool,
+):
+    """
+    A context manager to set if exception during alternative batch size verification
+    should be thrown.
+    """
+    global ALTERNATIVE_BATCH_SIZE_EXCEPTION_SHOULD_THROW
+    old_value = ALTERNATIVE_BATCH_SIZE_EXCEPTION_SHOULD_THROW
+    ALTERNATIVE_BATCH_SIZE_EXCEPTION_SHOULD_THROW = exception_should_throw
+    try:
+        yield
+    finally:
+        ALTERNATIVE_BATCH_SIZE_EXCEPTION_SHOULD_THROW = old_value
+
+
 def chain_passes(*passes: PassFunc) -> PassFunc:
     """
     Chains a sequence of pass functions to form a single pass function
     """
 
     def parent_pass(module: fx.GraphModule, input: Input) -> fx.GraphModule:
         for pass_ in passes:
@@ -96,19 +146,36 @@
         return module
 
     return parent_pass
 
 
 # (TODO(shirongwu): Add exception notification for fblearner flow when available, notify oncall
 # on pass that failed accuracy check.
-def validate_inference(rtol=None, atol=None):
+def validate_inference(
+    rtol=None, atol=None, run_alternative_batch_size: int = -1
+) -> "Decorator":
+    """
+    Returns a decorator on a PassFunc to sanity check the model outputs
+    difference before/after the transformation is within tolerance.
+
+    Args:
+        rtol: reletive tolerance
+        atol: absoluate tolerance
+        run_alternative_batch_size (int):
+            In addition to running inference at original batch size in the
+            input, also run at an alternative batch size. If set to -1, do not
+            run at alternative batch size. It must be smaller than the original
+            batch size. This is useful to check the model can run at different
+            batch sizes. Usually we can set this to 1.
+    """
+
     def _validate_inference(pass_: PassFunc) -> PassFunc:
         """
-        Wraps a pass function to validate that its inference results before and
-        after the pass run should be `close`.
+        A decorator to wrap a pass function to validate that its inference
+        results before and after the pass run should be `close`.
         """
 
         @wraps(pass_)
         def pass_with_validation(
             module: fx.GraphModule,
             input: Input,
             *args,
@@ -158,14 +225,128 @@
             return processed_module
 
         return pass_with_validation
 
     return _validate_inference
 
 
+def validate_variable_batch_sizes(run_alternative_batch_size: int = -1) -> "Decorator":
+    """
+    Returns a decorator on a PassFunc to verify the model can run with
+    different batch sizes before/after the transformation is within tolerance.
+
+    Args:
+        run_alternative_batch_size (int):
+            In addition to running inference at original batch size in the
+            input, also run at an alternative batch size. If set to -1, do not
+            run at alternative batch size. It must be smaller than the original
+            batch size. This is useful to check the model can run at different
+            batch sizes. Usually we can set this to 1.
+
+            If the global variable `ALTERNATIVE_BATCH_SIZE_OVERRIDE` is set, it
+            overrides `run_alternative_batch_size`.
+            `ALTERNATIVE_BATCH_SIZE_OVERRIDE` can be set via:
+
+                with override_alternative_batch_size(...): ...
+    """
+
+    def _run_alternative_batch_size(pass_: PassFunc) -> PassFunc:
+        """
+        A decorator for PassFunc to check that the model (both before and after
+        the transformation by pass func) can run at alternative batch size.
+        """
+
+        @wraps(pass_)
+        def pass_with_validation(
+            module: fx.GraphModule,
+            input: Input,
+            *args,
+            **kwargs,
+        ) -> fx.GraphModule:
+            _run_alternative_batch_size = (
+                ALTERNATIVE_BATCH_SIZE_OVERRIDE
+                if ALTERNATIVE_BATCH_SIZE_OVERRIDE is not None
+                else run_alternative_batch_size
+            )
+
+            if _run_alternative_batch_size < 0:
+                return pass_(module, input, *args, **kwargs)
+
+            if not isinstance(input, (list, tuple)):
+                _LOGGER.info(
+                    f"Skip run_alternative_batch_size: input must be list, tuple. Actual: {type(input)}"
+                )
+                return pass_(module, input, *args, **kwargs)
+
+            if not all(isinstance(x, torch.Tensor) for x in input):
+                _LOGGER.info(
+                    "Skip run_alternative_batch_size: input elements must all be tensors"
+                )
+                return pass_(module, input, *args, **kwargs)
+
+            if not all(len(x.shape) > 0 for x in input):
+                _LOGGER.info(
+                    "Skip run_alternative_batch_size: some input tensor(s) are scalar"
+                )
+                return pass_(module, input, *args, **kwargs)
+
+            batch_size_candidates = {x.shape[0] for x in input}
+            if len(batch_size_candidates) > 1:
+                _LOGGER.info(
+                    f"Skip run_alternative_batch_size: input tensors' first dim must be the same, actual: {batch_size_candidates}"
+                )
+                return pass_(module, input, *args, **kwargs)
+
+            batch_size = next(iter(batch_size_candidates))
+            assert (
+                _run_alternative_batch_size <= batch_size
+            ), f"{_run_alternative_batch_size=} must be smaller or equal to {batch_size=}"
+
+            input_alt_bs = [x[:_run_alternative_batch_size, ...] for x in input]
+
+            def run_module(mod, stage: str):
+                """Run module with full bs and alternative bs"""
+                _LOGGER.info(
+                    f"Running {stage} model at alternative batch size: {_run_alternative_batch_size}"
+                )
+                try:
+                    mod(*input)
+                    mod(*input_alt_bs)
+                except Exception as e:
+                    _LOGGER.warning(
+                        f"Failed running {stage} module at full or alternative batch size: {e}"
+                    )
+                    diagnostics.write(
+                        "lowering_diagnostics",
+                        json.dumps(
+                            {
+                                "validate_variable_batch_sizes_exception": repr(e),
+                                "validate_variable_batch_sizes_exception_type": type(
+                                    e
+                                ).__name__,
+                                "validate_variable_batch_sizes_exception_traceback": "".join(
+                                    TracebackException.from_exception(e).format()
+                                ),
+                            }
+                        ),
+                    )
+                    if ALTERNATIVE_BATCH_SIZE_EXCEPTION_SHOULD_THROW:
+                        raise
+
+            run_module(module, "original")
+            module_after = pass_(module, input, *args, **kwargs)
+            run_module(module_after, "transformed")
+
+            return module_after
+
+        return pass_with_validation
+
+    return _run_alternative_batch_size
+
+
 Decorator = Callable[[Callable], Callable]
 
 
 def decorate_method(dec_for_function: Decorator) -> Decorator:
     def dec_for_method(unbounded_method) -> Callable:
         def decorated_unbounded_method(self, *args, **kwargs):
             @dec_for_function
@@ -265,7 +446,71 @@
     def collect(x: fx.node.Argument) -> fx.node.Argument:
         if isinstance(x, torch.Tensor):
             res.append(x)
         return x
 
     fx.node.map_aggregate(arg, collect)
     return res
+
+
+class InputOutputDtypeInferInterpreter(torch.fx.Interpreter):
+    """
+    Interprete a graph to propagate the output tensor dtype from its inputs, extracing
+    input and output graph node that need dtype cast to float32/bfloat16.
+    """
+
+    def __init__(self, module: torch.fx.GraphModule):
+        super().__init__(module)
+        self.need_cast_to_float32 = []
+        self.need_cast_to_bfloat = []
+
+    def _need_cast(self, node: Node, run_result) -> None:
+        if node.op == "placeholder" and (
+            run_result.dtype not in (torch.int32, torch.int64)
+        ):
+            _LOGGER.info(
+                f"Encountered node: {node.format_node()} need dtype cast to float32."
+            )
+            self.need_cast_to_float32.append(node)
+        # Process node that will be used as final output
+        elif "output" in set(i.name for i in node.users.keys()):
+            if run_result.dtype not in (torch.int32, torch.int64):
+                _LOGGER.info(
+                    f"Encountered node: {node.format_node()} need dtype cast to bfloat16."
+                )
+                self.need_cast_to_bfloat.append(node)
+
+    def run_node(self, n: Node) -> Any:
+        run_result = super().run_node(n)
+
+        if torch.is_tensor(run_result):
+            n.meta["tensor_dtype"] = run_result.dtype
+            self._need_cast(n, run_result)
+        return run_result
+
+
+def apply_bfloat_float_conversion(
+    gm: torch.fx.GraphModule, inputs: Any, name: str
+) -> None:
+    _LOGGER.info("Apply bfloat-float32 conversion on {name}")
+    interpreter = InputOutputDtypeInferInterpreter(gm)
+    interpreter.run(*inputs)
+
+    def to_bfloat(x):
+        return x.to(torch.bfloat16)
+
+    def to_float(x):
+        return x.to(torch.float32)
+
+    for node in interpreter.need_cast_to_float32:
+        with gm.graph.inserting_after(node):
+            cast = gm.graph.call_function(
+                to_float,
+                (node,),
+                {},
+            )
+            node.replace_all_uses_with(cast)
+
+    for node in interpreter.need_cast_to_bfloat:
+        with gm.graph.inserting_after(node):
+            cast = gm.graph.call_function(to_bfloat, (node,), {})
+            node.replace_all_uses_with(cast)
```

## torch_tensorrt/fx/tools/common_fx2trt.py

```diff
@@ -1,12 +1,14 @@
 import logging
 import time
 import unittest
 from typing import Callable, List, Optional, Set, Tuple
 
+# @manual=//deeplearning/trt/python:py_tensorrt
+import tensorrt as trt
 import torch
 import torch.fx
 
 import torch_tensorrt.fx.tracer.acc_tracer.acc_tracer as acc_tracer
 import torch_tensorrt.fx.tracer.dispatch_tracer.aten_tracer as aten_tracer
 from torch.fx.experimental.normalize import NormalizeArgs
 from torch.fx.passes import shape_prop
@@ -253,14 +255,16 @@
         mod.eval()
         mod = acc_tracer.trace(mod, inputs)
 
         if apply_passes is not None:
             pass_tracer = chain_passes(*apply_passes)
             mod = pass_tracer(mod, inputs)
 
+        if trt.__version__ >= "8.6":
+            test_implicit_batch_dim = False
         if test_implicit_batch_dim:
             interp = TRTInterpreter(mod, InputTensorSpec.from_tensors(inputs))
             super().run_test(
                 mod, inputs, expected_ops, unexpected_ops, interp, rtol, atol, precision
             )
 
         if test_explicit_batch_dim:
```

## torch_tensorrt/fx/tools/model_packager.py

```diff
@@ -47,28 +47,49 @@
     model = flatten_model(model)
 
     INDENT = "    "
     lines = [
         "",
         "import torch",
         "from torch import nn",
+    ]
+    code = str(model.code)
+
+    import_modules = set()
+    import_map = {
+        "torch_tensorrt_fx_tracer_acc_tracer_acc_ops": "torch_tensorrt.fx.tracer.acc_tracer.acc_ops",
+        "torch_tensorrt_fx_passes_lower_basic_pass": "torch_tensorrt.fx.passes.lower_basic_pass",
+    }
+    for line in code.split("\n"):
+        for k, v in import_map.items():
+            if k in line:
+                sub_string = line.split("(")[0].split()[-1]
+                if sub_string.startswith(k):
+                    mod = sub_string.replace(k + "_", "")
+                    import_modules.add(
+                        "from " + v + " import " + mod + " as " + sub_string
+                    )
+    for mod in sorted(import_modules):
+        lines.append(mod)
+
+    lines += [
         "",
         "",
         "class ExportedModule(nn.Module):",
         f"{INDENT}def __init__(self):",
         f"{INDENT * 2}super().__init__()",
     ]
+
     for k, v in model._holder.named_parameters():
         shape = ", ".join([str(i) for i in v.shape])
         rand_func = "randn" if torch.is_floating_point(v) else "randint"
         int_range = "" if torch.is_floating_point(v) else "0, 5, "
         lines.append(
             f"{INDENT * 2}self.{k} = nn.Parameter(torch.{rand_func}({int_range}{shape}, dtype={v.dtype}))"
         )
-    code = str(model.code)
 
     def dump(f):
         f.write(prelude)
         f.write("\n".join(lines))
         f.write(
             "\n".join(
                 [
```

## torch_tensorrt/fx/tools/trt_splitter.py

```diff
@@ -30,16 +30,17 @@
                 support_dict[get_acc_ops_name(k)] = None
         elif k not in NO_EXPLICIT_BATCH_DIM_SUPPORT.keys():
             support_dict[get_acc_ops_name(k)] = None
     supported_if_converter_registered = ops.OperatorSupport(support_dict=support_dict)
 
     return ops.chain(
         ops.OpSupports.decline_if_node_in_names(exclude_support_node_name),
-        # 1. Node is not supported if it has args with int64 dtype:
+        # 1. Node is not supported if it has args with int64 or float64 dtype:
         ops.OpSupports.decline_if_input_dtype(torch.int64),
+        ops.OpSupports.decline_if_input_dtype(torch.float64),
         # 2. Node is supported if it has TRT converter:
         supported_if_converter_registered,
     )
 
 
 class TRTSplitterSetting(splitter_base._SplitterSettingBase):
     def __init__(self):
```

## torch_tensorrt/fx/tracer/acc_tracer/acc_normalizer.py

```diff
@@ -65,14 +65,15 @@
     # (tensor_meta_field_name, orginal_field_name)
     # when move_to_qparams is True, we'll move the field to qparams
     # dictionary, otherwise it will stay in TensorMeta itself
     kwargs_to_move_to_acc_out_ty: Optional[
         List[Union[Tuple[str, str, bool], Tuple[str, str]]]
     ]
     needs_shapes_for_normalization: bool
+    skip_normalization_if_none: bool
 
 
 # Dict from (op, target) to NormalizationInfo for that op.
 _normalization_dict: Dict[Tuple[str, Union[str, Callable]], NormalizationInfo] = {}
 
 # Set of all the acc ops.
 _acc_ops: Set[Callable] = set()
@@ -84,14 +85,15 @@
     new_fn_target: Optional[Callable] = None,
     custom_mapping_fn: Optional[Callable] = None,
     kwargs_to_move_to_acc_out_ty: Optional[
         List[Union[Tuple[str, str, bool], Tuple[str, str]]]
     ] = None,
     needs_shapes_for_normalization=False,
     allow_normalize_from_torch_package=False,
+    skip_normalization_if_none=False,
 ):
     if op_and_target[0] == "call_function":
         assert callable(op_and_target[1])
     elif op_and_target[0] == "call_method":
         assert isinstance(op_and_target[1], str)
     elif op_and_target[0] == "call_module":
         assert isinstance(op_and_target[1], type)
@@ -125,14 +127,15 @@
     assert op_and_target not in _normalization_dict.keys()
     norm_info = NormalizationInfo(
         new_fn_target=new_fn_target,  # type: ignore[arg-type]
         arg_replacement_tuples=final_arg_replacement_tuples,
         custom_mapping_fn=custom_mapping_fn,
         kwargs_to_move_to_acc_out_ty=kwargs_to_move_to_acc_out_ty,
         needs_shapes_for_normalization=needs_shapes_for_normalization,
+        skip_normalization_if_none=skip_normalization_if_none,
     )
     _normalization_dict[op_and_target] = norm_info
 
     # If allow_normalize_from_torch_package then add another entry to
     # _normalization_dict where we look for the qualified name of the target with the
     # torch_package module prefix. Note that we leave off any integer at the end of
     # "<torch_package_>" in order to allow for whatever mangling index is used.
@@ -213,22 +216,24 @@
         Union[
             Tuple[Union[str, Tuple[str, ...]], str],
             Tuple[Union[str, Tuple[str, ...]], str, bool],
         ]
     ],
     needs_shapes_for_normalization=False,
     allow_normalize_from_torch_package=False,
+    skip_normalization_if_none=False,
 ):
     def insert(custom_mapping_fn: Callable):
         _insert_fun(
             op_and_target=op_and_target,
             custom_mapping_fn=custom_mapping_fn,
             arg_replacement_tuples=arg_replacement_tuples,  # type: ignore[arg-type]
             needs_shapes_for_normalization=needs_shapes_for_normalization,
             allow_normalize_from_torch_package=allow_normalize_from_torch_package,
+            skip_normalization_if_none=skip_normalization_if_none,
         )
         return custom_mapping_fn
 
     return insert
 
 
 def move_kwargs_to_acc_out_ty(
@@ -359,20 +364,26 @@
         normalized_args: Tuple[Any, ...],
         normalized_kwargs: Dict[str, Any],
     ):
         # If there's a custom mapping function then use it.
         if normalization_info.custom_mapping_fn is not None:
             # For custom mapping, the normalized_kwargs are used for the original op,
             # i.e. *before* custom acc_ops normalization. Do that now.
+            if normalization_info.skip_normalization_if_none:
+                original_args = node.args
+                original_kwargs = node.kwargs
             node.args = normalized_args
             node.kwargs = normalized_kwargs
             new_node = normalization_info.custom_mapping_fn(node, mod)
             # If a new node is returned then use it to replace the old node. Otherwise
             # the custom mapping function did its own replacement, so return early.
             if new_node is None:
+                if normalization_info.skip_normalization_if_none:
+                    node.args = original_args
+                    node.kwargs = original_kwargs
                 return
         else:
             # If there's kwargs_to_move_to_acc_out_ty then use it to setup acc_out_ty in
             # normalized_kwargs, and remove the kwarg from normalized_kwargs.
             move_kwargs_to_acc_out_ty(normalization_info, normalized_kwargs)
 
             # All acc ops are functions. Create a call to the correct acc_ops target using
```

## torch_tensorrt/fx/tracer/acc_tracer/acc_ops.py

```diff
@@ -1,25 +1,28 @@
 # encoding: utf-8
+import logging
 import operator
 import warnings
 
 import torch  # isort:skip
-from typing import cast, Iterable, List, Sequence
+from typing import cast, Iterable, List, Optional, Sequence
 
 import torch.nn as nn
 from torch.fx.passes.shape_prop import _extract_tensor_metadata, TensorMetadata
 
 from . import acc_utils
 from .acc_normalizer import (
     register_acc_op,
     register_acc_op_mapping,
     register_custom_acc_mapper_fn,
 )
 from .acc_op_properties import AccOpProperty, register_acc_op_properties
 
+logger: logging.Logger = logging.getLogger(__name__)
+
 this_arg_is_optional = True
 move_to_qparams = True
 dont_move_to_qparams = False
 
 # A proxy embedding size. We use this for tracing proxy operators using XL
 # weights which we can't load into memory (because they're too large), we
 # instead substitute a smaller weight with embedding size =
@@ -157,14 +160,26 @@
         padding=padding,
         dilation=dilation,
         ceil_mode=ceil_mode,
         return_indices=return_indices,
     )
 
 
+@register_acc_op_mapping(op_and_target=("call_function", nn.functional.normalize))
+@register_acc_op
+def normalize(*, input, p, dim, eps, out):
+    return nn.functional.normalize(
+        input=input,
+        p=p,
+        dim=dim,
+        eps=eps,
+        out=out,
+    )
+
+
 @register_acc_op_mapping(
     op_and_target=("call_function", nn.functional.adaptive_avg_pool2d)
 )
 @register_acc_op
 def adaptive_avg_pool2d(*, input, output_size):
     return nn.functional.adaptive_avg_pool2d(input=input, output_size=output_size)
 
@@ -360,17 +375,18 @@
         with node.graph.inserting_before(node):
             getitem_node = node.graph.call_function(
                 getitem, kwargs={"input": input_obj, "idx": idx}
             )
             getitem_node.meta = node.meta.copy()
             return getitem_node
 
-    assert (
-        input_obj_type == torch.Tensor
-    ), f"Expected torch.Tensor type for {input_obj_type}"
+    assert input_obj_type in [
+        torch.Tensor,
+        torch.nn.parameter.Parameter,
+    ], f"Expected torch.Tensor type for {input_obj_type}"
     assert (
         attr_name == "shape" or attr_name == "device" or attr_name == "dtype"
     ), f"Only supporting shape, device and dtype getattr for now, not {attr_name}"
     if attr_name == "shape":
         func = size
     elif attr_name == "device":
         func = device
@@ -413,15 +429,18 @@
 
 
 @register_acc_op_properties(AccOpProperty.pointwise)
 @register_acc_op_mapping(op_and_target=("call_function", operator.add))
 @register_acc_op_mapping(op_and_target=("call_method", "add"))
 @register_acc_op
 def add(*, input, other):
-    return input + other
+    if not (isinstance(input, torch.Tensor) or isinstance(other, torch.Tensor)):
+        return operator.add(input, other)
+    else:
+        return input + other
 
 
 @register_acc_op_properties(AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_method", "unsqueeze"))
 @register_acc_op_mapping(op_and_target=("call_function", torch.unsqueeze))
 @register_acc_op
 def unsqueeze(*, input, dim: int):
@@ -438,22 +457,35 @@
 
 @register_custom_acc_mapper_fn(
     op_and_target=("call_method", "repeat"),
     arg_replacement_tuples=[
         ("input", "input"),
         ("*", "sizes"),
     ],
+    skip_normalization_if_none=True,
 )
-def repeat_mapper(node: torch.fx.Node, _: nn.Module) -> torch.fx.Node:
+def repeat_mapper(node: torch.fx.Node, _: nn.Module) -> Optional[torch.fx.Node]:
     """
     Map repeat to tile.
     """
     with node.graph.inserting_before(node):
         inputs = node.kwargs["input"]
         dims = node.kwargs["sizes"]
+        # Skip repeat mapping when the list of dims is not all ints (ie. contains
+        # some calculated value). torch.tile cannot support cases where dims
+        # are Proxy nodes
+        if (
+            isinstance(dims, (list, tuple))
+            and len(dims) > 0
+            and not all(isinstance(x, int) for x in dims)
+        ):
+            logger.info(
+                "Not mapping repeat to an acc op. We can't handle variable dims."
+            )
+            return
         new_node = node.graph.create_node(
             "call_function",
             tile,
             kwargs={"input": inputs, "dims": dims},
             name=f"{node.name}_repeat_map",
         )
         new_node.meta = node.meta.copy()
@@ -464,31 +496,35 @@
     op_and_target=("call_method", "repeat_interleave"),
     arg_replacement_tuples=[
         ("input", "input"),
         ("repeats", "repeats"),
         ("dim", "dim", this_arg_is_optional),
         ("output_size", "output_size", this_arg_is_optional),
     ],
+    skip_normalization_if_none=True,
 )
 @register_custom_acc_mapper_fn(
     op_and_target=("call_function", torch.repeat_interleave),
     arg_replacement_tuples=[
         ("input", "input"),
         ("repeats", "repeats"),
         ("dim", "dim", this_arg_is_optional),
         ("output_size", "output_size", this_arg_is_optional),
     ],
+    skip_normalization_if_none=True,
 )
 def repeat_interleave_mapper(node: torch.fx.Node, _: nn.Module):
     input_node = node.kwargs["input"]
     repeats = cast(int, node.kwargs["repeats"])
     dim = node.kwargs["dim"]
-    assert (
-        type(repeats) is int
-    ), "We currently only support `repeat_interleave` with int repeats"
+    if not (type(repeats) is int):
+        logger.info(
+            "Not mapping repeat_interleave to an acc op. We currently only support `repeat_interleave` with int repeats"
+        )
+        return
     rank = node.meta["tensor_rank"]
     if dim is None:
         repeat_dim = rank - 1
     else:
         assert type(dim) is int, "dim should be an int"
         repeat_dim = dim
     tile_dims = [1] * (rank + 1)
@@ -822,14 +858,26 @@
 
 
 @register_custom_acc_mapper_fn(
     op_and_target=("call_function", nn.functional.dropout),
     arg_replacement_tuples=[("input", "input")],
 )
 @register_custom_acc_mapper_fn(
+    op_and_target=("call_function", nn.functional.dropout1d),
+    arg_replacement_tuples=[("input", "input")],
+)
+@register_custom_acc_mapper_fn(
+    op_and_target=("call_function", nn.functional.dropout2d),
+    arg_replacement_tuples=[("input", "input")],
+)
+@register_custom_acc_mapper_fn(
+    op_and_target=("call_function", nn.functional.dropout3d),
+    arg_replacement_tuples=[("input", "input")],
+)
+@register_custom_acc_mapper_fn(
     op_and_target=("call_method", "detach"), arg_replacement_tuples=[("input", "input")]
 )
 @register_custom_acc_mapper_fn(
     op_and_target=("call_function", torch.detach),
     arg_replacement_tuples=[("input", "input")],
 )
 def dropout_mapper(node: torch.fx.Node, mod: nn.Module):
@@ -1051,26 +1099,42 @@
 
 @register_acc_op_properties(AccOpProperty.pointwise)
 @register_acc_op_mapping(op_and_target=("call_function", torch.sub))
 @register_acc_op_mapping(op_and_target=("call_function", operator.sub))
 @register_acc_op_mapping(op_and_target=("call_method", "sub"))
 @register_acc_op
 def sub(*, input, other):
-    return input - other
+    if not (isinstance(input, torch.Tensor) or isinstance(other, torch.Tensor)):
+        return operator.sub(input, other)
+    else:
+        return input - other
 
 
 @register_acc_op_properties(AccOpProperty.pointwise)
 @register_acc_op_mapping(op_and_target=("call_function", torch.mul))
 @register_acc_op_mapping(op_and_target=("call_function", operator.mul))
 @register_acc_op_mapping(op_and_target=("call_method", "mul"))
 @register_acc_op
 def mul(*, input, other):
     return input * other
 
 
+@register_acc_op_mapping(
+    op_and_target=("call_function", torch.ops.aten.threshold_backward.default),
+    arg_replacement_tuples=[
+        ("grad", "grad"),
+        ("self", "input"),
+        ("threshold", "threshold"),
+    ],
+)
+@register_acc_op
+def threshold_backward(*, grad, input, threshold):
+    return torch.ops.aten.threshold_backward.default(grad, input, threshold)
+
+
 @register_custom_acc_mapper_fn(
     op_and_target=("call_method", "div"),
     arg_replacement_tuples=[
         ("input", "input"),
         ("other", "other"),
         ("rounding_mode", "rounding_mode", this_arg_is_optional),
     ],
@@ -1363,15 +1427,15 @@
     ), "We currently do not support `std` with dim=None and keepdim=None"
 
     with node.graph.inserting_before(node):
         # mean(X)
         mean_kwargs = {
             "input": input_node,
             "dim": dim,
-            "keepdim": keepdim,
+            "keepdim": True,
         }
         mean_node = node.graph.call_function(mean, kwargs=mean_kwargs)
         mean_node.meta["type"] = torch.Tensor
         # X-mean(X)
         sub_kwargs = {
             "input": input_node,
             "other": mean_node,
@@ -1381,23 +1445,23 @@
         # pow(X-mean(X))
         pow_kwargs = {
             "input": sub_node,
             "exponent": 2.0,
         }
         pow_node = node.graph.call_function(pow, kwargs=pow_kwargs)
         pow_node.meta["type"] = torch.Tensor
-        # sum(pow(X-mean(X))))/N
+        # mean(pow(X-mean(X)))
         post_mean_kwargs = {
             "input": pow_node,
             "dim": dim,
             "keepdim": keepdim,
         }
         post_mean_node = node.graph.call_function(mean, kwargs=post_mean_kwargs)
         post_mean_node.meta["type"] = torch.Tensor
-        # sqrt(sum(pow(X-mean(X))))/N)
+        # sqrt( mean(pow(X-mean(X))) )
         sqrt_kwargs = {
             "input": post_mean_node,
         }
         sqrt_node = node.graph.call_function(sqrt, kwargs=sqrt_kwargs)
         sqrt_node.meta["type"] = torch.Tensor
 
         output_node = sqrt_node
@@ -1649,20 +1713,34 @@
 @register_acc_op
 def fmod(*, input, other):
     return torch.fmod(input=input, other=other)
 
 
 @register_acc_op_properties(AccOpProperty.pointwise, AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_function", torch.sigmoid))
+@register_acc_op_mapping(
+    op_and_target=("call_function", torch.ops.aten.sigmoid.default)
+)
 @register_acc_op_mapping(op_and_target=("call_method", "sigmoid"))
 @register_acc_op
 def sigmoid(*, input):
     return torch.sigmoid(input=input)
 
 
+@register_acc_op_properties(AccOpProperty.pointwise)
+@register_acc_op_mapping(
+    op_and_target=("call_function", torch.ops.aten.sigmoid_backward.default)
+)
+@register_acc_op_mapping(op_and_target=("call_method", "sigmoid_backward"))
+@register_acc_op
+# first argument's name needs to be input to use same_shape_and_dtype_as_input
+def sigmoid_backward(*, input, dest):
+    return torch.ops.aten.sigmoid_backward(grad_output=input, output=dest)
+
+
 @register_acc_op_properties(AccOpProperty.pointwise, AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_function", torch.sinh))
 @register_acc_op
 def sinh(*, input):
     return torch.sinh(input=input)
 
 
@@ -1712,14 +1790,31 @@
 @register_acc_op_properties(AccOpProperty.pointwise, AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_function", torch.log))
 @register_acc_op
 def log(*, input):
     return torch.log(input=input)
 
 
+@register_acc_op_properties(AccOpProperty.unary)
+@register_acc_op_mapping(
+    op_and_target=("call_function", torch.nn.functional.log_softmax),
+    arg_replacement_tuples=[
+        ("input", "input"),
+        ("dim", "dim"),
+        ("dtype", "dtype", this_arg_is_optional),
+    ],
+)
+@register_acc_op
+def log_softmax(*, input, dim, dtype=None):
+    """
+    _stacklevel are ignored here.
+    """
+    return torch.nn.functional.log_softmax(input=input, dim=dim, dtype=dtype)
+
+
 @register_acc_op_properties(AccOpProperty.pointwise, AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_function", torch.sqrt))
 @register_acc_op_mapping(op_and_target=("call_method", "sqrt"))
 @register_acc_op
 def sqrt(*, input):
     return torch.sqrt(input=input)
 
@@ -1769,15 +1864,18 @@
 
 
 @register_acc_op_properties(AccOpProperty.pointwise, AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_function", operator.neg))
 @register_acc_op_mapping(op_and_target=("call_function", torch.neg))
 @register_acc_op
 def neg(*, input):
-    return torch.neg(input=input)
+    if not isinstance(input, torch.Tensor):
+        return operator.neg(input)
+    else:
+        return torch.neg(input=input)
 
 
 @register_acc_op_properties(AccOpProperty.pointwise, AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_function", torch.floor))
 @register_acc_op
 def floor(*, input):
     return torch.floor(input=input)
@@ -2278,21 +2376,23 @@
         compressed_indices_mapping=compressed_indices_mapping,
         include_last_offset=include_last_offset,
     )
 
 
 @register_acc_op_properties(AccOpProperty.pointwise, AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_function", torch.sin))
+@register_acc_op_mapping(op_and_target=("call_method", "sin"))
 @register_acc_op
 def sin(*, input):
     return torch.sin(input=input)
 
 
 @register_acc_op_properties(AccOpProperty.pointwise, AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_function", torch.cos))
+@register_acc_op_mapping(op_and_target=("call_method", "cos"))
 @register_acc_op
 def cos(*, input):
     return torch.cos(input=input)
 
 
 @register_acc_op_properties(AccOpProperty.pointwise, AccOpProperty.unary)
 @register_acc_op_mapping(op_and_target=("call_function", torch.tan))
@@ -2310,21 +2410,61 @@
 
 @register_acc_op_mapping(op_and_target=("call_function", operator.getitem))
 @register_acc_op
 def getitem(*, input, idx):
     return input[idx]
 
 
-@register_acc_op_mapping(op_and_target=("call_function", torch.nan_to_num))
-@register_acc_op_mapping(op_and_target=("call_method", "nan_to_num"))
 @register_acc_op
-def nan_to_num(*, input, nan=0.0, posinf=None, neginf=None):
+def nan_to_num(*, input, nan=None, posinf=None, neginf=None):
     return torch.nan_to_num(input, nan=nan, posinf=posinf, neginf=neginf)
 
 
+@register_custom_acc_mapper_fn(
+    op_and_target=("call_function", torch.nan_to_num),
+    arg_replacement_tuples=[
+        ("input", "input"),
+        ("nan", "nan"),
+        ("posinf", "posinf"),
+        ("neginf", "neginf"),
+    ],
+)
+@register_custom_acc_mapper_fn(
+    op_and_target=("call_method", "nan_to_num"),
+    arg_replacement_tuples=[
+        ("input", "input"),
+        ("nan", "nan"),
+        ("posinf", "posinf"),
+        ("neginf", "neginf"),
+    ],
+)
+def custom_nan_to_num_mapper(node: torch.fx.Node, mod: nn.Module) -> torch.fx.Node:
+    nan_val, posinf, neginf = (
+        node.kwargs["nan"],
+        node.kwargs["posinf"],
+        node.kwargs["neginf"],
+    )
+    if nan_val is None:
+        nan_val = 0
+    if posinf is None:
+        posinf = torch.finfo(torch.float16).max
+    if neginf is None:
+        neginf = torch.finfo(torch.float16).min
+    kwargs = {
+        "input": node.kwargs["input"],
+        "nan": nan_val,
+        "posinf": posinf,
+        "neginf": neginf,
+    }
+    with node.graph.inserting_before(node):
+        new_node = node.graph.call_function(nan_to_num, kwargs=kwargs)
+    new_node.meta = node.meta.copy()
+    return new_node
+
+
 @register_acc_op_properties(AccOpProperty.unary)
 @register_acc_op_mapping(
     op_and_target=("call_method", "expand"),
     arg_replacement_tuples=[
         ("input", "input"),
         ("*", "sizes"),
     ],
@@ -2418,15 +2558,18 @@
         ("shape", "shape"),
     ],
     kwargs_to_move_to_acc_out_ty=[("shape", "shape")],
 )
 @register_acc_op
 def reshape(*, input, acc_out_ty=None):
     assert acc_out_ty is not None
-    return input.reshape(acc_out_ty.shape)
+    shape = acc_out_ty.shape
+    if len(shape) == 1 and not isinstance(shape[0], int):
+        return input.reshape(shape[0])
+    return input.reshape(shape)
 
 
 @register_custom_acc_mapper_fn(
     op_and_target=("call_method", "reshape"),
     arg_replacement_tuples=[
         ("input", "input"),
         ("*", "shape"),
@@ -2974,30 +3117,14 @@
         raise RuntimeError(
             f"Expected int, Iterable or Tensor for "
             f"indices_or_sections arg, got: {type(indices_or_sections)}"
         )
 
 
 @register_acc_op_mapping(
-    op_and_target=("call_method", "new_ones"),
-    arg_replacement_tuples=[
-        ("input", "input"),
-        ("size", "size"),
-        ("dtype", "dtype", this_arg_is_optional),
-        ("device", "device", this_arg_is_optional),
-        ("requires_grad", "requires_grad", this_arg_is_optional),
-    ],
-)
-@register_acc_op
-def new_ones(*, input, size, dtype=None, device=None, requires_grad=False):
-    assert requires_grad is False, f"requires_grad != False, it is {requires_grad}"
-    return input.new_ones(size, dtype=dtype, device=device)
-
-
-@register_acc_op_mapping(
     op_and_target=("call_method", "new_empty"),
     arg_replacement_tuples=[
         ("input", "input"),
         ("size", "size"),
         ("dtype", "dtype", this_arg_is_optional),
         ("device", "device", this_arg_is_optional),
         ("requires_grad", "requires_grad", this_arg_is_optional),
@@ -3077,41 +3204,14 @@
         proxy_shape: shape of substitute tensor
         dtype: dtype of substitute tensor
     """
     return torch.zeros(proxy_shape, dtype=dtype)
 
 
 @register_custom_acc_mapper_fn(
-    op_and_target=("call_function", torch.nn.functional.log_softmax),
-    arg_replacement_tuples=[
-        ("input", "input"),
-        ("dim", "dim"),
-        ("dtype", "dtype"),
-    ],
-)
-def log_softmax_mapper(node: torch.fx.Node, _: torch.nn.Module) -> torch.fx.Node:
-    with node.graph.inserting_after(node):
-
-        softmax_kwargs = {
-            "input": node.kwargs["input"],
-            "dim": node.kwargs["dim"],
-            "dtype": node.kwargs["dtype"],
-        }
-        softmax_node = node.graph.call_function(softmax, kwargs=softmax_kwargs)
-        softmax_node.meta = node.meta.copy()
-
-    with softmax_node.graph.inserting_after(softmax_node):
-        log_kwargs = {"input": softmax_node}
-        log_node = node.graph.call_function(log, kwargs=log_kwargs)
-        log_node.meta = node.meta.copy()
-
-        return log_node
-
-
-@register_custom_acc_mapper_fn(
     op_and_target=("call_function", torch.nn.functional.softplus),
     arg_replacement_tuples=[
         ("input", "input"),
         ("beta", "beta", this_arg_is_optional),
         ("threshold", "threshold", this_arg_is_optional),
     ],
 )
@@ -3252,12 +3352,130 @@
         add_node = node.graph.create_node(
             "call_function", add, kwargs=add_kwargs, name=f"{node.name}_add"
         )
         add_node.meta = node.meta.copy()
         return add_node
 
 
+@register_acc_op_mapping(op_and_target=("call_function", torch.clone))
+@register_acc_op_mapping(op_and_target=("call_method", "clone"))
+@register_acc_op
+def clone(*, input):
+    return torch.clone(input)
+
+
+@register_acc_op_mapping(op_and_target=("call_function", torch.unbind))
+@register_acc_op
+def unbind(*, input, dim=0):
+    return torch.unbind(input, dim=dim)
+
+
+@register_acc_op_mapping(
+    op_and_target=("call_function", torch.nn.functional.group_norm),
+    arg_replacement_tuples=[
+        ("input", "input"),
+        ("num_groups", "num_groups"),
+        ("weight", "weight"),
+        ("bias", "bias"),
+        ("eps", "eps"),
+    ],
+)
+@register_acc_op
+def group_norm(*, input, num_groups, weight=None, bias=None, eps=1e-05):
+    return torch.nn.functional.group_norm(
+        input, num_groups, weight=weight, bias=bias, eps=eps
+    )
+
+
+@register_acc_op_mapping(op_and_target=("call_method", "long"))
+@register_acc_op
+def long(*, input):
+    return input.long()
+
+
+@register_acc_op_mapping(
+    op_and_target=("call_method", "new_full"),
+    arg_replacement_tuples=[
+        ("input", "input"),
+        ("size", "size"),
+        ("fill_value", "fill_value"),
+        ("dtype", "dtype", this_arg_is_optional),
+        ("device", "device", this_arg_is_optional),
+        ("requires_grad", "requires_grad", this_arg_is_optional),
+    ],
+)
+@register_acc_op
+def new_full(*, input, size, fill_value, dtype=None, device=None, requires_grad=False):
+    return input.new_full(size, fill_value=fill_value, dtype=dtype, device=device)
+
+
+@register_acc_op_mapping(op_and_target=("call_function", torch.full_like))
+@register_acc_op
+def full_like(*, input, fill_value, dtype=None, device=None):
+    return torch.full_like(
+        input=input, fill_value=fill_value, dtype=dtype, device=device
+    )
+
+
+@register_acc_op_mapping(
+    op_and_target=("call_method", "new_ones"),
+    arg_replacement_tuples=[
+        ("input", "input"),
+        ("size", "size"),
+        ("dtype", "dtype", this_arg_is_optional),
+        ("device", "device", this_arg_is_optional),
+        ("requires_grad", "requires_grad", this_arg_is_optional),
+    ],
+)
+@register_acc_op
+def new_ones(*, input, size, dtype=None, device=None, requires_grad=False):
+    assert requires_grad is False, f"requires_grad != False, it is {requires_grad}"
+    return input.new_ones(size, dtype=dtype, device=device)
+
+
+@register_acc_op_mapping(op_and_target=("call_function", torch.ones_like))
+@register_acc_op
+def ones_like(*, input, dtype=None, device=None):
+    return torch.ones_like(input=input, dtype=dtype, device=device)
+
+
+@register_acc_op_mapping(
+    op_and_target=("call_method", "new_zeros"),
+    arg_replacement_tuples=[
+        ("input", "input"),
+        ("size", "size"),
+        ("dtype", "dtype", this_arg_is_optional),
+        ("device", "device", this_arg_is_optional),
+        ("requires_grad", "requires_grad", this_arg_is_optional),
+    ],
+)
+@register_acc_op
+def new_zeros(*, input, size, dtype=None, device=None, requires_grad=False):
+    return input.new_zeros(size, dtype=dtype, device=device)
+
+
+@register_acc_op_mapping(op_and_target=("call_function", torch.zeros_like))
+@register_acc_op
+def zeros_like(*, input, dtype=None, device=None):
+    return torch.zeros_like(input=input, dtype=dtype, device=device)
+
+
+@register_acc_op_mapping(
+    op_and_target=("call_method", "index_add_"),
+)
+@register_acc_op_mapping(op_and_target=("call_function", torch.index_add))
+@register_acc_op
+def index_add(*, input, dim, index, source, alpha=1):
+    return torch.index_add(input, dim, index, source, alpha=alpha)
+
+
+@register_acc_op_mapping(op_and_target=("call_function", torch.masked_select))
+@register_acc_op
+def masked_select(*, input, mask):
+    return torch.masked_select(input=input, mask=mask)
+
+
 ###############################################################################
 
 # Set ops as side-effectul, this prevents them from being optimized away or
 # being folded into constants.
 torch.fx.node._side_effectful_functions.add(xl_weight)
```

## torch_tensorrt/fx/tracer/acc_tracer/acc_tracer.py

```diff
@@ -577,17 +577,23 @@
             changed = _replace_transpose_last_dims_impl(node)
             if changed:
                 gm.graph.eliminate_dead_code()
                 gm.graph.lint()
                 gm.recompile()
 
 
-def rewriter_base_trace(mod, ast_rewriter_allow_list, leaf_module_list):
+def rewriter_base_trace(
+    mod,
+    ast_rewriter_allow_list,
+    leaf_module_list,
+    concrete_args: Optional[Dict[str, Any]] = None,
+):
     rewritten_graph, rewritten_mod = AccRewritingTracer().trace(
         mod,
+        concrete_args,
         ast_rewriter_allow_list=ast_rewriter_allow_list,
         leaf_module_list=leaf_module_list,
     )
 
     assert isinstance(rewritten_mod, nn.Module)
     # Note: use the rewritten_mod here as the root. This is necessary because
     # RewrittenModule includes a new module for the ConditionalExceptionWrapper.
@@ -601,14 +607,16 @@
     remove_exceptions: bool = True,
     use_acc_normalization: bool = True,
     ast_rewriter_allow_list: Optional[Set[Type[nn.Module]]] = None,
     leaf_module_list: Optional[Set[Type[nn.Module]]] = None,
     acc_normalization_block_list: Optional[
         Set[Tuple[str, Union[str, Callable]]]
     ] = None,
+    dont_retrace_gm: bool = False,
+    concrete_args: Optional[Dict[str, Any]] = None,
 ) -> torch.fx.GraphModule:
     """
     Performs tracing and arg normalization specialized for accelerator lowering.
 
     It first rewrites the AST of the module's methods (and all attr methods
     recursively) to transform un-tracable parts of the module to make them
     traceable.
@@ -649,26 +657,35 @@
                                             modules will not be traced into.
 
         acc_normalization_block_list (Optional[Set[Tuple[str, Union[str, Callable]]]]):
                                     Optional set of (op, target) pairs to not apply acc
                                     normalization to. Just like the register_acc_op decarators,
                                     the target can either be a string (e.g. for op == "call_method")
                                     or a callable (e.g. for op == "call_function").
+
+        dont_retrace_gm (bool): Optional bool for whether to re-trace the provided
+                                module if it's a graph module already.
+
     """
     if mod.training:
         warnings.warn(
             "acc_tracer does not support currently support models for training."
             " Calling eval on model before tracing."
         )
         mod.eval()
 
     assert isinstance(sample_inputs, (list, tuple))
 
     # Rewrite the module to make it symbolic traceable, and then trace it.
-    traced = rewriter_base_trace(mod, ast_rewriter_allow_list, leaf_module_list)
+    if dont_retrace_gm and isinstance(mod, torch.fx.GraphModule):
+        traced = mod
+    else:
+        traced = rewriter_base_trace(
+            mod, ast_rewriter_allow_list, leaf_module_list, concrete_args
+        )
 
     # Now remove all assertions and exceptions if requested.
     if remove_assertions:
         _remove_assertions(traced)
     if remove_exceptions:
         _remove_exceptions(traced)
```

## torch_tensorrt/fx/tracer/acc_tracer/acc_utils.py

```diff
@@ -106,15 +106,16 @@
 
 def get_model_info_str(gm: torch.fx.GraphModule, header: Optional[str] = None):
     """
     Print out info of the provided `gm`.
     If `header` is provided then it's included in the printed string.
     """
     ops_and_counts: Dict[Callable, int] = {}
-    placeholder_count = get_attr_count = call_method_count = call_module_count = 0
+    placeholder_count = get_attr_count = 0
+    call_method_count = call_module_count = output_count = 0
     for node in gm.graph.nodes:
         if node.op == "call_function":
             ops_and_counts[node.target] = ops_and_counts.get(node.target, 0) + 1
         elif node.op == "placeholder":
             placeholder_count += 1
         elif node.op == "get_attr":
             get_attr_count += 1
@@ -137,22 +138,31 @@
     if call_method_count != 0:
         model_info_str += f"> WARNING: call_method: {call_method_count}"
 
     # Sort and print all the other ops. Sort so it's deterministic between runs and
     # easier to parse.
     pretty_ops_and_counts: List[Tuple[str, int]] = []
     for op, count in ops_and_counts.items():
-        pretty_ops_and_counts.append((_get_qualified_name(op), count))
+        name = strip_module_prefixes(_get_qualified_name(op))
+        pretty_ops_and_counts.append((name, count))
     pretty_ops_and_counts.sort()
     for op_str, count in pretty_ops_and_counts:
         model_info_str += f"> {op_str}: {count}\n"
 
     return model_info_str
 
 
+def strip_module_prefixes(op_name):
+    return (
+        op_name.replace("torch_tensorrt.fx.tracer.acc_tracer.", "")
+        .replace("glow.fb.fx.acc_tracer.", "")
+        .replace("glow.fb.fx.", "")
+    )
+
+
 def get_unique_attr_name_in_module(mod_traced: torch.fx.GraphModule, name: str) -> str:
     """
     Make sure the name is unique (in a module) and can represents an attr.
     """
     # Delete all characters that are illegal in a Python identifier.
     name = re.sub("[^0-9a-zA-Z_]+", "_", name)
     if name[0].isdigit():
```

## torch_tensorrt/fx/tracer/dispatch_tracer/aten_tracer.py

```diff
@@ -5,15 +5,15 @@
 
 import torch
 
 if not torch.__version__.startswith("1"):
     import torch._dynamo as torchdynamo
 
 from torch.fx.passes.infra.pass_base import PassResult
-
+from torch_tensorrt.fx.utils import req_torch_version
 from torch_tensorrt.fx.passes.lower_basic_pass_aten import (
     compose_bmm,
     compose_chunk,
     compose_getitem_slice,
     remove_ops,
     replace_aten_op_with_indices,
     replace_aten_reshape_alias_with_replace,
@@ -38,36 +38,36 @@
     """
 
     def __init__(
         self,
         capture_scalar_outputs: bool = True,
         guard_nn_modules: bool = True,
         dynamic_shapes: bool = True,
-        specialize_int_float: bool = True,
+        specialize_int: bool = True,
         verbose: bool = True,
     ) -> None:
 
         self.capture_scalar_outputs = capture_scalar_outputs
         self.guard_nn_modules = guard_nn_modules
         self.dynamic_shapes = dynamic_shapes
-        self.specialize_int_float = specialize_int_float
+        self.specialize_int = specialize_int
         self.verbose = verbose
 
     def activate(self) -> None:
         torchdynamo.config.capture_scalar_outputs = self.capture_scalar_outputs
         torchdynamo.config.guard_nn_modules = self.guard_nn_modules
         torchdynamo.config.dynamic_shapes = self.dynamic_shapes
-        torchdynamo.config.specialize_int_float = self.specialize_int_float
+        torchdynamo.config.specialize_int = self.specialize_int
         torchdynamo.config.verbose = self.verbose
 
     def deactivate(self) -> None:
         torchdynamo.config.capture_scalar_outputs = True
         torchdynamo.config.guard_nn_modules = True
         torchdynamo.config.dynamic_shapes = True
-        torchdynamo.config.specialize_int_float = True
+        torchdynamo.config.specialize_int = True
         torchdynamo.config.verbose = True
 
 
 @contextmanager
 def using_config(config: DynamoConfig) -> Generator[DynamoConfig, None, None]:
     config.activate()
     try:
@@ -87,32 +87,28 @@
         sys.setrecursionlimit(limit)
     try:
         yield
     finally:
         sys.setrecursionlimit(default)
 
 
+@req_torch_version("2.dev")
 def dynamo_trace(
     f: Callable[..., Value],
     # pyre-ignore
     args: Tuple[Any, ...],
     aten_graph: bool,
     tracing_mode: str = "real",
     dynamo_config: Optional[DynamoConfig] = None,
 ) -> Tuple[torch.fx.GraphModule, Set]:
     """
     TODO: Once we fully migrate to torchdynamo frontend, we will remove
     this config option alltogether.  For now, it helps with quick
     experiments with playing around with TorchDynamo
     """
-    if torch.__version__.startswith("1"):
-        raise ValueError(
-            f"The aten tracer requires Torch version >= 2.0. Detected version {torch.__version__}"
-        )
-
     if dynamo_config is None:
         dynamo_config = DynamoConfig()
     with using_config(dynamo_config), setting_python_recursive_limit(2000):
         torchdynamo.reset()
         try:
             return torchdynamo.export(
                 f,
@@ -127,19 +123,21 @@
             ) from exc
         except Exception as exc:
             raise RuntimeError(
                 "torchdynamo internal error occured. Please see above stacktrace"
             ) from exc
 
 
+@req_torch_version("2.dev")
 def trace(f, args, *rest):
     graph_module, guards = dynamo_trace(f, args, True, "symbolic")
     return graph_module, guards
 
 
+@req_torch_version("2.dev")
 def opt_trace(f, args, *rest):
     """
     Optimized trace with necessary passes which re-compose some ops or replace some ops
     These passes should be general and functional purpose
     """
     passes_list = [
         compose_bmm,
```

## Comparing `torch_tensorrt_fx_only-1.4.0.dev0.dist-info/METADATA` & `torch_tensorrt_fx_only-1.5.0.dev0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-tensorrt-fx-only
-Version: 1.4.0.dev0
+Version: 1.5.0.dev0
 Summary: Unofficial Torch-TensorRT Python package built with FX path only
 Home-page: https://nvidia.github.io/torch-tensorrt
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch (>=1.13.1)
+Requires-Dist: torch (<2.2,>=2.0.1)
 
 # torch_tensorrt
 
 > Ahead of Time (AOT) compiling for PyTorch JIT
 
 Torch-TensorRT is a compiler for PyTorch/TorchScript, targeting NVIDIA GPUs via NVIDIA's TensorRT Deep Learning Optimizer and Runtime. Unlike PyTorch's Just-In-Time (JIT) compiler, Torch-TensorRT is an Ahead-of-Time (AOT) compiler, meaning that before you deploy your TorchScript code, you go through an explicit compile step to convert a standard TorchScript program into an module targeting a TensorRT engine. Torch-TensorRT operates as a PyTorch extention and compiles modules that integrate into the JIT runtime seamlessly. After compilation using the optimized graph should feel no different than running a TorchScript module. You also have access to TensorRT's suite of configurations at compile time, so you are able to specify operating precision (FP32/FP16/INT8) and other settings for your module.
```

### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: torch-tensorrt-fx-only Version: 1.4.0.dev0 Summary:
+Metadata-Version: 2.1 Name: torch-tensorrt-fx-only Version: 1.5.0.dev0 Summary:
 Unofficial Torch-TensorRT Python package built with FX path only Home-page:
 https://nvidia.github.io/torch-tensorrt License: BSD Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: License :: OSI Approved :: BSD License Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: C++ Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Topic ::
 Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Software Development Classifier:
-Topic :: Software Development :: Libraries Requires-Python: >=3.7 Description-
+Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch
-(>=1.13.1) # torch_tensorrt > Ahead of Time (AOT) compiling for PyTorch JIT
+(<2.2,>=2.0.1) # torch_tensorrt > Ahead of Time (AOT) compiling for PyTorch JIT
 Torch-TensorRT is a compiler for PyTorch/TorchScript, targeting NVIDIA GPUs via
 NVIDIA's TensorRT Deep Learning Optimizer and Runtime. Unlike PyTorch's Just-
 In-Time (JIT) compiler, Torch-TensorRT is an Ahead-of-Time (AOT) compiler,
 meaning that before you deploy your TorchScript code, you go through an
 explicit compile step to convert a standard TorchScript program into an module
 targeting a TensorRT engine. Torch-TensorRT operates as a PyTorch extention and
 compiles modules that integrate into the JIT runtime seamlessly. After
```

## Comparing `torch_tensorrt_fx_only-1.4.0.dev0.dist-info/RECORD` & `torch_tensorrt_fx_only-1.5.0.dev0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,70 @@
+torch_tensorrt/dynamo/__init__.py,sha256=6rb8JXuTP7U9vmPGkZ86VJK9uA0FfL7TQ1NlMpMFbII,78
+torch_tensorrt/dynamo/fx_ts_compat/__init__.py,sha256=HFrs3WdJbxrSMnKUCCfdbEvc-wMJEfWR4lmoh_m7weU,459
+torch_tensorrt/dynamo/fx_ts_compat/fx2trt.py,sha256=wEECWNi5C7UKCPfre1PYpknWwXxLOXC5xCdTpKAAB3Y,14997
+torch_tensorrt/dynamo/fx_ts_compat/input_tensor_spec.py,sha256=lO5mOaR6-S2Nd1e3zrjJauYWdhqFTBNLhD9B__Z0AL4,7093
+torch_tensorrt/dynamo/fx_ts_compat/lower.py,sha256=x-_0J8K9kNZ2mnL4DXux5fx9Rpcy9AuPE6viyLu2HZk,14366
+torch_tensorrt/dynamo/fx_ts_compat/lower_setting.py,sha256=7SMeIxR_Jmb5oT4thAzhwdRSnZYRcZ8Q1Dp9LxbUfWg,4407
+torch_tensorrt/dynamo/fx_ts_compat/passes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+torch_tensorrt/dynamo/fx_ts_compat/passes/lower_pass_manager_builder.py,sha256=3YxI0GHsdG_5K_Ntd_hTSpQ_kCM6bX6mz9grUatDyHU,13108
+torch_tensorrt/dynamo/fx_ts_compat/passes/pass_utils.py,sha256=9qXPNO4hcopqZpjPRmLjSFwkIn_AIDd7ujM1JG8ZDas,10929
+torch_tensorrt/dynamo/fx_ts_compat/tools/__init__.py,sha256=SF90jfdL6xvPeyDy3TVSIICz3E6UKbu66KZjvDGpYwQ,49
+torch_tensorrt/dynamo/fx_ts_compat/tools/common_fx2trt.py,sha256=trJUcD0VtLqJL-g9b19nwmDyYXfm_OidfdU3r-nCDG4,15762
+torch_tensorrt/dynamo/fx_ts_compat/tools/trt_minimizer.py,sha256=8fgpqwieya85zmIzX2UYfvc3g7YE6K3zsyuuxSntiwI,3622
 torch_tensorrt/fx/__init__.py,sha256=nyLYMgU8Mr-AH7pPDkKUzVt9-eQCc4nqyFCQ3a-xQXs,553
 torch_tensorrt/fx/converter_registry.py,sha256=qGjOpyLh-3Q1cE5ku9FhcFzzyEGd75EFkrCvA4EJIPQ,831
-torch_tensorrt/fx/diagnostics.py,sha256=oP33VOD7FH0UinORIk76f2XScnROyXA2dNr1Zbqh5Uc,9883
-torch_tensorrt/fx/fx2trt.py,sha256=WFHIOjIWg6_3dOrAHkn_VdgVoSSW0URMIA4rzkLYS9k,14884
-torch_tensorrt/fx/input_tensor_spec.py,sha256=o2EEd-j_AUiiglz2CPVXKN-YIEzR0hluTs3-0-VvLLo,7501
-torch_tensorrt/fx/lower.py,sha256=rshFxUyKNzMu46-oIlwHrXEN6F21UO2iZFhbjGuUh0Q,12922
+torch_tensorrt/fx/diagnostics.py,sha256=2ybpasE4PQYoWOOLROM_PozqvYWg1EJ8p2WzyxYNy60,10067
+torch_tensorrt/fx/fx2trt.py,sha256=a673tgfzODodM-1orMFdWcGLiv0_2wT2D7NyyBV9b5I,15161
+torch_tensorrt/fx/input_tensor_spec.py,sha256=_MDu6HBQ9FZe5eCvgFNWGbpe4kWkTpkIXxpVPqHK8Ww,9575
+torch_tensorrt/fx/lower.py,sha256=2Z2YdaL-LRMXLQLtvnH7q5sdUctJGntOcwOo8rjv64M,13066
 torch_tensorrt/fx/lower_setting.py,sha256=Rvg0Zk5f8MZc8j2LdMzhUKvS-5N2mB3H_0LSnwOD4bE,4861
 torch_tensorrt/fx/observer.py,sha256=-gKfnE1ekiXJwG7yF1ECJuyxaCbtJYFLcQWBMpwL5rs,6021
 torch_tensorrt/fx/trt_module.py,sha256=Fe76XMWClKkb8PdK9cNSydLei_0ErU-M1n0J75EVxHw,9987
 torch_tensorrt/fx/types.py,sha256=ZT80uWmWCvm8LsroEkrOFE53irjqTcabzwn7-8lOQK4,785
-torch_tensorrt/fx/utils.py,sha256=inNNjNpdrYZPOc84tus1okKDp7FBe89ZZPL_N5XH0i8,2688
+torch_tensorrt/fx/utils.py,sha256=D4JIB8GrPSkvo8dqhm9MyoXf0G8gW-dgGFU8QR4BI88,4401
 torch_tensorrt/fx/converters/__init__.py,sha256=kTN6O1SQPQ9KfaGGpVdzs9G7wcHnrWdksfLNutFKP_4,798
-torch_tensorrt/fx/converters/acc_ops_converters.py,sha256=_-_OsVc4y9Ebp3CkkVhyGlcB89Tp6tcrCSKfSAwZVMY,128855
+torch_tensorrt/fx/converters/acc_ops_converters.py,sha256=Uk8RBtuXFNh_GijrMdjfVJ8ETUeEL48qRANKLiycC6c,129037
 torch_tensorrt/fx/converters/activation.py,sha256=DVvyd5d3MSVBcF-bcZngK2Gifzu0q2Byr3UHuKYoOPA,2221
 torch_tensorrt/fx/converters/adaptive_avgpool.py,sha256=zpPyWRhInSnEzt0v0F8cD88hUgjHAzAShq08KR0H5P0,1211
 torch_tensorrt/fx/converters/add.py,sha256=7hmeo77xZ0DIfawGIfuJ9gfC4_dKlbSN36IfuNjFPC0,2521
-torch_tensorrt/fx/converters/aten_ops_converters.py,sha256=NE_vga3eB17KzyBjUID161xqbvK3fbHZck8bEH4M2mo,13705
+torch_tensorrt/fx/converters/aten_ops_converters.py,sha256=H4O5_raWnb-y_X09WQEqEQF89ejwXjGiGTFzdmDI7f4,14228
 torch_tensorrt/fx/converters/batchnorm.py,sha256=NNDWnPCq7t1vJL-NVl6QA1u5ZFSn9F-j3rfCFYrzYOQ,1824
 torch_tensorrt/fx/converters/converter_utils.py,sha256=nJXhi49zIztRzCke4ni_BniLFjqvL9pjdPxssV6jAbA,31945
 torch_tensorrt/fx/converters/convolution.py,sha256=I44QEx9bb__6Qktt9fxh0F3WDN7-7qA6xXh-9BIsrYA,6703
 torch_tensorrt/fx/converters/linear.py,sha256=jgn1TOI0Oi9REACaJQngTGhmIjV27CvWM3-ws_D8rvQ,2914
 torch_tensorrt/fx/converters/maxpool.py,sha256=X_zo1qb-eSkOI43p4T76DsDjmOkVnzcovoapYPgG2Lo,1496
 torch_tensorrt/fx/converters/mul.py,sha256=4FrNqX2ksG0Pr751JrCn4cxzT1-0l86VvFXQucC5tOU,1562
 torch_tensorrt/fx/converters/quantization.py,sha256=OaPReuCQwQ5cbNuKi2IHLpiwmd5qMiR9Pce0HSNiA58,2162
 torch_tensorrt/fx/converters/transformation.py,sha256=7a-etM0oxueh4sGBkpw8yzBpL0SYP7e-sEGSFhcYT7A,1547
 torch_tensorrt/fx/passes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torch_tensorrt/fx/passes/graph_opts.py,sha256=0fYXTVxDmdG7v68Z7zCby_G756aliYmeDhdO51oj754,2044
-torch_tensorrt/fx/passes/lower_basic_pass.py,sha256=Q_RiPvRpsckj23G_O_k-eprsWLKphHs8cgP5OXf8sxo,23744
+torch_tensorrt/fx/passes/lower_basic_pass.py,sha256=NOJVm7PVZBovUxq6uYZEOjz-OsWIPbSmcZBZR8paOXM,25182
 torch_tensorrt/fx/passes/lower_basic_pass_aten.py,sha256=j1FS5rNeOcBTpGbx7UslERP-P1lbZuoZ7LLCqmcXpgE,19757
-torch_tensorrt/fx/passes/lower_pass_manager_builder.py,sha256=j7TBbAjqriRVFFXiMXsjVJ6D1MPMO1LwyUwxswTf3Yw,12014
-torch_tensorrt/fx/passes/pass_utils.py,sha256=gpUEJz5P7-zHnq0s0MuvL7S_yxcfs9In7JAlN3rErEU,9875
+torch_tensorrt/fx/passes/lower_pass_manager_builder.py,sha256=EdMfaBmvRHFRV7nltQsk3hmDOq2l_aXmdZmcy-S9bV4,12274
+torch_tensorrt/fx/passes/pass_utils.py,sha256=iu7ISjANH5kGn0rj_yMcLiR7-DBTLodrzpJQyGjEE0M,19519
 torch_tensorrt/fx/passes/remove_duplicate_output_args.py,sha256=MdN6cIe5fPNfz3hfv2DE08hm2S6B7wDy-HhkZV7EgdM,4961
 torch_tensorrt/fx/tools/__init__.py,sha256=SF90jfdL6xvPeyDy3TVSIICz3E6UKbu66KZjvDGpYwQ,49
-torch_tensorrt/fx/tools/common_fx2trt.py,sha256=dh9KF43xIxaOVRss-CLyjELhzIk0DWu2gMMgnl3R-qg,15697
+torch_tensorrt/fx/tools/common_fx2trt.py,sha256=EwPihKHABb9auRJUDeYcWUdY8RN12Zc8xy4SrzGHPV8,15853
 torch_tensorrt/fx/tools/engine_layer_visualize.py,sha256=T7AGlwdc8V7u-cVcp02UMWBobbCI4spchH7ToHpO1HY,7067
 torch_tensorrt/fx/tools/graph_util.py,sha256=cT-RJV2sm6_rGHZ3JjLyu8J7ICwINblHniNSLfWhC4Y,2423
-torch_tensorrt/fx/tools/model_packager.py,sha256=cOKxNQGAUxyx76JwgYXPlH14akM4p3rU_8csNVOH1yA,3939
+torch_tensorrt/fx/tools/model_packager.py,sha256=cUrpgQOByDkiUUrl8R2OGisGyk5slAhy1WIi7IjexnE,4703
 torch_tensorrt/fx/tools/node_profiler.py,sha256=bl3sPBrzdcnD6pac_5mQ6roFsjnPBgMH-qykW6DP1Io,1777
 torch_tensorrt/fx/tools/tensor_prop.py,sha256=a1VQ9rjaTSwgqaOZrCBZM08bvZIN6EifXqOmaaOOOz0,1163
 torch_tensorrt/fx/tools/timing_cache_utils.py,sha256=J8mEoIlGalWd09bthMLEftP784IBk5wYdpgZ6tSwGKM,1451
 torch_tensorrt/fx/tools/trt_minimizer.py,sha256=CcT6n5JHST7hYnPkRjMOT1xKOYThr7iKlbOzGn2Kaow,3780
 torch_tensorrt/fx/tools/trt_profiler_sorted.py,sha256=p-jm_4gtsxt790m3A9Ehp6EEsbS9GFf6xKwJ3SFr6ps,2052
-torch_tensorrt/fx/tools/trt_splitter.py,sha256=b0G4zjrG5r_2KZJvyFKzBjOmdJzdzsEla-B3FrVkWyw,5518
+torch_tensorrt/fx/tools/trt_splitter.py,sha256=gvsavi4WSEaQ6RAqTPT2eezG10RBs1y80tILfWhoLso,5592
 torch_tensorrt/fx/tracer/acc_tracer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torch_tensorrt/fx/tracer/acc_tracer/acc_normalizer.py,sha256=82Hj67nAgRM5NYAUp232K4OXFFpRW2jZReKwdndIxsA,19889
+torch_tensorrt/fx/tracer/acc_tracer/acc_normalizer.py,sha256=kv-lrKSOpYDnxWp9FqrHAE2RebuHhLtKztvHt2L5BzI,20455
 torch_tensorrt/fx/tracer/acc_tracer/acc_op_properties.py,sha256=yZf0w7_sNLIPUPiTaliH-4cBQL9lmcQoRklIxsF9tOg,1573
-torch_tensorrt/fx/tracer/acc_tracer/acc_ops.py,sha256=H5AsZ9JBwRxo6AYF-cHnosEZcBaBxFdulpDYH8T-2ZQ,105950
+torch_tensorrt/fx/tracer/acc_tracer/acc_ops.py,sha256=_KVDo6Aq8K0jeuQE3BCWnV5DpUBWqXAjfqU_p8obilo,113034
 torch_tensorrt/fx/tracer/acc_tracer/acc_shape_prop.py,sha256=Tn_1vioY-EikoaTh4CgwQTLMhKJFcw-0QaurAy8RJAI,5557
-torch_tensorrt/fx/tracer/acc_tracer/acc_tracer.py,sha256=fbFsjrZSbBJtjqOm9m5GWvNGJ4uuQY7bdB0jPPHqFZw,28268
-torch_tensorrt/fx/tracer/acc_tracer/acc_utils.py,sha256=hFcJD06qt_uSp61M2I7LBuSEsDh34ZgT6UzkO_-7CoY,7148
+torch_tensorrt/fx/tracer/acc_tracer/acc_tracer.py,sha256=Nn8ezIAtnH3oDSgGkEtP3wJPC-R_1KwXCCCnBcwRKvg,28756
+torch_tensorrt/fx/tracer/acc_tracer/acc_utils.py,sha256=07z-k7BXZhpBHSdWqhzyAdLcyQP0Naoq7hjGjhWFRTc,7430
 torch_tensorrt/fx/tracer/dispatch_tracer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torch_tensorrt/fx/tracer/dispatch_tracer/aten_tracer.py,sha256=m9iZHtlVwfZ7PjJCzBx-FZTHn8ErWbUhiQVH42hXirE,5341
+torch_tensorrt/fx/tracer/dispatch_tracer/aten_tracer.py,sha256=JANcTk3JXQHQ6RN7HGKZT1cDTfmLX8GwaoP7lv1ogck,5262
 torch_tensorrt/fx/tracer/dispatch_tracer/tracer.py,sha256=ThVip0LDcc2WvG20q7d7w8pBHkaHzTiokZSEaYxH7bk,7785
-torch_tensorrt_fx_only-1.4.0.dev0.dist-info/LICENSE,sha256=Hogezyhi0B5uW8K4YeRohtKm-wFJnAxQiiCacnGxPPI,10
-torch_tensorrt_fx_only-1.4.0.dev0.dist-info/METADATA,sha256=OZpNH3_RF2pi2TyTijgkumfO_Yy36fFASt8CuLqRMwo,13818
-torch_tensorrt_fx_only-1.4.0.dev0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-torch_tensorrt_fx_only-1.4.0.dev0.dist-info/top_level.txt,sha256=iJxwcyhlIDXvQLvPYeQXIlHjLpAbMzUsyIVCHzU18ts,15
-torch_tensorrt_fx_only-1.4.0.dev0.dist-info/RECORD,,
+torch_tensorrt_fx_only-1.5.0.dev0.dist-info/LICENSE,sha256=Hogezyhi0B5uW8K4YeRohtKm-wFJnAxQiiCacnGxPPI,10
+torch_tensorrt_fx_only-1.5.0.dev0.dist-info/METADATA,sha256=g1urcEClB1QwDlrFRW32ZAREvWQ_cHUj3B4TMA7ltvw,13822
+torch_tensorrt_fx_only-1.5.0.dev0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+torch_tensorrt_fx_only-1.5.0.dev0.dist-info/top_level.txt,sha256=iJxwcyhlIDXvQLvPYeQXIlHjLpAbMzUsyIVCHzU18ts,15
+torch_tensorrt_fx_only-1.5.0.dev0.dist-info/RECORD,,
```

