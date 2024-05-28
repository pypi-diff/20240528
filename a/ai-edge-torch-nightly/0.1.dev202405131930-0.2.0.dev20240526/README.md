# Comparing `tmp/ai_edge_torch_nightly-0.1.dev202405131930-py3-none-any.whl.zip` & `tmp/ai_edge_torch_nightly-0.2.0.dev20240526-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,93 +1,101 @@
-Zip file size: 139003 bytes, number of entries: 91
--rw-r--r--  2.0 unx     1008 b- defN 24-May-13 23:42 ai_edge_torch/__init__.py
--rw-r--r--  2.0 unx     4243 b- defN 24-May-13 23:42 ai_edge_torch/model.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/convert/__init__.py
--rw-r--r--  2.0 unx     4043 b- defN 24-May-13 23:42 ai_edge_torch/convert/conversion.py
--rw-r--r--  2.0 unx    11021 b- defN 24-May-13 23:42 ai_edge_torch/convert/conversion_utils.py
--rw-r--r--  2.0 unx     6927 b- defN 24-May-13 23:42 ai_edge_torch/convert/converter.py
--rw-r--r--  2.0 unx     2825 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/__init__.py
--rw-r--r--  2.0 unx     1652 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/_pass_base.py
--rw-r--r--  2.0 unx     6150 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py
--rw-r--r--  2.0 unx     2607 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/build_upsample_bilinear2d_composite_pass.py
--rw-r--r--  2.0 unx     1673 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/canonicalize_pass.py
--rw-r--r--  2.0 unx     2448 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/inject_mlir_debuginfo_pass.py
--rw-r--r--  2.0 unx      795 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/__init__.py
--rw-r--r--  2.0 unx     6870 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_check.py
--rw-r--r--  2.0 unx     1560 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_mark.py
--rw-r--r--  2.0 unx    12438 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_rewrite.py
--rw-r--r--  2.0 unx      982 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/op_func_registry.py
--rw-r--r--  2.0 unx    10030 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/pass_body.py
--rw-r--r--  2.0 unx     2076 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/utils.py
--rw-r--r--  2.0 unx      715 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/__init__.py
--rw-r--r--  2.0 unx     2279 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/greedy.py
--rw-r--r--  2.0 unx     6432 b- defN 24-May-13 23:42 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/min_cut.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/convert/test/__init__.py
--rw-r--r--  2.0 unx     8092 b- defN 24-May-13 23:42 ai_edge_torch/convert/test/test_convert.py
--rw-r--r--  2.0 unx     6403 b- defN 24-May-13 23:42 ai_edge_torch/convert/test/test_convert_composites.py
--rw-r--r--  2.0 unx     4537 b- defN 24-May-13 23:42 ai_edge_torch/convert/test/test_convert_multisig.py
--rw-r--r--  2.0 unx      707 b- defN 24-May-13 23:42 ai_edge_torch/debug/__init__.py
--rw-r--r--  2.0 unx    12789 b- defN 24-May-13 23:42 ai_edge_torch/debug/culprit.py
--rw-r--r--  2.0 unx     1430 b- defN 24-May-13 23:42 ai_edge_torch/debug/utils.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/debug/test/__init__.py
--rw-r--r--  2.0 unx     3731 b- defN 24-May-13 23:42 ai_edge_torch/debug/test/test_culprit.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/experimental/__init__.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/generative/__init__.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/__init__.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/gemma/__init__.py
--rw-r--r--  2.0 unx     2538 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/gemma/convert_to_tflite.py
--rw-r--r--  2.0 unx     5913 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/gemma/gemma.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/phi2/__init__.py
--rw-r--r--  2.0 unx     2512 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/phi2/convert_to_tflite.py
--rw-r--r--  2.0 unx     5540 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/phi2/phi2.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/t5/__init__.py
--rw-r--r--  2.0 unx     4536 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/t5/convert_to_tflite.py
--rw-r--r--  2.0 unx    21065 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/t5/t5.py
--rw-r--r--  2.0 unx     8998 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/t5/t5_attention.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/test_models/__init__.py
--rw-r--r--  2.0 unx     3791 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/test_models/toy_model.py
--rw-r--r--  2.0 unx     4831 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/tiny_llama/__init__.py
--rw-r--r--  2.0 unx     2566 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/tiny_llama/convert_to_tflite.py
--rw-r--r--  2.0 unx     5629 b- defN 24-May-13 23:42 ai_edge_torch/generative/examples/tiny_llama/tiny_llama.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/generative/layers/__init__.py
--rw-r--r--  2.0 unx     9127 b- defN 24-May-13 23:42 ai_edge_torch/generative/layers/attention.py
--rw-r--r--  2.0 unx     6350 b- defN 24-May-13 23:42 ai_edge_torch/generative/layers/attention_utils.py
--rw-r--r--  2.0 unx     3201 b- defN 24-May-13 23:42 ai_edge_torch/generative/layers/builder.py
--rw-r--r--  2.0 unx     2820 b- defN 24-May-13 23:42 ai_edge_torch/generative/layers/feed_forward.py
--rw-r--r--  2.0 unx     3090 b- defN 24-May-13 23:42 ai_edge_torch/generative/layers/kv_cache.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-13 23:42 ai_edge_torch/generative/layers/model_config.py
--rw-r--r--  2.0 unx     1867 b- defN 24-May-13 23:42 ai_edge_torch/generative/layers/normalization.py
--rw-r--r--  2.0 unx     1383 b- defN 24-May-13 23:42 ai_edge_torch/generative/layers/rotary_position_embedding.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/generative/quantize/__init__.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-13 23:42 ai_edge_torch/generative/quantize/example.py
--rw-r--r--  2.0 unx     1862 b- defN 24-May-13 23:42 ai_edge_torch/generative/quantize/quant_attrs.py
--rw-r--r--  2.0 unx     3327 b- defN 24-May-13 23:42 ai_edge_torch/generative/quantize/quant_recipe.py
--rw-r--r--  2.0 unx     1913 b- defN 24-May-13 23:42 ai_edge_torch/generative/quantize/quant_recipe_utils.py
--rw-r--r--  2.0 unx     1798 b- defN 24-May-13 23:42 ai_edge_torch/generative/quantize/quant_recipes.py
--rw-r--r--  2.0 unx     1345 b- defN 24-May-13 23:42 ai_edge_torch/generative/quantize/supported_schemes.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/generative/test/__init__.py
--rw-r--r--  2.0 unx     6500 b- defN 24-May-13 23:42 ai_edge_torch/generative/test/test_model_conversion.py
--rw-r--r--  2.0 unx     3728 b- defN 24-May-13 23:42 ai_edge_torch/generative/test/test_quantize.py
--rw-r--r--  2.0 unx      720 b- defN 24-May-13 23:42 ai_edge_torch/generative/utilities/__init__.py
--rw-r--r--  2.0 unx    10029 b- defN 24-May-13 23:42 ai_edge_torch/generative/utilities/loader.py
--rw-r--r--  2.0 unx    16156 b- defN 24-May-13 23:42 ai_edge_torch/generative/utilities/t5_loader.py
--rw-r--r--  2.0 unx      752 b- defN 24-May-13 23:42 ai_edge_torch/hlfb/__init__.py
--rw-r--r--  2.0 unx     4799 b- defN 24-May-13 23:42 ai_edge_torch/hlfb/mark_pattern/__init__.py
--rw-r--r--  2.0 unx     1539 b- defN 24-May-13 23:42 ai_edge_torch/hlfb/mark_pattern/passes.py
--rw-r--r--  2.0 unx     9206 b- defN 24-May-13 23:42 ai_edge_torch/hlfb/mark_pattern/pattern.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/hlfb/test/__init__.py
--rw-r--r--  2.0 unx     4262 b- defN 24-May-13 23:42 ai_edge_torch/hlfb/test/test_mark_pattern.py
--rw-r--r--  2.0 unx     8190 b- defN 24-May-13 23:42 ai_edge_torch/hlfb/test/test_stablehlo_composite_builder.py
--rw-r--r--  2.0 unx      714 b- defN 24-May-13 23:42 ai_edge_torch/quantize/__init__.py
--rw-r--r--  2.0 unx    15602 b- defN 24-May-13 23:42 ai_edge_torch/quantize/pt2e_quantizer.py
--rw-r--r--  2.0 unx    36046 b- defN 24-May-13 23:42 ai_edge_torch/quantize/pt2e_quantizer_utils.py
--rw-r--r--  2.0 unx     3435 b- defN 24-May-13 23:42 ai_edge_torch/quantize/quant_config.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 23:42 ai_edge_torch/testing/__init__.py
--rw-r--r--  2.0 unx      765 b- defN 24-May-13 23:42 ai_edge_torch/testing/model_coverage/__init__.py
--rw-r--r--  2.0 unx     4286 b- defN 24-May-13 23:42 ai_edge_torch/testing/model_coverage/model_coverage.py
--rw-r--r--  2.0 unx    11358 b- defN 24-May-14 02:31 ai_edge_torch_nightly-0.1.dev202405131930.dist-info/LICENSE
--rw-r--r--  2.0 unx     1750 b- defN 24-May-14 02:31 ai_edge_torch_nightly-0.1.dev202405131930.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 02:31 ai_edge_torch_nightly-0.1.dev202405131930.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-May-14 02:31 ai_edge_torch_nightly-0.1.dev202405131930.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9745 b- defN 24-May-14 02:31 ai_edge_torch_nightly-0.1.dev202405131930.dist-info/RECORD
-91 files, 397825 bytes uncompressed, 122801 bytes compressed:  69.1%
+Zip file size: 149784 bytes, number of entries: 99
+-rw-r--r--  2.0 unx     1008 b- defN 24-May-22 17:27 ai_edge_torch/__init__.py
+-rw-r--r--  2.0 unx     4243 b- defN 24-May-22 17:27 ai_edge_torch/model.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/convert/__init__.py
+-rw-r--r--  2.0 unx     4043 b- defN 24-May-22 17:27 ai_edge_torch/convert/conversion.py
+-rw-r--r--  2.0 unx    11021 b- defN 24-May-22 17:27 ai_edge_torch/convert/conversion_utils.py
+-rw-r--r--  2.0 unx     6927 b- defN 24-May-22 17:27 ai_edge_torch/convert/converter.py
+-rw-r--r--  2.0 unx     2825 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/__init__.py
+-rw-r--r--  2.0 unx     1652 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/_pass_base.py
+-rw-r--r--  2.0 unx     6150 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py
+-rw-r--r--  2.0 unx     2607 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/build_upsample_bilinear2d_composite_pass.py
+-rw-r--r--  2.0 unx     1673 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/canonicalize_pass.py
+-rw-r--r--  2.0 unx     2448 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/inject_mlir_debuginfo_pass.py
+-rw-r--r--  2.0 unx      795 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/__init__.py
+-rw-r--r--  2.0 unx     6870 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_check.py
+-rw-r--r--  2.0 unx     1560 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_mark.py
+-rw-r--r--  2.0 unx    12438 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_rewrite.py
+-rw-r--r--  2.0 unx      982 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/op_func_registry.py
+-rw-r--r--  2.0 unx    10030 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/pass_body.py
+-rw-r--r--  2.0 unx     2076 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/utils.py
+-rw-r--r--  2.0 unx      715 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/__init__.py
+-rw-r--r--  2.0 unx     2279 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/greedy.py
+-rw-r--r--  2.0 unx     6432 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/min_cut.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/convert/test/__init__.py
+-rw-r--r--  2.0 unx     8092 b- defN 24-May-22 17:27 ai_edge_torch/convert/test/test_convert.py
+-rw-r--r--  2.0 unx     6403 b- defN 24-May-22 17:27 ai_edge_torch/convert/test/test_convert_composites.py
+-rw-r--r--  2.0 unx     4537 b- defN 24-May-22 17:27 ai_edge_torch/convert/test/test_convert_multisig.py
+-rw-r--r--  2.0 unx      707 b- defN 24-May-22 17:27 ai_edge_torch/debug/__init__.py
+-rw-r--r--  2.0 unx    12789 b- defN 24-May-22 17:27 ai_edge_torch/debug/culprit.py
+-rw-r--r--  2.0 unx     1430 b- defN 24-May-22 17:27 ai_edge_torch/debug/utils.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/debug/test/__init__.py
+-rw-r--r--  2.0 unx     3731 b- defN 24-May-22 17:27 ai_edge_torch/debug/test/test_culprit.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/experimental/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/gemma/__init__.py
+-rw-r--r--  2.0 unx     2538 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/gemma/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5913 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/gemma/gemma.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/phi2/__init__.py
+-rw-r--r--  2.0 unx     2512 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/phi2/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5540 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/phi2/phi2.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/__init__.py
+-rw-r--r--  2.0 unx     3535 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/attention.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/clip.py
+-rw-r--r--  2.0 unx     3239 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/decoder.py
+-rw-r--r--  2.0 unx    16200 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/diffusion.py
+-rw-r--r--  2.0 unx     2251 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/encoder.py
+-rw-r--r--  2.0 unx     2046 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/util.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/t5/__init__.py
+-rw-r--r--  2.0 unx     4536 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/t5/convert_to_tflite.py
+-rw-r--r--  2.0 unx    21065 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/t5/t5.py
+-rw-r--r--  2.0 unx     8998 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/t5/t5_attention.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/test_models/__init__.py
+-rw-r--r--  2.0 unx     3791 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/test_models/toy_model.py
+-rw-r--r--  2.0 unx     4831 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/tiny_llama/__init__.py
+-rw-r--r--  2.0 unx     2566 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/tiny_llama/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5629 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/tiny_llama/tiny_llama.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/__init__.py
+-rw-r--r--  2.0 unx     9127 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/attention.py
+-rw-r--r--  2.0 unx     6350 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/attention_utils.py
+-rw-r--r--  2.0 unx     3201 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/builder.py
+-rw-r--r--  2.0 unx     2820 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/feed_forward.py
+-rw-r--r--  2.0 unx     3090 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/kv_cache.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/model_config.py
+-rw-r--r--  2.0 unx     1867 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/normalization.py
+-rw-r--r--  2.0 unx     1383 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/rotary_position_embedding.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/__init__.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/example.py
+-rw-r--r--  2.0 unx     1862 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/quant_attrs.py
+-rw-r--r--  2.0 unx     3327 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/quant_recipe.py
+-rw-r--r--  2.0 unx     1913 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/quant_recipe_utils.py
+-rw-r--r--  2.0 unx     1798 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/quant_recipes.py
+-rw-r--r--  2.0 unx     1345 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/supported_schemes.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/test/__init__.py
+-rw-r--r--  2.0 unx     3317 b- defN 24-May-22 17:27 ai_edge_torch/generative/test/loader_test.py
+-rw-r--r--  2.0 unx     6500 b- defN 24-May-22 17:27 ai_edge_torch/generative/test/test_model_conversion.py
+-rw-r--r--  2.0 unx     3728 b- defN 24-May-22 17:27 ai_edge_torch/generative/test/test_quantize.py
+-rw-r--r--  2.0 unx      720 b- defN 24-May-22 17:27 ai_edge_torch/generative/utilities/__init__.py
+-rw-r--r--  2.0 unx    10107 b- defN 24-May-22 17:27 ai_edge_torch/generative/utilities/loader.py
+-rw-r--r--  2.0 unx    16156 b- defN 24-May-22 17:27 ai_edge_torch/generative/utilities/t5_loader.py
+-rw-r--r--  2.0 unx      752 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/__init__.py
+-rw-r--r--  2.0 unx     4799 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/mark_pattern/__init__.py
+-rw-r--r--  2.0 unx     1539 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/mark_pattern/passes.py
+-rw-r--r--  2.0 unx     9206 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/mark_pattern/pattern.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/test/__init__.py
+-rw-r--r--  2.0 unx     4262 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/test/test_mark_pattern.py
+-rw-r--r--  2.0 unx     8190 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/test/test_stablehlo_composite_builder.py
+-rw-r--r--  2.0 unx      714 b- defN 24-May-22 17:27 ai_edge_torch/quantize/__init__.py
+-rw-r--r--  2.0 unx    15602 b- defN 24-May-22 17:27 ai_edge_torch/quantize/pt2e_quantizer.py
+-rw-r--r--  2.0 unx    36046 b- defN 24-May-22 17:27 ai_edge_torch/quantize/pt2e_quantizer_utils.py
+-rw-r--r--  2.0 unx     3435 b- defN 24-May-22 17:27 ai_edge_torch/quantize/quant_config.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/testing/__init__.py
+-rw-r--r--  2.0 unx      765 b- defN 24-May-22 17:27 ai_edge_torch/testing/model_coverage/__init__.py
+-rw-r--r--  2.0 unx     4286 b- defN 24-May-22 17:27 ai_edge_torch/testing/model_coverage/model_coverage.py
+-rw-r--r--  2.0 unx    11358 b- defN 24-May-28 19:18 ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1748 b- defN 24-May-28 19:18 ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 19:18 ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-May-28 19:18 ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    10661 b- defN 24-May-28 19:18 ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/RECORD
+99 files, 432486 bytes uncompressed, 132054 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -114,14 +114,35 @@
 
 Filename: ai_edge_torch/generative/examples/phi2/convert_to_tflite.py
 Comment: 
 
 Filename: ai_edge_torch/generative/examples/phi2/phi2.py
 Comment: 
 
+Filename: ai_edge_torch/generative/examples/stable_diffusion/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/attention.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/clip.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/decoder.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/diffusion.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/encoder.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/util.py
+Comment: 
+
 Filename: ai_edge_torch/generative/examples/t5/__init__.py
 Comment: 
 
 Filename: ai_edge_torch/generative/examples/t5/convert_to_tflite.py
 Comment: 
 
 Filename: ai_edge_torch/generative/examples/t5/t5.py
@@ -195,14 +216,17 @@
 
 Filename: ai_edge_torch/generative/quantize/supported_schemes.py
 Comment: 
 
 Filename: ai_edge_torch/generative/test/__init__.py
 Comment: 
 
+Filename: ai_edge_torch/generative/test/loader_test.py
+Comment: 
+
 Filename: ai_edge_torch/generative/test/test_model_conversion.py
 Comment: 
 
 Filename: ai_edge_torch/generative/test/test_quantize.py
 Comment: 
 
 Filename: ai_edge_torch/generative/utilities/__init__.py
@@ -252,23 +276,23 @@
 
 Filename: ai_edge_torch/testing/model_coverage/__init__.py
 Comment: 
 
 Filename: ai_edge_torch/testing/model_coverage/model_coverage.py
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.1.dev202405131930.dist-info/LICENSE
+Filename: ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/LICENSE
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.1.dev202405131930.dist-info/METADATA
+Filename: ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/METADATA
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.1.dev202405131930.dist-info/WHEEL
+Filename: ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/WHEEL
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.1.dev202405131930.dist-info/top_level.txt
+Filename: ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/top_level.txt
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.1.dev202405131930.dist-info/RECORD
+Filename: ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ai_edge_torch/generative/utilities/loader.py

```diff
@@ -224,32 +224,36 @@
       state: Dict[str, torch.Tensor],
       converted_state: Dict[str, torch.Tensor],
   ):
     prefix = f"transformer_blocks.{idx}"
     q_name = self._names.attn_query_proj.format(idx)
     k_name = self._names.attn_key_proj.format(idx)
     v_name = self._names.attn_value_proj.format(idx)
-    converted_state[f"{prefix}.atten_func.attn.weight"] = self._fuse_qkv(
+    converted_state[f"{prefix}.atten_func.qkv_projection.weight"] = self._fuse_qkv(
         config,
         state.pop(f"{q_name}.weight"),
         state.pop(f"{k_name}.weight"),
         state.pop(f"{v_name}.weight"),
     )
     if config.attn_config.qkv_use_bias:
-      converted_state[f"{prefix}.atten_func.attn.bias"] = self._fuse_qkv(
+      converted_state[f"{prefix}.atten_func.qkv_projection.bias"] = self._fuse_qkv(
           config,
           state.pop(f"{q_name}.bias"),
           state.pop(f"{k_name}.bias"),
           state.pop(f"{v_name}.bias"),
       )
 
     o_name = self._names.attn_output_proj.format(idx)
-    converted_state[f"{prefix}.atten_func.proj.weight"] = state.pop(f"{o_name}.weight")
+    converted_state[f"{prefix}.atten_func.output_projection.weight"] = state.pop(
+        f"{o_name}.weight"
+    )
     if config.attn_config.output_proj_use_bias:
-      converted_state[f"{prefix}.atten_func.proj.bias"] = state.pop(f"{o_name}.bias")
+      converted_state[f"{prefix}.atten_func.output_projection.bias"] = state.pop(
+          f"{o_name}.bias"
+      )
 
   def _map_norm(
       self,
       idx: int,
       config: model_config.ModelConfig,
       state: Dict[str, torch.Tensor],
       converted_state: Dict[str, torch.Tensor],
```

## Comparing `ai_edge_torch_nightly-0.1.dev202405131930.dist-info/LICENSE` & `ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ai_edge_torch_nightly-0.1.dev202405131930.dist-info/METADATA` & `ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-edge-torch-nightly
-Version: 0.1.dev202405131930
+Version: 0.2.0.dev20240526
 Summary: Supporting PyTorch models with the Google AI Edge TFLite runtime.
 Home-page: https://github.com/google-ai-edge/ai-edge-torch
 Keywords: On-Device ML,AI,Google,TFLite,PyTorch,LLMs,GenAI
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -20,16 +20,16 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: safetensors
 Requires-Dist: scipy
+Requires-Dist: safetensors
 Requires-Dist: tabulate
 Requires-Dist: torch ==2.4.*
 
 Library that supports converting PyTorch models into a .tflite format, which can
 then be run with TensorFlow Lite and MediaPipe.  This enables applications for
 Android, iOS and IOT that can run models completely on-device.
```

## Comparing `ai_edge_torch_nightly-0.1.dev202405131930.dist-info/RECORD` & `ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,21 @@
 ai_edge_torch/generative/examples/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/generative/examples/gemma/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/generative/examples/gemma/convert_to_tflite.py,sha256=dZv3r24uHsTMokEdnl3nf7LpmV0q7FLnVtCuHn5AuUs,2538
 ai_edge_torch/generative/examples/gemma/gemma.py,sha256=YF4Ua-1lnL3qhQnh1sY5-HlYw2Dq6ZRm227XyDe7WAw,5913
 ai_edge_torch/generative/examples/phi2/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/generative/examples/phi2/convert_to_tflite.py,sha256=6nOuwx9q3AUlYcjXRRXSr_3M2JKqdJ-vUf-uE3VFYHE,2512
 ai_edge_torch/generative/examples/phi2/phi2.py,sha256=VvigzPQ_LJHeADTsMliwFwPe2BcnOhFgKDqr_WZ2JQ8,5540
+ai_edge_torch/generative/examples/stable_diffusion/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
+ai_edge_torch/generative/examples/stable_diffusion/attention.py,sha256=Lo4Dq7a3Kg-lyH56iqGtqCo5UaClQHRCTDdNagXGTo8,3535
+ai_edge_torch/generative/examples/stable_diffusion/clip.py,sha256=8W4X9PKdnMsWGxXbBfm5OX6mX4XhvaMZ2gZw8yCTScY,2410
+ai_edge_torch/generative/examples/stable_diffusion/decoder.py,sha256=beLCtogA32oYT2nlATpyT-1xzkyPF8zi4v3kfHpw6Mc,3239
+ai_edge_torch/generative/examples/stable_diffusion/diffusion.py,sha256=nnsfgjSeL16U3TVdjTkRycaoWA2ChFeitx2RjGLpwyA,16200
+ai_edge_torch/generative/examples/stable_diffusion/encoder.py,sha256=X6ekByU19KNHNh5OaztZEROv-QwcCwVm1xiJjm2SCoo,2251
+ai_edge_torch/generative/examples/stable_diffusion/util.py,sha256=pG_dsV4xIaB7B8MgoRgSXBvLCVqDlF6bNunPN3GIm-s,2046
 ai_edge_torch/generative/examples/t5/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/generative/examples/t5/convert_to_tflite.py,sha256=bWtwtUacvJOEDUpuYvLTgkP7oTkXKJA-Tf4FPxlD1Cw,4536
 ai_edge_torch/generative/examples/t5/t5.py,sha256=q2gG5RRo7RgNzvHXYC0Juh6Tgt5d_RTMSWFaYvOKiZU,21065
 ai_edge_torch/generative/examples/t5/t5_attention.py,sha256=anR99IrzR21x6yswFHYG5QQtPDZ7rVicf6STfMp54fU,8998
 ai_edge_torch/generative/examples/test_models/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/generative/examples/test_models/toy_model.py,sha256=EV07_MEG3fv9g0ZGu9gbBd5BjjrGkxCT1pv7dvhz4TI,3791
 ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py,sha256=MUr6fSj2hBuYSlNbZtrBBpzqB_0WY-l_xYcd_TFFUjY,4831
@@ -61,18 +68,19 @@
 ai_edge_torch/generative/quantize/example.py,sha256=t-YwyKSPAG-OZC1DfH-0vfie2RHHpTSQjxUY-tmhu5g,1543
 ai_edge_torch/generative/quantize/quant_attrs.py,sha256=ffBALrrbrfiG_mrOr-f3B1Gc6PlAma9gtvVnfP7SDzI,1862
 ai_edge_torch/generative/quantize/quant_recipe.py,sha256=BOk4E0FW-_YD8Y-oPVmIDsgXx_bPtvzsP_V1av5DvgU,3327
 ai_edge_torch/generative/quantize/quant_recipe_utils.py,sha256=9ktL7fT8C5j1dnY_7fkiFL4oWNLVs1dMWXkS_EuyA3Y,1913
 ai_edge_torch/generative/quantize/quant_recipes.py,sha256=CRA2ENevS-3usHqidWDe2wrf_epILE_7Hx-XfZQ9buk,1798
 ai_edge_torch/generative/quantize/supported_schemes.py,sha256=OQ4ghQXknA1PPjuY-xBgAmOpaIBgYFM8F2YAIot06hE,1345
 ai_edge_torch/generative/test/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
+ai_edge_torch/generative/test/loader_test.py,sha256=N88CbrLW7Q2x1EyurwdXQ6YjsA-ySQcPxpZH3QOGp-M,3317
 ai_edge_torch/generative/test/test_model_conversion.py,sha256=1NfZxKo9Gx6CmVfd86K1FkmsNQnjzIV1ojBS85UGvT0,6500
 ai_edge_torch/generative/test/test_quantize.py,sha256=f70sH1ZFzdCwYj0MG-eg54WOC4LasR0D8CTUYpjxZYM,3728
 ai_edge_torch/generative/utilities/__init__.py,sha256=-_jxnnFnCgnTU4oTm4MnRsvL5lqhomBNdFBbqfmfHPo,720
-ai_edge_torch/generative/utilities/loader.py,sha256=QrGZ3JlEN_tn8j6EdZOxVt_0u3yB5vBrR3KJtNaAwV8,10029
+ai_edge_torch/generative/utilities/loader.py,sha256=c-ZOIDBVnat_5l2W5sWU7HQm7CL-wducS8poSu5PlUg,10107
 ai_edge_torch/generative/utilities/t5_loader.py,sha256=guDTv-12UUvJGl4eDvvZX3t4rRKewfXO8SpcYXM6gbc,16156
 ai_edge_torch/hlfb/__init__.py,sha256=rrje8a2iuKboBoV96bVq7nlS9HsnuEMbHE5JiWmCxFA,752
 ai_edge_torch/hlfb/mark_pattern/__init__.py,sha256=2VXnHcGf23VOuP-1GriGIpuL98leBB8twp_qaScMnmc,4799
 ai_edge_torch/hlfb/mark_pattern/passes.py,sha256=YV2YKBkh7y7j7sd7EA81vf_1hUKUvTRiy1pfqZustXc,1539
 ai_edge_torch/hlfb/mark_pattern/pattern.py,sha256=H4047w-xwx27rYPKNqmeOSQ9M1Adkpd7drp81YdV7Hw,9206
 ai_edge_torch/hlfb/test/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/hlfb/test/test_mark_pattern.py,sha256=qYR3PRGS9W3OG-qX7UFqL69VxXuUSfyDBUJtCXtXcOE,4262
@@ -80,12 +88,12 @@
 ai_edge_torch/quantize/__init__.py,sha256=aB5dXot04bqyUhpsDFvxt9CIi15QAC4euvqOndJ0XLU,714
 ai_edge_torch/quantize/pt2e_quantizer.py,sha256=ye1f5vAZ0Vr4RWAtfrgU1o3JLs03Sa4inHRq3YxJDGo,15602
 ai_edge_torch/quantize/pt2e_quantizer_utils.py,sha256=yjzKoptnfEeW_sN7sODUfj3nCtUMXVzq3vHKxblsd5Y,36046
 ai_edge_torch/quantize/quant_config.py,sha256=ExThdTXqnWmGC3-F6sdXbXr8nYzkEe_qCziCfhsoMPA,3435
 ai_edge_torch/testing/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/testing/model_coverage/__init__.py,sha256=5P8J6Zk5YYtDvTBucFvB9NGSRI7Gw_24WnrbhXgycEE,765
 ai_edge_torch/testing/model_coverage/model_coverage.py,sha256=EIyKz-HY70DguWuSrJal8LpYXQ5ZSEUf3ZrVl7jikFM,4286
-ai_edge_torch_nightly-0.1.dev202405131930.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-ai_edge_torch_nightly-0.1.dev202405131930.dist-info/METADATA,sha256=lQcAb0esNisYUqkzDRHamW4S9luvrJ4QU75042IAqWc,1750
-ai_edge_torch_nightly-0.1.dev202405131930.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ai_edge_torch_nightly-0.1.dev202405131930.dist-info/top_level.txt,sha256=5KXRaF2hwkApYxf7Y8y_tVb9aulGTlbOoNdbx1aKRkE,14
-ai_edge_torch_nightly-0.1.dev202405131930.dist-info/RECORD,,
+ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/METADATA,sha256=ZErfXA6dGKS1ox_OWvGy5oT_7BVEEHCUlOQxq6kVMiE,1748
+ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/top_level.txt,sha256=5KXRaF2hwkApYxf7Y8y_tVb9aulGTlbOoNdbx1aKRkE,14
+ai_edge_torch_nightly-0.2.0.dev20240526.dist-info/RECORD,,
```

