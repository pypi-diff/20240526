# Comparing `tmp/zetascale-2.4.8.tar.gz` & `tmp/zetascale-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetascale-2.4.8.tar", max compression
+gzip compressed data, was "zetascale-2.5.1.tar", max compression
```

## Comparing `zetascale-2.4.8.tar` & `zetascale-2.5.1.tar`

### file list

```diff
@@ -1,386 +1,388 @@
--rw-r--r--   0        0        0    11342 2023-10-13 21:44:53.585497 zetascale-2.4.8/LICENSE
--rw-r--r--   0        0        0    20231 2024-04-06 16:41:06.878751 zetascale-2.4.8/README.md
--rw-r--r--   0        0        0     1333 2024-05-13 18:52:01.246082 zetascale-2.4.8/pyproject.toml
--rw-r--r--   0        0        0      589 2024-05-12 05:46:34.691574 zetascale-2.4.8/zeta/__init__.py
--rw-r--r--   0        0        0        0 2023-12-19 19:47:39.268788 zetascale-2.4.8/zeta/cli/__init__.py
--rw-r--r--   0        0        0     1937 2024-02-20 02:20:55.165790 zetascale-2.4.8/zeta/cli/main.py
--rw-r--r--   0        0        0      157 2024-02-20 03:07:47.757716 zetascale-2.4.8/zeta/cloud/__init__.py
--rw-r--r--   0        0        0     2071 2024-03-12 17:08:02.038250 zetascale-2.4.8/zeta/cloud/main.py
--rw-r--r--   0        0        0     6068 2024-05-12 05:58:58.805936 zetascale-2.4.8/zeta/cloud/sky_api.py
--rw-r--r--   0        0        0       59 2024-05-12 05:41:59.207175 zetascale-2.4.8/zeta/experimental/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 23:39:52.190261 zetascale-2.4.8/zeta/experimental/triton/__init__.py
--rw-r--r--   0        0        0     1656 2024-04-15 23:39:52.191052 zetascale-2.4.8/zeta/experimental/triton/activations/__init__.py
--rw-r--r--   0        0        0     2600 2024-05-01 15:39:09.414189 zetascale-2.4.8/zeta/experimental/triton/activations/activations.py
--rw-r--r--   0        0        0        0 2024-04-26 06:17:02.908501 zetascale-2.4.8/zeta/experimental/triton/activations/flash_mlp.py
--rw-r--r--   0        0        0     9532 2024-04-16 23:17:37.651487 zetascale-2.4.8/zeta/experimental/triton/activations/functions.py
--rw-r--r--   0        0        0        0 2024-04-26 06:07:35.941454 zetascale-2.4.8/zeta/experimental/triton/triton_modules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 06:09:19.979401 zetascale-2.4.8/zeta/experimental/triton/triton_modules/flash_mlp.py
--rw-r--r--   0        0        0     2806 2024-04-26 06:17:02.245347 zetascale-2.4.8/zeta/experimental/triton/triton_modules/linear_proj.py
--rw-r--r--   0        0        0     1809 2024-03-12 17:08:02.079698 zetascale-2.4.8/zeta/models/LongNet.py
--rw-r--r--   0        0        0        0 2023-07-10 01:12:17.230004 zetascale-2.4.8/zeta/models/Magneto.py
--rw-r--r--   0        0        0      603 2024-02-22 19:03:14.806609 zetascale-2.4.8/zeta/models/__init__.py
--rw-r--r--   0        0        0     3308 2024-04-06 16:42:16.819384 zetascale-2.4.8/zeta/models/andromeda.py
--rw-r--r--   0        0        0      135 2023-12-31 05:32:43.412544 zetascale-2.4.8/zeta/models/base.py
--rw-r--r--   0        0        0     3311 2024-03-12 17:08:02.117008 zetascale-2.4.8/zeta/models/beit3.py
--rw-r--r--   0        0        0     6752 2024-04-06 16:41:06.920915 zetascale-2.4.8/zeta/models/gpt4.py
--rw-r--r--   0        0        0     4288 2024-03-12 17:08:02.180350 zetascale-2.4.8/zeta/models/kosmos.py
--rw-r--r--   0        0        0      949 2024-04-06 16:41:06.963814 zetascale-2.4.8/zeta/models/llama.py
--rw-r--r--   0        0        0     3639 2024-03-12 17:08:02.150836 zetascale-2.4.8/zeta/models/max_vit.py
--rw-r--r--   0        0        0     6678 2024-03-12 17:08:02.311937 zetascale-2.4.8/zeta/models/mega_vit.py
--rw-r--r--   0        0        0     6927 2024-02-20 02:20:56.942968 zetascale-2.4.8/zeta/models/mm_mamba.py
--rw-r--r--   0        0        0    12991 2024-03-12 17:08:02.622848 zetascale-2.4.8/zeta/models/navit.py
--rw-r--r--   0        0        0     1884 2024-04-06 16:41:06.921869 zetascale-2.4.8/zeta/models/palme.py
--rw-r--r--   0        0        0     2762 2024-03-12 17:08:02.154861 zetascale-2.4.8/zeta/models/vit.py
--rw-r--r--   0        0        0      219 2024-02-20 03:07:47.976964 zetascale-2.4.8/zeta/nn/__init__.py
--rw-r--r--   0        0        0     1896 2024-05-13 18:51:51.885828 zetascale-2.4.8/zeta/nn/attention/__init__.py
--rw-r--r--   0        0        0     4184 2024-03-12 17:08:02.309118 zetascale-2.4.8/zeta/nn/attention/agent_attn.py
--rw-r--r--   0        0        0    14876 2024-03-12 17:08:02.715767 zetascale-2.4.8/zeta/nn/attention/attend.py
--rw-r--r--   0        0        0      244 2024-02-20 02:20:56.872011 zetascale-2.4.8/zeta/nn/attention/base.py
--rw-r--r--   0        0        0     4050 2024-03-12 17:08:02.358668 zetascale-2.4.8/zeta/nn/attention/cross_attention.py
--rw-r--r--   0        0        0     3236 2023-12-29 17:40:30.936298 zetascale-2.4.8/zeta/nn/attention/cross_attn_images.py
--rw-r--r--   0        0        0    10734 2024-03-12 17:08:02.527291 zetascale-2.4.8/zeta/nn/attention/dilated_attention.py
--rw-r--r--   0        0        0     8803 2024-03-12 17:08:02.448488 zetascale-2.4.8/zeta/nn/attention/flash_attention.py
--rw-r--r--   0        0        0     2161 2024-01-13 18:03:19.763236 zetascale-2.4.8/zeta/nn/attention/linear_attention.py
--rw-r--r--   0        0        0     2370 2024-03-12 17:08:02.307028 zetascale-2.4.8/zeta/nn/attention/linear_attn_l.py
--rw-r--r--   0        0        0     1679 2024-05-13 18:29:15.674496 zetascale-2.4.8/zeta/nn/attention/linearized_attention.py
--rw-r--r--   0        0        0     9794 2024-03-12 17:08:02.638502 zetascale-2.4.8/zeta/nn/attention/local_attention.py
--rw-r--r--   0        0        0     1966 2023-12-19 19:26:43.471021 zetascale-2.4.8/zeta/nn/attention/local_attention_mha.py
--rw-r--r--   0        0        0    18990 2024-03-12 17:08:03.268461 zetascale-2.4.8/zeta/nn/attention/mixture_attention.py
--rw-r--r--   0        0        0    12414 2024-03-19 16:54:57.559772 zetascale-2.4.8/zeta/nn/attention/multi_grouped_attn.py
--rw-r--r--   0        0        0     2729 2024-03-12 17:08:02.437305 zetascale-2.4.8/zeta/nn/attention/multi_modal_causal_attention.py
--rw-r--r--   0        0        0     3879 2023-12-29 18:02:53.657706 zetascale-2.4.8/zeta/nn/attention/multi_modal_cross_attn.py
--rw-r--r--   0        0        0     5769 2024-04-04 23:06:39.168105 zetascale-2.4.8/zeta/nn/attention/multihead_attention.py
--rw-r--r--   0        0        0    25390 2024-03-12 17:08:03.886143 zetascale-2.4.8/zeta/nn/attention/multiquery_attention.py
--rw-r--r--   0        0        0     3979 2024-04-06 02:43:03.176293 zetascale-2.4.8/zeta/nn/attention/scalable_img_self_attn.py
--rw-r--r--   0        0        0     2198 2024-02-20 02:21:01.439585 zetascale-2.4.8/zeta/nn/attention/shaped_attention.py
--rw-r--r--   0        0        0     4672 2024-02-20 02:21:02.943176 zetascale-2.4.8/zeta/nn/attention/sparse_attention.py
--rw-r--r--   0        0        0     1741 2024-03-12 17:08:02.503328 zetascale-2.4.8/zeta/nn/attention/spatial_linear_attention.py
--rw-r--r--   0        0        0     2973 2024-02-20 02:21:01.927064 zetascale-2.4.8/zeta/nn/attention/xc_attention.py
--rw-r--r--   0        0        0      482 2024-02-20 02:21:01.042463 zetascale-2.4.8/zeta/nn/biases/__init__.py
--rw-r--r--   0        0        0     3951 2024-03-12 17:08:02.722676 zetascale-2.4.8/zeta/nn/biases/alibi.py
--rw-r--r--   0        0        0      245 2024-02-20 02:21:01.653481 zetascale-2.4.8/zeta/nn/biases/base.py
--rw-r--r--   0        0        0     1348 2024-02-20 02:21:02.183763 zetascale-2.4.8/zeta/nn/biases/dynamic_position_bias.py
--rw-r--r--   0        0        0     2886 2024-03-12 17:08:02.668729 zetascale-2.4.8/zeta/nn/biases/relative_position_bias.py
--rw-r--r--   0        0        0     2069 2024-03-02 07:30:50.700992 zetascale-2.4.8/zeta/nn/embeddings/__init__.py
--rw-r--r--   0        0        0     1231 2023-12-23 05:23:23.147156 zetascale-2.4.8/zeta/nn/embeddings/abc_pos_emb.py
--rw-r--r--   0        0        0      255 2024-02-20 02:21:02.347272 zetascale-2.4.8/zeta/nn/embeddings/base.py
--rw-r--r--   0        0        0      723 2024-02-20 02:21:02.661920 zetascale-2.4.8/zeta/nn/embeddings/embedding.py
--rw-r--r--   0        0        0     2509 2024-01-07 05:11:05.739698 zetascale-2.4.8/zeta/nn/embeddings/multiway_network.py
--rw-r--r--   0        0        0      358 2024-02-20 02:21:02.600313 zetascale-2.4.8/zeta/nn/embeddings/nominal_embeddings.py
--rw-r--r--   0        0        0      900 2023-10-24 04:07:16.862154 zetascale-2.4.8/zeta/nn/embeddings/patch_embedding.py
--rw-r--r--   0        0        0     3120 2024-02-20 02:21:03.171183 zetascale-2.4.8/zeta/nn/embeddings/pi.md
--rw-r--r--   0        0        0     1996 2024-03-12 17:08:02.654239 zetascale-2.4.8/zeta/nn/embeddings/positional.py
--rw-r--r--   0        0        0     2584 2024-03-12 17:08:02.753885 zetascale-2.4.8/zeta/nn/embeddings/positional_interpolation.py
--rw-r--r--   0        0        0     3021 2024-03-12 17:08:02.747974 zetascale-2.4.8/zeta/nn/embeddings/qfsp_embeddings.py
--rw-r--r--   0        0        0     1668 2024-03-12 17:08:02.722910 zetascale-2.4.8/zeta/nn/embeddings/qft_embeddings.py
--rw-r--r--   0        0        0     2250 2024-02-20 02:21:03.986803 zetascale-2.4.8/zeta/nn/embeddings/rope.py
--rw-r--r--   0        0        0     1570 2024-03-02 07:30:50.701708 zetascale-2.4.8/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py
--rw-r--r--   0        0        0     2345 2024-03-12 17:08:02.798633 zetascale-2.4.8/zeta/nn/embeddings/sine_positional.py
--rw-r--r--   0        0        0     2650 2024-03-12 17:08:02.815289 zetascale-2.4.8/zeta/nn/embeddings/sinusoidal.py
--rw-r--r--   0        0        0     1810 2024-03-12 17:08:02.785699 zetascale-2.4.8/zeta/nn/embeddings/truncated_rope.py
--rw-r--r--   0        0        0     1003 2023-10-24 04:10:28.452387 zetascale-2.4.8/zeta/nn/embeddings/vis_lang_emb.py
--rw-r--r--   0        0        0     3195 2024-03-12 17:08:02.854455 zetascale-2.4.8/zeta/nn/embeddings/vision_emb.py
--rw-r--r--   0        0        0     3208 2023-11-24 07:50:24.220934 zetascale-2.4.8/zeta/nn/embeddings/xpos_relative_position.py
--rw-r--r--   0        0        0     6685 2024-03-12 17:08:03.090171 zetascale-2.4.8/zeta/nn/embeddings/yarn.py
--rw-r--r--   0        0        0     1150 2024-02-20 02:21:04.287040 zetascale-2.4.8/zeta/nn/masks/__init__.py
--rw-r--r--   0        0        0    31987 2024-03-12 17:08:04.258733 zetascale-2.4.8/zeta/nn/masks/attn_masks.py
--rw-r--r--   0        0        0     1248 2024-03-12 17:08:02.883585 zetascale-2.4.8/zeta/nn/masks/block_diagonal.py
--rw-r--r--   0        0        0    15253 2023-09-12 13:55:36.035815 zetascale-2.4.8/zeta/nn/modules/README.md
--rw-r--r--   0        0        0    13800 2024-05-13 03:47:11.311792 zetascale-2.4.8/zeta/nn/modules/__init__.py
--rw-r--r--   0        0        0     7658 2024-03-12 17:08:03.198677 zetascale-2.4.8/zeta/nn/modules/_activations.py
--rw-r--r--   0        0        0     3561 2024-03-12 17:08:03.078712 zetascale-2.4.8/zeta/nn/modules/adaptive_conv.py
--rw-r--r--   0        0        0     1572 2024-02-20 02:21:05.564114 zetascale-2.4.8/zeta/nn/modules/adaptive_layernorm.py
--rw-r--r--   0        0        0     1506 2024-02-20 02:21:05.599056 zetascale-2.4.8/zeta/nn/modules/adaptive_parameter_list.py
--rw-r--r--   0        0        0     2181 2024-03-12 17:08:03.031630 zetascale-2.4.8/zeta/nn/modules/adaptive_rmsnorm.py
--rw-r--r--   0        0        0      465 2024-02-20 02:21:05.714929 zetascale-2.4.8/zeta/nn/modules/add_norm.py
--rw-r--r--   0        0        0     1969 2024-03-12 17:08:03.054998 zetascale-2.4.8/zeta/nn/modules/alr_block.py
--rw-r--r--   0        0        0     1885 2024-02-20 02:21:07.006024 zetascale-2.4.8/zeta/nn/modules/attn.py
--rw-r--r--   0        0        0     1170 2024-02-20 02:21:06.839757 zetascale-2.4.8/zeta/nn/modules/audio_to_text.py
--rw-r--r--   0        0        0     2927 2024-03-12 17:08:03.099808 zetascale-2.4.8/zeta/nn/modules/avg_model_merger.py
--rw-r--r--   0        0        0      200 2023-12-19 19:26:43.426210 zetascale-2.4.8/zeta/nn/modules/batched_dp.py
--rw-r--r--   0        0        0     2355 2024-02-20 02:21:07.701284 zetascale-2.4.8/zeta/nn/modules/block_butterfly_mlp.py
--rw-r--r--   0        0        0    12708 2024-03-12 17:08:03.864220 zetascale-2.4.8/zeta/nn/modules/blockdiag_butterfly.py
--rw-r--r--   0        0        0      986 2024-04-06 02:43:02.103486 zetascale-2.4.8/zeta/nn/modules/chan_layer_norm.py
--rw-r--r--   0        0        0     7693 2024-03-12 17:08:03.471293 zetascale-2.4.8/zeta/nn/modules/clex.py
--rw-r--r--   0        0        0     2522 2024-03-12 17:08:03.192850 zetascale-2.4.8/zeta/nn/modules/clip_bottleneck.py
--rw-r--r--   0        0        0     1530 2024-03-12 17:08:03.171903 zetascale-2.4.8/zeta/nn/modules/cnn_text.py
--rw-r--r--   0        0        0     4281 2024-03-12 17:08:03.300302 zetascale-2.4.8/zeta/nn/modules/combined_linear.py
--rw-r--r--   0        0        0     1026 2024-02-20 02:21:08.160986 zetascale-2.4.8/zeta/nn/modules/conv_bn_relu.py
--rw-r--r--   0        0        0     2446 2024-03-12 17:08:03.304310 zetascale-2.4.8/zeta/nn/modules/conv_mlp.py
--rw-r--r--   0        0        0      888 2024-02-20 02:21:09.097401 zetascale-2.4.8/zeta/nn/modules/convnet.py
--rw-r--r--   0        0        0     1723 2023-12-29 18:03:56.299433 zetascale-2.4.8/zeta/nn/modules/cross_embed_layer.py
--rw-r--r--   0        0        0     7316 2024-03-12 17:08:03.415262 zetascale-2.4.8/zeta/nn/modules/cross_modal_reparametization.py
--rw-r--r--   0        0        0     3540 2024-03-12 17:08:03.361727 zetascale-2.4.8/zeta/nn/modules/decision_tree.py
--rw-r--r--   0        0        0     2648 2024-02-20 02:21:10.160405 zetascale-2.4.8/zeta/nn/modules/deepseek_moe.py
--rw-r--r--   0        0        0      794 2023-12-25 18:55:47.859671 zetascale-2.4.8/zeta/nn/modules/dense_connect.py
--rw-r--r--   0        0        0     2371 2024-02-20 02:21:09.798586 zetascale-2.4.8/zeta/nn/modules/diffusion.py
--rw-r--r--   0        0        0     1538 2024-04-04 01:08:54.948939 zetascale-2.4.8/zeta/nn/modules/droppath.py
--rw-r--r--   0        0        0      796 2023-12-25 19:11:45.652469 zetascale-2.4.8/zeta/nn/modules/dual_path_block.py
--rw-r--r--   0        0        0     4687 2024-02-20 02:21:11.437130 zetascale-2.4.8/zeta/nn/modules/dyna_conv.py
--rw-r--r--   0        0        0     2064 2024-02-20 02:21:10.627986 zetascale-2.4.8/zeta/nn/modules/dynamic_module.py
--rw-r--r--   0        0        0      980 2024-03-12 17:08:03.323481 zetascale-2.4.8/zeta/nn/modules/dynamic_routing_block.py
--rw-r--r--   0        0        0      786 2023-10-24 05:22:56.453163 zetascale-2.4.8/zeta/nn/modules/embedding_to_grid.py
--rw-r--r--   0        0        0    11202 2024-03-12 17:08:03.369914 zetascale-2.4.8/zeta/nn/modules/ether.py
--rw-r--r--   0        0        0     5338 2024-02-20 02:21:10.712472 zetascale-2.4.8/zeta/nn/modules/exo.py
--rw-r--r--   0        0        0       90 2024-05-13 03:46:35.602087 zetascale-2.4.8/zeta/nn/modules/expand.py
--rw-r--r--   0        0        0      888 2023-10-24 05:22:56.487707 zetascale-2.4.8/zeta/nn/modules/expand_channels.py
--rw-r--r--   0        0        0     1184 2024-01-08 00:23:23.966366 zetascale-2.4.8/zeta/nn/modules/expert.py
--rw-r--r--   0        0        0      678 2024-02-20 02:21:11.125020 zetascale-2.4.8/zeta/nn/modules/fast_text.py
--rw-r--r--   0        0        0     1004 2023-12-25 19:10:00.967347 zetascale-2.4.8/zeta/nn/modules/feedback_block.py
--rw-r--r--   0        0        0     4666 2024-05-12 05:48:56.439577 zetascale-2.4.8/zeta/nn/modules/feedforward.py
--rw-r--r--   0        0        0     4396 2024-03-12 17:08:03.564214 zetascale-2.4.8/zeta/nn/modules/feedforward_network.py
--rw-r--r--   0        0        0     3153 2024-03-12 17:08:03.438496 zetascale-2.4.8/zeta/nn/modules/film.py
--rw-r--r--   0        0        0     2607 2024-01-14 05:11:08.698323 zetascale-2.4.8/zeta/nn/modules/film_conditioning.py
--rw-r--r--   0        0        0     2657 2024-02-20 02:21:12.679701 zetascale-2.4.8/zeta/nn/modules/film_efficient_metb3.py
--rw-r--r--   0        0        0      363 2023-11-18 04:30:04.310707 zetascale-2.4.8/zeta/nn/modules/flash_conv.py
--rw-r--r--   0        0        0      817 2023-12-19 19:26:43.429076 zetascale-2.4.8/zeta/nn/modules/flatten_features.py
--rw-r--r--   0        0        0     3528 2024-03-12 17:08:03.523933 zetascale-2.4.8/zeta/nn/modules/flex_conv.py
--rw-r--r--   0        0        0     2694 2024-03-12 17:08:03.538134 zetascale-2.4.8/zeta/nn/modules/flexible_mlp.py
--rw-r--r--   0        0        0      845 2024-05-12 05:58:20.250517 zetascale-2.4.8/zeta/nn/modules/fractoral_norm.py
--rw-r--r--   0        0        0     2552 2024-03-12 17:08:03.528011 zetascale-2.4.8/zeta/nn/modules/fractorial_net.py
--rw-r--r--   0        0        0      769 2024-02-22 19:14:04.770478 zetascale-2.4.8/zeta/nn/modules/freeze_layers.py
--rw-r--r--   0        0        0     2408 2024-03-12 17:08:03.534463 zetascale-2.4.8/zeta/nn/modules/fused_dropout_add.py
--rw-r--r--   0        0        0     1223 2024-02-20 02:21:13.183242 zetascale-2.4.8/zeta/nn/modules/fused_dropout_layernom.py
--rw-r--r--   0        0        0     2268 2024-02-20 02:21:13.592327 zetascale-2.4.8/zeta/nn/modules/fused_gelu_dense.py
--rw-r--r--   0        0        0     1006 2024-02-20 02:21:13.298075 zetascale-2.4.8/zeta/nn/modules/fusion_ffn.py
--rw-r--r--   0        0        0    33392 2024-03-12 17:08:05.481194 zetascale-2.4.8/zeta/nn/modules/g_shard_moe.py
--rw-r--r--   0        0        0      707 2023-12-27 16:22:31.740775 zetascale-2.4.8/zeta/nn/modules/gated_residual_block.py
--rw-r--r--   0        0        0     4104 2024-03-12 17:08:03.702885 zetascale-2.4.8/zeta/nn/modules/gill_mapper.py
--rw-r--r--   0        0        0      920 2024-02-20 03:19:54.342658 zetascale-2.4.8/zeta/nn/modules/glu.py
--rw-r--r--   0        0        0     1826 2024-03-12 17:08:03.620762 zetascale-2.4.8/zeta/nn/modules/gru_gating.py
--rw-r--r--   0        0        0     2634 2023-11-30 08:00:40.761474 zetascale-2.4.8/zeta/nn/modules/h3.py
--rw-r--r--   0        0        0     2078 2024-02-20 02:21:13.917866 zetascale-2.4.8/zeta/nn/modules/hebbian.py
--rw-r--r--   0        0        0      809 2024-02-20 02:21:13.641036 zetascale-2.4.8/zeta/nn/modules/highway_layer.py
--rw-r--r--   0        0        0     3527 2024-03-12 17:08:03.674327 zetascale-2.4.8/zeta/nn/modules/image_projector.py
--rw-r--r--   0        0        0     1049 2024-02-20 02:21:14.054761 zetascale-2.4.8/zeta/nn/modules/image_to_text.py
--rw-r--r--   0        0        0     1385 2024-02-20 02:21:14.700462 zetascale-2.4.8/zeta/nn/modules/img_or_video_to_time.py
--rw-r--r--   0        0        0     1197 2023-12-21 06:04:56.833591 zetascale-2.4.8/zeta/nn/modules/img_patch_embed.py
--rw-r--r--   0        0        0      763 2023-10-24 05:22:56.462573 zetascale-2.4.8/zeta/nn/modules/img_reshape.py
--rw-r--r--   0        0        0     4024 2024-03-12 17:08:03.899369 zetascale-2.4.8/zeta/nn/modules/itca.py
--rw-r--r--   0        0        0    12420 2024-05-06 21:52:38.421607 zetascale-2.4.8/zeta/nn/modules/kan.py
--rw-r--r--   0        0        0     4656 2024-03-12 17:08:03.898644 zetascale-2.4.8/zeta/nn/modules/kv_cache.py
--rw-r--r--   0        0        0     2586 2024-05-12 14:28:32.087650 zetascale-2.4.8/zeta/nn/modules/kv_cache_update.py
--rw-r--r--   0        0        0     6221 2024-03-12 17:08:04.137958 zetascale-2.4.8/zeta/nn/modules/lambda_mask.py
--rw-r--r--   0        0        0     3504 2024-02-20 02:21:15.562473 zetascale-2.4.8/zeta/nn/modules/lang_conv_module.py
--rw-r--r--   0        0        0     2760 2024-02-20 02:21:15.370804 zetascale-2.4.8/zeta/nn/modules/laser.py
--rw-r--r--   0        0        0      919 2024-05-12 05:48:56.370543 zetascale-2.4.8/zeta/nn/modules/layer_scale.py
--rw-r--r--   0        0        0     2379 2024-02-20 02:21:15.528047 zetascale-2.4.8/zeta/nn/modules/layernorm.py
--rw-r--r--   0        0        0     1132 2024-02-20 02:21:15.732195 zetascale-2.4.8/zeta/nn/modules/leaky_relu.py
--rw-r--r--   0        0        0    24514 2024-03-12 17:08:04.551145 zetascale-2.4.8/zeta/nn/modules/log_ff.py
--rw-r--r--   0        0        0     1747 2023-12-29 16:19:54.276255 zetascale-2.4.8/zeta/nn/modules/lora.py
--rw-r--r--   0        0        0     3240 2024-03-12 17:08:03.982193 zetascale-2.4.8/zeta/nn/modules/matrix.py
--rw-r--r--   0        0        0     2993 2024-02-05 02:47:16.470298 zetascale-2.4.8/zeta/nn/modules/mbconv.py
--rw-r--r--   0        0        0     3127 2024-04-30 02:48:22.341238 zetascale-2.4.8/zeta/nn/modules/mixtape.py
--rw-r--r--   0        0        0     2125 2024-02-20 02:21:16.517619 zetascale-2.4.8/zeta/nn/modules/mixtral_expert.py
--rw-r--r--   0        0        0     1884 2024-03-12 17:08:03.941463 zetascale-2.4.8/zeta/nn/modules/mlp.py
--rw-r--r--   0        0        0     3729 2024-03-12 17:08:04.025060 zetascale-2.4.8/zeta/nn/modules/mlp_mixer.py
--rw-r--r--   0        0        0     2435 2024-02-20 02:21:17.308630 zetascale-2.4.8/zeta/nn/modules/mm_adapter.py
--rw-r--r--   0        0        0       87 2024-01-13 18:34:06.474255 zetascale-2.4.8/zeta/nn/modules/mm_fusion.py
--rw-r--r--   0        0        0     2340 2024-02-20 02:21:17.406784 zetascale-2.4.8/zeta/nn/modules/mm_layernorm.py
--rw-r--r--   0        0        0     1405 2024-03-12 17:08:03.947904 zetascale-2.4.8/zeta/nn/modules/mm_ops.py
--rw-r--r--   0        0        0     6234 2024-03-12 17:08:04.186893 zetascale-2.4.8/zeta/nn/modules/modality_adaptive_module.py
--rw-r--r--   0        0        0     2930 2024-01-12 20:34:35.589003 zetascale-2.4.8/zeta/nn/modules/moe.py
--rw-r--r--   0        0        0     3228 2024-03-12 17:08:04.066438 zetascale-2.4.8/zeta/nn/modules/moe_router.py
--rw-r--r--   0        0        0      776 2024-02-20 02:21:17.825560 zetascale-2.4.8/zeta/nn/modules/monarch_mlp.py
--rw-r--r--   0        0        0     1564 2024-03-06 07:48:51.576854 zetascale-2.4.8/zeta/nn/modules/mr_adapter.py
--rw-r--r--   0        0        0     6686 2024-04-30 13:48:05.441915 zetascale-2.4.8/zeta/nn/modules/multi_input_multi_output.py
--rw-r--r--   0        0        0      837 2024-02-20 02:21:18.368530 zetascale-2.4.8/zeta/nn/modules/multi_scale_block.py
--rw-r--r--   0        0        0        2 2023-11-10 22:26:53.685193 zetascale-2.4.8/zeta/nn/modules/multiclass_label.py
--rw-r--r--   0        0        0      225 2023-12-19 19:26:43.445812 zetascale-2.4.8/zeta/nn/modules/multimodal_concat.py
--rw-r--r--   0        0        0      472 2024-02-20 02:21:18.382142 zetascale-2.4.8/zeta/nn/modules/nearest_upsample.py
--rw-r--r--   0        0        0     8309 2024-03-12 17:08:04.427188 zetascale-2.4.8/zeta/nn/modules/nebula.py
--rw-r--r--   0        0        0     2590 2024-02-20 02:21:19.424059 zetascale-2.4.8/zeta/nn/modules/nfn_stem.py
--rw-r--r--   0        0        0     1456 2024-02-20 02:21:18.846159 zetascale-2.4.8/zeta/nn/modules/norm_fractorals.py
--rw-r--r--   0        0        0     2034 2024-01-13 01:44:35.836293 zetascale-2.4.8/zeta/nn/modules/norm_utils.py
--rw-r--r--   0        0        0     2842 2024-02-20 02:21:20.023982 zetascale-2.4.8/zeta/nn/modules/omnimodal_fusion.py
--rw-r--r--   0        0        0     3851 2024-01-13 22:08:51.525372 zetascale-2.4.8/zeta/nn/modules/p_scan.py
--rw-r--r--   0        0        0     2571 2024-02-23 08:38:09.264979 zetascale-2.4.8/zeta/nn/modules/palo_ldp.py
--rw-r--r--   0        0        0      601 2024-01-12 16:28:17.189839 zetascale-2.4.8/zeta/nn/modules/parallel_wrapper.py
--rw-r--r--   0        0        0      200 2024-02-20 02:21:19.576787 zetascale-2.4.8/zeta/nn/modules/patch_img.py
--rw-r--r--   0        0        0     6597 2024-04-06 16:39:25.176606 zetascale-2.4.8/zeta/nn/modules/patch_linear_flatten.py
--rw-r--r--   0        0        0      985 2024-01-11 04:33:38.594357 zetascale-2.4.8/zeta/nn/modules/patch_video.py
--rw-r--r--   0        0        0      783 2024-04-06 02:43:03.113003 zetascale-2.4.8/zeta/nn/modules/peg.py
--rw-r--r--   0        0        0     3180 2024-01-10 07:40:01.644421 zetascale-2.4.8/zeta/nn/modules/perceiver_layer.py
--rw-r--r--   0        0        0     6115 2024-03-12 17:08:04.440415 zetascale-2.4.8/zeta/nn/modules/perceiver_resampler.py
--rw-r--r--   0        0        0     2594 2024-04-26 16:25:55.402282 zetascale-2.4.8/zeta/nn/modules/pixel_shuffling.py
--rw-r--r--   0        0        0     1692 2024-03-12 17:08:04.160718 zetascale-2.4.8/zeta/nn/modules/poly_expert_fusion_network.py
--rw-r--r--   0        0        0     2045 2024-02-20 02:21:20.607131 zetascale-2.4.8/zeta/nn/modules/polymorphic_activation.py
--rw-r--r--   0        0        0     5804 2024-02-20 02:21:21.939907 zetascale-2.4.8/zeta/nn/modules/polymorphic_neuron.py
--rw-r--r--   0        0        0      527 2023-11-29 20:30:23.164354 zetascale-2.4.8/zeta/nn/modules/prenorm.py
--rw-r--r--   0        0        0     1299 2024-03-12 17:08:04.183108 zetascale-2.4.8/zeta/nn/modules/proj_then_softmax.py
--rw-r--r--   0        0        0     7164 2024-03-12 17:08:04.267345 zetascale-2.4.8/zeta/nn/modules/pulsar.py
--rw-r--r--   0        0        0     3451 2024-02-20 02:21:21.996199 zetascale-2.4.8/zeta/nn/modules/pyro.py
--rw-r--r--   0        0        0     9454 2024-03-12 17:08:04.485725 zetascale-2.4.8/zeta/nn/modules/qformer.py
--rw-r--r--   0        0        0      812 2024-01-15 23:55:29.316200 zetascale-2.4.8/zeta/nn/modules/qkv_norm.py
--rw-r--r--   0        0        0     1381 2024-02-20 02:21:22.210314 zetascale-2.4.8/zeta/nn/modules/quantized_layernorm.py
--rw-r--r--   0        0        0      983 2024-04-16 23:17:41.316433 zetascale-2.4.8/zeta/nn/modules/query_proposal.py
--rw-r--r--   0        0        0     1152 2024-03-12 17:08:04.219236 zetascale-2.4.8/zeta/nn/modules/recurrent_model.py
--rw-r--r--   0        0        0      903 2023-12-25 19:15:44.005559 zetascale-2.4.8/zeta/nn/modules/recursive_block.py
--rw-r--r--   0        0        0      369 2024-03-02 07:30:50.680921 zetascale-2.4.8/zeta/nn/modules/relu_squared.py
--rw-r--r--   0        0        0     5037 2024-03-12 17:08:04.445015 zetascale-2.4.8/zeta/nn/modules/res_net.py
--rw-r--r--   0        0        0      492 2023-10-24 04:20:58.291559 zetascale-2.4.8/zeta/nn/modules/residual.py
--rw-r--r--   0        0        0     2238 2024-02-20 02:21:23.245499 zetascale-2.4.8/zeta/nn/modules/resnet.py
--rw-r--r--   0        0        0     5349 2024-04-06 16:41:07.021184 zetascale-2.4.8/zeta/nn/modules/return_loss_text.py
--rw-r--r--   0        0        0      829 2024-02-20 02:21:22.626278 zetascale-2.4.8/zeta/nn/modules/rms_norm.py
--rw-r--r--   0        0        0     1646 2024-02-20 02:21:22.868825 zetascale-2.4.8/zeta/nn/modules/rnn_nlp.py
--rw-r--r--   0        0        0     3106 2024-03-12 17:08:04.350941 zetascale-2.4.8/zeta/nn/modules/s4.py
--rw-r--r--   0        0        0      818 2023-12-19 19:26:43.446233 zetascale-2.4.8/zeta/nn/modules/scale.py
--rw-r--r--   0        0        0      882 2024-03-02 07:30:51.064762 zetascale-2.4.8/zeta/nn/modules/scale_norm.py
--rw-r--r--   0        0        0     1433 2024-02-20 02:21:23.383643 zetascale-2.4.8/zeta/nn/modules/scaled_sinusoidal.py
--rw-r--r--   0        0        0      799 2023-10-24 15:36:34.861776 zetascale-2.4.8/zeta/nn/modules/scalenorm.py
--rw-r--r--   0        0        0     1858 2024-02-20 02:21:23.545588 zetascale-2.4.8/zeta/nn/modules/shift_tokens.py
--rw-r--r--   0        0        0     2877 2024-02-20 02:21:23.721206 zetascale-2.4.8/zeta/nn/modules/shufflenet.py
--rw-r--r--   0        0        0     8939 2024-03-12 17:08:04.608471 zetascale-2.4.8/zeta/nn/modules/sig_lip.py
--rw-r--r--   0        0        0      283 2023-11-09 00:22:32.316816 zetascale-2.4.8/zeta/nn/modules/simple_attention.py
--rw-r--r--   0        0        0      692 2023-11-12 15:13:51.606294 zetascale-2.4.8/zeta/nn/modules/simple_feedforward.py
--rw-r--r--   0        0        0     9719 2024-04-15 23:39:52.195609 zetascale-2.4.8/zeta/nn/modules/simple_mamba.py
--rw-r--r--   0        0        0      764 2023-12-19 19:26:43.436224 zetascale-2.4.8/zeta/nn/modules/simple_res_block.py
--rw-r--r--   0        0        0      978 2023-12-23 05:14:59.170325 zetascale-2.4.8/zeta/nn/modules/simple_resblock.py
--rw-r--r--   0        0        0      638 2023-12-19 19:26:43.443919 zetascale-2.4.8/zeta/nn/modules/simple_rmsnorm.py
--rw-r--r--   0        0        0      509 2023-12-25 18:55:47.862390 zetascale-2.4.8/zeta/nn/modules/skip_connect.py
--rw-r--r--   0        0        0     1194 2024-02-20 02:21:23.914746 zetascale-2.4.8/zeta/nn/modules/skipconnection.py
--rw-r--r--   0        0        0     3553 2024-03-12 17:08:04.540860 zetascale-2.4.8/zeta/nn/modules/slerp_model_merger.py
--rw-r--r--   0        0        0      765 2024-01-16 18:48:36.091054 zetascale-2.4.8/zeta/nn/modules/sp_act.py
--rw-r--r--   0        0        0    22039 2024-03-12 17:08:05.932332 zetascale-2.4.8/zeta/nn/modules/space_time_unet.py
--rw-r--r--   0        0        0     1346 2024-03-12 17:08:04.539605 zetascale-2.4.8/zeta/nn/modules/spacial_transformer.py
--rw-r--r--   0        0        0     4976 2024-02-20 02:21:25.283384 zetascale-2.4.8/zeta/nn/modules/sparq_attn.py
--rw-r--r--   0        0        0    13915 2024-04-01 18:09:39.794061 zetascale-2.4.8/zeta/nn/modules/sparse_moe.py
--rw-r--r--   0        0        0     2021 2024-02-20 02:21:24.433522 zetascale-2.4.8/zeta/nn/modules/spatial_downsample.py
--rw-r--r--   0        0        0     1346 2024-03-12 17:08:04.544222 zetascale-2.4.8/zeta/nn/modules/spatial_transformer.py
--rw-r--r--   0        0        0     5006 2024-05-06 18:59:13.507341 zetascale-2.4.8/zeta/nn/modules/splines.py
--rw-r--r--   0        0        0     1041 2024-02-20 02:21:24.810848 zetascale-2.4.8/zeta/nn/modules/squeeze_excitation.py
--rw-r--r--   0        0        0     4334 2024-03-12 17:08:04.701025 zetascale-2.4.8/zeta/nn/modules/ssm.py
--rw-r--r--   0        0        0     7305 2024-03-12 17:08:04.788869 zetascale-2.4.8/zeta/nn/modules/ssm_language.py
--rw-r--r--   0        0        0      942 2024-01-08 00:04:54.571884 zetascale-2.4.8/zeta/nn/modules/stoch_depth.py
--rw-r--r--   0        0        0      958 2023-12-27 16:23:01.966770 zetascale-2.4.8/zeta/nn/modules/stochastic_depth.py
--rw-r--r--   0        0        0     2032 2024-02-20 02:21:25.534554 zetascale-2.4.8/zeta/nn/modules/subln.py
--rw-r--r--   0        0        0      972 2024-02-20 02:21:25.575751 zetascale-2.4.8/zeta/nn/modules/super_resolution.py
--rw-r--r--   0        0        0     5626 2024-03-12 17:08:04.744143 zetascale-2.4.8/zeta/nn/modules/swarmalator.py
--rw-r--r--   0        0        0     1313 2024-02-20 02:21:25.712744 zetascale-2.4.8/zeta/nn/modules/swiglu.py
--rw-r--r--   0        0        0      715 2024-02-20 02:21:25.696562 zetascale-2.4.8/zeta/nn/modules/tensor.py
--rw-r--r--   0        0        0      865 2024-01-09 16:54:56.616879 zetascale-2.4.8/zeta/nn/modules/tensor_to_int.py
--rw-r--r--   0        0        0     3281 2024-03-12 17:08:04.639643 zetascale-2.4.8/zeta/nn/modules/text_scene_fusion.py
--rw-r--r--   0        0        0     2692 2024-03-12 17:08:04.672980 zetascale-2.4.8/zeta/nn/modules/text_video_fuse.py
--rw-r--r--   0        0        0     2104 2024-02-20 02:21:26.347288 zetascale-2.4.8/zeta/nn/modules/time_up_sample.py
--rw-r--r--   0        0        0      631 2024-03-12 17:08:04.667636 zetascale-2.4.8/zeta/nn/modules/to_logits.py
--rw-r--r--   0        0        0     2158 2024-03-12 17:08:04.706429 zetascale-2.4.8/zeta/nn/modules/token_learner.py
--rw-r--r--   0        0        0     1075 2024-02-20 02:21:26.152416 zetascale-2.4.8/zeta/nn/modules/token_mixer.py
--rw-r--r--   0        0        0      189 2023-10-07 02:00:01.902947 zetascale-2.4.8/zeta/nn/modules/token_shift.py
--rw-r--r--   0        0        0    10310 2024-03-12 17:08:05.210522 zetascale-2.4.8/zeta/nn/modules/top_n_gating.py
--rw-r--r--   0        0        0     4363 2024-02-20 02:21:27.101778 zetascale-2.4.8/zeta/nn/modules/transformations.py
--rw-r--r--   0        0        0      921 2024-02-20 02:21:26.371224 zetascale-2.4.8/zeta/nn/modules/triple_skip.py
--rw-r--r--   0        0        0     2193 2024-01-23 14:49:04.463435 zetascale-2.4.8/zeta/nn/modules/triton_rmsnorm.py
--rw-r--r--   0        0        0     4112 2024-01-10 18:04:05.447145 zetascale-2.4.8/zeta/nn/modules/u_mamba.py
--rw-r--r--   0        0        0     4717 2024-03-12 17:08:04.956574 zetascale-2.4.8/zeta/nn/modules/unet.py
--rw-r--r--   0        0        0      974 2024-02-20 02:21:26.656166 zetascale-2.4.8/zeta/nn/modules/v_layernorm.py
--rw-r--r--   0        0        0     1686 2024-03-12 17:08:04.807655 zetascale-2.4.8/zeta/nn/modules/v_pool.py
--rw-r--r--   0        0        0     2809 2024-02-20 02:21:27.251834 zetascale-2.4.8/zeta/nn/modules/video_autoencoder.py
--rw-r--r--   0        0        0     9239 2024-03-12 17:08:05.102603 zetascale-2.4.8/zeta/nn/modules/video_diffusion_modules.py
--rw-r--r--   0        0        0     1497 2024-01-09 02:18:08.376975 zetascale-2.4.8/zeta/nn/modules/video_to_tensor.py
--rw-r--r--   0        0        0     1067 2024-02-20 02:21:27.232331 zetascale-2.4.8/zeta/nn/modules/video_to_text.py
--rw-r--r--   0        0        0     2702 2024-02-20 02:21:27.552948 zetascale-2.4.8/zeta/nn/modules/vision_mamba.py
--rw-r--r--   0        0        0     2018 2024-03-12 17:08:04.833044 zetascale-2.4.8/zeta/nn/modules/vision_weighted_permute_mlp.py
--rw-r--r--   0        0        0     5445 2024-02-20 02:21:27.810272 zetascale-2.4.8/zeta/nn/modules/visual_expert.py
--rw-r--r--   0        0        0     6100 2024-03-12 17:08:05.088354 zetascale-2.4.8/zeta/nn/modules/vit_denoiser.py
--rw-r--r--   0        0        0     3099 2024-02-20 02:21:28.252160 zetascale-2.4.8/zeta/nn/modules/vss_block.py
--rw-r--r--   0        0        0     2775 2024-03-12 17:08:04.893657 zetascale-2.4.8/zeta/nn/modules/ws_conv2d.py
--rw-r--r--   0        0        0       86 2023-07-09 23:46:34.364954 zetascale-2.4.8/zeta/nn/modules/xmoe/__init__.py
--rw-r--r--   0        0        0     2351 2024-03-12 17:08:05.082817 zetascale-2.4.8/zeta/nn/modules/xmoe/global_groups.py
--rw-r--r--   0        0        0    12458 2024-03-12 17:08:05.702507 zetascale-2.4.8/zeta/nn/modules/xmoe/moe_layer.py
--rw-r--r--   0        0        0    18694 2024-03-12 17:08:06.021245 zetascale-2.4.8/zeta/nn/modules/xmoe/routing.py
--rw-r--r--   0        0        0     2302 2024-03-12 17:08:05.160919 zetascale-2.4.8/zeta/nn/modules/yolo.py
--rw-r--r--   0        0        0     2595 2024-02-20 02:21:28.852202 zetascale-2.4.8/zeta/ops/__init__.py
--rw-r--r--   0        0        0      287 2024-01-07 07:16:03.424289 zetascale-2.4.8/zeta/ops/absmax.py
--rw-r--r--   0        0        0     2652 2024-03-12 17:08:05.173619 zetascale-2.4.8/zeta/ops/async_softmax.py
--rw-r--r--   0        0        0     2054 2024-01-07 05:11:53.247763 zetascale-2.4.8/zeta/ops/dilated_attn_ops.py
--rw-r--r--   0        0        0     2017 2024-03-12 17:08:05.321616 zetascale-2.4.8/zeta/ops/einops_from_to.py
--rw-r--r--   0        0        0     1876 2024-03-12 17:08:05.320032 zetascale-2.4.8/zeta/ops/einops_poly.py
--rw-r--r--   0        0        0     2150 2024-03-19 17:49:56.995242 zetascale-2.4.8/zeta/ops/expand.py
--rw-r--r--   0        0        0     1262 2024-03-12 17:08:05.374955 zetascale-2.4.8/zeta/ops/laplace.py
--rw-r--r--   0        0        0    16138 2024-03-12 17:08:05.848451 zetascale-2.4.8/zeta/ops/main.py
--rw-r--r--   0        0        0     1392 2024-02-20 02:21:29.213231 zetascale-2.4.8/zeta/ops/misc_act.py
--rw-r--r--   0        0        0     1671 2023-12-29 21:30:30.265822 zetascale-2.4.8/zeta/ops/mm_rearranges.py
--rw-r--r--   0        0        0      996 2024-02-20 02:21:29.289328 zetascale-2.4.8/zeta/ops/mm_softmax.py
--rw-r--r--   0        0        0     1851 2024-03-12 17:08:05.371465 zetascale-2.4.8/zeta/ops/mos.py
--rw-r--r--   0        0        0      995 2023-10-13 18:22:25.535325 zetascale-2.4.8/zeta/ops/nonlinear.py
--rw-r--r--   0        0        0     5070 2024-03-12 17:08:05.555951 zetascale-2.4.8/zeta/ops/softmax.py
--rw-r--r--   0        0        0     1086 2024-03-12 17:08:05.438443 zetascale-2.4.8/zeta/ops/sparsemax.py
--rw-r--r--   0        0        0      453 2024-03-12 17:08:05.416222 zetascale-2.4.8/zeta/ops/unitwise_norm.py
--rw-r--r--   0        0        0      814 2024-02-20 02:21:29.633384 zetascale-2.4.8/zeta/optim/__init__.py
--rw-r--r--   0        0        0    41198 2024-03-12 17:08:07.066649 zetascale-2.4.8/zeta/optim/batched_optimizer.py
--rw-r--r--   0        0        0    10142 2024-03-12 17:08:05.816147 zetascale-2.4.8/zeta/optim/decoupled_lion.py
--rw-r--r--   0        0        0     6448 2024-04-04 01:08:55.007796 zetascale-2.4.8/zeta/optim/decoupled_optimizer.py
--rw-r--r--   0        0        0    12445 2024-03-12 17:08:05.927362 zetascale-2.4.8/zeta/optim/decoupled_sophia.py
--rw-r--r--   0        0        0     4709 2024-03-12 17:08:05.712989 zetascale-2.4.8/zeta/optim/gradient_ascent.py
--rw-r--r--   0        0        0     2752 2024-02-20 02:21:30.662791 zetascale-2.4.8/zeta/optim/gradient_equillibrum.py
--rw-r--r--   0        0        0    19017 2024-03-12 17:08:06.610046 zetascale-2.4.8/zeta/optim/lion8b.py
--rw-r--r--   0        0        0     3387 2024-03-12 17:20:04.940463 zetascale-2.4.8/zeta/optim/parallel_gradient_descent.py
--rw-r--r--   0        0        0     4536 2024-03-15 15:09:05.079449 zetascale-2.4.8/zeta/optim/stable_adam.py
--rw-r--r--   0        0        0      453 2024-02-20 02:21:30.894505 zetascale-2.4.8/zeta/quant/__init__.py
--rw-r--r--   0        0        0      405 2023-12-27 18:55:30.757913 zetascale-2.4.8/zeta/quant/absmax.py
--rw-r--r--   0        0        0     2098 2024-02-20 02:21:31.386209 zetascale-2.4.8/zeta/quant/bitlinear.py
--rw-r--r--   0        0        0     1947 2024-03-12 17:08:05.865471 zetascale-2.4.8/zeta/quant/half_bit_linear.py
--rw-r--r--   0        0        0    10942 2024-03-12 17:08:06.282121 zetascale-2.4.8/zeta/quant/lfq.py
--rw-r--r--   0        0        0     3126 2024-02-10 02:19:51.497983 zetascale-2.4.8/zeta/quant/niva.py
--rw-r--r--   0        0        0    25173 2024-03-12 17:08:07.085198 zetascale-2.4.8/zeta/quant/qlora.py
--rw-r--r--   0        0        0     6010 2024-03-12 17:08:06.587037 zetascale-2.4.8/zeta/quant/qmoe.py
--rw-r--r--   0        0        0     3785 2024-03-12 17:08:06.081447 zetascale-2.4.8/zeta/quant/quick.py
--rw-r--r--   0        0        0        0 2024-01-03 03:30:55.516534 zetascale-2.4.8/zeta/quant/random_proj_quan.py
--rw-r--r--   0        0        0     1602 2024-03-12 17:08:05.991815 zetascale-2.4.8/zeta/quant/residual_vq.py
--rw-r--r--   0        0        0     1547 2023-10-19 20:04:49.349438 zetascale-2.4.8/zeta/quant/ste.py
--rw-r--r--   0        0        0      522 2024-02-20 03:07:52.541603 zetascale-2.4.8/zeta/rl/__init__.py
--rw-r--r--   0        0        0     4286 2024-03-12 17:08:06.190420 zetascale-2.4.8/zeta/rl/actor_critic.py
--rw-r--r--   0        0        0     2509 2024-02-20 02:21:33.772653 zetascale-2.4.8/zeta/rl/dpo.py
--rw-r--r--   0        0        0     3381 2024-02-20 02:21:33.739053 zetascale-2.4.8/zeta/rl/hindsight_replay.py
--rw-r--r--   0        0        0     2033 2023-11-10 22:26:53.747770 zetascale-2.4.8/zeta/rl/language_reward.py
--rw-r--r--   0        0        0     4130 2024-03-12 17:08:06.213360 zetascale-2.4.8/zeta/rl/ppo.py
--rw-r--r--   0        0        0     4513 2024-03-12 17:08:06.473169 zetascale-2.4.8/zeta/rl/priortized_replay_buffer.py
--rw-r--r--   0        0        0     5765 2024-03-12 17:08:06.471789 zetascale-2.4.8/zeta/rl/priortized_rps.py
--rw-r--r--   0        0        0      128 2023-10-07 01:59:52.333319 zetascale-2.4.8/zeta/rl/rest.py
--rw-r--r--   0        0        0     4585 2024-02-10 02:19:59.618788 zetascale-2.4.8/zeta/rl/reward_model.py
--rw-r--r--   0        0        0     2987 2024-03-12 17:08:06.505750 zetascale-2.4.8/zeta/rl/sumtree.py
--rw-r--r--   0        0        0     3185 2024-03-12 17:08:06.615506 zetascale-2.4.8/zeta/rl/vision_model_rl.py
--rw-r--r--   0        0        0     1227 2024-04-06 16:37:52.391264 zetascale-2.4.8/zeta/structs/__init__.py
--rw-r--r--   0        0        0    11731 2024-04-06 16:41:06.901661 zetascale-2.4.8/zeta/structs/auto_regressive_wrapper.py
--rw-r--r--   0        0        0     3505 2024-03-12 17:08:06.675632 zetascale-2.4.8/zeta/structs/clip_encoder.py
--rw-r--r--   0        0        0     6600 2024-02-20 02:21:38.475830 zetascale-2.4.8/zeta/structs/efficient_net.py
--rw-r--r--   0        0        0     3219 2024-03-12 17:08:06.579407 zetascale-2.4.8/zeta/structs/encoder_decoder.py
--rw-r--r--   0        0        0    28639 2024-03-12 17:08:07.715978 zetascale-2.4.8/zeta/structs/hierarchical_transformer.py
--rw-r--r--   0        0        0     5946 2024-03-12 17:08:06.771710 zetascale-2.4.8/zeta/structs/local_transformer.py
--rw-r--r--   0        0        0     1665 2024-02-20 02:21:37.803384 zetascale-2.4.8/zeta/structs/multi_modal_projector.py
--rw-r--r--   0        0        0    10839 2024-04-06 16:41:06.901610 zetascale-2.4.8/zeta/structs/simple_transformer.py
--rw-r--r--   0        0        0     2468 2024-03-12 17:08:06.698283 zetascale-2.4.8/zeta/structs/simple_vision_encoder.py
--rw-r--r--   0        0        0    68945 2024-03-12 17:08:08.927611 zetascale-2.4.8/zeta/structs/transformer.py
--rw-r--r--   0        0        0     4490 2024-03-12 17:08:06.878786 zetascale-2.4.8/zeta/structs/transformer_block.py
--rw-r--r--   0        0        0      485 2024-04-04 01:10:13.946249 zetascale-2.4.8/zeta/tokenizers/__init__.py
--rw-r--r--   0        0        0     1438 2023-12-23 05:13:40.934254 zetascale-2.4.8/zeta/tokenizers/gptx_tokenizer.py
--rw-r--r--   0        0        0     3079 2024-03-12 17:08:06.850076 zetascale-2.4.8/zeta/tokenizers/llama_sentencepiece.py
--rw-r--r--   0        0        0     3651 2024-03-12 17:08:06.970562 zetascale-2.4.8/zeta/tokenizers/multi_modal_tokenizer.py
--rw-r--r--   0        0        0     3720 2024-03-12 17:08:06.997545 zetascale-2.4.8/zeta/tokenizers/sentence_piece.py
--rw-r--r--   0        0        0     9771 2023-12-19 19:26:43.476444 zetascale-2.4.8/zeta/tokenizers/tokenmonster.py
--rw-r--r--   0        0        0      460 2024-02-20 02:21:39.816336 zetascale-2.4.8/zeta/training/__init__.py
--rw-r--r--   0        0        0     5400 2024-02-20 02:21:40.381513 zetascale-2.4.8/zeta/training/activation_checkpoint.py
--rw-r--r--   0        0        0     2576 2024-03-12 17:08:07.002747 zetascale-2.4.8/zeta/training/dataloader.py
--rw-r--r--   0        0        0     3496 2024-03-12 17:08:07.184296 zetascale-2.4.8/zeta/training/fsdp.py
--rw-r--r--   0        0        0     3186 2024-03-16 00:52:50.202568 zetascale-2.4.8/zeta/training/galore.py
--rw-r--r--   0        0        0     6054 2024-03-12 17:08:07.228332 zetascale-2.4.8/zeta/training/hive_trainer.py
--rw-r--r--   0        0        0     1626 2023-10-23 03:27:31.592537 zetascale-2.4.8/zeta/training/parallel_wrapper.py
--rw-r--r--   0        0        0     2059 2024-03-12 17:08:07.154710 zetascale-2.4.8/zeta/training/scheduler.py
--rw-r--r--   0        0        0     9273 2024-03-12 17:08:07.389221 zetascale-2.4.8/zeta/training/train.py
--rw-r--r--   0        0        0     2347 2024-03-20 20:38:15.450877 zetascale-2.4.8/zeta/utils/__init__.py
--rw-r--r--   0        0        0     3464 2024-03-12 17:08:07.301138 zetascale-2.4.8/zeta/utils/benchmark.py
--rw-r--r--   0        0        0     1347 2024-03-12 17:08:07.197874 zetascale-2.4.8/zeta/utils/cuda_memory_wrapper.py
--rw-r--r--   0        0        0     6424 2024-03-12 17:08:07.321106 zetascale-2.4.8/zeta/utils/cuda_wrapper.py
--rw-r--r--   0        0        0     1337 2024-03-19 17:10:27.077564 zetascale-2.4.8/zeta/utils/disable_logging.py
--rw-r--r--   0        0        0     1184 2024-03-12 17:08:07.232349 zetascale-2.4.8/zeta/utils/enforce_types.py
--rw-r--r--   0        0        0     1110 2024-03-20 21:10:20.934445 zetascale-2.4.8/zeta/utils/img_to_tensor.py
--rw-r--r--   0        0        0     2953 2024-03-12 17:08:07.318804 zetascale-2.4.8/zeta/utils/log_pytorch_op.py
--rw-r--r--   0        0        0    19874 2024-03-12 17:08:07.939241 zetascale-2.4.8/zeta/utils/main.py
--rw-r--r--   0        0        0     1798 2024-03-12 17:08:07.328852 zetascale-2.4.8/zeta/utils/module_device.py
--rw-r--r--   0        0        0      703 2023-12-17 00:28:55.289752 zetascale-2.4.8/zeta/utils/params.py
--rw-r--r--   0        0        0     3966 2024-02-20 02:21:42.476410 zetascale-2.4.8/zeta/utils/save_load_wrapper.py
--rw-r--r--   0        0        0      846 2024-03-20 21:10:20.904725 zetascale-2.4.8/zeta/utils/text_to_tensor.py
--rw-r--r--   0        0        0      751 2024-02-20 02:21:41.805576 zetascale-2.4.8/zeta/utils/verbose_execution.py
--rw-r--r--   0        0        0    25931 2024-03-12 17:08:07.919574 zetascale-2.4.8/zeta/utils/vision_utils.py
--rw-r--r--   0        0        0    22392 1970-01-01 00:00:00.000000 zetascale-2.4.8/setup.py
--rw-r--r--   0        0        0    21440 1970-01-01 00:00:00.000000 zetascale-2.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11342 2024-05-21 00:22:21.733285 zetascale-2.5.1/LICENSE
+-rw-r--r--   0        0        0    20231 2024-05-21 00:22:21.733369 zetascale-2.5.1/README.md
+-rw-r--r--   0        0        0     1333 2024-05-25 22:02:47.085235 zetascale-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0      589 2024-05-21 00:22:21.765974 zetascale-2.5.1/zeta/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766028 zetascale-2.5.1/zeta/cli/__init__.py
+-rw-r--r--   0        0        0     1937 2024-05-21 00:22:21.766088 zetascale-2.5.1/zeta/cli/main.py
+-rw-r--r--   0        0        0      157 2024-05-21 00:22:21.766172 zetascale-2.5.1/zeta/cloud/__init__.py
+-rw-r--r--   0        0        0     2071 2024-05-21 00:22:21.766216 zetascale-2.5.1/zeta/cloud/main.py
+-rw-r--r--   0        0        0     6068 2024-05-21 00:22:21.766270 zetascale-2.5.1/zeta/cloud/sky_api.py
+-rw-r--r--   0        0        0       59 2024-05-21 00:22:21.766338 zetascale-2.5.1/zeta/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766382 zetascale-2.5.1/zeta/experimental/triton/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-21 00:22:21.766461 zetascale-2.5.1/zeta/experimental/triton/activations/__init__.py
+-rw-r--r--   0        0        0     2600 2024-05-21 00:22:21.766506 zetascale-2.5.1/zeta/experimental/triton/activations/activations.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766525 zetascale-2.5.1/zeta/experimental/triton/activations/flash_mlp.py
+-rw-r--r--   0        0        0     9532 2024-05-21 00:22:21.766605 zetascale-2.5.1/zeta/experimental/triton/activations/functions.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766648 zetascale-2.5.1/zeta/experimental/triton/triton_modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766675 zetascale-2.5.1/zeta/experimental/triton/triton_modules/flash_mlp.py
+-rw-r--r--   0        0        0     2806 2024-05-21 00:22:21.766729 zetascale-2.5.1/zeta/experimental/triton/triton_modules/linear_proj.py
+-rw-r--r--   0        0        0     3311 2024-05-21 00:22:21.766804 zetascale-2.5.1/zeta/models/BEiT3.py
+-rw-r--r--   0        0        0     1809 2024-05-21 00:22:21.766856 zetascale-2.5.1/zeta/models/LongNet.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766873 zetascale-2.5.1/zeta/models/Magneto.py
+-rw-r--r--   0        0        0      603 2024-05-21 00:22:21.766925 zetascale-2.5.1/zeta/models/__init__.py
+-rw-r--r--   0        0        0     3308 2024-05-21 00:22:21.766969 zetascale-2.5.1/zeta/models/andromeda.py
+-rw-r--r--   0        0        0      135 2024-05-21 00:22:21.767013 zetascale-2.5.1/zeta/models/base.py
+-rw-r--r--   0        0        0     6752 2024-05-21 00:22:21.767073 zetascale-2.5.1/zeta/models/gpt4.py
+-rw-r--r--   0        0        0     4288 2024-05-21 00:22:21.767120 zetascale-2.5.1/zeta/models/kosmos.py
+-rw-r--r--   0        0        0      949 2024-05-21 00:22:21.767166 zetascale-2.5.1/zeta/models/llama.py
+-rw-r--r--   0        0        0     3639 2024-05-21 00:22:21.767223 zetascale-2.5.1/zeta/models/max_vit.py
+-rw-r--r--   0        0        0     6678 2024-05-21 00:22:21.767283 zetascale-2.5.1/zeta/models/mega_vit.py
+-rw-r--r--   0        0        0     6927 2024-05-21 00:22:21.767340 zetascale-2.5.1/zeta/models/mm_mamba.py
+-rw-r--r--   0        0        0    12991 2024-05-21 00:22:21.767416 zetascale-2.5.1/zeta/models/navit.py
+-rw-r--r--   0        0        0     1884 2024-05-21 00:22:21.767454 zetascale-2.5.1/zeta/models/palme.py
+-rw-r--r--   0        0        0     2762 2024-05-21 00:22:21.767499 zetascale-2.5.1/zeta/models/vit.py
+-rw-r--r--   0        0        0      219 2024-05-21 00:22:21.767567 zetascale-2.5.1/zeta/nn/__init__.py
+-rw-r--r--   0        0        0     1895 2024-05-21 00:22:21.767637 zetascale-2.5.1/zeta/nn/attention/__init__.py
+-rw-r--r--   0        0        0     4184 2024-05-21 00:22:21.767693 zetascale-2.5.1/zeta/nn/attention/agent_attn.py
+-rw-r--r--   0        0        0    14876 2024-05-21 00:22:21.767772 zetascale-2.5.1/zeta/nn/attention/attend.py
+-rw-r--r--   0        0        0      244 2024-05-21 00:22:21.767819 zetascale-2.5.1/zeta/nn/attention/base.py
+-rw-r--r--   0        0        0     4050 2024-05-21 00:22:21.767875 zetascale-2.5.1/zeta/nn/attention/cross_attention.py
+-rw-r--r--   0        0        0     3236 2024-05-21 00:22:21.767922 zetascale-2.5.1/zeta/nn/attention/cross_attn_images.py
+-rw-r--r--   0        0        0    10734 2024-05-21 00:22:21.767991 zetascale-2.5.1/zeta/nn/attention/dilated_attention.py
+-rw-r--r--   0        0        0     8803 2024-05-21 00:22:21.768136 zetascale-2.5.1/zeta/nn/attention/flash_attention.py
+-rw-r--r--   0        0        0     2161 2024-05-21 00:22:21.768183 zetascale-2.5.1/zeta/nn/attention/linear_attention.py
+-rw-r--r--   0        0        0     2370 2024-05-21 00:22:21.768231 zetascale-2.5.1/zeta/nn/attention/linear_attn_l.py
+-rw-r--r--   0        0        0     2090 2024-05-21 00:37:46.889652 zetascale-2.5.1/zeta/nn/attention/linearized_attention.py
+-rw-r--r--   0        0        0     9794 2024-05-21 00:22:21.768347 zetascale-2.5.1/zeta/nn/attention/local_attention.py
+-rw-r--r--   0        0        0     1966 2024-05-21 00:22:21.768392 zetascale-2.5.1/zeta/nn/attention/local_attention_mha.py
+-rw-r--r--   0        0        0    18990 2024-05-21 00:22:21.768470 zetascale-2.5.1/zeta/nn/attention/mixture_attention.py
+-rw-r--r--   0        0        0    12414 2024-05-21 00:22:21.768567 zetascale-2.5.1/zeta/nn/attention/multi_grouped_attn.py
+-rw-r--r--   0        0        0     2729 2024-05-21 00:22:21.768617 zetascale-2.5.1/zeta/nn/attention/multi_modal_causal_attention.py
+-rw-r--r--   0        0        0     3879 2024-05-21 00:22:21.768670 zetascale-2.5.1/zeta/nn/attention/multi_modal_cross_attn.py
+-rw-r--r--   0        0        0     5769 2024-05-21 00:22:21.768725 zetascale-2.5.1/zeta/nn/attention/multihead_attention.py
+-rw-r--r--   0        0        0    25310 2024-05-21 00:37:47.151935 zetascale-2.5.1/zeta/nn/attention/multiquery_attention.py
+-rw-r--r--   0        0        0     3979 2024-05-21 00:22:21.768851 zetascale-2.5.1/zeta/nn/attention/scalable_img_self_attn.py
+-rw-r--r--   0        0        0     2198 2024-05-21 00:22:21.768897 zetascale-2.5.1/zeta/nn/attention/shaped_attention.py
+-rw-r--r--   0        0        0     4672 2024-05-21 00:22:21.768952 zetascale-2.5.1/zeta/nn/attention/sparse_attention.py
+-rw-r--r--   0        0        0     1741 2024-05-21 00:22:21.768998 zetascale-2.5.1/zeta/nn/attention/spatial_linear_attention.py
+-rw-r--r--   0        0        0     2973 2024-05-21 00:22:21.769048 zetascale-2.5.1/zeta/nn/attention/xc_attention.py
+-rw-r--r--   0        0        0      482 2024-05-21 00:22:21.769118 zetascale-2.5.1/zeta/nn/biases/__init__.py
+-rw-r--r--   0        0        0     3951 2024-05-21 00:22:21.769171 zetascale-2.5.1/zeta/nn/biases/alibi.py
+-rw-r--r--   0        0        0      245 2024-05-21 00:22:21.769209 zetascale-2.5.1/zeta/nn/biases/base.py
+-rw-r--r--   0        0        0     1348 2024-05-21 00:22:21.769251 zetascale-2.5.1/zeta/nn/biases/dynamic_position_bias.py
+-rw-r--r--   0        0        0     2886 2024-05-21 00:22:21.769300 zetascale-2.5.1/zeta/nn/biases/relative_position_bias.py
+-rw-r--r--   0        0        0     2069 2024-05-21 00:22:21.769370 zetascale-2.5.1/zeta/nn/embeddings/__init__.py
+-rw-r--r--   0        0        0     1231 2024-05-21 00:22:21.769427 zetascale-2.5.1/zeta/nn/embeddings/abc_pos_emb.py
+-rw-r--r--   0        0        0      255 2024-05-21 00:22:21.769468 zetascale-2.5.1/zeta/nn/embeddings/base.py
+-rw-r--r--   0        0        0      723 2024-05-21 00:22:21.769514 zetascale-2.5.1/zeta/nn/embeddings/embedding.py
+-rw-r--r--   0        0        0     2509 2024-05-21 00:22:21.769562 zetascale-2.5.1/zeta/nn/embeddings/multiway_network.py
+-rw-r--r--   0        0        0      358 2024-05-21 00:22:21.769604 zetascale-2.5.1/zeta/nn/embeddings/nominal_embeddings.py
+-rw-r--r--   0        0        0      900 2024-05-21 00:22:21.769647 zetascale-2.5.1/zeta/nn/embeddings/patch_embedding.py
+-rw-r--r--   0        0        0     3120 2024-05-21 00:22:21.769692 zetascale-2.5.1/zeta/nn/embeddings/pi.md
+-rw-r--r--   0        0        0     1996 2024-05-21 00:22:21.769737 zetascale-2.5.1/zeta/nn/embeddings/positional.py
+-rw-r--r--   0        0        0     2584 2024-05-21 00:22:21.769792 zetascale-2.5.1/zeta/nn/embeddings/positional_interpolation.py
+-rw-r--r--   0        0        0     3021 2024-05-21 00:22:21.769839 zetascale-2.5.1/zeta/nn/embeddings/qfsp_embeddings.py
+-rw-r--r--   0        0        0     1668 2024-05-21 00:22:21.769891 zetascale-2.5.1/zeta/nn/embeddings/qft_embeddings.py
+-rw-r--r--   0        0        0     2250 2024-05-21 00:22:21.769967 zetascale-2.5.1/zeta/nn/embeddings/rope.py
+-rw-r--r--   0        0        0     1570 2024-05-21 00:22:21.770017 zetascale-2.5.1/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py
+-rw-r--r--   0        0        0     2345 2024-05-21 00:22:21.770062 zetascale-2.5.1/zeta/nn/embeddings/sine_positional.py
+-rw-r--r--   0        0        0     2650 2024-05-21 00:22:21.770108 zetascale-2.5.1/zeta/nn/embeddings/sinusoidal.py
+-rw-r--r--   0        0        0     1810 2024-05-21 00:22:21.770156 zetascale-2.5.1/zeta/nn/embeddings/truncated_rope.py
+-rw-r--r--   0        0        0     1003 2024-05-21 00:22:21.770199 zetascale-2.5.1/zeta/nn/embeddings/vis_lang_emb.py
+-rw-r--r--   0        0        0     3195 2024-05-21 00:22:21.770249 zetascale-2.5.1/zeta/nn/embeddings/vision_emb.py
+-rw-r--r--   0        0        0     3208 2024-05-21 00:22:21.770299 zetascale-2.5.1/zeta/nn/embeddings/xpos_relative_position.py
+-rw-r--r--   0        0        0     6685 2024-05-21 00:22:21.770353 zetascale-2.5.1/zeta/nn/embeddings/yarn.py
+-rw-r--r--   0        0        0     1150 2024-05-21 00:22:21.770425 zetascale-2.5.1/zeta/nn/masks/__init__.py
+-rw-r--r--   0        0        0    31987 2024-05-21 00:22:21.770499 zetascale-2.5.1/zeta/nn/masks/attn_masks.py
+-rw-r--r--   0        0        0     1248 2024-05-21 00:22:21.770558 zetascale-2.5.1/zeta/nn/masks/block_diagonal.py
+-rw-r--r--   0        0        0    15253 2024-05-21 00:22:21.770674 zetascale-2.5.1/zeta/nn/modules/README.md
+-rw-r--r--   0        0        0    14062 2024-05-25 22:02:37.978001 zetascale-2.5.1/zeta/nn/modules/__init__.py
+-rw-r--r--   0        0        0     7658 2024-05-21 00:22:21.770820 zetascale-2.5.1/zeta/nn/modules/_activations.py
+-rw-r--r--   0        0        0     3561 2024-05-21 00:22:21.770869 zetascale-2.5.1/zeta/nn/modules/adaptive_conv.py
+-rw-r--r--   0        0        0     1572 2024-05-21 00:22:21.770917 zetascale-2.5.1/zeta/nn/modules/adaptive_layernorm.py
+-rw-r--r--   0        0        0     1506 2024-05-21 00:22:21.770965 zetascale-2.5.1/zeta/nn/modules/adaptive_parameter_list.py
+-rw-r--r--   0        0        0     2181 2024-05-21 00:22:21.771010 zetascale-2.5.1/zeta/nn/modules/adaptive_rmsnorm.py
+-rw-r--r--   0        0        0      465 2024-05-21 00:22:21.771057 zetascale-2.5.1/zeta/nn/modules/add_norm.py
+-rw-r--r--   0        0        0     1969 2024-05-21 00:22:21.771101 zetascale-2.5.1/zeta/nn/modules/alr_block.py
+-rw-r--r--   0        0        0     1885 2024-05-21 00:22:21.771145 zetascale-2.5.1/zeta/nn/modules/attn.py
+-rw-r--r--   0        0        0     1170 2024-05-21 00:22:21.771188 zetascale-2.5.1/zeta/nn/modules/audio_to_text.py
+-rw-r--r--   0        0        0     2927 2024-05-21 00:22:21.771233 zetascale-2.5.1/zeta/nn/modules/avg_model_merger.py
+-rw-r--r--   0        0        0      200 2024-05-21 00:22:21.771283 zetascale-2.5.1/zeta/nn/modules/batched_dp.py
+-rw-r--r--   0        0        0     2355 2024-05-21 00:22:21.771334 zetascale-2.5.1/zeta/nn/modules/block_butterfly_mlp.py
+-rw-r--r--   0        0        0    12691 2024-05-21 00:37:47.719254 zetascale-2.5.1/zeta/nn/modules/blockdiag_butterfly.py
+-rw-r--r--   0        0        0      986 2024-05-21 00:22:21.771470 zetascale-2.5.1/zeta/nn/modules/chan_layer_norm.py
+-rw-r--r--   0        0        0     7693 2024-05-21 00:22:21.771536 zetascale-2.5.1/zeta/nn/modules/clex.py
+-rw-r--r--   0        0        0     2522 2024-05-21 00:22:21.771589 zetascale-2.5.1/zeta/nn/modules/clip_bottleneck.py
+-rw-r--r--   0        0        0     1530 2024-05-21 00:22:21.771639 zetascale-2.5.1/zeta/nn/modules/cnn_text.py
+-rw-r--r--   0        0        0     4281 2024-05-21 00:22:21.771705 zetascale-2.5.1/zeta/nn/modules/combined_linear.py
+-rw-r--r--   0        0        0     1026 2024-05-21 00:22:21.771761 zetascale-2.5.1/zeta/nn/modules/conv_bn_relu.py
+-rw-r--r--   0        0        0     2422 2024-05-21 00:37:46.940310 zetascale-2.5.1/zeta/nn/modules/conv_mlp.py
+-rw-r--r--   0        0        0      888 2024-05-21 00:22:21.771867 zetascale-2.5.1/zeta/nn/modules/convnet.py
+-rw-r--r--   0        0        0     1723 2024-05-21 00:22:21.771923 zetascale-2.5.1/zeta/nn/modules/cross_embed_layer.py
+-rw-r--r--   0        0        0     7316 2024-05-21 00:22:21.771989 zetascale-2.5.1/zeta/nn/modules/cross_modal_reparametization.py
+-rw-r--r--   0        0        0     3540 2024-05-21 00:22:21.772043 zetascale-2.5.1/zeta/nn/modules/decision_tree.py
+-rw-r--r--   0        0        0     2648 2024-05-21 00:22:21.772100 zetascale-2.5.1/zeta/nn/modules/deepseek_moe.py
+-rw-r--r--   0        0        0      794 2024-05-21 00:22:21.772158 zetascale-2.5.1/zeta/nn/modules/dense_connect.py
+-rw-r--r--   0        0        0     2371 2024-05-21 00:22:21.772210 zetascale-2.5.1/zeta/nn/modules/diffusion.py
+-rw-r--r--   0        0        0     1538 2024-05-21 00:22:21.772263 zetascale-2.5.1/zeta/nn/modules/droppath.py
+-rw-r--r--   0        0        0      796 2024-05-21 00:22:21.772319 zetascale-2.5.1/zeta/nn/modules/dual_path_block.py
+-rw-r--r--   0        0        0     4687 2024-05-21 00:22:21.772383 zetascale-2.5.1/zeta/nn/modules/dyna_conv.py
+-rw-r--r--   0        0        0     2064 2024-05-21 00:22:21.772435 zetascale-2.5.1/zeta/nn/modules/dynamic_module.py
+-rw-r--r--   0        0        0      980 2024-05-21 00:22:21.772485 zetascale-2.5.1/zeta/nn/modules/dynamic_routing_block.py
+-rw-r--r--   0        0        0      786 2024-05-21 00:22:21.772538 zetascale-2.5.1/zeta/nn/modules/embedding_to_grid.py
+-rw-r--r--   0        0        0    11202 2024-05-21 00:22:21.772616 zetascale-2.5.1/zeta/nn/modules/ether.py
+-rw-r--r--   0        0        0     5338 2024-05-21 00:22:21.772683 zetascale-2.5.1/zeta/nn/modules/exo.py
+-rw-r--r--   0        0        0       92 2024-05-21 00:22:21.772729 zetascale-2.5.1/zeta/nn/modules/expand.py
+-rw-r--r--   0        0        0      888 2024-05-21 00:22:21.772777 zetascale-2.5.1/zeta/nn/modules/expand_channels.py
+-rw-r--r--   0        0        0     1184 2024-05-21 00:22:21.772828 zetascale-2.5.1/zeta/nn/modules/expert.py
+-rw-r--r--   0        0        0      678 2024-05-21 00:22:21.772881 zetascale-2.5.1/zeta/nn/modules/fast_text.py
+-rw-r--r--   0        0        0     1004 2024-05-21 00:22:21.772931 zetascale-2.5.1/zeta/nn/modules/feedback_block.py
+-rw-r--r--   0        0        0     4666 2024-05-21 00:22:21.772994 zetascale-2.5.1/zeta/nn/modules/feedforward.py
+-rw-r--r--   0        0        0     4396 2024-05-21 00:22:21.773060 zetascale-2.5.1/zeta/nn/modules/feedforward_network.py
+-rw-r--r--   0        0        0     3153 2024-05-21 00:22:21.773107 zetascale-2.5.1/zeta/nn/modules/film.py
+-rw-r--r--   0        0        0     2607 2024-05-21 00:22:21.773167 zetascale-2.5.1/zeta/nn/modules/film_conditioning.py
+-rw-r--r--   0        0        0     2657 2024-05-21 00:22:21.773220 zetascale-2.5.1/zeta/nn/modules/film_efficient_metb3.py
+-rw-r--r--   0        0        0      363 2024-05-21 00:22:21.773275 zetascale-2.5.1/zeta/nn/modules/flash_conv.py
+-rw-r--r--   0        0        0      817 2024-05-21 00:22:21.773327 zetascale-2.5.1/zeta/nn/modules/flatten_features.py
+-rw-r--r--   0        0        0     3528 2024-05-21 00:22:21.773378 zetascale-2.5.1/zeta/nn/modules/flex_conv.py
+-rw-r--r--   0        0        0     2694 2024-05-21 00:22:21.773439 zetascale-2.5.1/zeta/nn/modules/flexible_mlp.py
+-rw-r--r--   0        0        0      845 2024-05-21 00:22:21.773492 zetascale-2.5.1/zeta/nn/modules/fractoral_norm.py
+-rw-r--r--   0        0        0     2552 2024-05-21 00:22:21.773545 zetascale-2.5.1/zeta/nn/modules/fractorial_net.py
+-rw-r--r--   0        0        0      769 2024-05-21 00:22:21.773599 zetascale-2.5.1/zeta/nn/modules/freeze_layers.py
+-rw-r--r--   0        0        0     2408 2024-05-21 00:22:21.773650 zetascale-2.5.1/zeta/nn/modules/fused_dropout_add.py
+-rw-r--r--   0        0        0     1223 2024-05-21 00:22:21.773701 zetascale-2.5.1/zeta/nn/modules/fused_dropout_layernom.py
+-rw-r--r--   0        0        0     2268 2024-05-21 00:22:21.773755 zetascale-2.5.1/zeta/nn/modules/fused_gelu_dense.py
+-rw-r--r--   0        0        0     1006 2024-05-21 00:22:21.773804 zetascale-2.5.1/zeta/nn/modules/fusion_ffn.py
+-rw-r--r--   0        0        0    33392 2024-05-21 00:22:21.773904 zetascale-2.5.1/zeta/nn/modules/g_shard_moe.py
+-rw-r--r--   0        0        0     1800 2024-05-25 18:14:50.721305 zetascale-2.5.1/zeta/nn/modules/gated_cnn_block.py
+-rw-r--r--   0        0        0      707 2024-05-21 00:22:21.773969 zetascale-2.5.1/zeta/nn/modules/gated_residual_block.py
+-rw-r--r--   0        0        0     4104 2024-05-21 00:22:21.774037 zetascale-2.5.1/zeta/nn/modules/gill_mapper.py
+-rw-r--r--   0        0        0      920 2024-05-21 00:22:21.774094 zetascale-2.5.1/zeta/nn/modules/glu.py
+-rw-r--r--   0        0        0     1826 2024-05-21 00:22:21.774153 zetascale-2.5.1/zeta/nn/modules/gru_gating.py
+-rw-r--r--   0        0        0     2634 2024-05-21 00:22:21.774210 zetascale-2.5.1/zeta/nn/modules/h3.py
+-rw-r--r--   0        0        0     2078 2024-05-21 00:22:21.774272 zetascale-2.5.1/zeta/nn/modules/hebbian.py
+-rw-r--r--   0        0        0      809 2024-05-21 00:22:21.774328 zetascale-2.5.1/zeta/nn/modules/highway_layer.py
+-rw-r--r--   0        0        0     3527 2024-05-21 00:22:21.774388 zetascale-2.5.1/zeta/nn/modules/image_projector.py
+-rw-r--r--   0        0        0     1049 2024-05-21 00:22:21.774442 zetascale-2.5.1/zeta/nn/modules/image_to_text.py
+-rw-r--r--   0        0        0     1385 2024-05-21 00:22:21.774487 zetascale-2.5.1/zeta/nn/modules/img_or_video_to_time.py
+-rw-r--r--   0        0        0     1197 2024-05-21 00:22:21.774532 zetascale-2.5.1/zeta/nn/modules/img_patch_embed.py
+-rw-r--r--   0        0        0      763 2024-05-21 00:22:21.774576 zetascale-2.5.1/zeta/nn/modules/img_reshape.py
+-rw-r--r--   0        0        0     4024 2024-05-21 00:22:21.774623 zetascale-2.5.1/zeta/nn/modules/itca.py
+-rw-r--r--   0        0        0    12420 2024-05-21 00:22:21.774693 zetascale-2.5.1/zeta/nn/modules/kan.py
+-rw-r--r--   0        0        0     4656 2024-05-21 00:22:21.774746 zetascale-2.5.1/zeta/nn/modules/kv_cache.py
+-rw-r--r--   0        0        0     2586 2024-05-21 00:22:21.774792 zetascale-2.5.1/zeta/nn/modules/kv_cache_update.py
+-rw-r--r--   0        0        0     6221 2024-05-21 00:22:21.774846 zetascale-2.5.1/zeta/nn/modules/lambda_mask.py
+-rw-r--r--   0        0        0     3504 2024-05-21 00:22:21.774895 zetascale-2.5.1/zeta/nn/modules/lang_conv_module.py
+-rw-r--r--   0        0        0     2760 2024-05-21 00:22:21.774942 zetascale-2.5.1/zeta/nn/modules/laser.py
+-rw-r--r--   0        0        0      919 2024-05-21 00:22:21.774987 zetascale-2.5.1/zeta/nn/modules/layer_scale.py
+-rw-r--r--   0        0        0     2379 2024-05-21 00:22:21.775034 zetascale-2.5.1/zeta/nn/modules/layernorm.py
+-rw-r--r--   0        0        0     1132 2024-05-21 00:22:21.775081 zetascale-2.5.1/zeta/nn/modules/leaky_relu.py
+-rw-r--r--   0        0        0    24514 2024-05-21 00:22:21.775141 zetascale-2.5.1/zeta/nn/modules/log_ff.py
+-rw-r--r--   0        0        0     1747 2024-05-21 00:22:21.775199 zetascale-2.5.1/zeta/nn/modules/lora.py
+-rw-r--r--   0        0        0     3240 2024-05-21 00:22:21.775247 zetascale-2.5.1/zeta/nn/modules/matrix.py
+-rw-r--r--   0        0        0     2993 2024-05-21 00:22:21.775291 zetascale-2.5.1/zeta/nn/modules/mbconv.py
+-rw-r--r--   0        0        0     3127 2024-05-21 00:22:21.775334 zetascale-2.5.1/zeta/nn/modules/mixtape.py
+-rw-r--r--   0        0        0     2125 2024-05-21 00:22:21.775378 zetascale-2.5.1/zeta/nn/modules/mixtral_expert.py
+-rw-r--r--   0        0        0     1884 2024-05-21 00:22:21.775424 zetascale-2.5.1/zeta/nn/modules/mlp.py
+-rw-r--r--   0        0        0     3729 2024-05-21 00:22:21.775471 zetascale-2.5.1/zeta/nn/modules/mlp_mixer.py
+-rw-r--r--   0        0        0     2435 2024-05-21 00:22:21.775520 zetascale-2.5.1/zeta/nn/modules/mm_adapter.py
+-rw-r--r--   0        0        0       87 2024-05-21 00:22:21.775561 zetascale-2.5.1/zeta/nn/modules/mm_fusion.py
+-rw-r--r--   0        0        0     2340 2024-05-21 00:22:21.775609 zetascale-2.5.1/zeta/nn/modules/mm_layernorm.py
+-rw-r--r--   0        0        0     1405 2024-05-21 00:22:21.775649 zetascale-2.5.1/zeta/nn/modules/mm_ops.py
+-rw-r--r--   0        0        0     6234 2024-05-21 00:22:21.775711 zetascale-2.5.1/zeta/nn/modules/modality_adaptive_module.py
+-rw-r--r--   0        0        0     2930 2024-05-21 00:22:21.775756 zetascale-2.5.1/zeta/nn/modules/moe.py
+-rw-r--r--   0        0        0     3228 2024-05-21 00:22:21.775806 zetascale-2.5.1/zeta/nn/modules/moe_router.py
+-rw-r--r--   0        0        0      776 2024-05-21 00:22:21.775853 zetascale-2.5.1/zeta/nn/modules/monarch_mlp.py
+-rw-r--r--   0        0        0     1564 2024-05-21 00:22:21.775900 zetascale-2.5.1/zeta/nn/modules/mr_adapter.py
+-rw-r--r--   0        0        0     6686 2024-05-21 00:22:21.775960 zetascale-2.5.1/zeta/nn/modules/multi_input_multi_output.py
+-rw-r--r--   0        0        0      837 2024-05-21 00:22:21.776004 zetascale-2.5.1/zeta/nn/modules/multi_scale_block.py
+-rw-r--r--   0        0        0        2 2024-05-21 00:22:21.776046 zetascale-2.5.1/zeta/nn/modules/multiclass_label.py
+-rw-r--r--   0        0        0      225 2024-05-21 00:22:21.776089 zetascale-2.5.1/zeta/nn/modules/multimodal_concat.py
+-rw-r--r--   0        0        0      472 2024-05-21 00:22:21.776130 zetascale-2.5.1/zeta/nn/modules/nearest_upsample.py
+-rw-r--r--   0        0        0     8309 2024-05-21 00:22:21.776199 zetascale-2.5.1/zeta/nn/modules/nebula.py
+-rw-r--r--   0        0        0     2590 2024-05-21 00:22:21.776249 zetascale-2.5.1/zeta/nn/modules/nfn_stem.py
+-rw-r--r--   0        0        0     1456 2024-05-21 00:22:21.776295 zetascale-2.5.1/zeta/nn/modules/norm_fractorals.py
+-rw-r--r--   0        0        0     2034 2024-05-21 00:22:21.776341 zetascale-2.5.1/zeta/nn/modules/norm_utils.py
+-rw-r--r--   0        0        0     2842 2024-05-21 00:22:21.776388 zetascale-2.5.1/zeta/nn/modules/omnimodal_fusion.py
+-rw-r--r--   0        0        0     3851 2024-05-21 00:22:21.776438 zetascale-2.5.1/zeta/nn/modules/p_scan.py
+-rw-r--r--   0        0        0     2571 2024-05-21 00:22:21.776486 zetascale-2.5.1/zeta/nn/modules/palo_ldp.py
+-rw-r--r--   0        0        0      601 2024-05-21 00:22:21.776528 zetascale-2.5.1/zeta/nn/modules/parallel_wrapper.py
+-rw-r--r--   0        0        0      200 2024-05-21 00:22:21.776570 zetascale-2.5.1/zeta/nn/modules/patch_img.py
+-rw-r--r--   0        0        0     6597 2024-05-21 00:22:21.776626 zetascale-2.5.1/zeta/nn/modules/patch_linear_flatten.py
+-rw-r--r--   0        0        0      985 2024-05-21 00:22:21.776673 zetascale-2.5.1/zeta/nn/modules/patch_video.py
+-rw-r--r--   0        0        0      783 2024-05-21 00:22:21.776716 zetascale-2.5.1/zeta/nn/modules/peg.py
+-rw-r--r--   0        0        0     3180 2024-05-21 00:22:21.776764 zetascale-2.5.1/zeta/nn/modules/perceiver_layer.py
+-rw-r--r--   0        0        0     6115 2024-05-21 00:22:21.776830 zetascale-2.5.1/zeta/nn/modules/perceiver_resampler.py
+-rw-r--r--   0        0        0     2594 2024-05-21 00:22:21.776877 zetascale-2.5.1/zeta/nn/modules/pixel_shuffling.py
+-rw-r--r--   0        0        0     1692 2024-05-21 00:22:21.776921 zetascale-2.5.1/zeta/nn/modules/poly_expert_fusion_network.py
+-rw-r--r--   0        0        0     2045 2024-05-21 00:22:21.776970 zetascale-2.5.1/zeta/nn/modules/polymorphic_activation.py
+-rw-r--r--   0        0        0     5804 2024-05-21 00:22:21.777026 zetascale-2.5.1/zeta/nn/modules/polymorphic_neuron.py
+-rw-r--r--   0        0        0      527 2024-05-21 00:22:21.777070 zetascale-2.5.1/zeta/nn/modules/prenorm.py
+-rw-r--r--   0        0        0     1299 2024-05-21 00:22:21.777113 zetascale-2.5.1/zeta/nn/modules/proj_then_softmax.py
+-rw-r--r--   0        0        0     7164 2024-05-21 00:22:21.777170 zetascale-2.5.1/zeta/nn/modules/pulsar.py
+-rw-r--r--   0        0        0     3451 2024-05-21 00:22:21.777217 zetascale-2.5.1/zeta/nn/modules/pyro.py
+-rw-r--r--   0        0        0     9454 2024-05-21 00:22:21.777284 zetascale-2.5.1/zeta/nn/modules/qformer.py
+-rw-r--r--   0        0        0      812 2024-05-21 00:22:21.777328 zetascale-2.5.1/zeta/nn/modules/qkv_norm.py
+-rw-r--r--   0        0        0     1381 2024-05-21 00:22:21.777374 zetascale-2.5.1/zeta/nn/modules/quantized_layernorm.py
+-rw-r--r--   0        0        0      983 2024-05-21 00:22:21.777417 zetascale-2.5.1/zeta/nn/modules/query_proposal.py
+-rw-r--r--   0        0        0     1152 2024-05-21 00:22:21.777463 zetascale-2.5.1/zeta/nn/modules/recurrent_model.py
+-rw-r--r--   0        0        0      903 2024-05-21 00:22:21.777512 zetascale-2.5.1/zeta/nn/modules/recursive_block.py
+-rw-r--r--   0        0        0      369 2024-05-21 00:22:21.777555 zetascale-2.5.1/zeta/nn/modules/relu_squared.py
+-rw-r--r--   0        0        0     5037 2024-05-21 00:22:21.777610 zetascale-2.5.1/zeta/nn/modules/res_net.py
+-rw-r--r--   0        0        0      492 2024-05-21 00:22:21.777667 zetascale-2.5.1/zeta/nn/modules/residual.py
+-rw-r--r--   0        0        0     2238 2024-05-21 00:22:21.777714 zetascale-2.5.1/zeta/nn/modules/resnet.py
+-rw-r--r--   0        0        0     5349 2024-05-21 00:22:21.777769 zetascale-2.5.1/zeta/nn/modules/return_loss_text.py
+-rw-r--r--   0        0        0      829 2024-05-21 00:22:21.777812 zetascale-2.5.1/zeta/nn/modules/rms_norm.py
+-rw-r--r--   0        0        0     1646 2024-05-21 00:22:21.777856 zetascale-2.5.1/zeta/nn/modules/rnn_nlp.py
+-rw-r--r--   0        0        0     3106 2024-05-21 00:22:21.777902 zetascale-2.5.1/zeta/nn/modules/s4.py
+-rw-r--r--   0        0        0      818 2024-05-21 00:22:21.777947 zetascale-2.5.1/zeta/nn/modules/scale.py
+-rw-r--r--   0        0        0      882 2024-05-21 00:22:21.777993 zetascale-2.5.1/zeta/nn/modules/scale_norm.py
+-rw-r--r--   0        0        0     1433 2024-05-21 00:22:21.778037 zetascale-2.5.1/zeta/nn/modules/scaled_sinusoidal.py
+-rw-r--r--   0        0        0      799 2024-05-21 00:22:21.778086 zetascale-2.5.1/zeta/nn/modules/scalenorm.py
+-rw-r--r--   0        0        0     1858 2024-05-21 00:22:21.778139 zetascale-2.5.1/zeta/nn/modules/shift_tokens.py
+-rw-r--r--   0        0        0     2877 2024-05-21 00:22:21.778185 zetascale-2.5.1/zeta/nn/modules/shufflenet.py
+-rw-r--r--   0        0        0     8939 2024-05-21 00:22:21.778249 zetascale-2.5.1/zeta/nn/modules/sig_lip.py
+-rw-r--r--   0        0        0     2659 2024-05-25 16:41:31.796497 zetascale-2.5.1/zeta/nn/modules/sig_lip_loss.py
+-rw-r--r--   0        0        0      283 2024-05-21 00:22:21.778291 zetascale-2.5.1/zeta/nn/modules/simple_attention.py
+-rw-r--r--   0        0        0      692 2024-05-21 00:22:21.778338 zetascale-2.5.1/zeta/nn/modules/simple_feedforward.py
+-rw-r--r--   0        0        0     9719 2024-05-21 00:22:21.778406 zetascale-2.5.1/zeta/nn/modules/simple_mamba.py
+-rw-r--r--   0        0        0      764 2024-05-21 00:22:21.778454 zetascale-2.5.1/zeta/nn/modules/simple_res_block.py
+-rw-r--r--   0        0        0      978 2024-05-21 00:22:21.778496 zetascale-2.5.1/zeta/nn/modules/simple_resblock.py
+-rw-r--r--   0        0        0      638 2024-05-21 00:22:21.778535 zetascale-2.5.1/zeta/nn/modules/simple_rmsnorm.py
+-rw-r--r--   0        0        0      509 2024-05-21 00:22:21.778579 zetascale-2.5.1/zeta/nn/modules/skip_connect.py
+-rw-r--r--   0        0        0     1194 2024-05-21 00:22:21.778621 zetascale-2.5.1/zeta/nn/modules/skipconnection.py
+-rw-r--r--   0        0        0     3553 2024-05-21 00:22:21.778668 zetascale-2.5.1/zeta/nn/modules/slerp_model_merger.py
+-rw-r--r--   0        0        0      765 2024-05-21 00:22:21.778715 zetascale-2.5.1/zeta/nn/modules/sp_act.py
+-rw-r--r--   0        0        0    22085 2024-05-25 18:14:50.844937 zetascale-2.5.1/zeta/nn/modules/space_time_unet.py
+-rw-r--r--   0        0        0     1346 2024-05-21 00:22:21.778853 zetascale-2.5.1/zeta/nn/modules/spacial_transformer.py
+-rw-r--r--   0        0        0     4976 2024-05-21 00:22:21.778909 zetascale-2.5.1/zeta/nn/modules/sparq_attn.py
+-rw-r--r--   0        0        0    13915 2024-05-21 00:22:21.778984 zetascale-2.5.1/zeta/nn/modules/sparse_moe.py
+-rw-r--r--   0        0        0     7355 2024-05-25 22:02:37.956419 zetascale-2.5.1/zeta/nn/modules/sparse_token_integration.py
+-rw-r--r--   0        0        0     2021 2024-05-21 00:22:21.779039 zetascale-2.5.1/zeta/nn/modules/spatial_downsample.py
+-rw-r--r--   0        0        0     1346 2024-05-21 00:22:21.779080 zetascale-2.5.1/zeta/nn/modules/spatial_transformer.py
+-rw-r--r--   0        0        0     5006 2024-05-21 00:22:21.779136 zetascale-2.5.1/zeta/nn/modules/splines.py
+-rw-r--r--   0        0        0     1041 2024-05-21 00:22:21.779183 zetascale-2.5.1/zeta/nn/modules/squeeze_excitation.py
+-rw-r--r--   0        0        0     4334 2024-05-21 00:22:21.779242 zetascale-2.5.1/zeta/nn/modules/ssm.py
+-rw-r--r--   0        0        0     7305 2024-05-21 00:22:21.779306 zetascale-2.5.1/zeta/nn/modules/ssm_language.py
+-rw-r--r--   0        0        0      942 2024-05-21 00:22:21.779348 zetascale-2.5.1/zeta/nn/modules/stoch_depth.py
+-rw-r--r--   0        0        0      958 2024-05-21 00:22:21.779389 zetascale-2.5.1/zeta/nn/modules/stochastic_depth.py
+-rw-r--r--   0        0        0     2032 2024-05-21 00:22:21.779434 zetascale-2.5.1/zeta/nn/modules/subln.py
+-rw-r--r--   0        0        0      972 2024-05-21 00:22:21.779478 zetascale-2.5.1/zeta/nn/modules/super_resolution.py
+-rw-r--r--   0        0        0     5610 2024-05-21 00:37:47.055302 zetascale-2.5.1/zeta/nn/modules/swarmalator.py
+-rw-r--r--   0        0        0     1313 2024-05-21 00:22:21.779579 zetascale-2.5.1/zeta/nn/modules/swiglu.py
+-rw-r--r--   0        0        0      715 2024-05-21 00:22:21.779623 zetascale-2.5.1/zeta/nn/modules/tensor.py
+-rw-r--r--   0        0        0      865 2024-05-21 00:22:21.779670 zetascale-2.5.1/zeta/nn/modules/tensor_to_int.py
+-rw-r--r--   0        0        0     3281 2024-05-21 00:22:21.779722 zetascale-2.5.1/zeta/nn/modules/text_scene_fusion.py
+-rw-r--r--   0        0        0     2692 2024-05-21 00:22:21.779769 zetascale-2.5.1/zeta/nn/modules/text_video_fuse.py
+-rw-r--r--   0        0        0     2104 2024-05-21 00:22:21.779825 zetascale-2.5.1/zeta/nn/modules/time_up_sample.py
+-rw-r--r--   0        0        0      631 2024-05-21 00:22:21.779868 zetascale-2.5.1/zeta/nn/modules/to_logits.py
+-rw-r--r--   0        0        0     2158 2024-05-21 00:22:21.779914 zetascale-2.5.1/zeta/nn/modules/token_learner.py
+-rw-r--r--   0        0        0     1075 2024-05-21 00:22:21.779962 zetascale-2.5.1/zeta/nn/modules/token_mixer.py
+-rw-r--r--   0        0        0      189 2024-05-21 00:22:21.780004 zetascale-2.5.1/zeta/nn/modules/token_shift.py
+-rw-r--r--   0        0        0    10310 2024-05-21 00:22:21.780074 zetascale-2.5.1/zeta/nn/modules/top_n_gating.py
+-rw-r--r--   0        0        0     4363 2024-05-21 00:22:21.780127 zetascale-2.5.1/zeta/nn/modules/transformations.py
+-rw-r--r--   0        0        0      921 2024-05-21 00:22:21.780175 zetascale-2.5.1/zeta/nn/modules/triple_skip.py
+-rw-r--r--   0        0        0     2193 2024-05-21 00:22:21.780221 zetascale-2.5.1/zeta/nn/modules/triton_rmsnorm.py
+-rw-r--r--   0        0        0     4112 2024-05-21 00:22:21.780276 zetascale-2.5.1/zeta/nn/modules/u_mamba.py
+-rw-r--r--   0        0        0     4717 2024-05-21 00:22:21.780330 zetascale-2.5.1/zeta/nn/modules/unet.py
+-rw-r--r--   0        0        0      974 2024-05-21 00:22:21.780381 zetascale-2.5.1/zeta/nn/modules/v_layernorm.py
+-rw-r--r--   0        0        0     1686 2024-05-21 00:22:21.780429 zetascale-2.5.1/zeta/nn/modules/v_pool.py
+-rw-r--r--   0        0        0     2809 2024-05-21 00:22:21.780472 zetascale-2.5.1/zeta/nn/modules/video_autoencoder.py
+-rw-r--r--   0        0        0     9239 2024-05-21 00:22:21.780539 zetascale-2.5.1/zeta/nn/modules/video_diffusion_modules.py
+-rw-r--r--   0        0        0     1497 2024-05-21 00:22:21.780583 zetascale-2.5.1/zeta/nn/modules/video_to_tensor.py
+-rw-r--r--   0        0        0     1067 2024-05-21 00:22:21.780629 zetascale-2.5.1/zeta/nn/modules/video_to_text.py
+-rw-r--r--   0        0        0     2702 2024-05-21 00:22:21.780681 zetascale-2.5.1/zeta/nn/modules/vision_mamba.py
+-rw-r--r--   0        0        0     2018 2024-05-21 00:22:21.780733 zetascale-2.5.1/zeta/nn/modules/vision_weighted_permute_mlp.py
+-rw-r--r--   0        0        0     5445 2024-05-21 00:22:21.780804 zetascale-2.5.1/zeta/nn/modules/visual_expert.py
+-rw-r--r--   0        0        0     6103 2024-05-25 18:23:29.115939 zetascale-2.5.1/zeta/nn/modules/vit_denoiser.py
+-rw-r--r--   0        0        0     3099 2024-05-21 00:22:21.780910 zetascale-2.5.1/zeta/nn/modules/vss_block.py
+-rw-r--r--   0        0        0     2775 2024-05-21 00:22:21.780963 zetascale-2.5.1/zeta/nn/modules/ws_conv2d.py
+-rw-r--r--   0        0        0       86 2024-05-21 00:22:21.781034 zetascale-2.5.1/zeta/nn/modules/xmoe/__init__.py
+-rw-r--r--   0        0        0     2351 2024-05-21 00:22:21.781081 zetascale-2.5.1/zeta/nn/modules/xmoe/global_groups.py
+-rw-r--r--   0        0        0    12458 2024-05-21 00:22:21.781157 zetascale-2.5.1/zeta/nn/modules/xmoe/moe_layer.py
+-rw-r--r--   0        0        0    18694 2024-05-21 00:22:21.781205 zetascale-2.5.1/zeta/nn/modules/xmoe/routing.py
+-rw-r--r--   0        0        0     2302 2024-05-21 00:22:21.781262 zetascale-2.5.1/zeta/nn/modules/yolo.py
+-rw-r--r--   0        0        0     2595 2024-05-21 00:22:21.781338 zetascale-2.5.1/zeta/ops/__Init__.py
+-rw-r--r--   0        0        0      287 2024-05-21 00:22:21.781384 zetascale-2.5.1/zeta/ops/absmax.py
+-rw-r--r--   0        0        0     2652 2024-05-21 00:22:21.781432 zetascale-2.5.1/zeta/ops/async_softmax.py
+-rw-r--r--   0        0        0     2054 2024-05-21 00:22:21.781475 zetascale-2.5.1/zeta/ops/dilated_attn_ops.py
+-rw-r--r--   0        0        0     2017 2024-05-21 00:22:21.781530 zetascale-2.5.1/zeta/ops/einops_from_to.py
+-rw-r--r--   0        0        0     1876 2024-05-21 00:22:21.781580 zetascale-2.5.1/zeta/ops/einops_poly.py
+-rw-r--r--   0        0        0     2150 2024-05-21 00:22:21.781631 zetascale-2.5.1/zeta/ops/expand.py
+-rw-r--r--   0        0        0     1262 2024-05-21 00:22:21.781685 zetascale-2.5.1/zeta/ops/laplace.py
+-rw-r--r--   0        0        0    16114 2024-05-21 00:37:47.171297 zetascale-2.5.1/zeta/ops/main.py
+-rw-r--r--   0        0        0     1392 2024-05-21 00:22:21.781830 zetascale-2.5.1/zeta/ops/misc_act.py
+-rw-r--r--   0        0        0     1671 2024-05-21 00:22:21.781882 zetascale-2.5.1/zeta/ops/mm_rearranges.py
+-rw-r--r--   0        0        0      996 2024-05-21 00:22:21.781933 zetascale-2.5.1/zeta/ops/mm_softmax.py
+-rw-r--r--   0        0        0     1851 2024-05-21 00:22:21.781984 zetascale-2.5.1/zeta/ops/mos.py
+-rw-r--r--   0        0        0      995 2024-05-21 00:22:21.782043 zetascale-2.5.1/zeta/ops/nonlinear.py
+-rw-r--r--   0        0        0     5070 2024-05-21 00:22:21.782115 zetascale-2.5.1/zeta/ops/softmax.py
+-rw-r--r--   0        0        0     1086 2024-05-21 00:22:21.782171 zetascale-2.5.1/zeta/ops/sparsemax.py
+-rw-r--r--   0        0        0      453 2024-05-21 00:22:21.782225 zetascale-2.5.1/zeta/ops/unitwise_norm.py
+-rw-r--r--   0        0        0      814 2024-05-21 00:22:21.782317 zetascale-2.5.1/zeta/optim/__init__.py
+-rw-r--r--   0        0        0    41040 2024-05-21 00:37:47.266975 zetascale-2.5.1/zeta/optim/batched_optimizer.py
+-rw-r--r--   0        0        0    10142 2024-05-21 00:22:21.782511 zetascale-2.5.1/zeta/optim/decoupled_lion.py
+-rw-r--r--   0        0        0     6448 2024-05-21 00:22:21.782568 zetascale-2.5.1/zeta/optim/decoupled_optimizer.py
+-rw-r--r--   0        0        0    12445 2024-05-21 00:22:21.782643 zetascale-2.5.1/zeta/optim/decoupled_sophia.py
+-rw-r--r--   0        0        0     4709 2024-05-21 00:22:21.782696 zetascale-2.5.1/zeta/optim/gradient_ascent.py
+-rw-r--r--   0        0        0     2752 2024-05-21 00:22:21.782748 zetascale-2.5.1/zeta/optim/gradient_equillibrum.py
+-rw-r--r--   0        0        0    19017 2024-05-21 00:22:21.782817 zetascale-2.5.1/zeta/optim/lion8b.py
+-rw-r--r--   0        0        0     3387 2024-05-21 00:22:21.782876 zetascale-2.5.1/zeta/optim/parallel_gradient_descent.py
+-rw-r--r--   0        0        0     4456 2024-05-21 00:37:47.112761 zetascale-2.5.1/zeta/optim/stable_adam.py
+-rw-r--r--   0        0        0      453 2024-05-21 00:22:21.782994 zetascale-2.5.1/zeta/quant/__init__.py
+-rw-r--r--   0        0        0      405 2024-05-21 00:22:21.783040 zetascale-2.5.1/zeta/quant/absmax.py
+-rw-r--r--   0        0        0     2098 2024-05-21 00:22:21.783091 zetascale-2.5.1/zeta/quant/bitlinear.py
+-rw-r--r--   0        0        0     1947 2024-05-21 00:22:21.783141 zetascale-2.5.1/zeta/quant/half_bit_linear.py
+-rw-r--r--   0        0        0    10942 2024-05-21 00:22:21.783220 zetascale-2.5.1/zeta/quant/lfq.py
+-rw-r--r--   0        0        0     3126 2024-05-21 00:22:21.783269 zetascale-2.5.1/zeta/quant/niva.py
+-rw-r--r--   0        0        0    25173 2024-05-21 00:22:21.783337 zetascale-2.5.1/zeta/quant/qlora.py
+-rw-r--r--   0        0        0     6010 2024-05-21 00:22:21.783405 zetascale-2.5.1/zeta/quant/qmoe.py
+-rw-r--r--   0        0        0     3785 2024-05-21 00:22:21.783451 zetascale-2.5.1/zeta/quant/quick.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.783469 zetascale-2.5.1/zeta/quant/random_proj_quan.py
+-rw-r--r--   0        0        0     1602 2024-05-21 00:22:21.783524 zetascale-2.5.1/zeta/quant/residual_vq.py
+-rw-r--r--   0        0        0     1547 2024-05-21 00:22:21.783574 zetascale-2.5.1/zeta/quant/ste.py
+-rw-r--r--   0        0        0      522 2024-05-21 00:22:21.783655 zetascale-2.5.1/zeta/rl/__init__.py
+-rw-r--r--   0        0        0     4286 2024-05-21 00:22:21.783724 zetascale-2.5.1/zeta/rl/actor_critic.py
+-rw-r--r--   0        0        0     2509 2024-05-21 00:22:21.783780 zetascale-2.5.1/zeta/rl/dpo.py
+-rw-r--r--   0        0        0     3381 2024-05-21 00:22:21.783837 zetascale-2.5.1/zeta/rl/hindsight_replay.py
+-rw-r--r--   0        0        0     2033 2024-05-21 00:22:21.783886 zetascale-2.5.1/zeta/rl/language_reward.py
+-rw-r--r--   0        0        0     4130 2024-05-21 00:22:21.783936 zetascale-2.5.1/zeta/rl/ppo.py
+-rw-r--r--   0        0        0     4513 2024-05-21 00:22:21.784007 zetascale-2.5.1/zeta/rl/priortized_replay_buffer.py
+-rw-r--r--   0        0        0     5765 2024-05-21 00:22:21.784062 zetascale-2.5.1/zeta/rl/priortized_rps.py
+-rw-r--r--   0        0        0      128 2024-05-21 00:22:21.784116 zetascale-2.5.1/zeta/rl/rest.py
+-rw-r--r--   0        0        0     4585 2024-05-21 00:22:21.784178 zetascale-2.5.1/zeta/rl/reward_model.py
+-rw-r--r--   0        0        0     2987 2024-05-21 00:22:21.784233 zetascale-2.5.1/zeta/rl/sumtree.py
+-rw-r--r--   0        0        0     3185 2024-05-21 00:22:21.784290 zetascale-2.5.1/zeta/rl/vision_model_rl.py
+-rw-r--r--   0        0        0     1227 2024-05-21 00:22:21.784375 zetascale-2.5.1/zeta/structs/__init__.py
+-rw-r--r--   0        0        0    11731 2024-05-21 00:22:21.784455 zetascale-2.5.1/zeta/structs/auto_regressive_wrapper.py
+-rw-r--r--   0        0        0     3505 2024-05-21 00:22:21.784512 zetascale-2.5.1/zeta/structs/clip_encoder.py
+-rw-r--r--   0        0        0     6600 2024-05-21 00:22:21.784570 zetascale-2.5.1/zeta/structs/efficient_net.py
+-rw-r--r--   0        0        0     3219 2024-05-21 00:22:21.784620 zetascale-2.5.1/zeta/structs/encoder_decoder.py
+-rw-r--r--   0        0        0    28639 2024-05-21 00:22:21.784698 zetascale-2.5.1/zeta/structs/hierarchical_transformer.py
+-rw-r--r--   0        0        0     5946 2024-05-21 00:22:21.784771 zetascale-2.5.1/zeta/structs/local_transformer.py
+-rw-r--r--   0        0        0     1665 2024-05-21 00:22:21.784824 zetascale-2.5.1/zeta/structs/multi_modal_projector.py
+-rw-r--r--   0        0        0    10839 2024-05-21 00:22:21.784890 zetascale-2.5.1/zeta/structs/simple_transformer.py
+-rw-r--r--   0        0        0     2468 2024-05-21 00:22:21.784940 zetascale-2.5.1/zeta/structs/simple_vision_encoder.py
+-rw-r--r--   0        0        0    68945 2024-05-21 00:22:21.785012 zetascale-2.5.1/zeta/structs/transformer.py
+-rw-r--r--   0        0        0     4490 2024-05-21 00:22:21.785085 zetascale-2.5.1/zeta/structs/transformer_block.py
+-rw-r--r--   0        0        0      485 2024-05-21 00:22:21.785165 zetascale-2.5.1/zeta/tokenizers/__init__.py
+-rw-r--r--   0        0        0     1438 2024-05-21 00:22:21.785219 zetascale-2.5.1/zeta/tokenizers/gptx_tokenizer.py
+-rw-r--r--   0        0        0     3079 2024-05-21 00:22:21.785272 zetascale-2.5.1/zeta/tokenizers/llama_sentencepiece.py
+-rw-r--r--   0        0        0     3651 2024-05-21 00:22:21.785332 zetascale-2.5.1/zeta/tokenizers/multi_modal_tokenizer.py
+-rw-r--r--   0        0        0     3720 2024-05-21 00:22:21.785394 zetascale-2.5.1/zeta/tokenizers/sentence_piece.py
+-rw-r--r--   0        0        0     9771 2024-05-21 00:22:21.785468 zetascale-2.5.1/zeta/tokenizers/tokenmonster.py
+-rw-r--r--   0        0        0      460 2024-05-21 00:22:21.785556 zetascale-2.5.1/zeta/training/__init__.py
+-rw-r--r--   0        0        0     5400 2024-05-21 00:22:21.785622 zetascale-2.5.1/zeta/training/activation_checkpoint.py
+-rw-r--r--   0        0        0     2576 2024-05-21 00:22:21.785674 zetascale-2.5.1/zeta/training/dataloader.py
+-rw-r--r--   0        0        0     3496 2024-05-21 00:22:21.785729 zetascale-2.5.1/zeta/training/fsdp.py
+-rw-r--r--   0        0        0     3186 2024-05-21 00:22:21.785785 zetascale-2.5.1/zeta/training/galore.py
+-rw-r--r--   0        0        0     6054 2024-05-21 00:22:21.785852 zetascale-2.5.1/zeta/training/hive_trainer.py
+-rw-r--r--   0        0        0     1626 2024-05-21 00:22:21.785901 zetascale-2.5.1/zeta/training/parallel_wrapper.py
+-rw-r--r--   0        0        0     2076 2024-05-21 00:37:47.158519 zetascale-2.5.1/zeta/training/scheduler.py
+-rw-r--r--   0        0        0     9273 2024-05-21 00:22:21.786034 zetascale-2.5.1/zeta/training/train.py
+-rw-r--r--   0        0        0     2347 2024-05-21 00:22:21.786126 zetascale-2.5.1/zeta/utils/__init__.py
+-rw-r--r--   0        0        0     3464 2024-05-21 00:22:21.786186 zetascale-2.5.1/zeta/utils/benchmark.py
+-rw-r--r--   0        0        0     1347 2024-05-21 00:22:21.786243 zetascale-2.5.1/zeta/utils/cuda_memory_wrapper.py
+-rw-r--r--   0        0        0     6424 2024-05-21 00:22:21.786310 zetascale-2.5.1/zeta/utils/cuda_wrapper.py
+-rw-r--r--   0        0        0     1337 2024-05-21 00:22:21.786368 zetascale-2.5.1/zeta/utils/disable_logging.py
+-rw-r--r--   0        0        0     1184 2024-05-21 00:22:21.786416 zetascale-2.5.1/zeta/utils/enforce_types.py
+-rw-r--r--   0        0        0     1110 2024-05-21 00:22:21.786470 zetascale-2.5.1/zeta/utils/img_to_tensor.py
+-rw-r--r--   0        0        0     2953 2024-05-21 00:22:21.786528 zetascale-2.5.1/zeta/utils/log_pytorch_op.py
+-rw-r--r--   0        0        0    19874 2024-05-21 00:22:21.786616 zetascale-2.5.1/zeta/utils/main.py
+-rw-r--r--   0        0        0     1798 2024-05-21 00:22:21.786682 zetascale-2.5.1/zeta/utils/module_device.py
+-rw-r--r--   0        0        0      703 2024-05-21 00:22:21.786733 zetascale-2.5.1/zeta/utils/params.py
+-rw-r--r--   0        0        0     3966 2024-05-21 00:22:21.786789 zetascale-2.5.1/zeta/utils/save_load_wrapper.py
+-rw-r--r--   0        0        0      846 2024-05-21 00:22:21.786844 zetascale-2.5.1/zeta/utils/text_to_tensor.py
+-rw-r--r--   0        0        0      751 2024-05-21 00:22:21.786904 zetascale-2.5.1/zeta/utils/verbose_execution.py
+-rw-r--r--   0        0        0    25931 2024-05-21 00:22:21.786981 zetascale-2.5.1/zeta/utils/vision_utils.py
+-rw-r--r--   0        0        0    21443 1970-01-01 00:00:00.000000 zetascale-2.5.1/PKG-INFO
```

### Comparing `zetascale-2.4.8/LICENSE` & `zetascale-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/README.md` & `zetascale-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/pyproject.toml` & `zetascale-2.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zetascale"
-version = "2.4.8"
+version = "2.5.1"
 description = "Rapidly Build, Optimize, and Deploy SOTA AI Models"
 authors = ["Zeta Team <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kyegomez/zeta"
 keywords = ["Transformers", "zeta scale"]
 classifiers = [
@@ -14,22 +14,22 @@
     { include = "zeta" },
     { include = "zeta/**/*.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 torch = ">=2.1.1,<3.0"
-pytest = "8.1.1"
+pytest = "8.2.1"
 torchfix = "*"
 einops = "0.7.0"
 bitsandbytes = "0.43.0"
-transformers = "4.40.1"
+transformers = "4.41.0"
 einops-exts = "0.0.4"
 torchvision = "0.18.0"
-accelerate = "0.28.0"
+accelerate = "0.30.1"
 datasets = "*"
 loguru = "*"
 vector-quantize-pytorch = "1.14.7"
 scipy = "1.9.3"
 beartype = "0.17.2"
 tqdm = "4.66.3"
 rich = "13.7.1"
@@ -46,15 +46,15 @@
 ruff = ">=0.0.249,<0.3.5"
 types-toml = "^0.10.8.1"
 types-redis = "^4.3.21.6"
 types-pytz = ">=2023.3,<2025.0"
 black = ">=23.1,<25.0"
 types-chardet = "^5.0.4.6"
 mypy-protobuf = "^3.0.0"
-pytest = "8.1.1"
+pytest = "8.2.1"
 
 [tool.ruff]
 line-length = 80
 
 [tool.black]
 line-length = 80
 target-version = ['py38']
```

### Comparing `zetascale-2.4.8/zeta/__init__.py` & `zetascale-2.5.1/zeta/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/cli/main.py` & `zetascale-2.5.1/zeta/cli/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/cloud/main.py` & `zetascale-2.5.1/zeta/cloud/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/cloud/sky_api.py` & `zetascale-2.5.1/zeta/cloud/sky_api.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/experimental/triton/activations/__init__.py` & `zetascale-2.5.1/zeta/experimental/triton/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/experimental/triton/activations/activations.py` & `zetascale-2.5.1/zeta/experimental/triton/activations/activations.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/experimental/triton/activations/functions.py` & `zetascale-2.5.1/zeta/experimental/triton/activations/functions.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/experimental/triton/triton_modules/linear_proj.py` & `zetascale-2.5.1/zeta/experimental/triton/triton_modules/linear_proj.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/LongNet.py` & `zetascale-2.5.1/zeta/models/LongNet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/__init__.py` & `zetascale-2.5.1/zeta/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/andromeda.py` & `zetascale-2.5.1/zeta/models/andromeda.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/beit3.py` & `zetascale-2.5.1/zeta/models/BEiT3.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/gpt4.py` & `zetascale-2.5.1/zeta/models/gpt4.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/kosmos.py` & `zetascale-2.5.1/zeta/models/kosmos.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/llama.py` & `zetascale-2.5.1/zeta/models/llama.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/max_vit.py` & `zetascale-2.5.1/zeta/models/max_vit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/mega_vit.py` & `zetascale-2.5.1/zeta/models/mega_vit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/mm_mamba.py` & `zetascale-2.5.1/zeta/models/mm_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/navit.py` & `zetascale-2.5.1/zeta/models/navit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/palme.py` & `zetascale-2.5.1/zeta/models/palme.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/models/vit.py` & `zetascale-2.5.1/zeta/models/vit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/__init__.py` & `zetascale-2.5.1/zeta/nn/attention/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from zeta.nn.attention.spatial_linear_attention import SpatialLinearAttention
 from zeta.structs.transformer import Attention, AttentionLayers
 from zeta.nn.attention.multi_grouped_attn import MultiGroupedQueryAttn
 from zeta.nn.attention.scalable_img_self_attn import ScalableImgSelfAttention
 from zeta.nn.attention.linearized_attention import LinearizedAttention
 
 
-
 __all__ = [
     "Attend",
     "FlashAttention",
     "LocalAttention",
     "LocalMHA",
     "Intermediates",
     "MixtureOfAttention",
```

### Comparing `zetascale-2.4.8/zeta/nn/attention/agent_attn.py` & `zetascale-2.5.1/zeta/nn/attention/agent_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/attend.py` & `zetascale-2.5.1/zeta/nn/attention/attend.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/cross_attention.py` & `zetascale-2.5.1/zeta/nn/attention/cross_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/cross_attn_images.py` & `zetascale-2.5.1/zeta/nn/attention/cross_attn_images.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/dilated_attention.py` & `zetascale-2.5.1/zeta/nn/attention/dilated_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/flash_attention.py` & `zetascale-2.5.1/zeta/nn/attention/flash_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/linear_attention.py` & `zetascale-2.5.1/zeta/nn/attention/linear_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/linear_attn_l.py` & `zetascale-2.5.1/zeta/nn/attention/linear_attn_l.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/local_attention.py` & `zetascale-2.5.1/zeta/nn/attention/local_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/local_attention_mha.py` & `zetascale-2.5.1/zeta/nn/attention/local_attention_mha.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/mixture_attention.py` & `zetascale-2.5.1/zeta/nn/attention/mixture_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/multi_grouped_attn.py` & `zetascale-2.5.1/zeta/nn/attention/multi_grouped_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/multi_modal_causal_attention.py` & `zetascale-2.5.1/zeta/nn/attention/multi_modal_causal_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/multi_modal_cross_attn.py` & `zetascale-2.5.1/zeta/nn/attention/multi_modal_cross_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/multihead_attention.py` & `zetascale-2.5.1/zeta/nn/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/multiquery_attention.py` & `zetascale-2.5.1/zeta/nn/attention/multiquery_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -606,30 +606,28 @@
             self.attn_fn = triton_flash_attn_fn
             if verbose:
                 warnings.warn(
                     "While `attn_impl: triton` can be faster than `attn_impl:"
                     " flash` "
                     + "it uses more memory. When training larger models"
                     " this can"
-                    " trigger "
-                    + "alloc retries which hurts performance. If"
+                    " trigger " + "alloc retries which hurts performance. If"
                     " encountered, we"
                     " recommend "
                     + "using `attn_impl: flash` if your model does not use"
                     " `alibi` or `prefix_lm`."
                 )
         elif self.attn_impl == "torch":
             self.attn_fn = scaled_multihead_dot_product_attention
             if torch.cuda.is_available() and verbose:
                 warnings.warn(
                     "Using `attn_impl: torch`. If your model does not use"
                     " `alibi` or "
                     + "`prefix_lm` we recommend using `attn_impl: flash`"
-                    " otherwise "
-                    + "we recommend using `attn_impl: triton`."
+                    " otherwise " + "we recommend using `attn_impl: triton`."
                 )
         else:
             raise ValueError(f"{attn_impl=} is an invalid setting.")
 
         self.out_proj = FC_CLASS_REGISTRY[fc_type](
             self.d_model,
             self.d_model,
@@ -740,30 +738,28 @@
             self.attn_fn = triton_flash_attn_fn
             if verbose:
                 warnings.warn(
                     "While `attn_impl: triton` can be faster than `attn_impl:"
                     " flash` "
                     + "it uses more memory. When training larger models"
                     " this can"
-                    " trigger "
-                    + "alloc retries which hurts performance. If"
+                    " trigger " + "alloc retries which hurts performance. If"
                     " encountered, we"
                     " recommend "
                     + "using `attn_impl: flash` if your model does not use"
                     " `alibi` or `prefix_lm`."
                 )
         elif self.attn_impl == "torch":
             self.attn_fn = scaled_multihead_dot_product_attention
             if torch.cuda.is_available() and verbose:
                 warnings.warn(
                     "Using `attn_impl: torch`. If your model does not use"
                     " `alibi` or "
                     + "`prefix_lm` we recommend using `attn_impl: flash`"
-                    " otherwise "
-                    + "we recommend using `attn_impl: triton`."
+                    " otherwise " + "we recommend using `attn_impl: triton`."
                 )
         else:
             raise ValueError(f"{attn_impl=} is an invalid setting.")
 
         self.out_proj = FC_CLASS_REGISTRY[fc_type](
             self.d_model,
             self.d_model,
```

### Comparing `zetascale-2.4.8/zeta/nn/attention/scalable_img_self_attn.py` & `zetascale-2.5.1/zeta/nn/attention/scalable_img_self_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/shaped_attention.py` & `zetascale-2.5.1/zeta/nn/attention/shaped_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/sparse_attention.py` & `zetascale-2.5.1/zeta/nn/attention/sparse_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/spatial_linear_attention.py` & `zetascale-2.5.1/zeta/nn/attention/spatial_linear_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/attention/xc_attention.py` & `zetascale-2.5.1/zeta/nn/attention/xc_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/biases/alibi.py` & `zetascale-2.5.1/zeta/nn/biases/alibi.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/biases/dynamic_position_bias.py` & `zetascale-2.5.1/zeta/nn/biases/dynamic_position_bias.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/biases/relative_position_bias.py` & `zetascale-2.5.1/zeta/nn/biases/relative_position_bias.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/__init__.py` & `zetascale-2.5.1/zeta/nn/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/abc_pos_emb.py` & `zetascale-2.5.1/zeta/nn/embeddings/abc_pos_emb.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/embedding.py` & `zetascale-2.5.1/zeta/nn/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/multiway_network.py` & `zetascale-2.5.1/zeta/nn/embeddings/multiway_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/patch_embedding.py` & `zetascale-2.5.1/zeta/nn/embeddings/patch_embedding.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/pi.md` & `zetascale-2.5.1/zeta/nn/embeddings/pi.md`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/positional.py` & `zetascale-2.5.1/zeta/nn/embeddings/positional.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/positional_interpolation.py` & `zetascale-2.5.1/zeta/nn/embeddings/positional_interpolation.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/qfsp_embeddings.py` & `zetascale-2.5.1/zeta/nn/embeddings/qfsp_embeddings.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/qft_embeddings.py` & `zetascale-2.5.1/zeta/nn/embeddings/qft_embeddings.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/rope.py` & `zetascale-2.5.1/zeta/nn/embeddings/rope.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py` & `zetascale-2.5.1/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/sine_positional.py` & `zetascale-2.5.1/zeta/nn/embeddings/sine_positional.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/sinusoidal.py` & `zetascale-2.5.1/zeta/nn/embeddings/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/truncated_rope.py` & `zetascale-2.5.1/zeta/nn/embeddings/truncated_rope.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/vis_lang_emb.py` & `zetascale-2.5.1/zeta/nn/embeddings/vis_lang_emb.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/vision_emb.py` & `zetascale-2.5.1/zeta/nn/embeddings/vision_emb.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/xpos_relative_position.py` & `zetascale-2.5.1/zeta/nn/embeddings/xpos_relative_position.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/embeddings/yarn.py` & `zetascale-2.5.1/zeta/nn/embeddings/yarn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/masks/__init__.py` & `zetascale-2.5.1/zeta/nn/masks/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/masks/attn_masks.py` & `zetascale-2.5.1/zeta/nn/masks/attn_masks.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/masks/block_diagonal.py` & `zetascale-2.5.1/zeta/nn/masks/block_diagonal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/README.md` & `zetascale-2.5.1/zeta/nn/modules/README.md`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/__init__.py` & `zetascale-2.5.1/zeta/nn/modules/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,20 @@
 from zeta.nn.modules.query_proposal import TextHawkQueryProposal
 from zeta.nn.modules.pixel_shuffling import PixelShuffleDownscale
 from zeta.nn.modules.kan import KAN
 from zeta.nn.modules.layer_scale import LayerScale
 from zeta.nn.modules.fractoral_norm import FractoralNorm
 from zeta.nn.modules.kv_cache_update import kv_cache_with_update
 from zeta.nn.modules.expand import expand
+from zeta.nn.modules.sig_lip_loss import SigLipSigmoidLoss
+from zeta.nn.modules.sparse_token_integration import (
+    SparseTokenIntegration,
+    SparseChannelIntegration,
+)
+
 # from zeta.nn.modules.img_reshape import image_reshape
 # from zeta.nn.modules.flatten_features import flatten_features
 # from zeta.nn.modules.scaled_sinusoidal import ScaledSinuosidalEmbedding
 # from zeta.nn.modules.scale import Scale
 # from zeta.nn.modules.scalenorm import ScaleNorm
 # from zeta.nn.modules.simple_rmsnorm import SimpleRMSNorm
 # from zeta.nn.modules.gru_gating import GRUGating
@@ -429,8 +435,11 @@
     "TextHawkQueryProposal",
     "PixelShuffleDownscale",
     "KAN",
     "LayerScale",
     "FractoralNorm",
     "kv_cache_with_update",
     "expand",
+    "SigLipSigmoidLoss",
+    "SparseTokenIntegration",
+    "SparseChannelIntegration",
 ]
```

### Comparing `zetascale-2.4.8/zeta/nn/modules/_activations.py` & `zetascale-2.5.1/zeta/nn/modules/_activations.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/adaptive_conv.py` & `zetascale-2.5.1/zeta/nn/modules/adaptive_conv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/adaptive_layernorm.py` & `zetascale-2.5.1/zeta/nn/modules/adaptive_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/adaptive_parameter_list.py` & `zetascale-2.5.1/zeta/nn/modules/adaptive_parameter_list.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/adaptive_rmsnorm.py` & `zetascale-2.5.1/zeta/nn/modules/adaptive_rmsnorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/alr_block.py` & `zetascale-2.5.1/zeta/nn/modules/alr_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/attn.py` & `zetascale-2.5.1/zeta/nn/modules/attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/audio_to_text.py` & `zetascale-2.5.1/zeta/nn/modules/audio_to_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/avg_model_merger.py` & `zetascale-2.5.1/zeta/nn/modules/avg_model_merger.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/block_butterfly_mlp.py` & `zetascale-2.5.1/zeta/nn/modules/block_butterfly_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/blockdiag_butterfly.py` & `zetascale-2.5.1/zeta/nn/modules/blockdiag_butterfly.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import partial
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 from einops import rearrange
 from torch import nn
-from torch.nn import functional as F, init
+from torch.nn import init
 
 
 def blockdiag_butterfly_multiply_reference(x, w1_bfly, w2_bfly, version=2):
     """
     This implementation is slow but more likely to be correct.
     There are 3 implementations, which should all yield the same answer
     Arguments:
```

### Comparing `zetascale-2.4.8/zeta/nn/modules/chan_layer_norm.py` & `zetascale-2.5.1/zeta/nn/modules/chan_layer_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/clex.py` & `zetascale-2.5.1/zeta/nn/modules/clex.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/clip_bottleneck.py` & `zetascale-2.5.1/zeta/nn/modules/clip_bottleneck.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/cnn_text.py` & `zetascale-2.5.1/zeta/nn/modules/cnn_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/combined_linear.py` & `zetascale-2.5.1/zeta/nn/modules/combined_linear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/conv_bn_relu.py` & `zetascale-2.5.1/zeta/nn/modules/conv_bn_relu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/conv_mlp.py` & `zetascale-2.5.1/zeta/nn/modules/conv_mlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,17 +66,15 @@
 
         self.apply(init_module)
 
     def forward(self, x: Tensor) -> Tensor:
         # The conv layers expect NCHW, we have NLC by default
         B, L, C = x.shape
         HW = int(math.sqrt(x.shape[-2]))
-        assert (
-            HW**2 == L
-        ), "Conv2DFeedforward requires squared context lengths"
+        assert HW**2 == L, "Conv2DFeedforward requires squared context lengths"
 
         x = x.reshape((B, HW, HW, C)).swapdims(1, -1)
 
         # The actual FW, including the 2d convolutions
         x = self.conv_mlp(x)
 
         # back to NLC
```

### Comparing `zetascale-2.4.8/zeta/nn/modules/convnet.py` & `zetascale-2.5.1/zeta/nn/modules/convnet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/cross_embed_layer.py` & `zetascale-2.5.1/zeta/nn/modules/cross_embed_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/cross_modal_reparametization.py` & `zetascale-2.5.1/zeta/nn/modules/cross_modal_reparametization.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/decision_tree.py` & `zetascale-2.5.1/zeta/nn/modules/decision_tree.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/deepseek_moe.py` & `zetascale-2.5.1/zeta/nn/modules/deepseek_moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/dense_connect.py` & `zetascale-2.5.1/zeta/nn/modules/dense_connect.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/diffusion.py` & `zetascale-2.5.1/zeta/nn/modules/diffusion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/droppath.py` & `zetascale-2.5.1/zeta/nn/modules/droppath.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/dual_path_block.py` & `zetascale-2.5.1/zeta/nn/modules/dual_path_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/dyna_conv.py` & `zetascale-2.5.1/zeta/nn/modules/dyna_conv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/dynamic_module.py` & `zetascale-2.5.1/zeta/nn/modules/dynamic_module.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/dynamic_routing_block.py` & `zetascale-2.5.1/zeta/nn/modules/dynamic_routing_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/embedding_to_grid.py` & `zetascale-2.5.1/zeta/nn/modules/embedding_to_grid.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/ether.py` & `zetascale-2.5.1/zeta/nn/modules/ether.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/exo.py` & `zetascale-2.5.1/zeta/nn/modules/exo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/expand_channels.py` & `zetascale-2.5.1/zeta/nn/modules/expand_channels.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/expert.py` & `zetascale-2.5.1/zeta/nn/modules/expert.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/fast_text.py` & `zetascale-2.5.1/zeta/nn/modules/fast_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/feedback_block.py` & `zetascale-2.5.1/zeta/nn/modules/feedback_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/feedforward.py` & `zetascale-2.5.1/zeta/nn/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/feedforward_network.py` & `zetascale-2.5.1/zeta/nn/modules/feedforward_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/film.py` & `zetascale-2.5.1/zeta/nn/modules/film.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/film_conditioning.py` & `zetascale-2.5.1/zeta/nn/modules/film_conditioning.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/film_efficient_metb3.py` & `zetascale-2.5.1/zeta/nn/modules/film_efficient_metb3.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/flatten_features.py` & `zetascale-2.5.1/zeta/nn/modules/flatten_features.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/flex_conv.py` & `zetascale-2.5.1/zeta/nn/modules/flex_conv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/flexible_mlp.py` & `zetascale-2.5.1/zeta/nn/modules/flexible_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/fractoral_norm.py` & `zetascale-2.5.1/zeta/nn/modules/fractoral_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/fractorial_net.py` & `zetascale-2.5.1/zeta/nn/modules/fractorial_net.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/freeze_layers.py` & `zetascale-2.5.1/zeta/nn/modules/freeze_layers.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/fused_dropout_add.py` & `zetascale-2.5.1/zeta/nn/modules/fused_dropout_add.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/fused_dropout_layernom.py` & `zetascale-2.5.1/zeta/nn/modules/fused_dropout_layernom.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/fused_gelu_dense.py` & `zetascale-2.5.1/zeta/nn/modules/fused_gelu_dense.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/fusion_ffn.py` & `zetascale-2.5.1/zeta/nn/modules/fusion_ffn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/g_shard_moe.py` & `zetascale-2.5.1/zeta/nn/modules/g_shard_moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/gated_residual_block.py` & `zetascale-2.5.1/zeta/nn/modules/gated_residual_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/gill_mapper.py` & `zetascale-2.5.1/zeta/nn/modules/gill_mapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/glu.py` & `zetascale-2.5.1/zeta/nn/modules/glu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/gru_gating.py` & `zetascale-2.5.1/zeta/nn/modules/gru_gating.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/h3.py` & `zetascale-2.5.1/zeta/nn/modules/h3.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/hebbian.py` & `zetascale-2.5.1/zeta/nn/modules/hebbian.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/highway_layer.py` & `zetascale-2.5.1/zeta/nn/modules/highway_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/image_projector.py` & `zetascale-2.5.1/zeta/nn/modules/image_projector.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/image_to_text.py` & `zetascale-2.5.1/zeta/nn/modules/image_to_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/img_or_video_to_time.py` & `zetascale-2.5.1/zeta/nn/modules/img_or_video_to_time.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/img_patch_embed.py` & `zetascale-2.5.1/zeta/nn/modules/img_patch_embed.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/img_reshape.py` & `zetascale-2.5.1/zeta/nn/modules/img_reshape.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/itca.py` & `zetascale-2.5.1/zeta/nn/modules/itca.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/kan.py` & `zetascale-2.5.1/zeta/nn/modules/kan.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/kv_cache.py` & `zetascale-2.5.1/zeta/nn/modules/kv_cache.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/kv_cache_update.py` & `zetascale-2.5.1/zeta/nn/modules/kv_cache_update.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/lambda_mask.py` & `zetascale-2.5.1/zeta/nn/modules/lambda_mask.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/lang_conv_module.py` & `zetascale-2.5.1/zeta/nn/modules/lang_conv_module.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/laser.py` & `zetascale-2.5.1/zeta/nn/modules/laser.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/layer_scale.py` & `zetascale-2.5.1/zeta/nn/modules/layer_scale.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/layernorm.py` & `zetascale-2.5.1/zeta/nn/modules/layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/leaky_relu.py` & `zetascale-2.5.1/zeta/nn/modules/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/log_ff.py` & `zetascale-2.5.1/zeta/nn/modules/log_ff.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/lora.py` & `zetascale-2.5.1/zeta/nn/modules/lora.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/matrix.py` & `zetascale-2.5.1/zeta/nn/modules/matrix.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/mbconv.py` & `zetascale-2.5.1/zeta/nn/modules/mbconv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/mixtape.py` & `zetascale-2.5.1/zeta/nn/modules/mixtape.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/mixtral_expert.py` & `zetascale-2.5.1/zeta/nn/modules/mixtral_expert.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/mlp.py` & `zetascale-2.5.1/zeta/nn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/mlp_mixer.py` & `zetascale-2.5.1/zeta/nn/modules/mlp_mixer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/mm_adapter.py` & `zetascale-2.5.1/zeta/nn/modules/mm_adapter.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/mm_layernorm.py` & `zetascale-2.5.1/zeta/nn/modules/mm_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/mm_ops.py` & `zetascale-2.5.1/zeta/nn/modules/mm_ops.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/modality_adaptive_module.py` & `zetascale-2.5.1/zeta/nn/modules/modality_adaptive_module.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/moe.py` & `zetascale-2.5.1/zeta/nn/modules/moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/moe_router.py` & `zetascale-2.5.1/zeta/nn/modules/moe_router.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/monarch_mlp.py` & `zetascale-2.5.1/zeta/nn/modules/monarch_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/mr_adapter.py` & `zetascale-2.5.1/zeta/nn/modules/mr_adapter.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/multi_input_multi_output.py` & `zetascale-2.5.1/zeta/nn/modules/multi_input_multi_output.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/multi_scale_block.py` & `zetascale-2.5.1/zeta/nn/modules/multi_scale_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/nebula.py` & `zetascale-2.5.1/zeta/nn/modules/nebula.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/nfn_stem.py` & `zetascale-2.5.1/zeta/nn/modules/nfn_stem.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/norm_fractorals.py` & `zetascale-2.5.1/zeta/nn/modules/norm_fractorals.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/norm_utils.py` & `zetascale-2.5.1/zeta/nn/modules/norm_utils.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/omnimodal_fusion.py` & `zetascale-2.5.1/zeta/nn/modules/omnimodal_fusion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/p_scan.py` & `zetascale-2.5.1/zeta/nn/modules/p_scan.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/palo_ldp.py` & `zetascale-2.5.1/zeta/nn/modules/palo_ldp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/parallel_wrapper.py` & `zetascale-2.5.1/zeta/nn/modules/parallel_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/patch_linear_flatten.py` & `zetascale-2.5.1/zeta/nn/modules/patch_linear_flatten.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/patch_video.py` & `zetascale-2.5.1/zeta/nn/modules/patch_video.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/peg.py` & `zetascale-2.5.1/zeta/nn/modules/peg.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/perceiver_layer.py` & `zetascale-2.5.1/zeta/nn/modules/perceiver_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/perceiver_resampler.py` & `zetascale-2.5.1/zeta/nn/modules/perceiver_resampler.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/pixel_shuffling.py` & `zetascale-2.5.1/zeta/nn/modules/pixel_shuffling.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/poly_expert_fusion_network.py` & `zetascale-2.5.1/zeta/nn/modules/poly_expert_fusion_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/polymorphic_activation.py` & `zetascale-2.5.1/zeta/nn/modules/polymorphic_activation.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/polymorphic_neuron.py` & `zetascale-2.5.1/zeta/nn/modules/polymorphic_neuron.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/prenorm.py` & `zetascale-2.5.1/zeta/nn/modules/prenorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/proj_then_softmax.py` & `zetascale-2.5.1/zeta/nn/modules/proj_then_softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/pulsar.py` & `zetascale-2.5.1/zeta/nn/modules/pulsar.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/pyro.py` & `zetascale-2.5.1/zeta/nn/modules/pyro.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/qformer.py` & `zetascale-2.5.1/zeta/nn/modules/qformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/qkv_norm.py` & `zetascale-2.5.1/zeta/nn/modules/qkv_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/quantized_layernorm.py` & `zetascale-2.5.1/zeta/nn/modules/quantized_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/query_proposal.py` & `zetascale-2.5.1/zeta/nn/modules/query_proposal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/recurrent_model.py` & `zetascale-2.5.1/zeta/nn/modules/recurrent_model.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/recursive_block.py` & `zetascale-2.5.1/zeta/nn/modules/recursive_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/res_net.py` & `zetascale-2.5.1/zeta/nn/modules/res_net.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/resnet.py` & `zetascale-2.5.1/zeta/nn/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/return_loss_text.py` & `zetascale-2.5.1/zeta/nn/modules/return_loss_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/rms_norm.py` & `zetascale-2.5.1/zeta/nn/modules/rms_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/rnn_nlp.py` & `zetascale-2.5.1/zeta/nn/modules/rnn_nlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/s4.py` & `zetascale-2.5.1/zeta/nn/modules/s4.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/scale.py` & `zetascale-2.5.1/zeta/nn/modules/scale.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/scale_norm.py` & `zetascale-2.5.1/zeta/nn/modules/scale_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/scaled_sinusoidal.py` & `zetascale-2.5.1/zeta/nn/modules/scaled_sinusoidal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/scalenorm.py` & `zetascale-2.5.1/zeta/nn/modules/scalenorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/shift_tokens.py` & `zetascale-2.5.1/zeta/nn/modules/shift_tokens.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/shufflenet.py` & `zetascale-2.5.1/zeta/nn/modules/shufflenet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/sig_lip.py` & `zetascale-2.5.1/zeta/nn/modules/sig_lip.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/simple_feedforward.py` & `zetascale-2.5.1/zeta/nn/modules/simple_feedforward.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/simple_mamba.py` & `zetascale-2.5.1/zeta/nn/modules/simple_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/simple_res_block.py` & `zetascale-2.5.1/zeta/nn/modules/simple_res_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/simple_resblock.py` & `zetascale-2.5.1/zeta/nn/modules/simple_resblock.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/simple_rmsnorm.py` & `zetascale-2.5.1/zeta/nn/modules/simple_rmsnorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/skipconnection.py` & `zetascale-2.5.1/zeta/nn/modules/skipconnection.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/slerp_model_merger.py` & `zetascale-2.5.1/zeta/nn/modules/slerp_model_merger.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/sp_act.py` & `zetascale-2.5.1/zeta/nn/modules/sp_act.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/space_time_unet.py` & `zetascale-2.5.1/zeta/nn/modules/space_time_unet.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,19 @@
         return h + self.res_conv(x)
 
 
 # pixelshuffle upsamples and downsamples
 # where time dimension can be configured
 class Downsample(nn.Module):
     def __init__(
-        self, dim, downsample_space=True, downsample_time=False, nonlin=False
+        self,
+        dim: int,
+        downsample_space: bool = True,
+        downsample_time=False,
+        nonlin=False,
     ):
         super().__init__()
         assert downsample_space or downsample_time
 
         self.down_space = (
             nn.Sequential(
                 Rearrange("b c (h p1) (w p2) -> b (c p1 p2) h w", p1=2, p2=2),
```

### Comparing `zetascale-2.4.8/zeta/nn/modules/spacial_transformer.py` & `zetascale-2.5.1/zeta/nn/modules/spacial_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/sparq_attn.py` & `zetascale-2.5.1/zeta/nn/modules/sparq_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/sparse_moe.py` & `zetascale-2.5.1/zeta/nn/modules/sparse_moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/spatial_downsample.py` & `zetascale-2.5.1/zeta/nn/modules/spatial_downsample.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/spatial_transformer.py` & `zetascale-2.5.1/zeta/nn/modules/spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/splines.py` & `zetascale-2.5.1/zeta/nn/modules/splines.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/squeeze_excitation.py` & `zetascale-2.5.1/zeta/nn/modules/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/ssm.py` & `zetascale-2.5.1/zeta/nn/modules/ssm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/ssm_language.py` & `zetascale-2.5.1/zeta/nn/modules/ssm_language.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/stoch_depth.py` & `zetascale-2.5.1/zeta/nn/modules/stoch_depth.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/stochastic_depth.py` & `zetascale-2.5.1/zeta/nn/modules/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/subln.py` & `zetascale-2.5.1/zeta/nn/modules/subln.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/super_resolution.py` & `zetascale-2.5.1/zeta/nn/modules/super_resolution.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/swarmalator.py` & `zetascale-2.5.1/zeta/nn/modules/swarmalator.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,15 @@
     mask = (dists < R).float() - torch.eye(N)
 
     interaction_term = mask.unsqueeze(2) * (xi.unsqueeze(0) - xi.unsqueeze(1))
     interaction_sum = interaction_term.sum(1)
 
     # Define dynamics for sigma based on our assumptions
     d_sigma = (
-        gamma * interaction_sum
-        + epsilon_a * sigma_i
-        - epsilon_r * (sigma_i**3)
+        gamma * interaction_sum + epsilon_a * sigma_i - epsilon_r * (sigma_i**3)
     )
     return d_sigma
 
 
 def simulate_swarmalators(
     N, J, alpha, beta, gamma, epsilon_a, epsilon_r, R, D, T=100, dt=0.1
 ):
```

### Comparing `zetascale-2.4.8/zeta/nn/modules/swiglu.py` & `zetascale-2.5.1/zeta/nn/modules/swiglu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/tensor.py` & `zetascale-2.5.1/zeta/nn/modules/tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/tensor_to_int.py` & `zetascale-2.5.1/zeta/nn/modules/tensor_to_int.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/text_scene_fusion.py` & `zetascale-2.5.1/zeta/nn/modules/text_scene_fusion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/text_video_fuse.py` & `zetascale-2.5.1/zeta/nn/modules/text_video_fuse.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/time_up_sample.py` & `zetascale-2.5.1/zeta/nn/modules/time_up_sample.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/to_logits.py` & `zetascale-2.5.1/zeta/nn/modules/to_logits.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/token_learner.py` & `zetascale-2.5.1/zeta/nn/modules/token_learner.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/token_mixer.py` & `zetascale-2.5.1/zeta/nn/modules/token_mixer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/top_n_gating.py` & `zetascale-2.5.1/zeta/nn/modules/top_n_gating.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/transformations.py` & `zetascale-2.5.1/zeta/nn/modules/transformations.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/triple_skip.py` & `zetascale-2.5.1/zeta/nn/modules/triple_skip.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/triton_rmsnorm.py` & `zetascale-2.5.1/zeta/nn/modules/triton_rmsnorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/u_mamba.py` & `zetascale-2.5.1/zeta/nn/modules/u_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/unet.py` & `zetascale-2.5.1/zeta/nn/modules/unet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/v_layernorm.py` & `zetascale-2.5.1/zeta/nn/modules/v_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/v_pool.py` & `zetascale-2.5.1/zeta/nn/modules/v_pool.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/video_autoencoder.py` & `zetascale-2.5.1/zeta/nn/modules/video_autoencoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/video_diffusion_modules.py` & `zetascale-2.5.1/zeta/nn/modules/video_diffusion_modules.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/video_to_tensor.py` & `zetascale-2.5.1/zeta/nn/modules/video_to_tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/video_to_text.py` & `zetascale-2.5.1/zeta/nn/modules/video_to_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/vision_mamba.py` & `zetascale-2.5.1/zeta/nn/modules/vision_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/vision_weighted_permute_mlp.py` & `zetascale-2.5.1/zeta/nn/modules/vision_weighted_permute_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/visual_expert.py` & `zetascale-2.5.1/zeta/nn/modules/visual_expert.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/vit_denoiser.py` & `zetascale-2.5.1/zeta/nn/modules/vit_denoiser.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             "b c (h p1) (w p2) -> b (h w) (p1 p2 c)",
             p1=patch_size,
             p2=patch_size,
         ),
         nn.LayerNorm(patch_dim),
         nn.Linear(patch_dim, dim),
         nn.LayerNorm(dim),
-    )
+    )(x)
 
 
 def posemb_sincos_2d(
     patches,
     temperature: int = 10000,
     dtype=torch.float32,
 ):
```

### Comparing `zetascale-2.4.8/zeta/nn/modules/vss_block.py` & `zetascale-2.5.1/zeta/nn/modules/vss_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/ws_conv2d.py` & `zetascale-2.5.1/zeta/nn/modules/ws_conv2d.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/xmoe/global_groups.py` & `zetascale-2.5.1/zeta/nn/modules/xmoe/global_groups.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/xmoe/moe_layer.py` & `zetascale-2.5.1/zeta/nn/modules/xmoe/moe_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/xmoe/routing.py` & `zetascale-2.5.1/zeta/nn/modules/xmoe/routing.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/nn/modules/yolo.py` & `zetascale-2.5.1/zeta/nn/modules/yolo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/__init__.py` & `zetascale-2.5.1/zeta/ops/__Init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/async_softmax.py` & `zetascale-2.5.1/zeta/ops/async_softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/dilated_attn_ops.py` & `zetascale-2.5.1/zeta/ops/dilated_attn_ops.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/einops_from_to.py` & `zetascale-2.5.1/zeta/ops/einops_from_to.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/einops_poly.py` & `zetascale-2.5.1/zeta/ops/einops_poly.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/expand.py` & `zetascale-2.5.1/zeta/ops/expand.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/laplace.py` & `zetascale-2.5.1/zeta/ops/laplace.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/main.py` & `zetascale-2.5.1/zeta/ops/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,15 @@
             logging.warning(
                 "Newton did not converge and reached maximum number of"
                 " iterations!"
             )
     else:
         raise NotImplementedError(
             "Root inverse method is not implemented! Specified root inverse"
-            " method is "
-            + str(root_inv_method)
-            + "."
+            " method is " + str(root_inv_method) + "."
         )
 
     return X
 
 
 def matrix_root_diagonal(
     A: Tensor,
```

### Comparing `zetascale-2.4.8/zeta/ops/misc_act.py` & `zetascale-2.5.1/zeta/ops/misc_act.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/mm_rearranges.py` & `zetascale-2.5.1/zeta/ops/mm_rearranges.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/mm_softmax.py` & `zetascale-2.5.1/zeta/ops/mm_softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/mos.py` & `zetascale-2.5.1/zeta/ops/mos.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/nonlinear.py` & `zetascale-2.5.1/zeta/ops/nonlinear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/softmax.py` & `zetascale-2.5.1/zeta/ops/softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/ops/sparsemax.py` & `zetascale-2.5.1/zeta/ops/sparsemax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/optim/__init__.py` & `zetascale-2.5.1/zeta/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/optim/batched_optimizer.py` & `zetascale-2.5.1/zeta/optim/batched_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,17 +321,15 @@
         for p, state, param_names in tuples:
             grad = p.grad
             if grad.is_sparse:
                 raise RuntimeError(
                     "ScaledAdam optimizer does not support sparse gradients"
                 )
             if p.numel() == p.shape[0]:  # a batch of scalars
-                tot_sumsq += (
-                    grad**2
-                ).sum()  # sum() to change shape [1] to []
+                tot_sumsq += (grad**2).sum()  # sum() to change shape [1] to []
             else:
                 tot_sumsq += ((grad * state["param_rms"]) ** 2).sum()
 
         tot_norm = tot_sumsq.sqrt()
         if "model_norms" not in first_state:
             first_state["model_norms"] = torch.zeros(
                 clipping_update_period, device=p.device
@@ -486,17 +484,15 @@
             scale_grads = state["scale_grads"]
             scale_grads[step % size_update_period] = (p * grad).sum(
                 dim=list(range(1, p.ndim)), keepdim=True
             )
             if step % size_update_period == size_update_period - 1:
                 param_rms = state["param_rms"]  # shape: (batch_size, 1, 1, ..)
                 param_rms.copy_(
-                    (p**2)
-                    .mean(dim=list(range(1, p.ndim)), keepdim=True)
-                    .sqrt()
+                    (p**2).mean(dim=list(range(1, p.ndim)), keepdim=True).sqrt()
                 )
                 if step > 0:
                     # self._size_update() learns the overall scale on the
                     # parameter, by shrinking or expanding it.
                     self._size_update(group, scale_grads, p, state)
 
         if numel == 1:
@@ -539,33 +535,28 @@
         # faster decay at this level.
         beta2_corr = beta2**size_update_period
 
         scale_exp_avg_sq = state[
             "scale_exp_avg_sq"
         ]  # shape: (batch_size, 1, 1, ..)
         scale_exp_avg_sq.mul_(beta2_corr).add_(
-            (scale_grads**2).mean(
-                dim=0
-            ),  # mean over dim `size_update_period`
+            (scale_grads**2).mean(dim=0),  # mean over dim `size_update_period`
             alpha=1 - beta2_corr,
         )  # shape is (batch_size, 1, 1, ...)
 
         # The 1st time we reach here is when size_step == 1.
         size_step = (step + 1) // size_update_period
         bias_correction2 = 1 - beta2_corr**size_step
         # we don't bother with bias_correction1; this will help prevent divergence
         # at the start of training.
 
         denom = scale_exp_avg_sq.sqrt() + eps
 
         scale_step = (
-            -size_lr
-            * (bias_correction2**0.5)
-            * scale_grads.sum(dim=0)
-            / denom
+            -size_lr * (bias_correction2**0.5) * scale_grads.sum(dim=0) / denom
         )
 
         is_too_small = param_rms < param_min_rms
         is_too_large = param_rms > param_max_rms
 
         # when the param gets too small, just don't shrink it any further.
         scale_step.masked_fill_(is_too_small, 0.0)
@@ -769,16 +760,15 @@
         self.lr_epochs = lr_epochs
         self.warmup_batches = warmup_batches
 
     def get_lr(self):
         factor = (
             (self.batch**2 + self.lr_batches**2) / self.lr_batches**2
         ) ** -0.25 * (
-            ((self.epoch**2 + self.lr_epochs**2) / self.lr_epochs**2)
-            ** -0.25
+            ((self.epoch**2 + self.lr_epochs**2) / self.lr_epochs**2) ** -0.25
         )
         warmup_factor = (
             1.0
             if self.batch >= self.warmup_batches
             else 0.5 + 0.5 * (self.batch / self.warmup_batches)
         )
```

### Comparing `zetascale-2.4.8/zeta/optim/decoupled_lion.py` & `zetascale-2.5.1/zeta/optim/decoupled_lion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/optim/decoupled_optimizer.py` & `zetascale-2.5.1/zeta/optim/decoupled_optimizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/optim/decoupled_sophia.py` & `zetascale-2.5.1/zeta/optim/decoupled_sophia.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/optim/gradient_ascent.py` & `zetascale-2.5.1/zeta/optim/gradient_ascent.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/optim/gradient_equillibrum.py` & `zetascale-2.5.1/zeta/optim/gradient_equillibrum.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/optim/lion8b.py` & `zetascale-2.5.1/zeta/optim/lion8b.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/optim/parallel_gradient_descent.py` & `zetascale-2.5.1/zeta/optim/parallel_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/optim/stable_adam.py` & `zetascale-2.5.1/zeta/optim/stable_adam.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,20 +93,16 @@
                 if "exp_avg" not in param_state:
                     v = param_state["exp_avg"] = torch.zeros_like(theta)
                     u = param_state["exp_avg_sq"] = torch.zeros_like(theta)
                 else:
                     v = param_state["exp_avg"]
                     u = param_state["exp_avg_sq"]
 
-                beta1hat = (
-                    beta1 * (1 - beta1 ** (step - 1)) / (1 - beta1**step)
-                )
-                beta2hat = (
-                    beta2 * (1 - beta2 ** (step - 1)) / (1 - beta2**step)
-                )
+                beta1hat = beta1 * (1 - beta1 ** (step - 1)) / (1 - beta1**step)
+                beta2hat = beta2 * (1 - beta2 ** (step - 1)) / (1 - beta2**step)
 
                 v = v.mul_(beta1hat).add_(g, alpha=1.0 - beta1hat)
                 u = u.mul_(beta2hat).addcmul_(g, g, value=1.0 - beta2hat)
 
                 denominator = u.sqrt().add_(self.eps)
 
                 rms = (
```

### Comparing `zetascale-2.4.8/zeta/quant/bitlinear.py` & `zetascale-2.5.1/zeta/quant/bitlinear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/quant/half_bit_linear.py` & `zetascale-2.5.1/zeta/quant/half_bit_linear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/quant/lfq.py` & `zetascale-2.5.1/zeta/quant/lfq.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/quant/niva.py` & `zetascale-2.5.1/zeta/quant/niva.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/quant/qlora.py` & `zetascale-2.5.1/zeta/quant/qlora.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/quant/qmoe.py` & `zetascale-2.5.1/zeta/quant/qmoe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/quant/quick.py` & `zetascale-2.5.1/zeta/quant/quick.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/quant/residual_vq.py` & `zetascale-2.5.1/zeta/quant/residual_vq.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/quant/ste.py` & `zetascale-2.5.1/zeta/quant/ste.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/__init__.py` & `zetascale-2.5.1/zeta/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/actor_critic.py` & `zetascale-2.5.1/zeta/rl/actor_critic.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/dpo.py` & `zetascale-2.5.1/zeta/rl/dpo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/hindsight_replay.py` & `zetascale-2.5.1/zeta/rl/hindsight_replay.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/language_reward.py` & `zetascale-2.5.1/zeta/rl/language_reward.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/ppo.py` & `zetascale-2.5.1/zeta/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/priortized_replay_buffer.py` & `zetascale-2.5.1/zeta/rl/priortized_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/priortized_rps.py` & `zetascale-2.5.1/zeta/rl/priortized_rps.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/reward_model.py` & `zetascale-2.5.1/zeta/rl/reward_model.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/sumtree.py` & `zetascale-2.5.1/zeta/rl/sumtree.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/rl/vision_model_rl.py` & `zetascale-2.5.1/zeta/rl/vision_model_rl.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/__init__.py` & `zetascale-2.5.1/zeta/structs/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/auto_regressive_wrapper.py` & `zetascale-2.5.1/zeta/structs/auto_regressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/clip_encoder.py` & `zetascale-2.5.1/zeta/structs/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/efficient_net.py` & `zetascale-2.5.1/zeta/structs/efficient_net.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/encoder_decoder.py` & `zetascale-2.5.1/zeta/structs/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/hierarchical_transformer.py` & `zetascale-2.5.1/zeta/structs/hierarchical_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/local_transformer.py` & `zetascale-2.5.1/zeta/structs/local_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/multi_modal_projector.py` & `zetascale-2.5.1/zeta/structs/multi_modal_projector.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/simple_transformer.py` & `zetascale-2.5.1/zeta/structs/simple_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/simple_vision_encoder.py` & `zetascale-2.5.1/zeta/structs/simple_vision_encoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/transformer.py` & `zetascale-2.5.1/zeta/structs/transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/structs/transformer_block.py` & `zetascale-2.5.1/zeta/structs/transformer_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/tokenizers/gptx_tokenizer.py` & `zetascale-2.5.1/zeta/tokenizers/gptx_tokenizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/tokenizers/llama_sentencepiece.py` & `zetascale-2.5.1/zeta/tokenizers/llama_sentencepiece.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/tokenizers/multi_modal_tokenizer.py` & `zetascale-2.5.1/zeta/tokenizers/multi_modal_tokenizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/tokenizers/sentence_piece.py` & `zetascale-2.5.1/zeta/tokenizers/sentence_piece.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/tokenizers/tokenmonster.py` & `zetascale-2.5.1/zeta/tokenizers/tokenmonster.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/training/activation_checkpoint.py` & `zetascale-2.5.1/zeta/training/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/training/dataloader.py` & `zetascale-2.5.1/zeta/training/dataloader.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/training/fsdp.py` & `zetascale-2.5.1/zeta/training/fsdp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/training/galore.py` & `zetascale-2.5.1/zeta/training/galore.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/training/hive_trainer.py` & `zetascale-2.5.1/zeta/training/hive_trainer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/training/parallel_wrapper.py` & `zetascale-2.5.1/zeta/training/parallel_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/training/scheduler.py` & `zetascale-2.5.1/zeta/training/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,10 +45,11 @@
         return get_cosine_schedule_with_warmup(
             optimizer=optimizer,
             num_warmup_steps=NUM_WARMUP_STEPS * GRADIENT_ACCUMULATE_EVERY,
             num_training_steps=max_train_steps * GRADIENT_ACCUMULATE_EVERY,
         )
     else:
         raise ValueError(
-            "Invalid scheduler_type. Expected 'linear' or 'cosine', got: {}"
-            .format(scheduler_type)
+            "Invalid scheduler_type. Expected 'linear' or 'cosine', got: {}".format(
+                scheduler_type
+            )
         )
```

### Comparing `zetascale-2.4.8/zeta/training/train.py` & `zetascale-2.5.1/zeta/training/train.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/__init__.py` & `zetascale-2.5.1/zeta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/benchmark.py` & `zetascale-2.5.1/zeta/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/cuda_memory_wrapper.py` & `zetascale-2.5.1/zeta/utils/cuda_memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/cuda_wrapper.py` & `zetascale-2.5.1/zeta/utils/cuda_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/disable_logging.py` & `zetascale-2.5.1/zeta/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/enforce_types.py` & `zetascale-2.5.1/zeta/utils/enforce_types.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/img_to_tensor.py` & `zetascale-2.5.1/zeta/utils/img_to_tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/log_pytorch_op.py` & `zetascale-2.5.1/zeta/utils/log_pytorch_op.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/main.py` & `zetascale-2.5.1/zeta/utils/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/module_device.py` & `zetascale-2.5.1/zeta/utils/module_device.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/params.py` & `zetascale-2.5.1/zeta/utils/params.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/save_load_wrapper.py` & `zetascale-2.5.1/zeta/utils/save_load_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/text_to_tensor.py` & `zetascale-2.5.1/zeta/utils/text_to_tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/verbose_execution.py` & `zetascale-2.5.1/zeta/utils/verbose_execution.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/zeta/utils/vision_utils.py` & `zetascale-2.5.1/zeta/utils/vision_utils.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.4.8/setup.py` & `zetascale-2.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,1400 +1,1341 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 277a 6574 6127 2c0a 2027 7a65   \.['zeta',. 'ze
-00000050: 7461 2e63 6c69 272c 0a20 277a 6574 612e  ta.cli',. 'zeta.
-00000060: 636c 6f75 6427 2c0a 2027 7a65 7461 2e65  cloud',. 'zeta.e
-00000070: 7870 6572 696d 656e 7461 6c27 2c0a 2027  xperimental',. '
-00000080: 7a65 7461 2e65 7870 6572 696d 656e 7461  zeta.experimenta
-00000090: 6c2e 7472 6974 6f6e 272c 0a20 277a 6574  l.triton',. 'zet
-000000a0: 612e 6578 7065 7269 6d65 6e74 616c 2e74  a.experimental.t
-000000b0: 7269 746f 6e2e 6163 7469 7661 7469 6f6e  riton.activation
-000000c0: 7327 2c0a 2027 7a65 7461 2e65 7870 6572  s',. 'zeta.exper
-000000d0: 696d 656e 7461 6c2e 7472 6974 6f6e 2e74  imental.triton.t
-000000e0: 7269 746f 6e5f 6d6f 6475 6c65 7327 2c0a  riton_modules',.
-000000f0: 2027 7a65 7461 2e6d 6f64 656c 7327 2c0a   'zeta.models',.
-00000100: 2027 7a65 7461 2e6e 6e27 2c0a 2027 7a65   'zeta.nn',. 'ze
-00000110: 7461 2e6e 6e2e 6174 7465 6e74 696f 6e27  ta.nn.attention'
-00000120: 2c0a 2027 7a65 7461 2e6e 6e2e 6269 6173  ,. 'zeta.nn.bias
-00000130: 6573 272c 0a20 277a 6574 612e 6e6e 2e65  es',. 'zeta.nn.e
-00000140: 6d62 6564 6469 6e67 7327 2c0a 2027 7a65  mbeddings',. 'ze
-00000150: 7461 2e6e 6e2e 6d61 736b 7327 2c0a 2027  ta.nn.masks',. '
-00000160: 7a65 7461 2e6e 6e2e 6d6f 6475 6c65 7327  zeta.nn.modules'
-00000170: 2c0a 2027 7a65 7461 2e6e 6e2e 6d6f 6475  ,. 'zeta.nn.modu
-00000180: 6c65 732e 786d 6f65 272c 0a20 277a 6574  les.xmoe',. 'zet
-00000190: 612e 6f70 7327 2c0a 2027 7a65 7461 2e6f  a.ops',. 'zeta.o
-000001a0: 7074 696d 272c 0a20 277a 6574 612e 7175  ptim',. 'zeta.qu
-000001b0: 616e 7427 2c0a 2027 7a65 7461 2e72 6c27  ant',. 'zeta.rl'
-000001c0: 2c0a 2027 7a65 7461 2e73 7472 7563 7473  ,. 'zeta.structs
-000001d0: 272c 0a20 277a 6574 612e 746f 6b65 6e69  ',. 'zeta.tokeni
-000001e0: 7a65 7273 272c 0a20 277a 6574 612e 7472  zers',. 'zeta.tr
-000001f0: 6169 6e69 6e67 272c 0a20 277a 6574 612e  aining',. 'zeta.
-00000200: 7574 696c 7327 5d0a 0a70 6163 6b61 6765  utils']..package
-00000210: 5f64 6174 6120 3d20 5c0a 7b27 273a 205b  _data = \.{'': [
-00000220: 272a 275d 7d0a 0a69 6e73 7461 6c6c 5f72  '*']}..install_r
-00000230: 6571 7569 7265 7320 3d20 5c0a 5b27 6163  equires = \.['ac
-00000240: 6365 6c65 7261 7465 3d3d 302e 3238 2e30  celerate==0.28.0
-00000250: 272c 0a20 2761 7267 7061 7273 653e 3d31  ',. 'argparse>=1
-00000260: 2e34 2e30 2c3c 322e 302e 3027 2c0a 2027  .4.0,<2.0.0',. '
-00000270: 6265 6172 7479 7065 3d3d 302e 3137 2e32  beartype==0.17.2
-00000280: 272c 0a20 2762 6974 7361 6e64 6279 7465  ',. 'bitsandbyte
-00000290: 733d 3d30 2e34 332e 3027 2c0a 2027 636f  s==0.43.0',. 'co
-000002a0: 6c74 352d 6174 7465 6e74 696f 6e27 2c0a  lt5-attention',.
-000002b0: 2027 6461 7461 7365 7473 272c 0a20 2765   'datasets',. 'e
-000002c0: 696e 6f70 732d 6578 7473 3d3d 302e 302e  inops-exts==0.0.
-000002d0: 3427 2c0a 2027 6569 6e6f 7073 3d3d 302e  4',. 'einops==0.
-000002e0: 372e 3027 2c0a 2027 6c6f 6361 6c2d 6174  7.0',. 'local-at
-000002f0: 7465 6e74 696f 6e27 2c0a 2027 6c6f 6775  tention',. 'logu
-00000300: 7275 272c 0a20 2770 7974 6573 743d 3d38  ru',. 'pytest==8
-00000310: 2e31 2e31 272c 0a20 2772 6963 683d 3d31  .1.1',. 'rich==1
-00000320: 332e 372e 3127 2c0a 2027 7363 6970 793d  3.7.1',. 'scipy=
-00000330: 3d31 2e39 2e33 272c 0a20 2774 6f72 6368  =1.9.3',. 'torch
-00000340: 3e3d 322e 312e 312c 3c33 2e30 272c 0a20  >=2.1.1,<3.0',. 
-00000350: 2774 6f72 6368 6669 7827 2c0a 2027 746f  'torchfix',. 'to
-00000360: 7263 6876 6973 696f 6e3d 3d30 2e31 382e  rchvision==0.18.
-00000370: 3027 2c0a 2027 7471 646d 3d3d 342e 3636  0',. 'tqdm==4.66
-00000380: 2e33 272c 0a20 2774 7261 6e73 666f 726d  .3',. 'transform
-00000390: 6572 733d 3d34 2e34 302e 3127 2c0a 2027  ers==4.40.1',. '
-000003a0: 7665 6374 6f72 2d71 7561 6e74 697a 652d  vector-quantize-
-000003b0: 7079 746f 7263 683d 3d31 2e31 342e 3727  pytorch==1.14.7'
-000003c0: 5d0a 0a65 6e74 7279 5f70 6f69 6e74 7320  ]..entry_points 
-000003d0: 3d20 5c0a 7b27 636f 6e73 6f6c 655f 7363  = \.{'console_sc
-000003e0: 7269 7074 7327 3a20 5b27 7a65 7461 203d  ripts': ['zeta =
-000003f0: 207a 6574 612e 636c 692e 6d61 696e 3a6d   zeta.cli.main:m
-00000400: 6169 6e27 5d7d 0a0a 7365 7475 705f 6b77  ain']}..setup_kw
-00000410: 6172 6773 203d 207b 0a20 2020 2027 6e61  args = {.    'na
-00000420: 6d65 273a 2027 7a65 7461 7363 616c 6527  me': 'zetascale'
-00000430: 2c0a 2020 2020 2776 6572 7369 6f6e 273a  ,.    'version':
-00000440: 2027 322e 342e 3827 2c0a 2020 2020 2764   '2.4.8',.    'd
-00000450: 6573 6372 6970 7469 6f6e 273a 2027 5261  escription': 'Ra
-00000460: 7069 646c 7920 4275 696c 642c 204f 7074  pidly Build, Opt
-00000470: 696d 697a 652c 2061 6e64 2044 6570 6c6f  imize, and Deplo
-00000480: 7920 534f 5441 2041 4920 4d6f 6465 6c73  y SOTA AI Models
-00000490: 272c 0a20 2020 2027 6c6f 6e67 5f64 6573  ',.    'long_des
-000004a0: 6372 6970 7469 6f6e 273a 2027 5b21 5b4d  cription': '[![M
-000004b0: 756c 7469 2d4d 6f64 616c 6974 795d 2869  ulti-Modality](i
-000004c0: 6d61 6765 732f 6167 6f72 6162 616e 6e65  mages/agorabanne
-000004d0: 722e 706e 6729 5d28 6874 7470 733a 2f2f  r.png)](https://
-000004e0: 6469 7363 6f72 642e 6767 2f71 5574 786e  discord.gg/qUtxn
-000004f0: 4b32 4e4d 6629 5c6e 5c6e 215b 5a65 7461  K2NMf)\n\n![Zeta
-00000500: 2062 616e 6e65 725d 2869 6d61 6765 732f   banner](images/
-00000510: 7a65 7461 2e70 6e67 295c 6e42 7569 6c64  zeta.png)\nBuild
-00000520: 2053 4f54 4120 4149 204d 6f64 656c 7320   SOTA AI Models 
-00000530: 3830 2520 6661 7374 6572 2077 6974 6820  80% faster with 
-00000540: 6d6f 6475 6c61 722c 2068 6967 682d 7065  modular, high-pe
-00000550: 7266 6f72 6d61 6e63 652c 2061 6e64 2073  rformance, and s
-00000560: 6361 6c61 626c 6520 6275 696c 6469 6e67  calable building
-00000570: 2062 6c6f 636b 7321 5c6e 5c6e 5b21 5b44   blocks!\n\n[![D
-00000580: 6f63 735d 2868 7474 7073 3a2f 2f72 6561  ocs](https://rea
-00000590: 6474 6865 646f 6373 2e6f 7267 2f70 726f  dthedocs.org/pro
-000005a0: 6a65 6374 732f 7a65 7461 2f62 6164 6765  jects/zeta/badge
-000005b0: 2f29 5d28 6874 7470 733a 2f2f 7a65 7461  /)](https://zeta
-000005c0: 2e72 6561 6474 6865 646f 6373 2e69 6f29  .readthedocs.io)
-000005d0: 5c6e 5c6e 3c70 3e5c 6e20 203c 6120 6872  \n\n<p>\n  <a hr
-000005e0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000005f0: 7562 2e63 6f6d 2f6b 7965 676f 6d65 7a2f  ub.com/kyegomez/
-00000600: 7a65 7461 2f62 6c6f 622f 6d61 696e 2f4c  zeta/blob/main/L
-00000610: 4943 454e 5345 223e 3c69 6d67 2061 6c74  ICENSE"><img alt
-00000620: 3d22 4d49 5420 4c69 6365 6e73 6522 2073  ="MIT License" s
-00000630: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000640: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000650: 2f6c 6963 656e 7365 2d4d 4954 2d62 6c75  /license-MIT-blu
-00000660: 652e 7376 6722 202f 3e3c 2f61 3e5c 6e20  e.svg" /></a>\n 
-00000670: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000680: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000690: 6374 2f7a 6574 6173 6361 6c65 223e 3c69  ct/zetascale"><i
-000006a0: 6d67 2061 6c74 3d22 4d49 5420 4c69 6365  mg alt="MIT Lice
-000006b0: 6e73 6522 2073 7263 3d22 6874 7470 733a  nse" src="https:
-000006c0: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
-000006d0: 7079 2f7a 6574 6173 6361 6c65 2e73 7667  py/zetascale.svg
-000006e0: 2220 2f3e 3c2f 613e 5c6e 3c2f 703e 5c6e  " /></a>\n</p>\n
-000006f0: 5c6e 5b21 5b47 6974 4875 6220 6973 7375  \n[![GitHub issu
-00000700: 6573 5d28 6874 7470 733a 2f2f 696d 672e  es](https://img.
-00000710: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000720: 622f 6973 7375 6573 2f6b 7965 676f 6d65  b/issues/kyegome
-00000730: 7a2f 7a65 7461 295d 2868 7474 7073 3a2f  z/zeta)](https:/
-00000740: 2f67 6974 6875 622e 636f 6d2f 6b79 6567  /github.com/kyeg
-00000750: 6f6d 657a 2f7a 6574 612f 6973 7375 6573  omez/zeta/issues
-00000760: 2920 5b21 5b47 6974 4875 6220 666f 726b  ) [![GitHub fork
-00000770: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
-00000780: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000790: 2f66 6f72 6b73 2f6b 7965 676f 6d65 7a2f  /forks/kyegomez/
-000007a0: 7a65 7461 295d 2868 7474 7073 3a2f 2f67  zeta)](https://g
-000007b0: 6974 6875 622e 636f 6d2f 6b79 6567 6f6d  ithub.com/kyegom
-000007c0: 657a 2f7a 6574 612f 6e65 7477 6f72 6b29  ez/zeta/network)
-000007d0: 205b 215b 4769 7448 7562 2073 7461 7273   [![GitHub stars
-000007e0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000007f0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000800: 7374 6172 732f 6b79 6567 6f6d 657a 2f7a  stars/kyegomez/z
-00000810: 6574 6129 5d28 6874 7470 733a 2f2f 6769  eta)](https://gi
-00000820: 7468 7562 2e63 6f6d 2f6b 7965 676f 6d65  thub.com/kyegome
-00000830: 7a2f 7a65 7461 2f73 7461 7267 617a 6572  z/zeta/stargazer
-00000840: 7329 205b 215b 4769 7448 7562 206c 6963  s) [![GitHub lic
-00000850: 656e 7365 5d28 6874 7470 733a 2f2f 696d  ense](https://im
-00000860: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00000870: 6875 622f 6c69 6365 6e73 652f 6b79 6567  hub/license/kyeg
-00000880: 6f6d 657a 2f7a 6574 6129 5d28 6874 7470  omez/zeta)](http
-00000890: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-000008a0: 7965 676f 6d65 7a2f 7a65 7461 2f62 6c6f  yegomez/zeta/blo
-000008b0: 622f 6d61 696e 2f4c 4943 454e 5345 295b  b/main/LICENSE)[
-000008c0: 215b 4769 7448 7562 2073 7461 7220 6368  ![GitHub star ch
-000008d0: 6172 745d 2868 7474 7073 3a2f 2f69 6d67  art](https://img
-000008e0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-000008f0: 7562 2f73 7461 7273 2f6b 7965 676f 6d65  ub/stars/kyegome
-00000900: 7a2f 7a65 7461 3f73 7479 6c65 3d73 6f63  z/zeta?style=soc
-00000910: 6961 6c29 5d28 6874 7470 733a 2f2f 7374  ial)](https://st
-00000920: 6172 2d68 6973 746f 7279 2e63 6f6d 2f23  ar-history.com/#
-00000930: 6b79 6567 6f6d 657a 2f7a 6574 6129 5b21  kyegomez/zeta)[!
-00000940: 5b44 6570 656e 6465 6e63 7920 5374 6174  [Dependency Stat
-00000950: 7573 5d28 6874 7470 733a 2f2f 696d 672e  us](https://img.
-00000960: 7368 6965 6c64 732e 696f 2f6c 6962 7261  shields.io/libra
-00000970: 7269 6573 696f 2f67 6974 6875 622f 6b79  riesio/github/ky
-00000980: 6567 6f6d 657a 2f7a 6574 6129 5d28 6874  egomez/zeta)](ht
-00000990: 7470 733a 2f2f 6c69 6272 6172 6965 732e  tps://libraries.
-000009a0: 696f 2f67 6974 6875 622f 6b79 6567 6f6d  io/github/kyegom
-000009b0: 657a 2f7a 6574 6129 205b 215b 446f 776e  ez/zeta) [![Down
-000009c0: 6c6f 6164 735d 2868 7474 7073 3a2f 2f73  loads](https://s
-000009d0: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
-000009e0: 6261 6467 652f 7a65 7461 2f6d 6f6e 7468  badge/zeta/month
-000009f0: 295d 2868 7474 7073 3a2f 2f70 6570 792e  )](https://pepy.
-00000a00: 7465 6368 2f70 726f 6a65 6374 2f7a 6574  tech/project/zet
-00000a10: 6129 5c6e 5c6e 5b21 5b4a 6f69 6e20 7468  a)\n\n[![Join th
-00000a20: 6520 4167 6f72 6120 6469 7363 6f72 645d  e Agora discord]
-00000a30: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000a40: 656c 6473 2e69 6f2f 6469 7363 6f72 642f  elds.io/discord/
-00000a50: 3131 3130 3931 3032 3737 3131 3037 3433  1110910277110743
-00000a60: 3130 333f 6c61 6265 6c3d 4469 7363 6f72  103?label=Discor
-00000a70: 6426 6c6f 676f 3d64 6973 636f 7264 266c  d&logo=discord&l
-00000a80: 6f67 6f43 6f6c 6f72 3d77 6869 7465 2673  ogoColor=white&s
-00000a90: 7479 6c65 3d70 6c61 7374 6963 2663 6f6c  tyle=plastic&col
-00000aa0: 6f72 3d64 3762 3032 3329 215b 5368 6172  or=d7b023)![Shar
-00000ab0: 6520 6f6e 2054 7769 7474 6572 5d28 6874  e on Twitter](ht
-00000ac0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000ad0: 732e 696f 2f74 7769 7474 6572 2f75 726c  s.io/twitter/url
-00000ae0: 2f68 7474 7073 2f74 7769 7474 6572 2e63  /https/twitter.c
-00000af0: 6f6d 2f63 6c6f 7564 706f 7373 652e 7376  om/cloudposse.sv
-00000b00: 673f 7374 796c 653d 736f 6369 616c 266c  g?style=social&l
-00000b10: 6162 656c 3d53 6861 7265 2532 3025 3430  abel=Share%20%40
-00000b20: 6b79 6567 6f6d 657a 2f7a 6574 6129 5d28  kyegomez/zeta)](
-00000b30: 6874 7470 733a 2f2f 7477 6974 7465 722e  https://twitter.
-00000b40: 636f 6d2f 696e 7465 6e74 2f74 7765 6574  com/intent/tweet
-00000b50: 3f74 6578 743d 4368 6563 6b25 3230 6f75  ?text=Check%20ou
-00000b60: 7425 3230 7468 6973 2532 3061 6d61 7a69  t%20this%20amazi
-00000b70: 6e67 2532 3041 4925 3230 7072 6f6a 6563  ng%20AI%20projec
-00000b80: 743a 2532 3026 7572 6c3d 6874 7470 7325  t:%20&url=https%
-00000b90: 3341 2532 4625 3246 6769 7468 7562 2e63  3A%2F%2Fgithub.c
-00000ba0: 6f6d 2532 466b 7965 676f 6d65 7a25 3246  om%2Fkyegomez%2F
-00000bb0: 7a65 7461 2920 5b21 5b53 6861 7265 206f  zeta) [![Share o
-00000bc0: 6e20 4661 6365 626f 6f6b 5d28 6874 7470  n Facebook](http
-00000bd0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000be0: 696f 2f62 6164 6765 2f53 6861 7265 2d25  io/badge/Share-%
-00000bf0: 3230 6661 6365 626f 6f6b 2d62 6c75 6529  20facebook-blue)
-00000c00: 5d28 6874 7470 733a 2f2f 7777 772e 6661  ](https://www.fa
-00000c10: 6365 626f 6f6b 2e63 6f6d 2f73 6861 7265  cebook.com/share
-00000c20: 722f 7368 6172 6572 2e70 6870 3f75 3d68  r/sharer.php?u=h
-00000c30: 7474 7073 2533 4125 3246 2532 4667 6974  ttps%3A%2F%2Fgit
-00000c40: 6875 622e 636f 6d25 3246 6b79 6567 6f6d  hub.com%2Fkyegom
-00000c50: 657a 2532 467a 6574 6129 205b 215b 5368  ez%2Fzeta) [![Sh
-00000c60: 6172 6520 6f6e 204c 696e 6b65 6449 6e5d  are on LinkedIn]
-00000c70: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000c80: 656c 6473 2e69 6f2f 6261 6467 652f 5368  elds.io/badge/Sh
-00000c90: 6172 652d 2532 306c 696e 6b65 6469 6e2d  are-%20linkedin-
-00000ca0: 626c 7565 295d 2868 7474 7073 3a2f 2f77  blue)](https://w
-00000cb0: 7777 2e6c 696e 6b65 6469 6e2e 636f 6d2f  ww.linkedin.com/
-00000cc0: 7368 6172 6541 7274 6963 6c65 3f6d 696e  shareArticle?min
-00000cd0: 693d 7472 7565 2675 726c 3d68 7474 7073  i=true&url=https
-00000ce0: 2533 4125 3246 2532 4667 6974 6875 622e  %3A%2F%2Fgithub.
-00000cf0: 636f 6d25 3246 6b79 6567 6f6d 657a 2532  com%2Fkyegomez%2
-00000d00: 467a 6574 6126 7469 746c 653d 2673 756d  Fzeta&title=&sum
-00000d10: 6d61 7279 3d26 736f 7572 6365 3d29 5c6e  mary=&source=)\n
-00000d20: 5c6e 5b21 5b53 6861 7265 206f 6e20 5265  \n[![Share on Re
-00000d30: 6464 6974 5d28 6874 7470 733a 2f2f 696d  ddit](https://im
-00000d40: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000d50: 6765 2f2d 5368 6172 6525 3230 6f6e 2532  ge/-Share%20on%2
-00000d60: 3052 6564 6469 742d 6f72 616e 6765 295d  0Reddit-orange)]
-00000d70: 2868 7474 7073 3a2f 2f77 7777 2e72 6564  (https://www.red
-00000d80: 6469 742e 636f 6d2f 7375 626d 6974 3f75  dit.com/submit?u
-00000d90: 726c 3d68 7474 7073 2533 4125 3246 2532  rl=https%3A%2F%2
-00000da0: 4667 6974 6875 622e 636f 6d25 3246 6b79  Fgithub.com%2Fky
-00000db0: 6567 6f6d 657a 2532 467a 6574 6126 7469  egomez%2Fzeta&ti
-00000dc0: 746c 653d 7a65 7461 2532 302d 2532 3074  tle=zeta%20-%20t
-00000dd0: 6865 2532 3066 7574 7572 6525 3230 6f66  he%20future%20of
-00000de0: 2532 3041 4929 205b 215b 5368 6172 6520  %20AI) [![Share 
-00000df0: 6f6e 2048 6163 6b65 7220 4e65 7773 5d28  on Hacker News](
-00000e00: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000e10: 6c64 732e 696f 2f62 6164 6765 2f2d 5368  lds.io/badge/-Sh
-00000e20: 6172 6525 3230 6f6e 2532 3048 6163 6b65  are%20on%20Hacke
-00000e30: 7225 3230 4e65 7773 2d6f 7261 6e67 6529  r%20News-orange)
-00000e40: 5d28 6874 7470 733a 2f2f 6e65 7773 2e79  ](https://news.y
-00000e50: 636f 6d62 696e 6174 6f72 2e63 6f6d 2f73  combinator.com/s
-00000e60: 7562 6d69 746c 696e 6b3f 753d 6874 7470  ubmitlink?u=http
-00000e70: 7325 3341 2532 4625 3246 6769 7468 7562  s%3A%2F%2Fgithub
-00000e80: 2e63 6f6d 2532 466b 7965 676f 6d65 7a25  .com%2Fkyegomez%
-00000e90: 3246 7a65 7461 2674 3d7a 6574 6125 3230  2Fzeta&t=zeta%20
-00000ea0: 2d25 3230 7468 6525 3230 6675 7475 7265  -%20the%20future
-00000eb0: 2532 306f 6625 3230 4149 2920 5b21 5b53  %20of%20AI) [![S
-00000ec0: 6861 7265 206f 6e20 5069 6e74 6572 6573  hare on Pinteres
-00000ed0: 745d 2868 7474 7073 3a2f 2f69 6d67 2e73  t](https://img.s
-00000ee0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000ef0: 2d53 6861 7265 2532 306f 6e25 3230 5069  -Share%20on%20Pi
-00000f00: 6e74 6572 6573 742d 7265 6429 5d28 6874  nterest-red)](ht
-00000f10: 7470 733a 2f2f 7069 6e74 6572 6573 742e  tps://pinterest.
-00000f20: 636f 6d2f 7069 6e2f 6372 6561 7465 2f62  com/pin/create/b
-00000f30: 7574 746f 6e2f 3f75 726c 3d68 7474 7073  utton/?url=https
-00000f40: 2533 4125 3246 2532 4667 6974 6875 622e  %3A%2F%2Fgithub.
-00000f50: 636f 6d25 3246 6b79 6567 6f6d 657a 2532  com%2Fkyegomez%2
-00000f60: 467a 6574 6126 6d65 6469 613d 6874 7470  Fzeta&media=http
-00000f70: 7325 3341 2532 4625 3246 6578 616d 706c  s%3A%2F%2Fexampl
-00000f80: 652e 636f 6d25 3246 696d 6167 652e 6a70  e.com%2Fimage.jp
-00000f90: 6726 6465 7363 7269 7074 696f 6e3d 7a65  g&description=ze
-00000fa0: 7461 2532 302d 2532 3074 6865 2532 3066  ta%20-%20the%20f
-00000fb0: 7574 7572 6525 3230 6f66 2532 3041 4929  uture%20of%20AI)
-00000fc0: 205b 215b 5368 6172 6520 6f6e 2057 6861   [![Share on Wha
-00000fd0: 7473 4170 705d 2868 7474 7073 3a2f 2f69  tsApp](https://i
-00000fe0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000ff0: 6467 652f 2d53 6861 7265 2532 306f 6e25  dge/-Share%20on%
-00001000: 3230 5768 6174 7341 7070 2d67 7265 656e  20WhatsApp-green
-00001010: 295d 2868 7474 7073 3a2f 2f61 7069 2e77  )](https://api.w
-00001020: 6861 7473 6170 702e 636f 6d2f 7365 6e64  hatsapp.com/send
-00001030: 3f74 6578 743d 4368 6563 6b25 3230 6f75  ?text=Check%20ou
-00001040: 7425 3230 7a65 7461 2532 302d 2532 3074  t%20zeta%20-%20t
-00001050: 6865 2532 3066 7574 7572 6525 3230 6f66  he%20future%20of
-00001060: 2532 3041 4925 3230 2532 337a 6574 6125  %20AI%20%23zeta%
-00001070: 3230 2532 3341 4925 3041 2530 4168 7474  20%23AI%0A%0Ahtt
-00001080: 7073 2533 4125 3246 2532 4667 6974 6875  ps%3A%2F%2Fgithu
-00001090: 622e 636f 6d25 3246 6b79 6567 6f6d 657a  b.com%2Fkyegomez
-000010a0: 2532 467a 6574 6129 5c6e 5c6e 4166 7465  %2Fzeta)\n\nAfte
-000010b0: 7220 6275 696c 6469 6e67 206f 7574 2074  r building out t
-000010c0: 686f 7573 616e 6473 206f 6620 6e65 7572  housands of neur
-000010d0: 616c 206e 6574 7320 616e 6420 6661 6369  al nets and faci
-000010e0: 6e67 2074 6865 2073 616d 6520 616e 6e6f  ng the same anno
-000010f0: 7969 6e67 2062 6f74 746c 656e 6563 6b73  ying bottlenecks
-00001100: 206f 6620 6368 616f 7469 6320 636f 6465   of chaotic code
-00001110: 6261 7365 7320 7769 7468 206e 6f20 6d6f  bases with no mo
-00001120: 6475 6c61 7269 7479 2061 6e64 206c 6f77  dularity and low
-00001130: 2070 6572 666f 726d 616e 6365 206d 6f64   performance mod
-00001140: 756c 6573 2c20 5a65 7461 206e 6565 6465  ules, Zeta neede
-00001150: 6420 746f 2062 6520 626f 726e 2074 6f20  d to be born to 
-00001160: 656e 6162 6c65 206d 6520 616e 6420 6f74  enable me and ot
-00001170: 6865 7273 2074 6f20 7175 6963 6b6c 7920  hers to quickly 
-00001180: 7072 6f74 6f74 7970 652c 2074 7261 696e  prototype, train
-00001190: 2c20 616e 6420 6f70 7469 6d69 7a65 2074  , and optimize t
-000011a0: 6865 206c 6174 6573 7420 534f 5441 206e  he latest SOTA n
-000011b0: 6575 7261 6c20 6e65 7473 2061 6e64 2064  eural nets and d
-000011c0: 6570 6c6f 7920 7468 656d 2069 6e74 6f20  eploy them into 
-000011d0: 7072 6f64 7563 7469 6f6e 2e20 5c6e 5c6e  production. \n\n
-000011e0: 5a65 7461 2070 6c61 6365 7320 6120 7261  Zeta places a ra
-000011f0: 6469 6361 6c20 656d 7068 6173 6973 206f  dical emphasis o
-00001200: 6e20 7573 6561 6269 6c69 7479 2c20 6d6f  n useability, mo
-00001210: 6475 6c61 7269 7479 2c20 616e 6420 7065  dularity, and pe
-00001220: 7266 6f72 6d61 6e63 652e 205a 6574 6120  rformance. Zeta 
-00001230: 6973 206e 6f77 2063 7572 7265 6e74 6c79  is now currently
-00001240: 2065 6d70 6c6f 7965 6420 696e 2031 3030   employed in 100
-00001250: 7320 6f66 206d 6f64 656c 7320 6163 726f  s of models acro
-00001260: 7373 206d 7920 6769 7468 7562 2061 6e64  ss my github and
-00001270: 2061 6372 6f73 7320 6f74 6865 7273 2e20   across others. 
-00001280: 5c6e 4765 7420 7374 6172 7465 6420 6265  \nGet started be
-00001290: 6c6f 7720 616e 6420 4c4d 4b20 6966 2079  low and LMK if y
-000012a0: 6f75 2077 616e 7420 6d79 2068 656c 7020  ou want my help 
-000012b0: 6275 696c 6469 6e67 2061 6e79 206d 6f64  building any mod
-000012c0: 656c 2c20 495c 276d 2068 6572 6520 666f  el, I\'m here fo
-000012d0: 7220 796f 7520 f09f 988a 20f0 9f92 9c20  r you .... .... 
-000012e0: 5c6e 5c6e 5c6e 2320 496e 7374 616c 6c5c  \n\n\n# Install\
-000012f0: 6e5c 6e60 2420 7069 7033 2069 6e73 7461  n\n`$ pip3 insta
-00001300: 6c6c 202d 5520 7a65 7461 7363 616c 6560  ll -U zetascale`
-00001310: 5c6e 5c6e 2320 5573 6167 655c 6e5c 6e23  \n\n# Usage\n\n#
-00001320: 2320 5374 6172 7469 6e67 2059 6f75 7220  # Starting Your 
-00001330: 4a6f 7572 6e65 795c 6e5c 6e43 7265 6174  Journey\n\nCreat
-00001340: 696e 6720 6120 6d6f 6465 6c20 656d 706f  ing a model empo
-00001350: 7765 7265 6420 7769 7468 2074 6865 2061  wered with the a
-00001360: 666f 7265 6d65 6e74 696f 6e65 6420 6272  forementioned br
-00001370: 6561 6b74 6872 6f75 6768 2072 6573 6561  eakthrough resea
-00001380: 7263 6820 6665 6174 7572 6573 2069 7320  rch features is 
-00001390: 6120 6272 6565 7a65 2e20 4865 7265 5c27  a breeze. Here\'
-000013a0: 7320 686f 7720 746f 2071 7569 636b 6c79  s how to quickly
-000013b0: 206d 6174 6572 6961 6c69 7a65 2074 6865   materialize the
-000013c0: 2072 656e 6f77 6e65 6420 466c 6173 6820   renowned Flash 
-000013d0: 4174 7465 6e74 696f 6e5c 6e5c 6e60 6060  Attention\n\n```
-000013e0: 7079 7468 6f6e 5c6e 696d 706f 7274 2074  python\nimport t
-000013f0: 6f72 6368 5c6e 5c6e 6672 6f6d 207a 6574  orch\n\nfrom zet
-00001400: 612e 6e6e 2069 6d70 6f72 7420 466c 6173  a.nn import Flas
-00001410: 6841 7474 656e 7469 6f6e 5c6e 5c6e 7120  hAttention\n\nq 
-00001420: 3d20 746f 7263 682e 7261 6e64 6e28 322c  = torch.randn(2,
-00001430: 2034 2c20 362c 2038 295c 6e6b 203d 2074   4, 6, 8)\nk = t
-00001440: 6f72 6368 2e72 616e 646e 2832 2c20 342c  orch.randn(2, 4,
-00001450: 2031 302c 2038 295c 6e76 203d 2074 6f72   10, 8)\nv = tor
-00001460: 6368 2e72 616e 646e 2832 2c20 342c 2031  ch.randn(2, 4, 1
-00001470: 302c 2038 295c 6e5c 6e61 7474 656e 7469  0, 8)\n\nattenti
-00001480: 6f6e 203d 2046 6c61 7368 4174 7465 6e74  on = FlashAttent
-00001490: 696f 6e28 6361 7573 616c 3d46 616c 7365  ion(causal=False
-000014a0: 2c20 6472 6f70 6f75 743d 302e 312c 2066  , dropout=0.1, f
-000014b0: 6c61 7368 3d54 7275 6529 5c6e 6f75 7470  lash=True)\noutp
-000014c0: 7574 203d 2061 7474 656e 7469 6f6e 2871  ut = attention(q
-000014d0: 2c20 6b2c 2076 295c 6e5c 6e70 7269 6e74  , k, v)\n\nprint
-000014e0: 286f 7574 7075 742e 7368 6170 6529 5c6e  (output.shape)\n
-000014f0: 6060 605c 6e5c 6e5c 6e5c 6e23 2323 2060  ```\n\n\n\n### `
-00001500: 5377 6947 4c55 605c 6e2d 2050 6f77 6572  SwiGLU`\n- Power
-00001510: 7320 5472 616e 7366 6f72 6d65 7220 6d6f  s Transformer mo
-00001520: 6465 6c73 5c6e 6060 6070 7974 686f 6e5c  dels\n```python\
-00001530: 6e69 6d70 6f72 7420 746f 7263 685c 6e5c  nimport torch\n\
-00001540: 6e66 726f 6d20 7a65 7461 2e6e 6e20 696d  nfrom zeta.nn im
-00001550: 706f 7274 2053 7769 474c 5553 7461 636b  port SwiGLUStack
-00001560: 6564 5c6e 5c6e 7820 3d20 746f 7263 682e  ed\n\nx = torch.
-00001570: 7261 6e64 6e28 352c 2031 3029 5c6e 7377  randn(5, 10)\nsw
-00001580: 6967 6c75 203d 2053 7769 474c 5553 7461  iglu = SwiGLUSta
-00001590: 636b 6564 2831 302c 2032 3029 5c6e 7377  cked(10, 20)\nsw
-000015a0: 6967 6c75 2878 292e 7368 6170 655c 6e60  iglu(x).shape\n`
-000015b0: 6060 5c6e 5c6e 2323 2320 6060 6052 656c  ``\n\n### ```Rel
-000015c0: 6174 6976 6550 6f73 6974 696f 6e42 6961  ativePositionBia
-000015d0: 7360 6060 5c6e 2d20 6060 6052 656c 6174  s```\n- ```Relat
-000015e0: 6976 6550 6f73 6974 696f 6e42 6961 7360  ivePositionBias`
-000015f0: 6060 2071 7561 6e74 697a 6573 2074 6865  `` quantizes the
-00001600: 2064 6973 7461 6e63 6520 6265 7477 6565   distance betwee
-00001610: 6e20 7477 6f20 706f 7369 7469 6f6e 7320  n two positions 
-00001620: 696e 746f 2061 2063 6572 7461 696e 206e  into a certain n
-00001630: 756d 6265 7220 6f66 2062 7563 6b65 7473  umber of buckets
-00001640: 2061 6e64 2074 6865 6e20 7573 6573 2061   and then uses a
-00001650: 6e20 656d 6265 6464 696e 6720 746f 2067  n embedding to g
-00001660: 6574 2074 6865 2072 656c 6174 6976 6520  et the relative 
-00001670: 706f 7369 7469 6f6e 2062 6961 732e 2054  position bias. T
-00001680: 6869 7320 6d65 6368 616e 6973 6d20 6169  his mechanism ai
-00001690: 6473 2069 6e20 7468 6520 6174 7465 6e74  ds in the attent
-000016a0: 696f 6e20 6d65 6368 616e 6973 6d20 6279  ion mechanism by
-000016b0: 2070 726f 7669 6469 6e67 2062 6961 7365   providing biase
-000016c0: 7320 6261 7365 6420 6f6e 2072 656c 6174  s based on relat
-000016d0: 6976 6520 706f 7369 7469 6f6e 7320 6265  ive positions be
-000016e0: 7477 6565 6e20 7468 6520 7175 6572 7920  tween the query 
-000016f0: 616e 6420 6b65 792c 2072 6174 6865 7220  and key, rather 
-00001700: 7468 616e 2072 656c 7969 6e67 2073 6f6c  than relying sol
-00001710: 656c 7920 6f6e 2074 6865 6972 2061 6273  ely on their abs
-00001720: 6f6c 7574 6520 706f 7369 7469 6f6e 732e  olute positions.
-00001730: 5c6e 6060 6070 7974 686f 6e5c 6e69 6d70  \n```python\nimp
-00001740: 6f72 7420 746f 7263 685c 6e66 726f 6d20  ort torch\nfrom 
-00001750: 746f 7263 6820 696d 706f 7274 206e 6e5c  torch import nn\
-00001760: 6e5c 6e66 726f 6d20 7a65 7461 2e6e 6e20  n\nfrom zeta.nn 
-00001770: 696d 706f 7274 2052 656c 6174 6976 6550  import RelativeP
-00001780: 6f73 6974 696f 6e42 6961 735c 6e5c 6e23  ositionBias\n\n#
-00001790: 2049 6e69 7469 616c 697a 6520 7468 6520   Initialize the 
-000017a0: 5265 6c61 7469 7665 506f 7369 7469 6f6e  RelativePosition
-000017b0: 4269 6173 206d 6f64 756c 655c 6e72 656c  Bias module\nrel
-000017c0: 5f70 6f73 5f62 6961 7320 3d20 5265 6c61  _pos_bias = Rela
-000017d0: 7469 7665 506f 7369 7469 6f6e 4269 6173  tivePositionBias
-000017e0: 2829 5c6e 5c6e 2320 4578 616d 706c 6520  ()\n\n# Example 
-000017f0: 313a 2043 6f6d 7075 7465 2062 6961 7320  1: Compute bias 
-00001800: 666f 7220 6120 7369 6e67 6c65 2062 6174  for a single bat
-00001810: 6368 5c6e 6269 6173 5f6d 6174 7269 7820  ch\nbias_matrix 
-00001820: 3d20 7265 6c5f 706f 735f 6269 6173 2831  = rel_pos_bias(1
-00001830: 2c20 3130 2c20 3130 295c 6e5c 6e5c 6e23  , 10, 10)\n\n\n#
-00001840: 2045 7861 6d70 6c65 2032 3a20 5574 696c   Example 2: Util
-00001850: 697a 6520 696e 2063 6f6e 6a75 6e63 7469  ize in conjuncti
-00001860: 6f6e 2077 6974 6820 616e 2061 7474 656e  on with an atten
-00001870: 7469 6f6e 206d 6563 6861 6e69 736d 5c6e  tion mechanism\n
-00001880: 2320 4e4f 5445 3a20 5468 6973 2069 7320  # NOTE: This is 
-00001890: 6120 6d6f 636b 2065 7861 6d70 6c65 2c20  a mock example, 
-000018a0: 616e 6420 6d61 7920 6e6f 7420 7265 7072  and may not repr
-000018b0: 6573 656e 7420 616e 2061 6374 7561 6c20  esent an actual 
-000018c0: 6174 7465 6e74 696f 6e20 6d65 6368 616e  attention mechan
-000018d0: 6973 6d5c 2773 2063 6f6d 706c 6574 6520  ism\'s complete 
-000018e0: 696d 706c 656d 656e 7461 7469 6f6e 2e5c  implementation.\
-000018f0: 6e63 6c61 7373 204d 6f63 6b41 7474 656e  nclass MockAtten
-00001900: 7469 6f6e 286e 6e2e 4d6f 6475 6c65 293a  tion(nn.Module):
-00001910: 5c6e 2020 2020 6465 6620 5f5f 696e 6974  \n    def __init
-00001920: 5f5f 2873 656c 6629 3a5c 6e20 2020 2020  __(self):\n     
-00001930: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00001940: 745f 5f28 295c 6e20 2020 2020 2020 2073  t__()\n        s
-00001950: 656c 662e 7265 6c5f 706f 735f 6269 6173  elf.rel_pos_bias
-00001960: 203d 2052 656c 6174 6976 6550 6f73 6974   = RelativePosit
-00001970: 696f 6e42 6961 7328 295c 6e5c 6e20 2020  ionBias()\n\n   
-00001980: 2064 6566 2066 6f72 7761 7264 2873 656c   def forward(sel
-00001990: 662c 2071 7565 7269 6573 2c20 6b65 7973  f, queries, keys
-000019a0: 293a 5c6e 2020 2020 2020 2020 6269 6173  ):\n        bias
-000019b0: 203d 2073 656c 662e 7265 6c5f 706f 735f   = self.rel_pos_
-000019c0: 6269 6173 2871 7565 7269 6573 2e73 697a  bias(queries.siz
-000019d0: 6528 3029 2c20 7175 6572 6965 732e 7369  e(0), queries.si
-000019e0: 7a65 2831 292c 206b 6579 732e 7369 7a65  ze(1), keys.size
-000019f0: 2831 2929 5c6e 2020 2020 2020 2020 2320  (1))\n        # 
-00001a00: 4675 7274 6865 7220 636f 6d70 7574 6174  Further computat
-00001a10: 696f 6e73 2077 6974 6820 6269 6173 2069  ions with bias i
-00001a20: 6e20 7468 6520 6174 7465 6e74 696f 6e20  n the attention 
-00001a30: 6d65 6368 616e 6973 6d2e 2e2e 5c6e 2020  mechanism...\n  
-00001a40: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00001a50: 6520 2023 2050 6c61 6365 686f 6c64 6572  e  # Placeholder
-00001a60: 5c6e 5c6e 5c6e 2320 4578 616d 706c 6520  \n\n\n# Example 
-00001a70: 333a 204d 6f64 6966 7920 6465 6661 756c  3: Modify defaul
-00001a80: 7420 636f 6e66 6967 7572 6174 696f 6e73  t configurations
-00001a90: 5c6e 6375 7374 6f6d 5f72 656c 5f70 6f73  \ncustom_rel_pos
-00001aa0: 5f62 6961 7320 3d20 5265 6c61 7469 7665  _bias = Relative
-00001ab0: 506f 7369 7469 6f6e 4269 6173 285c 6e20  PositionBias(\n 
-00001ac0: 2020 2062 6964 6972 6563 7469 6f6e 616c     bidirectional
-00001ad0: 3d46 616c 7365 2c20 6e75 6d5f 6275 636b  =False, num_buck
-00001ae0: 6574 733d 3634 2c20 6d61 785f 6469 7374  ets=64, max_dist
-00001af0: 616e 6365 3d32 3536 2c20 6e75 6d5f 6865  ance=256, num_he
-00001b00: 6164 733d 385c 6e29 5c6e 6060 605c 6e5c  ads=8\n)\n```\n\
-00001b10: 6e23 2323 2060 4665 6564 466f 7277 6172  n### `FeedForwar
-00001b20: 6460 5c6e 5468 6520 4665 6564 466f 7277  d`\nThe FeedForw
-00001b30: 6172 6420 6d6f 6475 6c65 2070 6572 666f  ard module perfo
-00001b40: 726d 7320 6120 6665 6564 666f 7277 6172  rms a feedforwar
-00001b50: 6420 6f70 6572 6174 696f 6e20 6f6e 2074  d operation on t
-00001b60: 6865 2069 6e70 7574 2074 656e 736f 7220  he input tensor 
-00001b70: 782e 2049 7420 636f 6e73 6973 7473 206f  x. It consists o
-00001b80: 6620 6120 6d75 6c74 692d 6c61 7965 7220  f a multi-layer 
-00001b90: 7065 7263 6570 7472 6f6e 2028 4d4c 5029  perceptron (MLP)
-00001ba0: 2077 6974 6820 616e 206f 7074 696f 6e61   with an optiona
-00001bb0: 6c20 6163 7469 7661 7469 6f6e 2066 756e  l activation fun
-00001bc0: 6374 696f 6e20 616e 6420 4c61 7965 724e  ction and LayerN
-00001bd0: 6f72 6d2e 205c 6e55 7365 6420 696e 206d  orm. \nUsed in m
-00001be0: 6f73 7420 6c61 6e67 7561 6765 2c20 6d75  ost language, mu
-00001bf0: 6c74 692d 6d6f 6461 6c2c 2061 6e64 206d  lti-modal, and m
-00001c00: 6f64 6572 6e20 6e65 7572 616c 206e 6574  odern neural net
-00001c10: 776f 726b 732e 5c6e 5c6e 6060 6070 7974  works.\n\n```pyt
-00001c20: 686f 6e5c 6e69 6d70 6f72 7420 746f 7263  hon\nimport torc
-00001c30: 685c 6e5c 6e66 726f 6d20 7a65 7461 2e6e  h\n\nfrom zeta.n
-00001c40: 6e20 696d 706f 7274 2046 6565 6446 6f72  n import FeedFor
-00001c50: 7761 7264 5c6e 5c6e 6d6f 6465 6c20 3d20  ward\n\nmodel = 
-00001c60: 4665 6564 466f 7277 6172 6428 3235 362c  FeedForward(256,
-00001c70: 2035 3132 2c20 676c 753d 5472 7565 2c20   512, glu=True, 
-00001c80: 706f 7374 5f61 6374 5f6c 6e3d 5472 7565  post_act_ln=True
-00001c90: 2c20 6472 6f70 6f75 743d 302e 3229 5c6e  , dropout=0.2)\n
-00001ca0: 5c6e 7820 3d20 746f 7263 682e 7261 6e64  \nx = torch.rand
-00001cb0: 6e28 312c 2032 3536 295c 6e5c 6e6f 7574  n(1, 256)\n\nout
-00001cc0: 7075 7420 3d20 6d6f 6465 6c28 7829 5c6e  put = model(x)\n
-00001cd0: 7072 696e 7428 6f75 7470 7574 2e73 6861  print(output.sha
-00001ce0: 7065 295c 6e60 6060 5c6e 5c6e 2323 2320  pe)\n```\n\n### 
-00001cf0: 6042 6974 4c69 6e65 6172 605c 6e2d 2054  `BitLinear`\n- T
-00001d00: 6865 2042 6974 4c69 6e65 6172 206d 6f64  he BitLinear mod
-00001d10: 756c 6520 7065 7266 6f72 6d73 206c 696e  ule performs lin
-00001d20: 6561 7220 7472 616e 7366 6f72 6d61 7469  ear transformati
-00001d30: 6f6e 206f 6e20 7468 6520 696e 7075 7420  on on the input 
-00001d40: 6461 7461 2c20 666f 6c6c 6f77 6564 2062  data, followed b
-00001d50: 7920 7175 616e 7469 7a61 7469 6f6e 2061  y quantization a
-00001d60: 6e64 2064 6571 7561 6e74 697a 6174 696f  nd dequantizatio
-00001d70: 6e2e 2054 6865 2071 7561 6e74 697a 6174  n. The quantizat
-00001d80: 696f 6e20 7072 6f63 6573 7320 6973 2070  ion process is p
-00001d90: 6572 666f 726d 6564 2075 7369 6e67 2074  erformed using t
-00001da0: 6865 2061 6273 6d61 785f 7175 616e 7469  he absmax_quanti
-00001db0: 7a65 2066 756e 6374 696f 6e2c 2077 6869  ze function, whi
-00001dc0: 6368 2071 7561 6e74 697a 6573 2074 6865  ch quantizes the
-00001dd0: 2069 6e70 7574 2074 656e 736f 7220 6261   input tensor ba
-00001de0: 7365 6420 6f6e 2074 6865 2061 6273 6f6c  sed on the absol
-00001df0: 7574 6520 6d61 7869 6d75 6d20 7661 6c75  ute maximum valu
-00001e00: 652c 205b 6672 6f6d 2074 6865 2070 6170  e, [from the pap
-00001e10: 6572 5d28 6874 7470 733a 2f2f 6172 7869  er](https://arxi
-00001e20: 762e 6f72 672f 6162 732f 3233 3130 2e31  v.org/abs/2310.1
-00001e30: 3134 3533 295c 6e60 6060 7079 7468 6f6e  1453)\n```python
-00001e40: 5c6e 696d 706f 7274 2074 6f72 6368 5c6e  \nimport torch\n
-00001e50: 6672 6f6d 2074 6f72 6368 2069 6d70 6f72  from torch impor
-00001e60: 7420 6e6e 5c6e 5c6e 696d 706f 7274 207a  t nn\n\nimport z
-00001e70: 6574 612e 7175 616e 7420 6173 2071 745c  eta.quant as qt\
-00001e80: 6e5c 6e5c 6e63 6c61 7373 204d 794d 6f64  n\n\nclass MyMod
-00001e90: 656c 286e 6e2e 4d6f 6475 6c65 293a 5c6e  el(nn.Module):\n
-00001ea0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00001eb0: 2873 656c 6629 3a5c 6e20 2020 2020 2020  (self):\n       
-00001ec0: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-00001ed0: 5f28 295c 6e20 2020 2020 2020 2073 656c  _()\n        sel
-00001ee0: 662e 6c69 6e65 6172 203d 2071 742e 4269  f.linear = qt.Bi
-00001ef0: 744c 696e 6561 7228 3130 2c20 3230 295c  tLinear(10, 20)\
-00001f00: 6e5c 6e20 2020 2064 6566 2066 6f72 7761  n\n    def forwa
-00001f10: 7264 2873 656c 662c 2078 293a 5c6e 2020  rd(self, x):\n  
-00001f20: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001f30: 662e 6c69 6e65 6172 2878 295c 6e5c 6e5c  f.linear(x)\n\n\
-00001f40: 6e23 2049 6e69 7469 616c 697a 6520 7468  n# Initialize th
-00001f50: 6520 6d6f 6465 6c5c 6e6d 6f64 656c 203d  e model\nmodel =
-00001f60: 204d 794d 6f64 656c 2829 5c6e 5c6e 2320   MyModel()\n\n# 
-00001f70: 4372 6561 7465 2061 2072 616e 646f 6d20  Create a random 
-00001f80: 7465 6e73 6f72 206f 6620 7369 7a65 2028  tensor of size (
-00001f90: 3132 382c 2031 3029 5c6e 696e 7075 7420  128, 10)\ninput 
-00001fa0: 3d20 746f 7263 682e 7261 6e64 6e28 3132  = torch.randn(12
-00001fb0: 382c 2031 3029 5c6e 5c6e 2320 5065 7266  8, 10)\n\n# Perf
-00001fc0: 6f72 6d20 7468 6520 666f 7277 6172 6420  orm the forward 
-00001fd0: 7061 7373 5c6e 6f75 7470 7574 203d 206d  pass\noutput = m
-00001fe0: 6f64 656c 2869 6e70 7574 295c 6e5c 6e23  odel(input)\n\n#
-00001ff0: 2050 7269 6e74 2074 6865 2073 697a 6520   Print the size 
-00002000: 6f66 2074 6865 206f 7574 7075 745c 6e70  of the output\np
-00002010: 7269 6e74 286f 7574 7075 742e 7369 7a65  rint(output.size
-00002020: 2829 2920 2023 2074 6f72 6368 2e53 697a  ())  # torch.Siz
-00002030: 6528 5b31 3238 2c20 3230 5d29 5c6e 6060  e([128, 20])\n``
-00002040: 605c 6e5c 6e23 2323 2060 5061 6c6d 4560  `\n\n### `PalmE`
-00002050: 5c6e 2d20 5468 6973 2069 7320 616e 2069  \n- This is an i
-00002060: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
-00002070: 2074 6865 206d 756c 7469 2d6d 6f64 616c   the multi-modal
-00002080: 2050 616c 6d2d 4520 6d6f 6465 6c20 7573   Palm-E model us
-00002090: 696e 6720 6120 6465 636f 6465 7220 6c6c  ing a decoder ll
-000020a0: 6d20 6173 2074 6865 2062 6163 6b62 6f6e  m as the backbon
-000020b0: 6520 7769 7468 2061 6e20 5649 5420 696d  e with an VIT im
-000020c0: 6167 6520 656e 636f 6465 7220 746f 2070  age encoder to p
-000020d0: 726f 6365 7373 2076 6973 696f 6e2c 2069  rocess vision, i
-000020e0: 745c 2773 2076 6572 7920 7369 6d69 6c69  t\'s very simili
-000020f0: 6172 2074 6f20 4750 5434 2c20 4b6f 736d  ar to GPT4, Kosm
-00002100: 6f73 2c20 5254 5832 2c20 616e 6420 6d61  os, RTX2, and ma
-00002110: 6e79 206f 7468 6572 206d 756c 7469 2d6d  ny other multi-m
-00002120: 6f64 616c 6974 7920 6d6f 6465 6c20 6172  odality model ar
-00002130: 6368 6974 6563 7475 7265 735c 6e5c 6e60  chitectures\n\n`
-00002140: 6060 7079 7468 6f6e 5c6e 696d 706f 7274  ``python\nimport
-00002150: 2074 6f72 6368 5c6e 5c6e 6672 6f6d 207a   torch\n\nfrom z
-00002160: 6574 612e 7374 7275 6374 7320 696d 706f  eta.structs impo
-00002170: 7274 2028 5c6e 2020 2020 4175 746f 5265  rt (\n    AutoRe
-00002180: 6772 6573 7369 7665 5772 6170 7065 722c  gressiveWrapper,
-00002190: 5c6e 2020 2020 4465 636f 6465 722c 5c6e  \n    Decoder,\n
-000021a0: 2020 2020 456e 636f 6465 722c 5c6e 2020      Encoder,\n  
-000021b0: 2020 5472 616e 7366 6f72 6d65 722c 5c6e    Transformer,\n
-000021c0: 2020 2020 5669 5472 616e 7366 6f72 6d65      ViTransforme
-000021d0: 7257 7261 7070 6572 2c5c 6e29 5c6e 5c6e  rWrapper,\n)\n\n
-000021e0: 5c6e 636c 6173 7320 5061 6c6d 4528 746f  \nclass PalmE(to
-000021f0: 7263 682e 6e6e 2e4d 6f64 756c 6529 3a5c  rch.nn.Module):\
-00002200: 6e20 2020 2022 2222 5c6e 2020 2020 2020  n    """\n      
-00002210: 2020 5061 6c6d 4520 6973 2061 2074 7261    PalmE is a tra
-00002220: 6e73 666f 726d 6572 2061 7263 6869 7465  nsformer archite
-00002230: 6374 7572 6520 7468 6174 2075 7365 7320  cture that uses 
-00002240: 6120 5669 5420 656e 636f 6465 7220 616e  a ViT encoder an
-00002250: 6420 6120 7472 616e 7366 6f72 6d65 7220  d a transformer 
-00002260: 6465 636f 6465 722e 5c6e 5c6e 2020 2020  decoder.\n\n    
-00002270: 2020 2020 4172 6773 3a5c 6e5c 6e20 2020      Args:\n\n   
-00002280: 2020 2020 2020 2020 2069 6d61 6765 5f73           image_s
-00002290: 697a 6520 2869 6e74 293a 2053 697a 6520  ize (int): Size 
-000022a0: 6f66 2074 6865 2069 6d61 6765 2e5c 6e20  of the image.\n 
-000022b0: 2020 2020 2020 2020 2020 2070 6174 6368             patch
-000022c0: 5f73 697a 6520 2869 6e74 293a 2053 697a  _size (int): Siz
-000022d0: 6520 6f66 2074 6865 2070 6174 6368 2e5c  e of the patch.\
-000022e0: 6e20 2020 2020 2020 2020 2020 2065 6e63  n            enc
-000022f0: 6f64 6572 5f64 696d 2028 696e 7429 3a20  oder_dim (int): 
-00002300: 4469 6d65 6e73 696f 6e20 6f66 2074 6865  Dimension of the
-00002310: 2065 6e63 6f64 6572 2e5c 6e20 2020 2020   encoder.\n     
-00002320: 2020 2020 2020 2065 6e63 6f64 6572 5f64         encoder_d
-00002330: 6570 7468 2028 696e 7429 3a20 4465 7074  epth (int): Dept
-00002340: 6820 6f66 2074 6865 2065 6e63 6f64 6572  h of the encoder
-00002350: 2e5c 6e20 2020 2020 2020 2020 2020 2065  .\n            e
-00002360: 6e63 6f64 6572 5f68 6561 6473 2028 696e  ncoder_heads (in
-00002370: 7429 3a20 4e75 6d62 6572 206f 6620 6865  t): Number of he
-00002380: 6164 7320 696e 2074 6865 2065 6e63 6f64  ads in the encod
-00002390: 6572 2e5c 6e20 2020 2020 2020 2020 2020  er.\n           
-000023a0: 206e 756d 5f74 6f6b 656e 7320 2869 6e74   num_tokens (int
-000023b0: 293a 204e 756d 6265 7220 6f66 2074 6f6b  ): Number of tok
-000023c0: 656e 732e 5c6e 2020 2020 2020 2020 2020  ens.\n          
-000023d0: 2020 6d61 785f 7365 715f 6c65 6e20 2869    max_seq_len (i
-000023e0: 6e74 293a 204d 6178 696d 756d 2073 6571  nt): Maximum seq
-000023f0: 7565 6e63 6520 6c65 6e67 7468 2e5c 6e20  uence length.\n 
-00002400: 2020 2020 2020 2020 2020 2064 6563 6f64             decod
-00002410: 6572 5f64 696d 2028 696e 7429 3a20 4469  er_dim (int): Di
-00002420: 6d65 6e73 696f 6e20 6f66 2074 6865 2064  mension of the d
-00002430: 6563 6f64 6572 2e5c 6e20 2020 2020 2020  ecoder.\n       
-00002440: 2020 2020 2064 6563 6f64 6572 5f64 6570       decoder_dep
-00002450: 7468 2028 696e 7429 3a20 4465 7074 6820  th (int): Depth 
-00002460: 6f66 2074 6865 2064 6563 6f64 6572 2e5c  of the decoder.\
-00002470: 6e20 2020 2020 2020 2020 2020 2064 6563  n            dec
-00002480: 6f64 6572 5f68 6561 6473 2028 696e 7429  oder_heads (int)
-00002490: 3a20 4e75 6d62 6572 206f 6620 6865 6164  : Number of head
-000024a0: 7320 696e 2074 6865 2064 6563 6f64 6572  s in the decoder
-000024b0: 2e5c 6e20 2020 2020 2020 2020 2020 2061  .\n            a
-000024c0: 6c69 6269 5f6e 756d 5f68 6561 6473 2028  libi_num_heads (
-000024d0: 696e 7429 3a20 4e75 6d62 6572 206f 6620  int): Number of 
-000024e0: 6865 6164 7320 696e 2074 6865 2061 6c69  heads in the ali
-000024f0: 6269 2061 7474 656e 7469 6f6e 2e5c 6e20  bi attention.\n 
-00002500: 2020 2020 2020 2020 2020 2061 7474 6e5f             attn_
-00002510: 6b76 5f68 6561 6473 2028 696e 7429 3a20  kv_heads (int): 
-00002520: 4e75 6d62 6572 206f 6620 6865 6164 7320  Number of heads 
-00002530: 696e 2074 6865 2061 7474 656e 7469 6f6e  in the attention
-00002540: 206b 6579 2d76 616c 7565 2070 726f 6a65   key-value proje
-00002550: 6374 696f 6e2e 5c6e 2020 2020 2020 2020  ction.\n        
-00002560: 2020 2020 7573 655f 6162 735f 706f 735f      use_abs_pos_
-00002570: 656d 6220 2862 6f6f 6c29 3a20 5768 6574  emb (bool): Whet
-00002580: 6865 7220 746f 2075 7365 2061 6273 6f6c  her to use absol
-00002590: 7574 6520 706f 7369 7469 6f6e 616c 2065  ute positional e
-000025a0: 6d62 6564 6469 6e67 732e 5c6e 2020 2020  mbeddings.\n    
-000025b0: 2020 2020 2020 2020 6372 6f73 735f 6174          cross_at
-000025c0: 7465 6e64 2028 626f 6f6c 293a 2057 6865  tend (bool): Whe
-000025d0: 7468 6572 2074 6f20 6372 6f73 7320 6174  ther to cross at
-000025e0: 7465 6e64 2069 6e20 7468 6520 6465 636f  tend in the deco
-000025f0: 6465 722e 5c6e 2020 2020 2020 2020 2020  der.\n          
-00002600: 2020 616c 6962 695f 706f 735f 6269 6173    alibi_pos_bias
-00002610: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
-00002620: 2074 6f20 7573 6520 706f 7369 7469 6f6e   to use position
-00002630: 616c 2062 6961 7320 696e 2074 6865 2061  al bias in the a
-00002640: 6c69 6269 2061 7474 656e 7469 6f6e 2e5c  libi attention.\
-00002650: 6e20 2020 2020 2020 2020 2020 2072 6f74  n            rot
-00002660: 6172 795f 7870 6f73 2028 626f 6f6c 293a  ary_xpos (bool):
-00002670: 2057 6865 7468 6572 2074 6f20 7573 6520   Whether to use 
-00002680: 726f 7461 7279 2070 6f73 6974 696f 6e61  rotary positiona
-00002690: 6c20 656d 6265 6464 696e 6773 2e5c 6e20  l embeddings.\n 
-000026a0: 2020 2020 2020 2020 2020 2061 7474 6e5f             attn_
-000026b0: 666c 6173 6820 2862 6f6f 6c29 3a20 5768  flash (bool): Wh
-000026c0: 6574 6865 7220 746f 2075 7365 2061 7474  ether to use att
-000026d0: 656e 7469 6f6e 2066 6c61 7368 2e5c 6e20  ention flash.\n 
-000026e0: 2020 2020 2020 2020 2020 2071 6b5f 6e6f             qk_no
-000026f0: 726d 2028 626f 6f6c 293a 2057 6865 7468  rm (bool): Wheth
-00002700: 6572 2074 6f20 6e6f 726d 616c 697a 6520  er to normalize 
-00002710: 7468 6520 7175 6572 7920 616e 6420 6b65  the query and ke
-00002720: 7920 696e 2074 6865 2061 7474 656e 7469  y in the attenti
-00002730: 6f6e 206c 6179 6572 2e5c 6e5c 6e20 2020  on layer.\n\n   
-00002740: 2020 2020 2052 6574 7572 6e73 3a5c 6e5c       Returns:\n\
-00002750: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00002760: 2074 6f72 6368 2e54 656e 736f 723a 2054   torch.Tensor: T
-00002770: 6865 206f 7574 7075 7420 6f66 2074 6865  he output of the
-00002780: 206d 6f64 656c 2e5c 6e5c 6e20 2020 2020   model.\n\n     
-00002790: 2020 2055 7361 6765 3a5c 6e5c 6e20 2020     Usage:\n\n   
-000027a0: 2069 6d67 203d 2074 6f72 6368 2e72 616e   img = torch.ran
-000027b0: 646e 2831 2c20 332c 2032 3536 2c20 3235  dn(1, 3, 256, 25
-000027c0: 3629 5c6e 2020 2020 7465 7874 203d 2074  6)\n    text = t
-000027d0: 6f72 6368 2e72 616e 6469 6e74 2830 2c20  orch.randint(0, 
-000027e0: 3230 3030 302c 2028 312c 2031 3032 3429  20000, (1, 1024)
-000027f0: 295c 6e20 2020 206d 6f64 656c 203d 2050  )\n    model = P
-00002800: 616c 6d45 2829 5c6e 2020 2020 6f75 7470  almE()\n    outp
-00002810: 7574 203d 206d 6f64 656c 2869 6d67 2c20  ut = model(img, 
-00002820: 7465 7874 295c 6e20 2020 2070 7269 6e74  text)\n    print
-00002830: 286f 7574 7075 7429 5c6e 5c6e 2020 2020  (output)\n\n    
-00002840: 2222 225c 6e5c 6e20 2020 2064 6566 205f  """\n\n    def _
-00002850: 5f69 6e69 745f 5f28 5c6e 2020 2020 2020  _init__(\n      
-00002860: 2020 7365 6c66 2c5c 6e20 2020 2020 2020    self,\n       
-00002870: 2069 6d61 6765 5f73 697a 653d 3235 362c   image_size=256,
-00002880: 5c6e 2020 2020 2020 2020 7061 7463 685f  \n        patch_
-00002890: 7369 7a65 3d33 322c 5c6e 2020 2020 2020  size=32,\n      
-000028a0: 2020 656e 636f 6465 725f 6469 6d3d 3531    encoder_dim=51
-000028b0: 322c 5c6e 2020 2020 2020 2020 656e 636f  2,\n        enco
-000028c0: 6465 725f 6465 7074 683d 362c 5c6e 2020  der_depth=6,\n  
-000028d0: 2020 2020 2020 656e 636f 6465 725f 6865        encoder_he
-000028e0: 6164 733d 382c 5c6e 2020 2020 2020 2020  ads=8,\n        
-000028f0: 6e75 6d5f 746f 6b65 6e73 3d32 3030 3030  num_tokens=20000
-00002900: 2c5c 6e20 2020 2020 2020 206d 6178 5f73  ,\n        max_s
-00002910: 6571 5f6c 656e 3d31 3032 342c 5c6e 2020  eq_len=1024,\n  
-00002920: 2020 2020 2020 6465 636f 6465 725f 6469        decoder_di
-00002930: 6d3d 3531 322c 5c6e 2020 2020 2020 2020  m=512,\n        
-00002940: 6465 636f 6465 725f 6465 7074 683d 362c  decoder_depth=6,
-00002950: 5c6e 2020 2020 2020 2020 6465 636f 6465  \n        decode
-00002960: 725f 6865 6164 733d 382c 5c6e 2020 2020  r_heads=8,\n    
-00002970: 2020 2020 616c 6962 695f 6e75 6d5f 6865      alibi_num_he
-00002980: 6164 733d 342c 5c6e 2020 2020 2020 2020  ads=4,\n        
-00002990: 6174 746e 5f6b 765f 6865 6164 733d 322c  attn_kv_heads=2,
-000029a0: 5c6e 2020 2020 2020 2020 7573 655f 6162  \n        use_ab
-000029b0: 735f 706f 735f 656d 623d 4661 6c73 652c  s_pos_emb=False,
-000029c0: 5c6e 2020 2020 2020 2020 6372 6f73 735f  \n        cross_
-000029d0: 6174 7465 6e64 3d54 7275 652c 5c6e 2020  attend=True,\n  
-000029e0: 2020 2020 2020 616c 6962 695f 706f 735f        alibi_pos_
-000029f0: 6269 6173 3d54 7275 652c 5c6e 2020 2020  bias=True,\n    
-00002a00: 2020 2020 726f 7461 7279 5f78 706f 733d      rotary_xpos=
-00002a10: 5472 7565 2c5c 6e20 2020 2020 2020 2061  True,\n        a
-00002a20: 7474 6e5f 666c 6173 683d 5472 7565 2c5c  ttn_flash=True,\
-00002a30: 6e20 2020 2020 2020 2071 6b5f 6e6f 726d  n        qk_norm
-00002a40: 3d54 7275 652c 5c6e 2020 2020 293a 5c6e  =True,\n    ):\n
-00002a50: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00002a60: 5f5f 696e 6974 5f5f 2829 5c6e 5c6e 2020  __init__()\n\n  
-00002a70: 2020 2020 2020 2320 7669 7420 6172 6368        # vit arch
-00002a80: 6974 6563 7475 7265 5c6e 2020 2020 2020  itecture\n      
-00002a90: 2020 7365 6c66 2e65 6e63 6f64 6572 203d    self.encoder =
-00002aa0: 2056 6954 7261 6e73 666f 726d 6572 5772   ViTransformerWr
-00002ab0: 6170 7065 7228 5c6e 2020 2020 2020 2020  apper(\n        
-00002ac0: 2020 2020 696d 6167 655f 7369 7a65 3d69      image_size=i
-00002ad0: 6d61 6765 5f73 697a 652c 5c6e 2020 2020  mage_size,\n    
-00002ae0: 2020 2020 2020 2020 7061 7463 685f 7369          patch_si
-00002af0: 7a65 3d70 6174 6368 5f73 697a 652c 5c6e  ze=patch_size,\n
-00002b00: 2020 2020 2020 2020 2020 2020 6174 746e              attn
-00002b10: 5f6c 6179 6572 733d 456e 636f 6465 7228  _layers=Encoder(
-00002b20: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00002b30: 2020 6469 6d3d 656e 636f 6465 725f 6469    dim=encoder_di
-00002b40: 6d2c 2064 6570 7468 3d65 6e63 6f64 6572  m, depth=encoder
-00002b50: 5f64 6570 7468 2c20 6865 6164 733d 656e  _depth, heads=en
-00002b60: 636f 6465 725f 6865 6164 735c 6e20 2020  coder_heads\n   
-00002b70: 2020 2020 2020 2020 2029 2c5c 6e20 2020           ),\n   
-00002b80: 2020 2020 2029 5c6e 5c6e 2020 2020 2020       )\n\n      
-00002b90: 2020 2320 7061 6c6d 206d 6f64 656c 2061    # palm model a
-00002ba0: 7263 6869 7465 6374 7572 655c 6e20 2020  rchitecture\n   
-00002bb0: 2020 2020 2073 656c 662e 6465 636f 6465       self.decode
-00002bc0: 7220 3d20 5472 616e 7366 6f72 6d65 7228  r = Transformer(
-00002bd0: 5c6e 2020 2020 2020 2020 2020 2020 6e75  \n            nu
-00002be0: 6d5f 746f 6b65 6e73 3d6e 756d 5f74 6f6b  m_tokens=num_tok
-00002bf0: 656e 732c 5c6e 2020 2020 2020 2020 2020  ens,\n          
-00002c00: 2020 6d61 785f 7365 715f 6c65 6e3d 6d61    max_seq_len=ma
-00002c10: 785f 7365 715f 6c65 6e2c 5c6e 2020 2020  x_seq_len,\n    
-00002c20: 2020 2020 2020 2020 7573 655f 6162 735f          use_abs_
-00002c30: 706f 735f 656d 623d 7573 655f 6162 735f  pos_emb=use_abs_
-00002c40: 706f 735f 656d 622c 5c6e 2020 2020 2020  pos_emb,\n      
-00002c50: 2020 2020 2020 6174 746e 5f6c 6179 6572        attn_layer
-00002c60: 733d 4465 636f 6465 7228 5c6e 2020 2020  s=Decoder(\n    
-00002c70: 2020 2020 2020 2020 2020 2020 6469 6d3d              dim=
-00002c80: 6465 636f 6465 725f 6469 6d2c 5c6e 2020  decoder_dim,\n  
-00002c90: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00002ca0: 7074 683d 6465 636f 6465 725f 6465 7074  pth=decoder_dept
-00002cb0: 682c 5c6e 2020 2020 2020 2020 2020 2020  h,\n            
-00002cc0: 2020 2020 6865 6164 733d 6465 636f 6465      heads=decode
-00002cd0: 725f 6865 6164 732c 5c6e 2020 2020 2020  r_heads,\n      
-00002ce0: 2020 2020 2020 2020 2020 6372 6f73 735f            cross_
-00002cf0: 6174 7465 6e64 3d63 726f 7373 5f61 7474  attend=cross_att
-00002d00: 656e 642c 5c6e 2020 2020 2020 2020 2020  end,\n          
-00002d10: 2020 2020 2020 616c 6962 695f 706f 735f        alibi_pos_
-00002d20: 6269 6173 3d61 6c69 6269 5f70 6f73 5f62  bias=alibi_pos_b
-00002d30: 6961 732c 5c6e 2020 2020 2020 2020 2020  ias,\n          
-00002d40: 2020 2020 2020 616c 6962 695f 6e75 6d5f        alibi_num_
-00002d50: 6865 6164 733d 616c 6962 695f 6e75 6d5f  heads=alibi_num_
-00002d60: 6865 6164 732c 5c6e 2020 2020 2020 2020  heads,\n        
-00002d70: 2020 2020 2020 2020 726f 7461 7279 5f78          rotary_x
-00002d80: 706f 733d 726f 7461 7279 5f78 706f 732c  pos=rotary_xpos,
-00002d90: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00002da0: 2020 6174 746e 5f6b 765f 6865 6164 733d    attn_kv_heads=
-00002db0: 6174 746e 5f6b 765f 6865 6164 732c 5c6e  attn_kv_heads,\n
-00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dd0: 6174 746e 5f66 6c61 7368 3d61 7474 6e5f  attn_flash=attn_
-00002de0: 666c 6173 682c 5c6e 2020 2020 2020 2020  flash,\n        
-00002df0: 2020 2020 2020 2020 716b 5f6e 6f72 6d3d          qk_norm=
-00002e00: 716b 5f6e 6f72 6d2c 5c6e 2020 2020 2020  qk_norm,\n      
-00002e10: 2020 2020 2020 292c 5c6e 2020 2020 2020        ),\n      
-00002e20: 2020 295c 6e5c 6e20 2020 2020 2020 2023    )\n\n        #
-00002e30: 2061 7574 6f72 6567 7265 7373 6976 6520   autoregressive 
-00002e40: 7772 6170 7065 7220 746f 2065 6e61 626c  wrapper to enabl
-00002e50: 6520 6765 6e65 7261 7469 6f6e 206f 6620  e generation of 
-00002e60: 746f 6b65 6e73 5c6e 2020 2020 2020 2020  tokens\n        
-00002e70: 7365 6c66 2e64 6563 6f64 6572 203d 2041  self.decoder = A
-00002e80: 7574 6f52 6567 7265 7373 6976 6557 7261  utoRegressiveWra
-00002e90: 7070 6572 2873 656c 662e 6465 636f 6465  pper(self.decode
-00002ea0: 7229 5c6e 5c6e 2020 2020 6465 6620 666f  r)\n\n    def fo
-00002eb0: 7277 6172 6428 7365 6c66 2c20 696d 673a  rward(self, img:
-00002ec0: 2074 6f72 6368 2e54 656e 736f 722c 2074   torch.Tensor, t
-00002ed0: 6578 743a 2074 6f72 6368 2e54 656e 736f  ext: torch.Tenso
-00002ee0: 7229 3a5c 6e20 2020 2020 2020 2022 2222  r):\n        """
-00002ef0: 466f 7277 6172 6420 7061 7373 206f 6620  Forward pass of 
-00002f00: 7468 6520 6d6f 6465 6c2e 2222 225c 6e20  the model."""\n 
-00002f10: 2020 2020 2020 2074 7279 3a5c 6e20 2020         try:\n   
-00002f20: 2020 2020 2020 2020 2065 6e63 6f64 6564           encoded
-00002f30: 203d 2073 656c 662e 656e 636f 6465 7228   = self.encoder(
-00002f40: 696d 672c 2072 6574 7572 6e5f 656d 6265  img, return_embe
-00002f50: 6464 696e 6773 3d54 7275 6529 5c6e 2020  ddings=True)\n  
-00002f60: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002f70: 2073 656c 662e 6465 636f 6465 7228 7465   self.decoder(te
-00002f80: 7874 2c20 636f 6e74 6578 743d 656e 636f  xt, context=enco
-00002f90: 6465 6429 5c6e 2020 2020 2020 2020 6578  ded)\n        ex
-00002fa0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00002fb0: 7320 6572 726f 723a 5c6e 2020 2020 2020  s error:\n      
-00002fc0: 2020 2020 2020 7072 696e 7428 6622 4661        print(f"Fa
-00002fd0: 696c 6564 2069 6e20 666f 7277 6172 6420  iled in forward 
-00002fe0: 6d65 7468 6f64 3a20 7b65 7272 6f72 7d22  method: {error}"
-00002ff0: 295c 6e20 2020 2020 2020 2020 2020 2072  )\n            r
-00003000: 6169 7365 5c6e 5c6e 5c6e 2320 5573 6167  aise\n\n\n# Usag
-00003010: 6520 7769 7468 2072 616e 646f 6d20 696e  e with random in
-00003020: 7075 7473 5c6e 696d 6720 3d20 746f 7263  puts\nimg = torc
-00003030: 682e 7261 6e64 6e28 312c 2033 2c20 3235  h.randn(1, 3, 25
-00003040: 362c 2032 3536 295c 6e74 6578 7420 3d20  6, 256)\ntext = 
-00003050: 746f 7263 682e 7261 6e64 696e 7428 302c  torch.randint(0,
-00003060: 2032 3030 3030 2c20 2831 2c20 3130 3234   20000, (1, 1024
-00003070: 2929 5c6e 5c6e 2320 496e 6974 696c 6961  ))\n\n# Initilia
-00003080: 7a65 2074 6865 206d 6f64 656c 5c6e 6d6f  ze the model\nmo
-00003090: 6465 6c20 3d20 5061 6c6d 4528 295c 6e6f  del = PalmE()\no
-000030a0: 7574 7075 7420 3d20 6d6f 6465 6c28 696d  utput = model(im
-000030b0: 672c 2074 6578 7429 5c6e 7072 696e 7428  g, text)\nprint(
-000030c0: 6f75 7470 7574 295c 6e60 6060 5c6e 5c6e  output)\n```\n\n
-000030d0: 5c6e 2323 2320 6055 6e65 7460 5c6e 556e  \n### `Unet`\nUn
-000030e0: 6574 2069 7320 6120 6661 6d6f 7573 2063  et is a famous c
-000030f0: 6f6e 766f 6c75 7469 6f6e 616c 206e 6575  onvolutional neu
-00003100: 7261 6c20 6e65 7477 6f72 6b20 6172 6368  ral network arch
-00003110: 6974 6563 7475 7265 206f 7269 6769 6e61  itecture origina
-00003120: 6c6c 7920 7573 6564 2066 6f72 2062 696f  lly used for bio
-00003130: 6d65 6469 6361 6c20 696d 6167 6520 7365  medical image se
-00003140: 676d 656e 7461 7469 6f6e 2062 7574 2073  gmentation but s
-00003150: 6f6f 6e20 6265 6361 6d65 2074 6865 2062  oon became the b
-00003160: 6163 6b62 6f6e 6520 6f66 2074 6865 2067  ackbone of the g
-00003170: 656e 6572 6174 6976 6520 4149 204d 6567  enerative AI Meg
-00003180: 612d 7265 766f 6c75 7469 6f6e 2e20 5468  a-revolution. Th
-00003190: 6520 6172 6368 6974 6563 7475 7265 2063  e architecture c
-000031a0: 6f6d 7072 6973 6573 2074 776f 2070 7269  omprises two pri
-000031b0: 6d61 7279 2070 6174 6877 6179 733a 2064  mary pathways: d
-000031c0: 6f77 6e73 616d 706c 696e 6720 616e 6420  ownsampling and 
-000031d0: 7570 7361 6d70 6c69 6e67 2c20 666f 6c6c  upsampling, foll
-000031e0: 6f77 6564 2062 7920 616e 206f 7574 7075  owed by an outpu
-000031f0: 7420 636f 6e76 6f6c 7574 696f 6e2e 2044  t convolution. D
-00003200: 7565 2074 6f20 6974 7320 552d 7368 6170  ue to its U-shap
-00003210: 652c 2074 6865 2061 7263 6869 7465 6374  e, the architect
-00003220: 7572 6520 6973 206e 616d 6564 2055 2d4e  ure is named U-N
-00003230: 6574 2e20 4974 7320 7379 6d6d 6574 7269  et. Its symmetri
-00003240: 6320 6172 6368 6974 6563 7475 7265 2065  c architecture e
-00003250: 6e73 7572 6573 2074 6861 7420 7468 6520  nsures that the 
-00003260: 636f 6e74 6578 7420 2866 726f 6d20 646f  context (from do
-00003270: 776e 7361 6d70 6c69 6e67 2920 616e 6420  wnsampling) and 
-00003280: 7468 6520 6c6f 6361 6c69 7a61 7469 6f6e  the localization
-00003290: 2028 6672 6f6d 2075 7073 616d 706c 696e   (from upsamplin
-000032a0: 6729 2061 7265 2063 6170 7475 7265 6420  g) are captured 
-000032b0: 6566 6665 6374 6976 656c 792e 5c6e 5c6e  effectively.\n\n
-000032c0: 6060 6070 7974 686f 6e5c 6e69 6d70 6f72  ```python\nimpor
-000032d0: 7420 746f 7263 685c 6e5c 6e66 726f 6d20  t torch\n\nfrom 
-000032e0: 7a65 7461 2e6e 6e20 696d 706f 7274 2055  zeta.nn import U
-000032f0: 6e65 745c 6e5c 6e23 2049 6e69 7469 616c  net\n\n# Initial
-00003300: 697a 6520 7468 6520 552d 4e65 7420 6d6f  ize the U-Net mo
-00003310: 6465 6c5c 6e6d 6f64 656c 203d 2055 6e65  del\nmodel = Une
-00003320: 7428 6e5f 6368 616e 6e65 6c73 3d31 2c20  t(n_channels=1, 
-00003330: 6e5f 636c 6173 7365 733d 3229 5c6e 5c6e  n_classes=2)\n\n
-00003340: 2320 5261 6e64 6f6d 2069 6e70 7574 2074  # Random input t
-00003350: 656e 736f 7220 7769 7468 2064 696d 656e  ensor with dimen
-00003360: 7369 6f6e 7320 5b62 6174 6368 5f73 697a  sions [batch_siz
-00003370: 652c 2063 6861 6e6e 656c 732c 2068 6569  e, channels, hei
-00003380: 6768 742c 2077 6964 7468 5d5c 6e78 203d  ght, width]\nx =
-00003390: 2074 6f72 6368 2e72 616e 646e 2831 2c20   torch.randn(1, 
-000033a0: 312c 2035 3732 2c20 3537 3229 5c6e 5c6e  1, 572, 572)\n\n
-000033b0: 2320 466f 7277 6172 6420 7061 7373 2074  # Forward pass t
-000033c0: 6872 6f75 6768 2074 6865 206d 6f64 656c  hrough the model
-000033d0: 5c6e 7920 3d20 6d6f 6465 6c28 7829 5c6e  \ny = model(x)\n
-000033e0: 5c6e 2320 4f75 7470 7574 5c6e 7072 696e  \n# Output\nprin
-000033f0: 7428 6622 496e 7075 7420 7368 6170 653a  t(f"Input shape:
-00003400: 207b 782e 7368 6170 657d 2229 5c6e 7072   {x.shape}")\npr
-00003410: 696e 7428 6622 4f75 7470 7574 2073 6861  int(f"Output sha
-00003420: 7065 3a20 7b79 2e73 6861 7065 7d22 295c  pe: {y.shape}")\
-00003430: 6e60 6060 5c6e 5c6e 5c6e 2323 2320 6056  n```\n\n\n### `V
-00003440: 6973 696f 6e45 6d62 6564 6469 6e67 7360  isionEmbeddings`
-00003450: 5c6e 5468 6520 5669 7369 6f6e 456d 6265  \nThe VisionEmbe
-00003460: 6464 696e 6720 636c 6173 7320 6973 2064  dding class is d
-00003470: 6573 6967 6e65 6420 666f 7220 636f 6e76  esigned for conv
-00003480: 6572 7469 6e67 2069 6d61 6765 7320 696e  erting images in
-00003490: 746f 2070 6174 6368 2065 6d62 6564 6469  to patch embeddi
-000034a0: 6e67 732c 206d 616b 696e 6720 7468 656d  ngs, making them
-000034b0: 2073 7569 7461 626c 6520 666f 7220 7072   suitable for pr
-000034c0: 6f63 6573 7369 6e67 2062 7920 7472 616e  ocessing by tran
-000034d0: 7366 6f72 6d65 722d 6261 7365 6420 6d6f  sformer-based mo
-000034e0: 6465 6c73 2e20 5468 6973 2063 6c61 7373  dels. This class
-000034f0: 2070 6c61 7973 2061 2063 7275 6369 616c   plays a crucial
-00003500: 2072 6f6c 6520 696e 2076 6172 696f 7573   role in various
-00003510: 2063 6f6d 7075 7465 7220 7669 7369 6f6e   computer vision
-00003520: 2074 6173 6b73 2061 6e64 2065 6e61 626c   tasks and enabl
-00003530: 6573 2074 6865 2069 6e74 6567 7261 7469  es the integrati
-00003540: 6f6e 206f 6620 7669 7369 6f6e 2064 6174  on of vision dat
-00003550: 6120 696e 746f 2074 7261 6e73 666f 726d  a into transform
-00003560: 6572 2061 7263 6869 7465 6374 7572 6573  er architectures
-00003570: 215c 6e5c 6e60 6060 7079 7468 6f6e 5c6e  !\n\n```python\n
-00003580: 696d 706f 7274 2074 6f72 6368 5c6e 5c6e  import torch\n\n
-00003590: 6672 6f6d 207a 6574 612e 6e6e 2069 6d70  from zeta.nn imp
-000035a0: 6f72 7420 5669 7369 6f6e 456d 6265 6464  ort VisionEmbedd
-000035b0: 696e 675c 6e5c 6e23 2043 7265 6174 6520  ing\n\n# Create 
-000035c0: 616e 2069 6e73 7461 6e63 6520 6f66 2056  an instance of V
-000035d0: 6973 696f 6e45 6d62 6564 6469 6e67 5c6e  isionEmbedding\n
-000035e0: 7669 7369 6f6e 5f65 6d62 6564 6469 6e67  vision_embedding
-000035f0: 203d 2056 6973 696f 6e45 6d62 6564 6469   = VisionEmbeddi
-00003600: 6e67 285c 6e20 2020 2069 6d67 5f73 697a  ng(\n    img_siz
-00003610: 653d 3232 342c 5c6e 2020 2020 7061 7463  e=224,\n    patc
-00003620: 685f 7369 7a65 3d31 362c 5c6e 2020 2020  h_size=16,\n    
-00003630: 696e 5f63 6861 6e73 3d33 2c5c 6e20 2020  in_chans=3,\n   
-00003640: 2065 6d62 6564 5f64 696d 3d37 3638 2c5c   embed_dim=768,\
-00003650: 6e20 2020 2063 6f6e 7461 696e 5f6d 6173  n    contain_mas
-00003660: 6b5f 746f 6b65 6e3d 5472 7565 2c5c 6e20  k_token=True,\n 
-00003670: 2020 2070 7265 7065 6e64 5f63 6c73 5f74     prepend_cls_t
-00003680: 6f6b 656e 3d54 7275 652c 5c6e 295c 6e5c  oken=True,\n)\n\
-00003690: 6e23 204c 6f61 6420 616e 2065 7861 6d70  n# Load an examp
-000036a0: 6c65 2069 6d61 6765 2028 3320 6368 616e  le image (3 chan
-000036b0: 6e65 6c73 2c20 3232 3478 3232 3429 5c6e  nels, 224x224)\n
-000036c0: 696e 7075 745f 696d 6167 6520 3d20 746f  input_image = to
-000036d0: 7263 682e 7261 6e64 2831 2c20 332c 2032  rch.rand(1, 3, 2
-000036e0: 3234 2c20 3232 3429 5c6e 5c6e 2320 5065  24, 224)\n\n# Pe
-000036f0: 7266 6f72 6d20 696d 6167 652d 746f 2d70  rform image-to-p
-00003700: 6174 6368 2065 6d62 6564 6469 6e67 5c6e  atch embedding\n
-00003710: 6f75 7470 7574 203d 2076 6973 696f 6e5f  output = vision_
-00003720: 656d 6265 6464 696e 6728 696e 7075 745f  embedding(input_
-00003730: 696d 6167 6529 5c6e 5c6e 2320 5468 6520  image)\n\n# The 
-00003740: 6f75 7470 7574 206e 6f77 2063 6f6e 7461  output now conta
-00003750: 696e 7320 7061 7463 6820 656d 6265 6464  ins patch embedd
-00003760: 696e 6773 2c20 7265 6164 7920 666f 7220  ings, ready for 
-00003770: 696e 7075 7420 746f 2061 2074 7261 6e73  input to a trans
-00003780: 666f 726d 6572 206d 6f64 656c 5c6e 6060  former model\n``
-00003790: 605c 6e5c 6e5c 6e23 2323 2060 6e69 7661  `\n\n\n### `niva
-000037a0: 605c 6e2d 204e 6976 6120 666f 6375 7365  `\n- Niva focuse
-000037b0: 7320 6f6e 2077 6569 6768 7473 206f 6620  s on weights of 
-000037c0: 6365 7274 6169 6e20 6c61 7965 7273 2028  certain layers (
-000037d0: 7370 6563 6966 6965 6420 6279 2071 7561  specified by qua
-000037e0: 6e74 697a 655f 6c61 7965 7273 292e 2049  ntize_layers). I
-000037f0: 6465 616c 2066 6f72 206d 6f64 656c 7320  deal for models 
-00003800: 7768 6572 6520 7275 6e74 696d 6520 6163  where runtime ac
-00003810: 7469 7661 7469 6f6e 2069 7320 7661 7269  tivation is vari
-00003820: 6162 6c65 2e20 f09f 9181 efb8 8f20 4578  able. ....... Ex
-00003830: 616d 706c 6520 4c61 7965 7273 3a20 6e6e  ample Layers: nn
-00003840: 2e45 6d62 6564 6469 6e67 2c20 6e6e 2e4c  .Embedding, nn.L
-00003850: 5354 4d2e 205c 6e5c 6e60 6060 7079 7468  STM. \n\n```pyth
-00003860: 6f6e 5c6e 696d 706f 7274 2074 6f72 6368  on\nimport torch
-00003870: 5c6e 5c6e 6672 6f6d 207a 6574 6120 696d  \n\nfrom zeta im
-00003880: 706f 7274 206e 6976 615c 6e5c 6e23 204c  port niva\n\n# L
-00003890: 6f61 6420 6120 7072 652d 7472 6169 6e65  oad a pre-traine
-000038a0: 6420 6d6f 6465 6c5c 6e6d 6f64 656c 203d  d model\nmodel =
-000038b0: 2059 6f75 724d 6f64 656c 436c 6173 7328   YourModelClass(
-000038c0: 295c 6e5c 6e23 2051 7561 6e74 697a 6520  )\n\n# Quantize 
-000038d0: 7468 6520 6d6f 6465 6c20 6479 6e61 6d69  the model dynami
-000038e0: 6361 6c6c 792c 2073 7065 6369 6679 696e  cally, specifyin
-000038f0: 6720 6c61 7965 7273 2074 6f20 7175 616e  g layers to quan
-00003900: 7469 7a65 5c6e 6e69 7661 285c 6e20 2020  tize\nniva(\n   
-00003910: 206d 6f64 656c 3d6d 6f64 656c 2c5c 6e20   model=model,\n 
-00003920: 2020 206d 6f64 656c 5f70 6174 683d 2270     model_path="p
-00003930: 6174 685f 746f 5f70 7265 7472 6169 6e65  ath_to_pretraine
-00003940: 645f 6d6f 6465 6c5f 7765 6967 6874 732e  d_model_weights.
-00003950: 7074 222c 5c6e 2020 2020 6f75 7470 7574  pt",\n    output
-00003960: 5f70 6174 683d 2271 7561 6e74 697a 6564  _path="quantized
-00003970: 5f6d 6f64 656c 2e70 7422 2c5c 6e20 2020  _model.pt",\n   
-00003980: 2071 7561 6e74 5f74 7970 653d 2264 796e   quant_type="dyn
-00003990: 616d 6963 222c 5c6e 2020 2020 7175 616e  amic",\n    quan
-000039a0: 7469 7a65 5f6c 6179 6572 733d 5b6e 6e2e  tize_layers=[nn.
-000039b0: 4c69 6e65 6172 2c20 6e6e 2e43 6f6e 7632  Linear, nn.Conv2
-000039c0: 645d 2c5c 6e20 2020 2064 7479 7065 3d74  d],\n    dtype=t
-000039d0: 6f72 6368 2e71 696e 7438 2c5c 6e29 5c6e  orch.qint8,\n)\n
-000039e0: 6060 605c 6e5c 6e5c 6e23 2323 2060 4675  ```\n\n\n### `Fu
-000039f0: 7365 6444 656e 7365 4745 4c55 4465 6e73  sedDenseGELUDens
-00003a00: 6560 5c6e 2d20 496e 6372 6561 7365 206d  e`\n- Increase m
-00003a10: 6f64 656c 2073 7065 6564 2062 7920 3278  odel speed by 2x
-00003a20: 2077 6974 6820 7468 6973 206d 6f64 756c   with this modul
-00003a30: 6520 7468 6174 2066 7573 6573 2074 6f67  e that fuses tog
-00003a40: 6574 6865 7220 3220 6879 7065 722d 6f70  ether 2 hyper-op
-00003a50: 7469 6d69 7a65 6420 6465 6e73 6520 6f70  timized dense op
-00003a60: 7320 6672 6f6d 2062 6974 7320 616e 6420  s from bits and 
-00003a70: 6279 7465 7320 616e 6420 6120 6765 6c75  bytes and a gelu
-00003a80: 2074 6f67 6574 6865 7221 5c6e 5c6e 6060   together!\n\n``
-00003a90: 6070 7974 686f 6e5c 6e69 6d70 6f72 7420  `python\nimport 
-00003aa0: 746f 7263 685c 6e5c 6e66 726f 6d20 7a65  torch\n\nfrom ze
-00003ab0: 7461 2e6e 6e20 696d 706f 7274 2046 7573  ta.nn import Fus
-00003ac0: 6564 4465 6e73 6547 454c 5544 656e 7365  edDenseGELUDense
-00003ad0: 5c6e 5c6e 7820 3d20 746f 7263 682e 7261  \n\nx = torch.ra
-00003ae0: 6e64 6e28 312c 2035 3132 295c 6e6d 6f64  ndn(1, 512)\nmod
-00003af0: 656c 203d 2046 7573 6564 4465 6e73 6547  el = FusedDenseG
-00003b00: 454c 5544 656e 7365 2835 3132 2c20 3130  ELUDense(512, 10
-00003b10: 3234 295c 6e6f 7574 203d 206d 6f64 656c  24)\nout = model
-00003b20: 2878 295c 6e6f 7574 2e73 6861 7065 5c6e  (x)\nout.shape\n
-00003b30: 6060 605c 6e5c 6e5c 6e23 2323 2060 4675  ```\n\n\n### `Fu
-00003b40: 7365 6444 726f 706f 7574 4c61 7965 724e  sedDropoutLayerN
-00003b50: 6f72 6d60 5c6e 2d20 4675 7365 6444 726f  orm`\n- FusedDro
-00003b60: 706f 7574 4c61 7965 724e 6f72 6d20 6973  poutLayerNorm is
-00003b70: 2061 2066 7573 6564 206b 6572 6e65 6c20   a fused kernel 
-00003b80: 6f66 2064 726f 706f 7574 2061 6e64 206c  of dropout and l
-00003b90: 6179 6572 6e6f 726d 2074 6f20 7370 6565  ayernorm to spee
-00003ba0: 6420 7570 2046 464e 7320 6f72 204d 4c50  d up FFNs or MLP
-00003bb0: 5320 6279 2032 585c 6e5c 6e60 6060 7079  S by 2X\n\n```py
-00003bc0: 7468 6f6e 5c6e 696d 706f 7274 2074 6f72  thon\nimport tor
-00003bd0: 6368 5c6e 6672 6f6d 2074 6f72 6368 2069  ch\nfrom torch i
-00003be0: 6d70 6f72 7420 6e6e 5c6e 5c6e 6672 6f6d  mport nn\n\nfrom
-00003bf0: 207a 6574 612e 6e6e 2069 6d70 6f72 7420   zeta.nn import 
-00003c00: 4675 7365 6444 726f 706f 7574 4c61 7965  FusedDropoutLaye
-00003c10: 724e 6f72 6d5c 6e5c 6e23 2049 6e69 7469  rNorm\n\n# Initi
-00003c20: 616c 697a 6520 7468 6520 6d6f 6475 6c65  alize the module
-00003c30: 5c6e 6d6f 6465 6c20 3d20 4675 7365 6444  \nmodel = FusedD
-00003c40: 726f 706f 7574 4c61 7965 724e 6f72 6d28  ropoutLayerNorm(
-00003c50: 6469 6d3d 3531 3229 5c6e 5c6e 2320 4372  dim=512)\n\n# Cr
-00003c60: 6561 7465 2061 2073 616d 706c 6520 696e  eate a sample in
-00003c70: 7075 7420 7465 6e73 6f72 5c6e 7820 3d20  put tensor\nx = 
-00003c80: 746f 7263 682e 7261 6e64 6e28 312c 2035  torch.randn(1, 5
-00003c90: 3132 295c 6e5c 6e23 2046 6f72 7761 7264  12)\n\n# Forward
-00003ca0: 2070 6173 735c 6e6f 7574 7075 7420 3d20   pass\noutput = 
-00003cb0: 6d6f 6465 6c28 7829 5c6e 5c6e 2320 4368  model(x)\n\n# Ch
-00003cc0: 6563 6b20 6f75 7470 7574 2073 6861 7065  eck output shape
-00003cd0: 5c6e 7072 696e 7428 6f75 7470 7574 2e73  \nprint(output.s
-00003ce0: 6861 7065 2920 2023 2045 7870 6563 7465  hape)  # Expecte
-00003cf0: 643a 2074 6f72 6368 2e53 697a 6528 5b31  d: torch.Size([1
-00003d00: 2c20 3531 325d 295c 6e60 6060 5c6e 5c6e  , 512])\n```\n\n
-00003d10: 5c6e 2323 2320 604d 616d 6261 605c 6e2d  \n### `Mamba`\n-
-00003d20: 2050 7974 6f72 6368 2069 6d70 6c65 6d65   Pytorch impleme
-00003d30: 6e74 6174 696f 6e20 6f66 2074 6865 206e  ntation of the n
-00003d40: 6577 2053 534d 206d 6f64 656c 2061 7263  ew SSM model arc
-00003d50: 6869 7465 6374 7572 6520 4d61 6d62 615c  hitecture Mamba\
-00003d60: 6e5c 6e60 6060 7079 7468 6f6e 5c6e 696d  n\n```python\nim
-00003d70: 706f 7274 2074 6f72 6368 5c6e 5c6e 6672  port torch\n\nfr
-00003d80: 6f6d 207a 6574 612e 6e6e 2069 6d70 6f72  om zeta.nn impor
-00003d90: 7420 4d61 6d62 6142 6c6f 636b 5c6e 5c6e  t MambaBlock\n\n
-00003da0: 2320 496e 6974 6961 6c69 7a65 204d 616d  # Initialize Mam
-00003db0: 6261 5c6e 626c 6f63 6b20 3d20 4d61 6d62  ba\nblock = Mamb
-00003dc0: 6142 6c6f 636b 2864 696d 3d36 342c 2064  aBlock(dim=64, d
-00003dd0: 6570 7468 3d31 295c 6e5c 6e23 2052 616e  epth=1)\n\n# Ran
-00003de0: 646f 6d20 696e 7075 745c 6e78 203d 2074  dom input\nx = t
-00003df0: 6f72 6368 2e72 616e 646e 2831 2c20 3130  orch.randn(1, 10
-00003e00: 2c20 3634 295c 6e5c 6e23 2041 7070 6c79  , 64)\n\n# Apply
-00003e10: 2074 6865 206d 6f64 656c 2074 6f20 7468   the model to th
-00003e20: 6520 626c 6f63 6b5c 6e79 203d 2062 6c6f  e block\ny = blo
-00003e30: 636b 2878 295c 6e5c 6e70 7269 6e74 2879  ck(x)\n\nprint(y
-00003e40: 2e73 6861 7065 295c 6e23 2074 6f72 6368  .shape)\n# torch
-00003e50: 2e53 697a 6528 5b31 2c20 3130 2c20 3634  .Size([1, 10, 64
-00003e60: 5d29 5c6e 6060 605c 6e5c 6e23 2323 2060  ])\n```\n\n### `
-00003e70: 4669 4c4d 605c 6e5c 6e60 6060 7079 7468  FiLM`\n\n```pyth
-00003e80: 6f6e 5c6e 696d 706f 7274 2074 6f72 6368  on\nimport torch
-00003e90: 5c6e 5c6e 6672 6f6d 207a 6574 612e 6e6e  \n\nfrom zeta.nn
-00003ea0: 2069 6d70 6f72 7420 4669 6c6d 5c6e 5c6e   import Film\n\n
-00003eb0: 2320 496e 6974 6961 6c69 7a65 2074 6865  # Initialize the
-00003ec0: 2046 696c 6d20 6c61 7965 725c 6e66 696c   Film layer\nfil
-00003ed0: 6d5f 6c61 7965 7220 3d20 4669 6c6d 2864  m_layer = Film(d
-00003ee0: 696d 3d31 3238 2c20 6869 6464 656e 5f64  im=128, hidden_d
-00003ef0: 696d 3d36 342c 2065 7870 616e 7365 5f72  im=64, expanse_r
-00003f00: 6174 696f 3d34 295c 6e5c 6e23 2043 7265  atio=4)\n\n# Cre
-00003f10: 6174 6520 736f 6d65 2064 756d 6d79 2064  ate some dummy d
-00003f20: 6174 6120 666f 7220 636f 6e64 6974 696f  ata for conditio
-00003f30: 6e73 2061 6e64 2068 6964 6465 6e73 5c6e  ns and hiddens\n
-00003f40: 636f 6e64 6974 696f 6e73 203d 2074 6f72  conditions = tor
-00003f50: 6368 2e72 616e 646e 2831 302c 2031 3238  ch.randn(10, 128
-00003f60: 2920 2023 2042 6174 6368 2073 697a 6520  )  # Batch size 
-00003f70: 6973 2031 302c 2066 6561 7475 7265 2073  is 10, feature s
-00003f80: 697a 6520 6973 2031 3238 5c6e 6869 6464  ize is 128\nhidd
-00003f90: 656e 7320 3d20 746f 7263 682e 7261 6e64  ens = torch.rand
-00003fa0: 6e28 5c6e 2020 2020 3130 2c20 312c 2031  n(\n    10, 1, 1
-00003fb0: 3238 5c6e 2920 2023 2042 6174 6368 2073  28\n)  # Batch s
-00003fc0: 697a 6520 6973 2031 302c 2073 6571 7565  ize is 10, seque
-00003fd0: 6e63 6520 6c65 6e67 7468 2069 7320 312c  nce length is 1,
-00003fe0: 2066 6561 7475 7265 2073 697a 6520 6973   feature size is
-00003ff0: 2031 3238 5c6e 5c6e 2320 5061 7373 2074   128\n\n# Pass t
-00004000: 6865 2064 6174 6120 7468 726f 7567 6820  he data through 
-00004010: 7468 6520 4669 6c6d 206c 6179 6572 5c6e  the Film layer\n
-00004020: 6d6f 6475 6c61 7465 645f 6665 6174 7572  modulated_featur
-00004030: 6573 203d 2066 696c 6d5f 6c61 7965 7228  es = film_layer(
-00004040: 636f 6e64 6974 696f 6e73 2c20 6869 6464  conditions, hidd
-00004050: 656e 7329 5c6e 5c6e 2320 5072 696e 7420  ens)\n\n# Print 
-00004060: 7468 6520 7368 6170 6520 6f66 2074 6865  the shape of the
-00004070: 206f 7574 7075 745c 6e70 7269 6e74 286d   output\nprint(m
-00004080: 6f64 756c 6174 6564 5f66 6561 7475 7265  odulated_feature
-00004090: 732e 7368 6170 6529 2020 2320 5368 6f75  s.shape)  # Shou
-000040a0: 6c64 2062 6520 5b31 302c 2031 2c20 3132  ld be [10, 1, 12
-000040b0: 385d 5c6e 6060 605c 6e5c 6e23 2323 2060  8]\n```\n\n### `
-000040c0: 6879 7065 725f 6f70 7469 6d69 7a65 605c  hyper_optimize`\
-000040d0: 6e2d 2041 2073 696e 676c 6520 7772 6170  n- A single wrap
-000040e0: 7065 7220 666f 7220 746f 7263 682e 6678  per for torch.fx
-000040f0: 2c20 746f 7263 682e 7363 7269 7074 2c20  , torch.script, 
-00004100: 746f 7263 682e 636f 6d70 696c 652c 2064  torch.compile, d
-00004110: 796e 616d 6963 2071 7561 6e74 697a 6174  ynamic quantizat
-00004120: 696f 6e2c 206d 6978 6564 2070 7265 6369  ion, mixed preci
-00004130: 7369 6f6e 2074 6872 6f75 6768 2074 6f72  sion through tor
-00004140: 6368 2e61 6d70 2c20 7769 7468 2065 7865  ch.amp, with exe
-00004150: 6375 7469 6f6e 2074 696d 6520 6d65 7472  cution time metr
-00004160: 6963 7320 616c 6c20 696e 206f 6e63 6520  ics all in once 
-00004170: 706c 6163 6521 5c6e 6060 6070 7974 686f  place!\n```pytho
-00004180: 6e5c 6e69 6d70 6f72 7420 746f 7263 685c  n\nimport torch\
-00004190: 6e5c 6e66 726f 6d20 7a65 7461 2e6e 6e20  n\nfrom zeta.nn 
-000041a0: 696d 706f 7274 2068 7970 6572 5f6f 7074  import hyper_opt
-000041b0: 696d 697a 655c 6e5c 6e5c 6e40 6879 7065  imize\n\n\n@hype
-000041c0: 725f 6f70 7469 6d69 7a65 285c 6e20 2020  r_optimize(\n   
-000041d0: 2074 6f72 6368 5f66 783d 4661 6c73 652c   torch_fx=False,
-000041e0: 5c6e 2020 2020 746f 7263 685f 7363 7269  \n    torch_scri
-000041f0: 7074 3d46 616c 7365 2c5c 6e20 2020 2074  pt=False,\n    t
-00004200: 6f72 6368 5f63 6f6d 7069 6c65 3d54 7275  orch_compile=Tru
-00004210: 652c 5c6e 2020 2020 7175 616e 7469 7a65  e,\n    quantize
-00004220: 3d54 7275 652c 5c6e 2020 2020 6d69 7865  =True,\n    mixe
-00004230: 645f 7072 6563 6973 696f 6e3d 5472 7565  d_precision=True
-00004240: 2c5c 6e20 2020 2065 6e61 626c 655f 6d65  ,\n    enable_me
-00004250: 7472 6963 733d 5472 7565 2c5c 6e29 5c6e  trics=True,\n)\n
-00004260: 6465 6620 6d6f 6465 6c28 7829 3a5c 6e20  def model(x):\n 
-00004270: 2020 2072 6574 7572 6e20 7820 4020 785c     return x @ x\
-00004280: 6e5c 6e5c 6e6f 7574 203d 206d 6f64 656c  n\n\nout = model
-00004290: 2874 6f72 6368 2e72 616e 646e 2831 2c20  (torch.randn(1, 
-000042a0: 332c 2033 322c 2033 3229 295c 6e70 7269  3, 32, 32))\npri
-000042b0: 6e74 286f 7574 295c 6e60 6060 5c6e 5c6e  nt(out)\n```\n\n
-000042c0: 5c6e 2323 2320 4450 4f20 2d20 4469 7265  \n### DPO - Dire
-000042d0: 6374 2050 6f6c 6963 7920 4f70 7469 6d69  ct Policy Optimi
-000042e0: 7a61 7469 6f6e 5c6e 4469 7265 6374 2050  zation\nDirect P
-000042f0: 6f6c 6963 7920 4f70 7469 6d69 7a61 7469  olicy Optimizati
-00004300: 6f6e 2065 6d70 6c6f 7965 6420 666f 7220  on employed for 
-00004310: 6d61 6e79 2052 4c48 4620 6170 706c 6963  many RLHF applic
-00004320: 6174 696f 6e73 2066 6f72 204c 4c4d 732e  ations for LLMs.
-00004330: 5c6e 5c6e 6060 6070 7974 686f 6e5c 6e69  \n\n```python\ni
-00004340: 6d70 6f72 7420 746f 7263 685c 6e66 726f  mport torch\nfro
-00004350: 6d20 746f 7263 6820 696d 706f 7274 206e  m torch import n
-00004360: 6e5c 6e5c 6e66 726f 6d20 7a65 7461 2e72  n\n\nfrom zeta.r
-00004370: 6c20 696d 706f 7274 2044 504f 5c6e 5c6e  l import DPO\n\n
-00004380: 5c6e 2320 4465 6669 6e65 2061 2073 696d  \n# Define a sim
-00004390: 706c 6520 706f 6c69 6379 206d 6f64 656c  ple policy model
-000043a0: 5c6e 636c 6173 7320 506f 6c69 6379 4d6f  \nclass PolicyMo
-000043b0: 6465 6c28 6e6e 2e4d 6f64 756c 6529 3a5c  del(nn.Module):\
-000043c0: 6e20 2020 2064 6566 205f 5f69 6e69 745f  n    def __init_
-000043d0: 5f28 7365 6c66 2c20 696e 7075 745f 6469  _(self, input_di
-000043e0: 6d2c 206f 7574 7075 745f 6469 6d29 3a5c  m, output_dim):\
-000043f0: 6e20 2020 2020 2020 2073 7570 6572 2829  n        super()
-00004400: 2e5f 5f69 6e69 745f 5f28 295c 6e20 2020  .__init__()\n   
-00004410: 2020 2020 2073 656c 662e 6663 203d 206e       self.fc = n
-00004420: 6e2e 4c69 6e65 6172 2869 6e70 7574 5f64  n.Linear(input_d
-00004430: 696d 2c20 6f75 7470 7574 5f64 696d 295c  im, output_dim)\
-00004440: 6e5c 6e20 2020 2064 6566 2066 6f72 7761  n\n    def forwa
-00004450: 7264 2873 656c 662c 2078 293a 5c6e 2020  rd(self, x):\n  
-00004460: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00004470: 662e 6663 2878 295c 6e5c 6e5c 6e69 6e70  f.fc(x)\n\n\ninp
-00004480: 7574 5f64 696d 203d 2031 305c 6e6f 7574  ut_dim = 10\nout
-00004490: 7075 745f 6469 6d20 3d20 355c 6e70 6f6c  put_dim = 5\npol
-000044a0: 6963 795f 6d6f 6465 6c20 3d20 506f 6c69  icy_model = Poli
-000044b0: 6379 4d6f 6465 6c28 696e 7075 745f 6469  cyModel(input_di
-000044c0: 6d2c 206f 7574 7075 745f 6469 6d29 5c6e  m, output_dim)\n
-000044d0: 5c6e 2320 496e 6974 6961 6c69 7a65 2044  \n# Initialize D
-000044e0: 504f 2077 6974 6820 7468 6520 706f 6c69  PO with the poli
-000044f0: 6379 206d 6f64 656c 5c6e 6470 6f5f 6d6f  cy model\ndpo_mo
-00004500: 6465 6c20 3d20 4450 4f28 6d6f 6465 6c3d  del = DPO(model=
-00004510: 706f 6c69 6379 5f6d 6f64 656c 2c20 6265  policy_model, be
-00004520: 7461 3d30 2e31 295c 6e5c 6e23 2053 616d  ta=0.1)\n\n# Sam
-00004530: 706c 6520 7072 6566 6572 7265 6420 616e  ple preferred an
-00004540: 6420 756e 7072 6566 6572 7265 6420 7365  d unpreferred se
-00004550: 7175 656e 6365 735c 6e70 7265 6665 7272  quences\npreferr
-00004560: 6564 5f73 6571 203d 2074 6f72 6368 2e72  ed_seq = torch.r
-00004570: 616e 6469 6e74 2830 2c20 6f75 7470 7574  andint(0, output
-00004580: 5f64 696d 2c20 2833 2c20 696e 7075 745f  _dim, (3, input_
-00004590: 6469 6d29 295c 6e75 6e70 7265 6665 7272  dim))\nunpreferr
-000045a0: 6564 5f73 6571 203d 2074 6f72 6368 2e72  ed_seq = torch.r
-000045b0: 616e 6469 6e74 2830 2c20 6f75 7470 7574  andint(0, output
-000045c0: 5f64 696d 2c20 2833 2c20 696e 7075 745f  _dim, (3, input_
-000045d0: 6469 6d29 295c 6e5c 6e23 2043 6f6d 7075  dim))\n\n# Compu
-000045e0: 7465 206c 6f73 735c 6e6c 6f73 7320 3d20  te loss\nloss = 
-000045f0: 6470 6f5f 6d6f 6465 6c28 7072 6566 6572  dpo_model(prefer
-00004600: 7265 645f 7365 712c 2075 6e70 7265 6665  red_seq, unprefe
-00004610: 7272 6564 5f73 6571 295c 6e70 7269 6e74  rred_seq)\nprint
-00004620: 286c 6f73 7329 5c6e 6060 605c 6e5c 6e5c  (loss)\n```\n\n\
-00004630: 6e23 2323 205a 6574 6143 6c6f 7564 5c6e  n### ZetaCloud\n
-00004640: 5472 6169 6e20 6f72 2066 696e 6574 756e  Train or finetun
-00004650: 6520 616e 7920 6d6f 6465 6c20 6f6e 2061  e any model on a
-00004660: 6e79 2063 6c75 7374 6572 2069 6e20 3120  ny cluster in 1 
-00004670: 636c 6963 6b20 7769 7468 207a 6574 6163  click with zetac
-00004680: 6c6f 7564 2c20 6a75 7374 2070 6173 7320  loud, just pass 
-00004690: 696e 2079 6f75 7220 6669 6c65 2061 6e64  in your file and
-000046a0: 2074 6865 2047 5055 2074 7970 6520 616e   the GPU type an
-000046b0: 6420 7175 616e 7469 7479 2079 6f75 2077  d quantity you w
-000046c0: 616e 7421 2054 6f20 6761 696e 2061 6363  ant! To gain acc
-000046d0: 6573 7320 6669 7273 7420 6070 6970 2069  ess first `pip i
-000046e0: 6e73 7461 6c6c 207a 6574 6173 6361 6c65  nstall zetascale
-000046f0: 6020 7468 656e 2072 756e 2060 7a65 7461  ` then run `zeta
-00004700: 202d 6860 2069 6e20 7468 6520 7465 726d   -h` in the term
-00004710: 696e 616c 2e20 5b48 6572 6520 6973 2074  inal. [Here is t
-00004720: 6865 2064 6f63 7320 666f 7220 6d6f 7265  he docs for more
-00004730: 5d28 6874 7470 733a 2f2f 7a65 7461 2e61  ](https://zeta.a
-00004740: 7061 632e 6169 2f65 6e2f 6c61 7465 7374  pac.ai/en/latest
-00004750: 2f7a 6574 612f 636c 6f75 642f 6d61 696e  /zeta/cloud/main
-00004760: 2f29 5c6e 5c6e 2d20 466c 6578 6962 6c65  /)\n\n- Flexible
-00004770: 2050 7269 6369 6e67 2077 6974 6820 706f   Pricing with po
-00004780: 6f6c 696e 6720 6672 6f6d 206d 616e 7920  oling from many 
-00004790: 636c 6f75 6473 5c6e 2d20 4561 7379 2044  clouds\n- Easy D
-000047a0: 6570 6c6f 796d 656e 7420 7769 7468 2031  eployment with 1
-000047b0: 2063 6c69 636b 5c6e 2d20 5661 7269 6f75   click\n- Variou
-000047c0: 7320 6f70 7469 6f6e 7320 666f 7220 636c  s options for cl
-000047d0: 6f75 6420 7072 6f76 6964 6572 7321 5c6e  oud providers!\n
-000047e0: 5c6e 6060 6062 6173 685c 6e5a 6574 6163  \n```bash\nZetac
-000047f0: 6c6f 7564 2043 4c49 5c6e 5c6e 6f70 7469  loud CLI\n\nopti
-00004800: 6f6e 733a 5c6e 2020 2d68 2c20 2d2d 6865  ons:\n  -h, --he
-00004810: 6c70 2020 2020 2020 2020 2020 2020 7368  lp            sh
-00004820: 6f77 2074 6869 7320 6865 6c70 206d 6573  ow this help mes
-00004830: 7361 6765 2061 6e64 2065 7869 745c 6e20  sage and exit\n 
-00004840: 202d 7420 5441 534b 5f4e 414d 452c 202d   -t TASK_NAME, -
-00004850: 2d74 6173 6b5f 6e61 6d65 2054 4153 4b5f  -task_name TASK_
-00004860: 4e41 4d45 5c6e 2020 2020 2020 2020 2020  NAME\n          
-00004870: 2020 2020 2020 2020 2020 2020 2020 5461                Ta
-00004880: 736b 206e 616d 655c 6e20 202d 6320 434c  sk name\n  -c CL
-00004890: 5553 5445 525f 4e41 4d45 2c20 2d2d 636c  USTER_NAME, --cl
-000048a0: 7573 7465 725f 6e61 6d65 2043 4c55 5354  uster_name CLUST
-000048b0: 4552 5f4e 414d 455c 6e20 2020 2020 2020  ER_NAME\n       
-000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048d0: 2043 6c75 7374 6572 206e 616d 655c 6e20   Cluster name\n 
-000048e0: 202d 636c 2043 4c4f 5544 2c20 2d2d 636c   -cl CLOUD, --cl
-000048f0: 6f75 6420 434c 4f55 445c 6e20 2020 2020  oud CLOUD\n     
-00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004910: 2020 2043 6c6f 7564 2070 726f 7669 6465     Cloud provide
-00004920: 725c 6e20 202d 6720 4750 5553 2c20 2d2d  r\n  -g GPUS, --
-00004930: 6770 7573 2047 5055 5320 2047 5055 735c  gpus GPUS  GPUs\
-00004940: 6e20 202d 6620 4649 4c45 4e41 4d45 2c20  n  -f FILENAME, 
-00004950: 2d2d 6669 6c65 6e61 6d65 2046 494c 454e  --filename FILEN
-00004960: 414d 455c 6e20 2020 2020 2020 2020 2020  AME\n           
-00004970: 2020 2020 2020 2020 2020 2020 2046 696c               Fil
-00004980: 656e 616d 655c 6e20 202d 732c 202d 2d73  ename\n  -s, --s
-00004990: 746f 7020 2020 2020 2020 2020 2020 2053  top            S
-000049a0: 746f 7020 666c 6167 5c6e 2020 2d64 2c20  top flag\n  -d, 
-000049b0: 2d2d 646f 776e 2020 2020 2020 2020 2020  --down          
-000049c0: 2020 446f 776e 2066 6c61 675c 6e20 202d    Down flag\n  -
-000049d0: 7372 2c20 2d2d 7374 6174 7573 5f72 6570  sr, --status_rep
-000049e0: 6f72 7420 2053 7461 7475 7320 7265 706f  ort  Status repo
-000049f0: 7274 2066 6c61 675c 6e5c 6e60 6060 5c6e  rt flag\n\n```\n
-00004a00: 5c6e 2d20 4120 7369 6d70 6c65 2072 756e  \n- A simple run
-00004a10: 2065 7861 6d70 6c65 2063 6f64 6520 776f   example code wo
-00004a20: 756c 6420 6265 206c 696b 653a 5c6e 5c6e  uld be like:\n\n
-00004a30: 6060 6062 6173 685c 6e7a 6574 6120 2d66  ```bash\nzeta -f
-00004a40: 2074 7261 696e 2e70 7920 2d67 2041 3130   train.py -g A10
-00004a50: 303a 385c 6e60 6060 5c6e 2d2d 2d2d 5c6e  0:8\n```\n----\n
-00004a60: 5c6e 5c6e 2320 446f 6375 6d65 6e74 6174  \n\n# Documentat
-00004a70: 696f 6e5c 6e41 6c6c 2063 6c61 7373 6573  ion\nAll classes
-00004a80: 206d 7573 7420 6861 7665 2064 6f63 756d   must have docum
-00004a90: 656e 7461 7469 6f6e 2069 6620 796f 7520  entation if you 
-00004aa0: 7365 6520 6120 636c 6173 7320 6f72 2066  see a class or f
-00004ab0: 756e 6374 696f 6e20 7769 7468 6f75 7420  unction without 
-00004ac0: 646f 6375 6d65 6e74 6174 696f 6e20 7468  documentation th
-00004ad0: 656e 2070 6c65 6173 6520 7265 706f 7274  en please report
-00004ae0: 2069 7420 746f 206d 6520 6174 206b 7965   it to me at kye
-00004af0: 4061 7061 632e 6169 2c5c 6e5c 6e44 6f63  @apac.ai,\n\nDoc
-00004b00: 756d 656e 7461 7469 6f6e 2069 7320 6174  umentation is at
-00004b10: 205b 7a65 7461 2e61 7061 632e 6169 5d28   [zeta.apac.ai](
-00004b20: 6874 7470 733a 2f2f 7a65 7461 2e61 7061  https://zeta.apa
-00004b30: 632e 6169 2f29 5c6e 5c6e 5c6e 2d2d 2d2d  c.ai/)\n\n\n----
-00004b40: 2d2d 2d5c 6e5c 6e5c 6e23 2052 756e 6e69  ---\n\n\n# Runni
-00004b50: 6e67 2074 6573 7473 5c6e 596f 7520 7368  ng tests\nYou sh
-00004b60: 6f75 6c64 2069 6e73 7461 6c6c 2074 6865  ould install the
-00004b70: 2070 7265 2d63 6f6d 6d69 7420 686f 6f6b   pre-commit hook
-00004b80: 7320 7769 7468 2070 7265 2d63 6f6d 6d69  s with pre-commi
-00004b90: 7420 696e 7374 616c 6c2e 2054 6869 7320  t install. This 
-00004ba0: 7769 6c6c 2072 756e 2074 6865 206c 696e  will run the lin
-00004bb0: 7465 722c 206d 7970 792c 2061 6e64 2061  ter, mypy, and a
-00004bc0: 2073 7562 7365 7420 6f66 2074 6865 2074   subset of the t
-00004bd0: 6573 7473 206f 6e20 6576 6572 7920 636f  ests on every co
-00004be0: 6d6d 6974 2e5c 6e5c 6e46 6f72 206d 6f72  mmit.\n\nFor mor
-00004bf0: 6520 6578 616d 706c 6573 206f 6e20 686f  e examples on ho
-00004c00: 7720 746f 2072 756e 2074 6865 2066 756c  w to run the ful
-00004c10: 6c20 7465 7374 2073 7569 7465 2070 6c65  l test suite ple
-00004c20: 6173 6520 7265 6665 7220 746f 2074 6865  ase refer to the
-00004c30: 2043 4920 776f 726b 666c 6f77 2e5c 6e5c   CI workflow.\n\
-00004c40: 6e53 6f6d 6520 6578 616d 706c 6573 206f  nSome examples o
-00004c50: 6620 7275 6e6e 696e 6720 7465 7374 7320  f running tests 
-00004c60: 6c6f 6361 6c6c 793a 5c6e 5c6e 6060 6062  locally:\n\n```b
-00004c70: 6173 685c 6e70 7974 686f 6e33 202d 6d20  ash\npython3 -m 
-00004c80: 7069 7020 696e 7374 616c 6c20 2d65 205c  pip install -e \
-00004c90: 272e 5b74 6573 7469 6e67 5d5c 2720 2023  '.[testing]\'  #
-00004ca0: 2069 6e73 7461 6c6c 2065 7874 7261 2064   install extra d
-00004cb0: 6570 7320 666f 7220 7465 7374 696e 675c  eps for testing\
-00004cc0: 6e70 7974 686f 6e33 202d 6d20 7079 7465  npython3 -m pyte
-00004cd0: 7374 2074 6573 7473 2f20 2020 2020 2020  st tests/       
-00004ce0: 2020 2020 2020 2020 2020 2320 7768 6f6c            # whol
-00004cf0: 6520 7465 7374 2073 7569 7465 5c6e 6060  e test suite\n``
-00004d00: 605c 6e2d 2d2d 2d5c 6e5c 6e23 2320 436f  `\n----\n\n## Co
-00004d10: 6d6d 756e 6974 795c 6e5c 6e4a 6f69 6e20  mmunity\n\nJoin 
-00004d20: 6f75 7220 6772 6f77 696e 6720 636f 6d6d  our growing comm
-00004d30: 756e 6974 7920 6172 6f75 6e64 2074 6865  unity around the
-00004d40: 2077 6f72 6c64 2c20 666f 7220 7265 616c   world, for real
-00004d50: 2d74 696d 6520 7375 7070 6f72 742c 2069  -time support, i
-00004d60: 6465 6173 2c20 616e 6420 6469 7363 7573  deas, and discus
-00004d70: 7369 6f6e 7320 6f6e 2068 6f77 2074 6f20  sions on how to 
-00004d80: 6275 696c 6420 6265 7474 6572 206d 6f64  build better mod
-00004d90: 656c 7320 f09f 988a 205c 6e5c 6e2d 2056  els .... \n\n- V
-00004da0: 6965 7720 6f75 7220 6f66 6669 6369 616c  iew our official
-00004db0: 205b 446f 6373 5d28 6874 7470 733a 2f2f   [Docs](https://
-00004dc0: 7a65 7461 2e61 7061 632e 6169 295c 6e2d  zeta.apac.ai)\n-
-00004dd0: 2043 6861 7420 6c69 7665 2077 6974 6820   Chat live with 
-00004de0: 7573 206f 6e20 5b44 6973 636f 7264 5d28  us on [Discord](
-00004df0: 6874 7470 733a 2f2f 6469 7363 6f72 642e  https://discord.
-00004e00: 6767 2f6b 5333 7277 4b73 335a 4329 5c6e  gg/kS3rwKs3ZC)\n
-00004e10: 2d20 466f 6c6c 6f77 2075 7320 6f6e 205b  - Follow us on [
-00004e20: 5477 6974 7465 725d 2868 7474 7073 3a2f  Twitter](https:/
-00004e30: 2f74 7769 7474 6572 2e63 6f6d 2f6b 7965  /twitter.com/kye
-00004e40: 676f 6d65 7a29 5c6e 2d20 436f 6e6e 6563  gomez)\n- Connec
-00004e50: 7420 7769 7468 2075 7320 6f6e 205b 4c69  t with us on [Li
-00004e60: 6e6b 6564 496e 5d28 6874 7470 733a 2f2f  nkedIn](https://
-00004e70: 7777 772e 6c69 6e6b 6564 696e 2e63 6f6d  www.linkedin.com
-00004e80: 2f63 6f6d 7061 6e79 2f74 6865 2d73 7761  /company/the-swa
-00004e90: 726d 2d63 6f72 706f 7261 7469 6f6e 295c  rm-corporation)\
-00004ea0: 6e2d 2056 6973 6974 2075 7320 6f6e 205b  n- Visit us on [
-00004eb0: 596f 7554 7562 655d 2868 7474 7073 3a2f  YouTube](https:/
-00004ec0: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
-00004ed0: 2f63 6861 6e6e 656c 2f55 4339 7958 7969  /channel/UC9yXyi
-00004ee0: 746b 6255 5f57 5379 3762 645f 3431 5371  tkbU_WSy7bd_41Sq
-00004ef0: 5129 5c6e 2d20 5b4a 6f69 6e20 7468 6520  Q)\n- [Join the 
-00004f00: 5377 6172 6d73 2063 6f6d 6d75 6e69 7479  Swarms community
-00004f10: 206f 6e20 4469 7363 6f72 6421 5d28 6874   on Discord!](ht
-00004f20: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
-00004f30: 2f41 4a61 7a42 6d68 4b6e 7229 5c6e 5c6e  /AJazBmhKnr)\n\n
-00004f40: 2d2d 2d5c 6e5c 6e23 20f0 9fa4 9d20 5363  ---\n\n# .... Sc
-00004f50: 6865 6475 6c65 2061 2031 2d6f 6e2d 3120  hedule a 1-on-1 
-00004f60: 5365 7373 696f 6e5c 6e57 616e 7420 746f  Session\nWant to
-00004f70: 2074 7261 696e 2061 2063 7573 746f 6d20   train a custom 
-00004f80: 4149 206d 6f64 656c 2066 6f72 2061 2072  AI model for a r
-00004f90: 6561 6c2d 776f 726c 6420 7461 736b 206c  eal-world task l
-00004fa0: 696b 6520 4765 6e65 7261 6c20 4d75 6c74  ike General Mult
-00004fb0: 692d 4d6f 6461 6c20 4d6f 6465 6c73 2c20  i-Modal Models, 
-00004fc0: 4661 6369 616c 2052 6563 6f67 6e69 7469  Facial Recogniti
-00004fd0: 6f6e 732c 2044 7275 6720 4469 7363 6f76  ons, Drug Discov
-00004fe0: 6572 792c 2048 756d 616e 6f69 6420 526f  ery, Humanoid Ro
-00004ff0: 626f 7469 6373 3f20 495c 276c 6c20 6865  botics? I\'ll he
-00005000: 6c70 2079 6f75 2063 7265 6174 6520 7468  lp you create th
-00005010: 6520 6d6f 6465 6c20 6172 6368 6974 6563  e model architec
-00005020: 7475 7265 2074 6865 6e20 7472 6169 6e20  ture then train 
-00005030: 7468 6520 6d6f 6465 6c20 616e 6420 7468  the model and th
-00005040: 656e 206f 7074 696d 697a 6520 6974 2074  en optimize it t
-00005050: 6f20 6d65 6574 2079 6f75 7220 7175 616c  o meet your qual
-00005060: 6974 7920 6173 7375 7261 6e63 6520 7374  ity assurance st
-00005070: 616e 6461 7264 732e 5c6e 5c6e 426f 6f6b  andards.\n\nBook
-00005080: 2061 205b 312d 6f6e 2d31 2053 6573 7369   a [1-on-1 Sessi
-00005090: 6f6e 2077 6974 6820 4b79 6520 6865 7265  on with Kye here
-000050a0: 2e5d 2868 7474 7073 3a2f 2f63 616c 656e  .](https://calen
-000050b0: 646c 792e 636f 6d2f 6170 6163 6169 2f61  dly.com/apacai/a
-000050c0: 676f 7261 292c 2074 6865 2043 7265 6174  gora), the Creat
-000050d0: 6f72 2c20 746f 2064 6973 6375 7373 2061  or, to discuss a
-000050e0: 6e79 2069 7373 7565 732c 2070 726f 7669  ny issues, provi
-000050f0: 6465 2066 6565 6462 6163 6b2c 206f 7220  de feedback, or 
-00005100: 6578 706c 6f72 6520 686f 7720 7765 2063  explore how we c
-00005110: 616e 2069 6d70 726f 7665 205a 6574 6120  an improve Zeta 
-00005120: 666f 7220 796f 7520 6f72 2068 656c 7020  for you or help 
-00005130: 796f 7520 6275 696c 6420 796f 7572 206f  you build your o
-00005140: 776e 2063 7573 746f 6d20 6d6f 6465 6c73  wn custom models
-00005150: 215c 6e5c 6e23 2320 f09f abb6 2043 6f6e  !\n\n## .... Con
-00005160: 7472 6962 7574 696f 6e73 3a5c 6e5c 6e54  tributions:\n\nT
-00005170: 6865 2065 6173 6965 7374 2077 6179 2074  he easiest way t
-00005180: 6f20 636f 6e74 7269 6275 7465 2069 7320  o contribute is 
-00005190: 746f 2070 6963 6b20 616e 7920 6973 7375  to pick any issu
-000051a0: 6520 7769 7468 2074 6865 2060 676f 6f64  e with the `good
-000051b0: 2066 6972 7374 2069 7373 7565 6020 7461   first issue` ta
-000051c0: 6720 f09f 92aa 2e20 5265 6164 2074 6865  g ..... Read the
-000051d0: 2043 6f6e 7472 6962 7574 696e 6720 6775   Contributing gu
-000051e0: 6964 656c 696e 6573 205b 6865 7265 5d28  idelines [here](
-000051f0: 2f43 4f4e 5452 4942 5554 494e 472e 6d64  /CONTRIBUTING.md
-00005200: 292e 2042 7567 2052 6570 6f72 743f 205b  ). Bug Report? [
-00005210: 4669 6c65 2068 6572 655d 2868 7474 7073  File here](https
-00005220: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b79  ://github.com/ky
-00005230: 6567 6f6d 657a 2f7a 6574 612f 6973 7375  egomez/zeta/issu
-00005240: 6573 2f6e 6577 2f63 686f 6f73 6529 207c  es/new/choose) |
-00005250: 2046 6561 7475 7265 2052 6571 7565 7374   Feature Request
-00005260: 3f20 5b46 696c 6520 6865 7265 5d28 6874  ? [File here](ht
-00005270: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00005280: 2f6b 7965 676f 6d65 7a2f 7a65 7461 2f69  /kyegomez/zeta/i
-00005290: 7373 7565 732f 6e65 772f 6368 6f6f 7365  ssues/new/choose
-000052a0: 295c 6e5c 6e5a 6574 6120 6973 2061 6e20  )\n\nZeta is an 
-000052b0: 6f70 656e 2d73 6f75 7263 6520 7072 6f6a  open-source proj
-000052c0: 6563 742c 2061 6e64 2063 6f6e 7472 6962  ect, and contrib
-000052d0: 7574 696f 6e73 2061 7265 2056 4552 5920  utions are VERY 
-000052e0: 7765 6c63 6f6d 652e 2049 6620 796f 7520  welcome. If you 
-000052f0: 7761 6e74 2074 6f20 636f 6e74 7269 6275  want to contribu
-00005300: 7465 2c20 796f 7520 6361 6e20 6372 6561  te, you can crea
-00005310: 7465 206e 6577 2066 6561 7475 7265 732c  te new features,
-00005320: 2066 6978 2062 7567 732c 206f 7220 696d   fix bugs, or im
-00005330: 7072 6f76 6520 7468 6520 696e 6672 6173  prove the infras
-00005340: 7472 7563 7475 7265 2e20 506c 6561 7365  tructure. Please
-00005350: 2072 6566 6572 2074 6f20 7468 6520 5b43   refer to the [C
-00005360: 4f4e 5452 4942 5554 494e 472e 6d64 5d28  ONTRIBUTING.md](
-00005370: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00005380: 6f6d 2f6b 7965 676f 6d65 7a2f 7a65 7461  om/kyegomez/zeta
-00005390: 2f62 6c6f 622f 6d61 7374 6572 2f43 4f4e  /blob/master/CON
-000053a0: 5452 4942 5554 494e 472e 6d64 2920 616e  TRIBUTING.md) an
-000053b0: 6420 6f75 7220 5b63 6f6e 7472 6962 7574  d our [contribut
-000053c0: 696e 6720 626f 6172 645d 2868 7474 7073  ing board](https
-000053d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7573  ://github.com/us
-000053e0: 6572 732f 6b79 6567 6f6d 657a 2f70 726f  ers/kyegomez/pro
-000053f0: 6a65 6374 732f 3129 2074 6f20 7061 7274  jects/1) to part
-00005400: 6963 6970 6174 6520 696e 2052 6f61 646d  icipate in Roadm
-00005410: 6170 2064 6973 6375 7373 696f 6e73 215c  ap discussions!\
-00005420: 6e5c 6e3c 6120 6872 6566 3d22 6874 7470  n\n<a href="http
-00005430: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-00005440: 7965 676f 6d65 7a2f 7a65 7461 2f67 7261  yegomez/zeta/gra
-00005450: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
-00005460: 223e 5c6e 2020 3c69 6d67 2073 7263 3d22  ">\n  <img src="
-00005470: 6874 7470 733a 2f2f 636f 6e74 7269 622e  https://contrib.
-00005480: 726f 636b 732f 696d 6167 653f 7265 706f  rocks/image?repo
-00005490: 3d6b 7965 676f 6d65 7a2f 7a65 7461 2220  =kyegomez/zeta" 
-000054a0: 2f3e 5c6e 3c2f 613e 5c6e 5c6e 2d2d 2d2d  />\n</a>\n\n----
-000054b0: 5c6e 5c6e 2323 2041 6363 656c 6572 6174  \n\n## Accelerat
-000054c0: 6520 4261 636b 6c6f 675c 6e48 656c 7020  e Backlog\nHelp 
-000054d0: 7573 2061 6363 656c 6572 6174 6520 6f75  us accelerate ou
-000054e0: 7220 6261 636b 6c6f 6720 6279 2073 7570  r backlog by sup
-000054f0: 706f 7274 696e 6720 7573 2066 696e 616e  porting us finan
-00005500: 6369 616c 6c79 2120 4e6f 7465 2c20 7765  cially! Note, we
-00005510: 5c27 7265 2061 6e20 6f70 656e 2073 6f75  \'re an open sou
-00005520: 7263 6520 636f 7270 6f72 6174 696f 6e20  rce corporation 
-00005530: 616e 6420 736f 2061 6c6c 2074 6865 2072  and so all the r
-00005540: 6576 656e 7565 2077 6520 6765 6e65 7261  evenue we genera
-00005550: 7465 2069 7320 7468 726f 7567 6820 646f  te is through do
-00005560: 6e61 7469 6f6e 7320 6174 2074 6865 206d  nations at the m
-00005570: 6f6d 656e 7420 3b29 5c6e 5c6e 3c61 2068  oment ;)\n\n<a h
-00005580: 7265 663d 2268 7474 7073 3a2f 2f70 6f6c  ref="https://pol
-00005590: 6172 2e73 682f 6b79 6567 6f6d 657a 223e  ar.sh/kyegomez">
-000055a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000055b0: 2f2f 706f 6c61 722e 7368 2f65 6d62 6564  //polar.sh/embed
-000055c0: 2f66 756e 642d 6f75 722d 6261 636b 6c6f  /fund-our-backlo
-000055d0: 672e 7376 673f 6f72 673d 6b79 6567 6f6d  g.svg?org=kyegom
-000055e0: 657a 2220 2f3e 3c2f 613e 5c6e 5c6e 5c6e  ez" /></a>\n\n\n
-000055f0: 2320 4c69 6365 6e73 6520 5c6e 2d20 4170  # License \n- Ap
-00005600: 6163 6865 5c6e 272c 0a20 2020 2027 6175  ache\n',.    'au
-00005610: 7468 6f72 273a 2027 5a65 7461 2054 6561  thor': 'Zeta Tea
-00005620: 6d27 2c0a 2020 2020 2761 7574 686f 725f  m',.    'author_
-00005630: 656d 6169 6c27 3a20 276b 7965 4061 7061  email': 'kye@apa
-00005640: 632e 6169 272c 0a20 2020 2027 6d61 696e  c.ai',.    'main
-00005650: 7461 696e 6572 273a 2027 4e6f 6e65 272c  tainer': 'None',
-00005660: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-00005670: 5f65 6d61 696c 273a 2027 4e6f 6e65 272c  _email': 'None',
-00005680: 0a20 2020 2027 7572 6c27 3a20 2768 7474  .    'url': 'htt
-00005690: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000056a0: 6b79 6567 6f6d 657a 2f7a 6574 6127 2c0a  kyegomez/zeta',.
-000056b0: 2020 2020 2770 6163 6b61 6765 7327 3a20      'packages': 
-000056c0: 7061 636b 6167 6573 2c0a 2020 2020 2770  packages,.    'p
-000056d0: 6163 6b61 6765 5f64 6174 6127 3a20 7061  ackage_data': pa
-000056e0: 636b 6167 655f 6461 7461 2c0a 2020 2020  ckage_data,.    
-000056f0: 2769 6e73 7461 6c6c 5f72 6571 7569 7265  'install_require
-00005700: 7327 3a20 696e 7374 616c 6c5f 7265 7175  s': install_requ
-00005710: 6972 6573 2c0a 2020 2020 2765 6e74 7279  ires,.    'entry
-00005720: 5f70 6f69 6e74 7327 3a20 656e 7472 795f  _points': entry_
-00005730: 706f 696e 7473 2c0a 2020 2020 2770 7974  points,.    'pyt
-00005740: 686f 6e5f 7265 7175 6972 6573 273a 2027  hon_requires': '
-00005750: 3e3d 332e 3130 2c3c 342e 3027 2c0a 7d0a  >=3.10,<4.0',.}.
-00005760: 0a0a 7365 7475 7028 2a2a 7365 7475 705f  ..setup(**setup_
-00005770: 6b77 6172 6773 290a                      kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7a65 7461  : 2.1.Name: zeta
+00000020: 7363 616c 650a 5665 7273 696f 6e3a 2032  scale.Version: 2
+00000030: 2e35 2e31 0a53 756d 6d61 7279 3a20 5261  .5.1.Summary: Ra
+00000040: 7069 646c 7920 4275 696c 642c 204f 7074  pidly Build, Opt
+00000050: 696d 697a 652c 2061 6e64 2044 6570 6c6f  imize, and Deplo
+00000060: 7920 534f 5441 2041 4920 4d6f 6465 6c73  y SOTA AI Models
+00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
+00000080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+00000090: 7965 676f 6d65 7a2f 7a65 7461 0a4c 6963  yegomez/zeta.Lic
+000000a0: 656e 7365 3a20 4d49 540a 4b65 7977 6f72  ense: MIT.Keywor
+000000b0: 6473 3a20 5472 616e 7366 6f72 6d65 7273  ds: Transformers
+000000c0: 2c7a 6574 6120 7363 616c 650a 4175 7468  ,zeta scale.Auth
+000000d0: 6f72 3a20 5a65 7461 2054 6561 6d0a 4175  or: Zeta Team.Au
+000000e0: 7468 6f72 2d65 6d61 696c 3a20 6b79 6540  thor-email: kye@
+000000f0: 6170 6163 2e61 690a 5265 7175 6972 6573  apac.ai.Requires
+00000100: 2d50 7974 686f 6e3a 203e 3d33 2e31 302c  -Python: >=3.10,
+00000110: 3c34 2e30 0a43 6c61 7373 6966 6965 723a  <4.0.Classifier:
+00000120: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+00000130: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000140: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+00000150: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000160: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000170: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
+00000180: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000190: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001a0: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+000001b0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001c0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001d0: 7974 686f 6e20 3a3a 2033 2e31 310a 436c  ython :: 3.11.Cl
+000001e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000001f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000200: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
+00000210: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000220: 6163 6365 6c65 7261 7465 2028 3d3d 302e  accelerate (==0.
+00000230: 3330 2e31 290a 5265 7175 6972 6573 2d44  30.1).Requires-D
+00000240: 6973 743a 2061 7267 7061 7273 6520 283e  ist: argparse (>
+00000250: 3d31 2e34 2e30 2c3c 322e 302e 3029 0a52  =1.4.0,<2.0.0).R
+00000260: 6571 7569 7265 732d 4469 7374 3a20 6265  equires-Dist: be
+00000270: 6172 7479 7065 2028 3d3d 302e 3137 2e32  artype (==0.17.2
+00000280: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+00000290: 2062 6974 7361 6e64 6279 7465 7320 283d   bitsandbytes (=
+000002a0: 3d30 2e34 332e 3029 0a52 6571 7569 7265  =0.43.0).Require
+000002b0: 732d 4469 7374 3a20 636f 6c74 352d 6174  s-Dist: colt5-at
+000002c0: 7465 6e74 696f 6e0a 5265 7175 6972 6573  tention.Requires
+000002d0: 2d44 6973 743a 2064 6174 6173 6574 730a  -Dist: datasets.
+000002e0: 5265 7175 6972 6573 2d44 6973 743a 2065  Requires-Dist: e
+000002f0: 696e 6f70 7320 283d 3d30 2e37 2e30 290a  inops (==0.7.0).
+00000300: 5265 7175 6972 6573 2d44 6973 743a 2065  Requires-Dist: e
+00000310: 696e 6f70 732d 6578 7473 2028 3d3d 302e  inops-exts (==0.
+00000320: 302e 3429 0a52 6571 7569 7265 732d 4469  0.4).Requires-Di
+00000330: 7374 3a20 6c6f 6361 6c2d 6174 7465 6e74  st: local-attent
+00000340: 696f 6e0a 5265 7175 6972 6573 2d44 6973  ion.Requires-Dis
+00000350: 743a 206c 6f67 7572 750a 5265 7175 6972  t: loguru.Requir
+00000360: 6573 2d44 6973 743a 2070 7974 6573 7420  es-Dist: pytest 
+00000370: 283d 3d38 2e32 2e31 290a 5265 7175 6972  (==8.2.1).Requir
+00000380: 6573 2d44 6973 743a 2072 6963 6820 283d  es-Dist: rich (=
+00000390: 3d31 332e 372e 3129 0a52 6571 7569 7265  =13.7.1).Require
+000003a0: 732d 4469 7374 3a20 7363 6970 7920 283d  s-Dist: scipy (=
+000003b0: 3d31 2e39 2e33 290a 5265 7175 6972 6573  =1.9.3).Requires
+000003c0: 2d44 6973 743a 2074 6f72 6368 2028 3e3d  -Dist: torch (>=
+000003d0: 322e 312e 312c 3c33 2e30 290a 5265 7175  2.1.1,<3.0).Requ
+000003e0: 6972 6573 2d44 6973 743a 2074 6f72 6368  ires-Dist: torch
+000003f0: 6669 780a 5265 7175 6972 6573 2d44 6973  fix.Requires-Dis
+00000400: 743a 2074 6f72 6368 7669 7369 6f6e 2028  t: torchvision (
+00000410: 3d3d 302e 3138 2e30 290a 5265 7175 6972  ==0.18.0).Requir
+00000420: 6573 2d44 6973 743a 2074 7164 6d20 283d  es-Dist: tqdm (=
+00000430: 3d34 2e36 362e 3329 0a52 6571 7569 7265  =4.66.3).Require
+00000440: 732d 4469 7374 3a20 7472 616e 7366 6f72  s-Dist: transfor
+00000450: 6d65 7273 2028 3d3d 342e 3431 2e30 290a  mers (==4.41.0).
+00000460: 5265 7175 6972 6573 2d44 6973 743a 2076  Requires-Dist: v
+00000470: 6563 746f 722d 7175 616e 7469 7a65 2d70  ector-quantize-p
+00000480: 7974 6f72 6368 2028 3d3d 312e 3134 2e37  ytorch (==1.14.7
+00000490: 290a 4465 7363 7269 7074 696f 6e2d 436f  ).Description-Co
+000004a0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+000004b0: 2f6d 6172 6b64 6f77 6e0a 0a5b 215b 4d75  /markdown..[![Mu
+000004c0: 6c74 692d 4d6f 6461 6c69 7479 5d28 696d  lti-Modality](im
+000004d0: 6167 6573 2f61 676f 7261 6261 6e6e 6572  ages/agorabanner
+000004e0: 2e70 6e67 295d 2868 7474 7073 3a2f 2f64  .png)](https://d
+000004f0: 6973 636f 7264 2e67 672f 7155 7478 6e4b  iscord.gg/qUtxnK
+00000500: 324e 4d66 290a 0a21 5b5a 6574 6120 6261  2NMf)..![Zeta ba
+00000510: 6e6e 6572 5d28 696d 6167 6573 2f7a 6574  nner](images/zet
+00000520: 612e 706e 6729 0a42 7569 6c64 2053 4f54  a.png).Build SOT
+00000530: 4120 4149 204d 6f64 656c 7320 3830 2520  A AI Models 80% 
+00000540: 6661 7374 6572 2077 6974 6820 6d6f 6475  faster with modu
+00000550: 6c61 722c 2068 6967 682d 7065 7266 6f72  lar, high-perfor
+00000560: 6d61 6e63 652c 2061 6e64 2073 6361 6c61  mance, and scala
+00000570: 626c 6520 6275 696c 6469 6e67 2062 6c6f  ble building blo
+00000580: 636b 7321 0a0a 5b21 5b44 6f63 735d 2868  cks!..[![Docs](h
+00000590: 7474 7073 3a2f 2f72 6561 6474 6865 646f  ttps://readthedo
+000005a0: 6373 2e6f 7267 2f70 726f 6a65 6374 732f  cs.org/projects/
+000005b0: 7a65 7461 2f62 6164 6765 2f29 5d28 6874  zeta/badge/)](ht
+000005c0: 7470 733a 2f2f 7a65 7461 2e72 6561 6474  tps://zeta.readt
+000005d0: 6865 646f 6373 2e69 6f29 0a0a 3c70 3e0a  hedocs.io)..<p>.
+000005e0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000005f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b79  ://github.com/ky
+00000600: 6567 6f6d 657a 2f7a 6574 612f 626c 6f62  egomez/zeta/blob
+00000610: 2f6d 6169 6e2f 4c49 4345 4e53 4522 3e3c  /main/LICENSE"><
+00000620: 696d 6720 616c 743d 224d 4954 204c 6963  img alt="MIT Lic
+00000630: 656e 7365 2220 7372 633d 2268 7474 7073  ense" src="https
+00000640: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000650: 6f2f 6261 6467 652f 6c69 6365 6e73 652d  o/badge/license-
+00000660: 4d49 542d 626c 7565 2e73 7667 2220 2f3e  MIT-blue.svg" />
+00000670: 3c2f 613e 0a20 203c 6120 6872 6566 3d22  </a>.  <a href="
+00000680: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000690: 2f70 726f 6a65 6374 2f7a 6574 6173 6361  /project/zetasca
+000006a0: 6c65 223e 3c69 6d67 2061 6c74 3d22 4d49  le"><img alt="MI
+000006b0: 5420 4c69 6365 6e73 6522 2073 7263 3d22  T License" src="
+000006c0: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+000006d0: 7279 2e69 6f2f 7079 2f7a 6574 6173 6361  ry.io/py/zetasca
+000006e0: 6c65 2e73 7667 2220 2f3e 3c2f 613e 0a3c  le.svg" /></a>.<
+000006f0: 2f70 3e0a 0a5b 215b 4769 7448 7562 2069  /p>..[![GitHub i
+00000700: 7373 7565 735d 2868 7474 7073 3a2f 2f69  ssues](https://i
+00000710: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000720: 7468 7562 2f69 7373 7565 732f 6b79 6567  thub/issues/kyeg
+00000730: 6f6d 657a 2f7a 6574 6129 5d28 6874 7470  omez/zeta)](http
+00000740: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+00000750: 7965 676f 6d65 7a2f 7a65 7461 2f69 7373  yegomez/zeta/iss
+00000760: 7565 7329 205b 215b 4769 7448 7562 2066  ues) [![GitHub f
+00000770: 6f72 6b73 5d28 6874 7470 733a 2f2f 696d  orks](https://im
+00000780: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000790: 6875 622f 666f 726b 732f 6b79 6567 6f6d  hub/forks/kyegom
+000007a0: 657a 2f7a 6574 6129 5d28 6874 7470 733a  ez/zeta)](https:
+000007b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 7965  //github.com/kye
+000007c0: 676f 6d65 7a2f 7a65 7461 2f6e 6574 776f  gomez/zeta/netwo
+000007d0: 726b 2920 5b21 5b47 6974 4875 6220 7374  rk) [![GitHub st
+000007e0: 6172 735d 2868 7474 7073 3a2f 2f69 6d67  ars](https://img
+000007f0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000800: 7562 2f73 7461 7273 2f6b 7965 676f 6d65  ub/stars/kyegome
+00000810: 7a2f 7a65 7461 295d 2868 7474 7073 3a2f  z/zeta)](https:/
+00000820: 2f67 6974 6875 622e 636f 6d2f 6b79 6567  /github.com/kyeg
+00000830: 6f6d 657a 2f7a 6574 612f 7374 6172 6761  omez/zeta/starga
+00000840: 7a65 7273 2920 5b21 5b47 6974 4875 6220  zers) [![GitHub 
+00000850: 6c69 6365 6e73 655d 2868 7474 7073 3a2f  license](https:/
+00000860: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000870: 6769 7468 7562 2f6c 6963 656e 7365 2f6b  github/license/k
+00000880: 7965 676f 6d65 7a2f 7a65 7461 295d 2868  yegomez/zeta)](h
+00000890: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000008a0: 6d2f 6b79 6567 6f6d 657a 2f7a 6574 612f  m/kyegomez/zeta/
+000008b0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+000008c0: 4529 5b21 5b47 6974 4875 6220 7374 6172  E)[![GitHub star
+000008d0: 2063 6861 7274 5d28 6874 7470 733a 2f2f   chart](https://
+000008e0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+000008f0: 6974 6875 622f 7374 6172 732f 6b79 6567  ithub/stars/kyeg
+00000900: 6f6d 657a 2f7a 6574 613f 7374 796c 653d  omez/zeta?style=
+00000910: 736f 6369 616c 295d 2868 7474 7073 3a2f  social)](https:/
+00000920: 2f73 7461 722d 6869 7374 6f72 792e 636f  /star-history.co
+00000930: 6d2f 236b 7965 676f 6d65 7a2f 7a65 7461  m/#kyegomez/zeta
+00000940: 295b 215b 4465 7065 6e64 656e 6379 2053  )[![Dependency S
+00000950: 7461 7475 735d 2868 7474 7073 3a2f 2f69  tatus](https://i
+00000960: 6d67 2e73 6869 656c 6473 2e69 6f2f 6c69  mg.shields.io/li
+00000970: 6272 6172 6965 7369 6f2f 6769 7468 7562  brariesio/github
+00000980: 2f6b 7965 676f 6d65 7a2f 7a65 7461 295d  /kyegomez/zeta)]
+00000990: 2868 7474 7073 3a2f 2f6c 6962 7261 7269  (https://librari
+000009a0: 6573 2e69 6f2f 6769 7468 7562 2f6b 7965  es.io/github/kye
+000009b0: 676f 6d65 7a2f 7a65 7461 2920 5b21 5b44  gomez/zeta) [![D
+000009c0: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+000009d0: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
+000009e0: 6368 2f62 6164 6765 2f7a 6574 612f 6d6f  ch/badge/zeta/mo
+000009f0: 6e74 6829 5d28 6874 7470 733a 2f2f 7065  nth)](https://pe
+00000a00: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
+00000a10: 7a65 7461 290a 0a5b 215b 4a6f 696e 2074  zeta)..[![Join t
+00000a20: 6865 2041 676f 7261 2064 6973 636f 7264  he Agora discord
+00000a30: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000a40: 6965 6c64 732e 696f 2f64 6973 636f 7264  ields.io/discord
+00000a50: 2f31 3131 3039 3130 3237 3731 3130 3734  /111091027711074
+00000a60: 3331 3033 3f6c 6162 656c 3d44 6973 636f  3103?label=Disco
+00000a70: 7264 266c 6f67 6f3d 6469 7363 6f72 6426  rd&logo=discord&
+00000a80: 6c6f 676f 436f 6c6f 723d 7768 6974 6526  logoColor=white&
+00000a90: 7374 796c 653d 706c 6173 7469 6326 636f  style=plastic&co
+00000aa0: 6c6f 723d 6437 6230 3233 2921 5b53 6861  lor=d7b023)![Sha
+00000ab0: 7265 206f 6e20 5477 6974 7465 725d 2868  re on Twitter](h
+00000ac0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000ad0: 6473 2e69 6f2f 7477 6974 7465 722f 7572  ds.io/twitter/ur
+00000ae0: 6c2f 6874 7470 732f 7477 6974 7465 722e  l/https/twitter.
+00000af0: 636f 6d2f 636c 6f75 6470 6f73 7365 2e73  com/cloudposse.s
+00000b00: 7667 3f73 7479 6c65 3d73 6f63 6961 6c26  vg?style=social&
+00000b10: 6c61 6265 6c3d 5368 6172 6525 3230 2534  label=Share%20%4
+00000b20: 306b 7965 676f 6d65 7a2f 7a65 7461 295d  0kyegomez/zeta)]
+00000b30: 2868 7474 7073 3a2f 2f74 7769 7474 6572  (https://twitter
+00000b40: 2e63 6f6d 2f69 6e74 656e 742f 7477 6565  .com/intent/twee
+00000b50: 743f 7465 7874 3d43 6865 636b 2532 306f  t?text=Check%20o
+00000b60: 7574 2532 3074 6869 7325 3230 616d 617a  ut%20this%20amaz
+00000b70: 696e 6725 3230 4149 2532 3070 726f 6a65  ing%20AI%20proje
+00000b80: 6374 3a25 3230 2675 726c 3d68 7474 7073  ct:%20&url=https
+00000b90: 2533 4125 3246 2532 4667 6974 6875 622e  %3A%2F%2Fgithub.
+00000ba0: 636f 6d25 3246 6b79 6567 6f6d 657a 2532  com%2Fkyegomez%2
+00000bb0: 467a 6574 6129 205b 215b 5368 6172 6520  Fzeta) [![Share 
+00000bc0: 6f6e 2046 6163 6562 6f6f 6b5d 2868 7474  on Facebook](htt
+00000bd0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000be0: 2e69 6f2f 6261 6467 652f 5368 6172 652d  .io/badge/Share-
+00000bf0: 2532 3066 6163 6562 6f6f 6b2d 626c 7565  %20facebook-blue
+00000c00: 295d 2868 7474 7073 3a2f 2f77 7777 2e66  )](https://www.f
+00000c10: 6163 6562 6f6f 6b2e 636f 6d2f 7368 6172  acebook.com/shar
+00000c20: 6572 2f73 6861 7265 722e 7068 703f 753d  er/sharer.php?u=
+00000c30: 6874 7470 7325 3341 2532 4625 3246 6769  https%3A%2F%2Fgi
+00000c40: 7468 7562 2e63 6f6d 2532 466b 7965 676f  thub.com%2Fkyego
+00000c50: 6d65 7a25 3246 7a65 7461 2920 5b21 5b53  mez%2Fzeta) [![S
+00000c60: 6861 7265 206f 6e20 4c69 6e6b 6564 496e  hare on LinkedIn
+00000c70: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000c80: 6965 6c64 732e 696f 2f62 6164 6765 2f53  ields.io/badge/S
+00000c90: 6861 7265 2d25 3230 6c69 6e6b 6564 696e  hare-%20linkedin
+00000ca0: 2d62 6c75 6529 5d28 6874 7470 733a 2f2f  -blue)](https://
+00000cb0: 7777 772e 6c69 6e6b 6564 696e 2e63 6f6d  www.linkedin.com
+00000cc0: 2f73 6861 7265 4172 7469 636c 653f 6d69  /shareArticle?mi
+00000cd0: 6e69 3d74 7275 6526 7572 6c3d 6874 7470  ni=true&url=http
+00000ce0: 7325 3341 2532 4625 3246 6769 7468 7562  s%3A%2F%2Fgithub
+00000cf0: 2e63 6f6d 2532 466b 7965 676f 6d65 7a25  .com%2Fkyegomez%
+00000d00: 3246 7a65 7461 2674 6974 6c65 3d26 7375  2Fzeta&title=&su
+00000d10: 6d6d 6172 793d 2673 6f75 7263 653d 290a  mmary=&source=).
+00000d20: 0a5b 215b 5368 6172 6520 6f6e 2052 6564  .[![Share on Red
+00000d30: 6469 745d 2868 7474 7073 3a2f 2f69 6d67  dit](https://img
+00000d40: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000d50: 652f 2d53 6861 7265 2532 306f 6e25 3230  e/-Share%20on%20
+00000d60: 5265 6464 6974 2d6f 7261 6e67 6529 5d28  Reddit-orange)](
+00000d70: 6874 7470 733a 2f2f 7777 772e 7265 6464  https://www.redd
+00000d80: 6974 2e63 6f6d 2f73 7562 6d69 743f 7572  it.com/submit?ur
+00000d90: 6c3d 6874 7470 7325 3341 2532 4625 3246  l=https%3A%2F%2F
+00000da0: 6769 7468 7562 2e63 6f6d 2532 466b 7965  github.com%2Fkye
+00000db0: 676f 6d65 7a25 3246 7a65 7461 2674 6974  gomez%2Fzeta&tit
+00000dc0: 6c65 3d7a 6574 6125 3230 2d25 3230 7468  le=zeta%20-%20th
+00000dd0: 6525 3230 6675 7475 7265 2532 306f 6625  e%20future%20of%
+00000de0: 3230 4149 2920 5b21 5b53 6861 7265 206f  20AI) [![Share o
+00000df0: 6e20 4861 636b 6572 204e 6577 735d 2868  n Hacker News](h
+00000e00: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000e10: 6473 2e69 6f2f 6261 6467 652f 2d53 6861  ds.io/badge/-Sha
+00000e20: 7265 2532 306f 6e25 3230 4861 636b 6572  re%20on%20Hacker
+00000e30: 2532 304e 6577 732d 6f72 616e 6765 295d  %20News-orange)]
+00000e40: 2868 7474 7073 3a2f 2f6e 6577 732e 7963  (https://news.yc
+00000e50: 6f6d 6269 6e61 746f 722e 636f 6d2f 7375  ombinator.com/su
+00000e60: 626d 6974 6c69 6e6b 3f75 3d68 7474 7073  bmitlink?u=https
+00000e70: 2533 4125 3246 2532 4667 6974 6875 622e  %3A%2F%2Fgithub.
+00000e80: 636f 6d25 3246 6b79 6567 6f6d 657a 2532  com%2Fkyegomez%2
+00000e90: 467a 6574 6126 743d 7a65 7461 2532 302d  Fzeta&t=zeta%20-
+00000ea0: 2532 3074 6865 2532 3066 7574 7572 6525  %20the%20future%
+00000eb0: 3230 6f66 2532 3041 4929 205b 215b 5368  20of%20AI) [![Sh
+00000ec0: 6172 6520 6f6e 2050 696e 7465 7265 7374  are on Pinterest
+00000ed0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000ee0: 6965 6c64 732e 696f 2f62 6164 6765 2f2d  ields.io/badge/-
+00000ef0: 5368 6172 6525 3230 6f6e 2532 3050 696e  Share%20on%20Pin
+00000f00: 7465 7265 7374 2d72 6564 295d 2868 7474  terest-red)](htt
+00000f10: 7073 3a2f 2f70 696e 7465 7265 7374 2e63  ps://pinterest.c
+00000f20: 6f6d 2f70 696e 2f63 7265 6174 652f 6275  om/pin/create/bu
+00000f30: 7474 6f6e 2f3f 7572 6c3d 6874 7470 7325  tton/?url=https%
+00000f40: 3341 2532 4625 3246 6769 7468 7562 2e63  3A%2F%2Fgithub.c
+00000f50: 6f6d 2532 466b 7965 676f 6d65 7a25 3246  om%2Fkyegomez%2F
+00000f60: 7a65 7461 266d 6564 6961 3d68 7474 7073  zeta&media=https
+00000f70: 2533 4125 3246 2532 4665 7861 6d70 6c65  %3A%2F%2Fexample
+00000f80: 2e63 6f6d 2532 4669 6d61 6765 2e6a 7067  .com%2Fimage.jpg
+00000f90: 2664 6573 6372 6970 7469 6f6e 3d7a 6574  &description=zet
+00000fa0: 6125 3230 2d25 3230 7468 6525 3230 6675  a%20-%20the%20fu
+00000fb0: 7475 7265 2532 306f 6625 3230 4149 2920  ture%20of%20AI) 
+00000fc0: 5b21 5b53 6861 7265 206f 6e20 5768 6174  [![Share on What
+00000fd0: 7341 7070 5d28 6874 7470 733a 2f2f 696d  sApp](https://im
+00000fe0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000ff0: 6765 2f2d 5368 6172 6525 3230 6f6e 2532  ge/-Share%20on%2
+00001000: 3057 6861 7473 4170 702d 6772 6565 6e29  0WhatsApp-green)
+00001010: 5d28 6874 7470 733a 2f2f 6170 692e 7768  ](https://api.wh
+00001020: 6174 7361 7070 2e63 6f6d 2f73 656e 643f  atsapp.com/send?
+00001030: 7465 7874 3d43 6865 636b 2532 306f 7574  text=Check%20out
+00001040: 2532 307a 6574 6125 3230 2d25 3230 7468  %20zeta%20-%20th
+00001050: 6525 3230 6675 7475 7265 2532 306f 6625  e%20future%20of%
+00001060: 3230 4149 2532 3025 3233 7a65 7461 2532  20AI%20%23zeta%2
+00001070: 3025 3233 4149 2530 4125 3041 6874 7470  0%23AI%0A%0Ahttp
+00001080: 7325 3341 2532 4625 3246 6769 7468 7562  s%3A%2F%2Fgithub
+00001090: 2e63 6f6d 2532 466b 7965 676f 6d65 7a25  .com%2Fkyegomez%
+000010a0: 3246 7a65 7461 290a 0a41 6674 6572 2062  2Fzeta)..After b
+000010b0: 7569 6c64 696e 6720 6f75 7420 7468 6f75  uilding out thou
+000010c0: 7361 6e64 7320 6f66 206e 6575 7261 6c20  sands of neural 
+000010d0: 6e65 7473 2061 6e64 2066 6163 696e 6720  nets and facing 
+000010e0: 7468 6520 7361 6d65 2061 6e6e 6f79 696e  the same annoyin
+000010f0: 6720 626f 7474 6c65 6e65 636b 7320 6f66  g bottlenecks of
+00001100: 2063 6861 6f74 6963 2063 6f64 6562 6173   chaotic codebas
+00001110: 6573 2077 6974 6820 6e6f 206d 6f64 756c  es with no modul
+00001120: 6172 6974 7920 616e 6420 6c6f 7720 7065  arity and low pe
+00001130: 7266 6f72 6d61 6e63 6520 6d6f 6475 6c65  rformance module
+00001140: 732c 205a 6574 6120 6e65 6564 6564 2074  s, Zeta needed t
+00001150: 6f20 6265 2062 6f72 6e20 746f 2065 6e61  o be born to ena
+00001160: 626c 6520 6d65 2061 6e64 206f 7468 6572  ble me and other
+00001170: 7320 746f 2071 7569 636b 6c79 2070 726f  s to quickly pro
+00001180: 746f 7479 7065 2c20 7472 6169 6e2c 2061  totype, train, a
+00001190: 6e64 206f 7074 696d 697a 6520 7468 6520  nd optimize the 
+000011a0: 6c61 7465 7374 2053 4f54 4120 6e65 7572  latest SOTA neur
+000011b0: 616c 206e 6574 7320 616e 6420 6465 706c  al nets and depl
+000011c0: 6f79 2074 6865 6d20 696e 746f 2070 726f  oy them into pro
+000011d0: 6475 6374 696f 6e2e 200a 0a5a 6574 6120  duction. ..Zeta 
+000011e0: 706c 6163 6573 2061 2072 6164 6963 616c  places a radical
+000011f0: 2065 6d70 6861 7369 7320 6f6e 2075 7365   emphasis on use
+00001200: 6162 696c 6974 792c 206d 6f64 756c 6172  ability, modular
+00001210: 6974 792c 2061 6e64 2070 6572 666f 726d  ity, and perform
+00001220: 616e 6365 2e20 5a65 7461 2069 7320 6e6f  ance. Zeta is no
+00001230: 7720 6375 7272 656e 746c 7920 656d 706c  w currently empl
+00001240: 6f79 6564 2069 6e20 3130 3073 206f 6620  oyed in 100s of 
+00001250: 6d6f 6465 6c73 2061 6372 6f73 7320 6d79  models across my
+00001260: 2067 6974 6875 6220 616e 6420 6163 726f   github and acro
+00001270: 7373 206f 7468 6572 732e 200a 4765 7420  ss others. .Get 
+00001280: 7374 6172 7465 6420 6265 6c6f 7720 616e  started below an
+00001290: 6420 4c4d 4b20 6966 2079 6f75 2077 616e  d LMK if you wan
+000012a0: 7420 6d79 2068 656c 7020 6275 696c 6469  t my help buildi
+000012b0: 6e67 2061 6e79 206d 6f64 656c 2c20 4927  ng any model, I'
+000012c0: 6d20 6865 7265 2066 6f72 2079 6f75 20f0  m here for you .
+000012d0: 9f98 8a20 f09f 929c 200a 0a0a 2320 496e  ... .... ...# In
+000012e0: 7374 616c 6c0a 0a60 2420 7069 7033 2069  stall..`$ pip3 i
+000012f0: 6e73 7461 6c6c 202d 5520 7a65 7461 7363  nstall -U zetasc
+00001300: 616c 6560 0a0a 2320 5573 6167 650a 0a23  ale`..# Usage..#
+00001310: 2320 5374 6172 7469 6e67 2059 6f75 7220  # Starting Your 
+00001320: 4a6f 7572 6e65 790a 0a43 7265 6174 696e  Journey..Creatin
+00001330: 6720 6120 6d6f 6465 6c20 656d 706f 7765  g a model empowe
+00001340: 7265 6420 7769 7468 2074 6865 2061 666f  red with the afo
+00001350: 7265 6d65 6e74 696f 6e65 6420 6272 6561  rementioned brea
+00001360: 6b74 6872 6f75 6768 2072 6573 6561 7263  kthrough researc
+00001370: 6820 6665 6174 7572 6573 2069 7320 6120  h features is a 
+00001380: 6272 6565 7a65 2e20 4865 7265 2773 2068  breeze. Here's h
+00001390: 6f77 2074 6f20 7175 6963 6b6c 7920 6d61  ow to quickly ma
+000013a0: 7465 7269 616c 697a 6520 7468 6520 7265  terialize the re
+000013b0: 6e6f 776e 6564 2046 6c61 7368 2041 7474  nowned Flash Att
+000013c0: 656e 7469 6f6e 0a0a 6060 6070 7974 686f  ention..```pytho
+000013d0: 6e0a 696d 706f 7274 2074 6f72 6368 0a0a  n.import torch..
+000013e0: 6672 6f6d 207a 6574 612e 6e6e 2069 6d70  from zeta.nn imp
+000013f0: 6f72 7420 466c 6173 6841 7474 656e 7469  ort FlashAttenti
+00001400: 6f6e 0a0a 7120 3d20 746f 7263 682e 7261  on..q = torch.ra
+00001410: 6e64 6e28 322c 2034 2c20 362c 2038 290a  ndn(2, 4, 6, 8).
+00001420: 6b20 3d20 746f 7263 682e 7261 6e64 6e28  k = torch.randn(
+00001430: 322c 2034 2c20 3130 2c20 3829 0a76 203d  2, 4, 10, 8).v =
+00001440: 2074 6f72 6368 2e72 616e 646e 2832 2c20   torch.randn(2, 
+00001450: 342c 2031 302c 2038 290a 0a61 7474 656e  4, 10, 8)..atten
+00001460: 7469 6f6e 203d 2046 6c61 7368 4174 7465  tion = FlashAtte
+00001470: 6e74 696f 6e28 6361 7573 616c 3d46 616c  ntion(causal=Fal
+00001480: 7365 2c20 6472 6f70 6f75 743d 302e 312c  se, dropout=0.1,
+00001490: 2066 6c61 7368 3d54 7275 6529 0a6f 7574   flash=True).out
+000014a0: 7075 7420 3d20 6174 7465 6e74 696f 6e28  put = attention(
+000014b0: 712c 206b 2c20 7629 0a0a 7072 696e 7428  q, k, v)..print(
+000014c0: 6f75 7470 7574 2e73 6861 7065 290a 6060  output.shape).``
+000014d0: 600a 0a0a 0a23 2323 2060 5377 6947 4c55  `....### `SwiGLU
+000014e0: 600a 2d20 506f 7765 7273 2054 7261 6e73  `.- Powers Trans
+000014f0: 666f 726d 6572 206d 6f64 656c 730a 6060  former models.``
+00001500: 6070 7974 686f 6e0a 696d 706f 7274 2074  `python.import t
+00001510: 6f72 6368 0a0a 6672 6f6d 207a 6574 612e  orch..from zeta.
+00001520: 6e6e 2069 6d70 6f72 7420 5377 6947 4c55  nn import SwiGLU
+00001530: 5374 6163 6b65 640a 0a78 203d 2074 6f72  Stacked..x = tor
+00001540: 6368 2e72 616e 646e 2835 2c20 3130 290a  ch.randn(5, 10).
+00001550: 7377 6967 6c75 203d 2053 7769 474c 5553  swiglu = SwiGLUS
+00001560: 7461 636b 6564 2831 302c 2032 3029 0a73  tacked(10, 20).s
+00001570: 7769 676c 7528 7829 2e73 6861 7065 0a60  wiglu(x).shape.`
+00001580: 6060 0a0a 2323 2320 6060 6052 656c 6174  ``..### ```Relat
+00001590: 6976 6550 6f73 6974 696f 6e42 6961 7360  ivePositionBias`
+000015a0: 6060 0a2d 2060 6060 5265 6c61 7469 7665  ``.- ```Relative
+000015b0: 506f 7369 7469 6f6e 4269 6173 6060 6020  PositionBias``` 
+000015c0: 7175 616e 7469 7a65 7320 7468 6520 6469  quantizes the di
+000015d0: 7374 616e 6365 2062 6574 7765 656e 2074  stance between t
+000015e0: 776f 2070 6f73 6974 696f 6e73 2069 6e74  wo positions int
+000015f0: 6f20 6120 6365 7274 6169 6e20 6e75 6d62  o a certain numb
+00001600: 6572 206f 6620 6275 636b 6574 7320 616e  er of buckets an
+00001610: 6420 7468 656e 2075 7365 7320 616e 2065  d then uses an e
+00001620: 6d62 6564 6469 6e67 2074 6f20 6765 7420  mbedding to get 
+00001630: 7468 6520 7265 6c61 7469 7665 2070 6f73  the relative pos
+00001640: 6974 696f 6e20 6269 6173 2e20 5468 6973  ition bias. This
+00001650: 206d 6563 6861 6e69 736d 2061 6964 7320   mechanism aids 
+00001660: 696e 2074 6865 2061 7474 656e 7469 6f6e  in the attention
+00001670: 206d 6563 6861 6e69 736d 2062 7920 7072   mechanism by pr
+00001680: 6f76 6964 696e 6720 6269 6173 6573 2062  oviding biases b
+00001690: 6173 6564 206f 6e20 7265 6c61 7469 7665  ased on relative
+000016a0: 2070 6f73 6974 696f 6e73 2062 6574 7765   positions betwe
+000016b0: 656e 2074 6865 2071 7565 7279 2061 6e64  en the query and
+000016c0: 206b 6579 2c20 7261 7468 6572 2074 6861   key, rather tha
+000016d0: 6e20 7265 6c79 696e 6720 736f 6c65 6c79  n relying solely
+000016e0: 206f 6e20 7468 6569 7220 6162 736f 6c75   on their absolu
+000016f0: 7465 2070 6f73 6974 696f 6e73 2e0a 6060  te positions..``
+00001700: 6070 7974 686f 6e0a 696d 706f 7274 2074  `python.import t
+00001710: 6f72 6368 0a66 726f 6d20 746f 7263 6820  orch.from torch 
+00001720: 696d 706f 7274 206e 6e0a 0a66 726f 6d20  import nn..from 
+00001730: 7a65 7461 2e6e 6e20 696d 706f 7274 2052  zeta.nn import R
+00001740: 656c 6174 6976 6550 6f73 6974 696f 6e42  elativePositionB
+00001750: 6961 730a 0a23 2049 6e69 7469 616c 697a  ias..# Initializ
+00001760: 6520 7468 6520 5265 6c61 7469 7665 506f  e the RelativePo
+00001770: 7369 7469 6f6e 4269 6173 206d 6f64 756c  sitionBias modul
+00001780: 650a 7265 6c5f 706f 735f 6269 6173 203d  e.rel_pos_bias =
+00001790: 2052 656c 6174 6976 6550 6f73 6974 696f   RelativePositio
+000017a0: 6e42 6961 7328 290a 0a23 2045 7861 6d70  nBias()..# Examp
+000017b0: 6c65 2031 3a20 436f 6d70 7574 6520 6269  le 1: Compute bi
+000017c0: 6173 2066 6f72 2061 2073 696e 676c 6520  as for a single 
+000017d0: 6261 7463 680a 6269 6173 5f6d 6174 7269  batch.bias_matri
+000017e0: 7820 3d20 7265 6c5f 706f 735f 6269 6173  x = rel_pos_bias
+000017f0: 2831 2c20 3130 2c20 3130 290a 0a0a 2320  (1, 10, 10)...# 
+00001800: 4578 616d 706c 6520 323a 2055 7469 6c69  Example 2: Utili
+00001810: 7a65 2069 6e20 636f 6e6a 756e 6374 696f  ze in conjunctio
+00001820: 6e20 7769 7468 2061 6e20 6174 7465 6e74  n with an attent
+00001830: 696f 6e20 6d65 6368 616e 6973 6d0a 2320  ion mechanism.# 
+00001840: 4e4f 5445 3a20 5468 6973 2069 7320 6120  NOTE: This is a 
+00001850: 6d6f 636b 2065 7861 6d70 6c65 2c20 616e  mock example, an
+00001860: 6420 6d61 7920 6e6f 7420 7265 7072 6573  d may not repres
+00001870: 656e 7420 616e 2061 6374 7561 6c20 6174  ent an actual at
+00001880: 7465 6e74 696f 6e20 6d65 6368 616e 6973  tention mechanis
+00001890: 6d27 7320 636f 6d70 6c65 7465 2069 6d70  m's complete imp
+000018a0: 6c65 6d65 6e74 6174 696f 6e2e 0a63 6c61  lementation..cla
+000018b0: 7373 204d 6f63 6b41 7474 656e 7469 6f6e  ss MockAttention
+000018c0: 286e 6e2e 4d6f 6475 6c65 293a 0a20 2020  (nn.Module):.   
+000018d0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000018e0: 6c66 293a 0a20 2020 2020 2020 2073 7570  lf):.        sup
+000018f0: 6572 2829 2e5f 5f69 6e69 745f 5f28 290a  er().__init__().
+00001900: 2020 2020 2020 2020 7365 6c66 2e72 656c          self.rel
+00001910: 5f70 6f73 5f62 6961 7320 3d20 5265 6c61  _pos_bias = Rela
+00001920: 7469 7665 506f 7369 7469 6f6e 4269 6173  tivePositionBias
+00001930: 2829 0a0a 2020 2020 6465 6620 666f 7277  ()..    def forw
+00001940: 6172 6428 7365 6c66 2c20 7175 6572 6965  ard(self, querie
+00001950: 732c 206b 6579 7329 3a0a 2020 2020 2020  s, keys):.      
+00001960: 2020 6269 6173 203d 2073 656c 662e 7265    bias = self.re
+00001970: 6c5f 706f 735f 6269 6173 2871 7565 7269  l_pos_bias(queri
+00001980: 6573 2e73 697a 6528 3029 2c20 7175 6572  es.size(0), quer
+00001990: 6965 732e 7369 7a65 2831 292c 206b 6579  ies.size(1), key
+000019a0: 732e 7369 7a65 2831 2929 0a20 2020 2020  s.size(1)).     
+000019b0: 2020 2023 2046 7572 7468 6572 2063 6f6d     # Further com
+000019c0: 7075 7461 7469 6f6e 7320 7769 7468 2062  putations with b
+000019d0: 6961 7320 696e 2074 6865 2061 7474 656e  ias in the atten
+000019e0: 7469 6f6e 206d 6563 6861 6e69 736d 2e2e  tion mechanism..
+000019f0: 2e0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001a00: 204e 6f6e 6520 2023 2050 6c61 6365 686f   None  # Placeho
+00001a10: 6c64 6572 0a0a 0a23 2045 7861 6d70 6c65  lder...# Example
+00001a20: 2033 3a20 4d6f 6469 6679 2064 6566 6175   3: Modify defau
+00001a30: 6c74 2063 6f6e 6669 6775 7261 7469 6f6e  lt configuration
+00001a40: 730a 6375 7374 6f6d 5f72 656c 5f70 6f73  s.custom_rel_pos
+00001a50: 5f62 6961 7320 3d20 5265 6c61 7469 7665  _bias = Relative
+00001a60: 506f 7369 7469 6f6e 4269 6173 280a 2020  PositionBias(.  
+00001a70: 2020 6269 6469 7265 6374 696f 6e61 6c3d    bidirectional=
+00001a80: 4661 6c73 652c 206e 756d 5f62 7563 6b65  False, num_bucke
+00001a90: 7473 3d36 342c 206d 6178 5f64 6973 7461  ts=64, max_dista
+00001aa0: 6e63 653d 3235 362c 206e 756d 5f68 6561  nce=256, num_hea
+00001ab0: 6473 3d38 0a29 0a60 6060 0a0a 2323 2320  ds=8.).```..### 
+00001ac0: 6046 6565 6446 6f72 7761 7264 600a 5468  `FeedForward`.Th
+00001ad0: 6520 4665 6564 466f 7277 6172 6420 6d6f  e FeedForward mo
+00001ae0: 6475 6c65 2070 6572 666f 726d 7320 6120  dule performs a 
+00001af0: 6665 6564 666f 7277 6172 6420 6f70 6572  feedforward oper
+00001b00: 6174 696f 6e20 6f6e 2074 6865 2069 6e70  ation on the inp
+00001b10: 7574 2074 656e 736f 7220 782e 2049 7420  ut tensor x. It 
+00001b20: 636f 6e73 6973 7473 206f 6620 6120 6d75  consists of a mu
+00001b30: 6c74 692d 6c61 7965 7220 7065 7263 6570  lti-layer percep
+00001b40: 7472 6f6e 2028 4d4c 5029 2077 6974 6820  tron (MLP) with 
+00001b50: 616e 206f 7074 696f 6e61 6c20 6163 7469  an optional acti
+00001b60: 7661 7469 6f6e 2066 756e 6374 696f 6e20  vation function 
+00001b70: 616e 6420 4c61 7965 724e 6f72 6d2e 200a  and LayerNorm. .
+00001b80: 5573 6564 2069 6e20 6d6f 7374 206c 616e  Used in most lan
+00001b90: 6775 6167 652c 206d 756c 7469 2d6d 6f64  guage, multi-mod
+00001ba0: 616c 2c20 616e 6420 6d6f 6465 726e 206e  al, and modern n
+00001bb0: 6575 7261 6c20 6e65 7477 6f72 6b73 2e0a  eural networks..
+00001bc0: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00001bd0: 7420 746f 7263 680a 0a66 726f 6d20 7a65  t torch..from ze
+00001be0: 7461 2e6e 6e20 696d 706f 7274 2046 6565  ta.nn import Fee
+00001bf0: 6446 6f72 7761 7264 0a0a 6d6f 6465 6c20  dForward..model 
+00001c00: 3d20 4665 6564 466f 7277 6172 6428 3235  = FeedForward(25
+00001c10: 362c 2035 3132 2c20 676c 753d 5472 7565  6, 512, glu=True
+00001c20: 2c20 706f 7374 5f61 6374 5f6c 6e3d 5472  , post_act_ln=Tr
+00001c30: 7565 2c20 6472 6f70 6f75 743d 302e 3229  ue, dropout=0.2)
+00001c40: 0a0a 7820 3d20 746f 7263 682e 7261 6e64  ..x = torch.rand
+00001c50: 6e28 312c 2032 3536 290a 0a6f 7574 7075  n(1, 256)..outpu
+00001c60: 7420 3d20 6d6f 6465 6c28 7829 0a70 7269  t = model(x).pri
+00001c70: 6e74 286f 7574 7075 742e 7368 6170 6529  nt(output.shape)
+00001c80: 0a60 6060 0a0a 2323 2320 6042 6974 4c69  .```..### `BitLi
+00001c90: 6e65 6172 600a 2d20 5468 6520 4269 744c  near`.- The BitL
+00001ca0: 696e 6561 7220 6d6f 6475 6c65 2070 6572  inear module per
+00001cb0: 666f 726d 7320 6c69 6e65 6172 2074 7261  forms linear tra
+00001cc0: 6e73 666f 726d 6174 696f 6e20 6f6e 2074  nsformation on t
+00001cd0: 6865 2069 6e70 7574 2064 6174 612c 2066  he input data, f
+00001ce0: 6f6c 6c6f 7765 6420 6279 2071 7561 6e74  ollowed by quant
+00001cf0: 697a 6174 696f 6e20 616e 6420 6465 7175  ization and dequ
+00001d00: 616e 7469 7a61 7469 6f6e 2e20 5468 6520  antization. The 
+00001d10: 7175 616e 7469 7a61 7469 6f6e 2070 726f  quantization pro
+00001d20: 6365 7373 2069 7320 7065 7266 6f72 6d65  cess is performe
+00001d30: 6420 7573 696e 6720 7468 6520 6162 736d  d using the absm
+00001d40: 6178 5f71 7561 6e74 697a 6520 6675 6e63  ax_quantize func
+00001d50: 7469 6f6e 2c20 7768 6963 6820 7175 616e  tion, which quan
+00001d60: 7469 7a65 7320 7468 6520 696e 7075 7420  tizes the input 
+00001d70: 7465 6e73 6f72 2062 6173 6564 206f 6e20  tensor based on 
+00001d80: 7468 6520 6162 736f 6c75 7465 206d 6178  the absolute max
+00001d90: 696d 756d 2076 616c 7565 2c20 5b66 726f  imum value, [fro
+00001da0: 6d20 7468 6520 7061 7065 725d 2868 7474  m the paper](htt
+00001db0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00001dc0: 6273 2f32 3331 302e 3131 3435 3329 0a60  bs/2310.11453).`
+00001dd0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00001de0: 746f 7263 680a 6672 6f6d 2074 6f72 6368  torch.from torch
+00001df0: 2069 6d70 6f72 7420 6e6e 0a0a 696d 706f   import nn..impo
+00001e00: 7274 207a 6574 612e 7175 616e 7420 6173  rt zeta.quant as
+00001e10: 2071 740a 0a0a 636c 6173 7320 4d79 4d6f   qt...class MyMo
+00001e20: 6465 6c28 6e6e 2e4d 6f64 756c 6529 3a0a  del(nn.Module):.
+00001e30: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00001e40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00001e50: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00001e60: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00001e70: 6c69 6e65 6172 203d 2071 742e 4269 744c  linear = qt.BitL
+00001e80: 696e 6561 7228 3130 2c20 3230 290a 0a20  inear(10, 20).. 
+00001e90: 2020 2064 6566 2066 6f72 7761 7264 2873     def forward(s
+00001ea0: 656c 662c 2078 293a 0a20 2020 2020 2020  elf, x):.       
+00001eb0: 2072 6574 7572 6e20 7365 6c66 2e6c 696e   return self.lin
+00001ec0: 6561 7228 7829 0a0a 0a23 2049 6e69 7469  ear(x)...# Initi
+00001ed0: 616c 697a 6520 7468 6520 6d6f 6465 6c0a  alize the model.
+00001ee0: 6d6f 6465 6c20 3d20 4d79 4d6f 6465 6c28  model = MyModel(
+00001ef0: 290a 0a23 2043 7265 6174 6520 6120 7261  )..# Create a ra
+00001f00: 6e64 6f6d 2074 656e 736f 7220 6f66 2073  ndom tensor of s
+00001f10: 697a 6520 2831 3238 2c20 3130 290a 696e  ize (128, 10).in
+00001f20: 7075 7420 3d20 746f 7263 682e 7261 6e64  put = torch.rand
+00001f30: 6e28 3132 382c 2031 3029 0a0a 2320 5065  n(128, 10)..# Pe
+00001f40: 7266 6f72 6d20 7468 6520 666f 7277 6172  rform the forwar
+00001f50: 6420 7061 7373 0a6f 7574 7075 7420 3d20  d pass.output = 
+00001f60: 6d6f 6465 6c28 696e 7075 7429 0a0a 2320  model(input)..# 
+00001f70: 5072 696e 7420 7468 6520 7369 7a65 206f  Print the size o
+00001f80: 6620 7468 6520 6f75 7470 7574 0a70 7269  f the output.pri
+00001f90: 6e74 286f 7574 7075 742e 7369 7a65 2829  nt(output.size()
+00001fa0: 2920 2023 2074 6f72 6368 2e53 697a 6528  )  # torch.Size(
+00001fb0: 5b31 3238 2c20 3230 5d29 0a60 6060 0a0a  [128, 20]).```..
+00001fc0: 2323 2320 6050 616c 6d45 600a 2d20 5468  ### `PalmE`.- Th
+00001fd0: 6973 2069 7320 616e 2069 6d70 6c65 6d65  is is an impleme
+00001fe0: 6e74 6174 696f 6e20 6f66 2074 6865 206d  ntation of the m
+00001ff0: 756c 7469 2d6d 6f64 616c 2050 616c 6d2d  ulti-modal Palm-
+00002000: 4520 6d6f 6465 6c20 7573 696e 6720 6120  E model using a 
+00002010: 6465 636f 6465 7220 6c6c 6d20 6173 2074  decoder llm as t
+00002020: 6865 2062 6163 6b62 6f6e 6520 7769 7468  he backbone with
+00002030: 2061 6e20 5649 5420 696d 6167 6520 656e   an VIT image en
+00002040: 636f 6465 7220 746f 2070 726f 6365 7373  coder to process
+00002050: 2076 6973 696f 6e2c 2069 7427 7320 7665   vision, it's ve
+00002060: 7279 2073 696d 696c 6961 7220 746f 2047  ry similiar to G
+00002070: 5054 342c 204b 6f73 6d6f 732c 2052 5458  PT4, Kosmos, RTX
+00002080: 322c 2061 6e64 206d 616e 7920 6f74 6865  2, and many othe
+00002090: 7220 6d75 6c74 692d 6d6f 6461 6c69 7479  r multi-modality
+000020a0: 206d 6f64 656c 2061 7263 6869 7465 6374   model architect
+000020b0: 7572 6573 0a0a 6060 6070 7974 686f 6e0a  ures..```python.
+000020c0: 696d 706f 7274 2074 6f72 6368 0a0a 6672  import torch..fr
+000020d0: 6f6d 207a 6574 612e 7374 7275 6374 7320  om zeta.structs 
+000020e0: 696d 706f 7274 2028 0a20 2020 2041 7574  import (.    Aut
+000020f0: 6f52 6567 7265 7373 6976 6557 7261 7070  oRegressiveWrapp
+00002100: 6572 2c0a 2020 2020 4465 636f 6465 722c  er,.    Decoder,
+00002110: 0a20 2020 2045 6e63 6f64 6572 2c0a 2020  .    Encoder,.  
+00002120: 2020 5472 616e 7366 6f72 6d65 722c 0a20    Transformer,. 
+00002130: 2020 2056 6954 7261 6e73 666f 726d 6572     ViTransformer
+00002140: 5772 6170 7065 722c 0a29 0a0a 0a63 6c61  Wrapper,.)...cla
+00002150: 7373 2050 616c 6d45 2874 6f72 6368 2e6e  ss PalmE(torch.n
+00002160: 6e2e 4d6f 6475 6c65 293a 0a20 2020 2022  n.Module):.    "
+00002170: 2222 0a20 2020 2020 2020 2050 616c 6d45  "".        PalmE
+00002180: 2069 7320 6120 7472 616e 7366 6f72 6d65   is a transforme
+00002190: 7220 6172 6368 6974 6563 7475 7265 2074  r architecture t
+000021a0: 6861 7420 7573 6573 2061 2056 6954 2065  hat uses a ViT e
+000021b0: 6e63 6f64 6572 2061 6e64 2061 2074 7261  ncoder and a tra
+000021c0: 6e73 666f 726d 6572 2064 6563 6f64 6572  nsformer decoder
+000021d0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+000021e0: 0a0a 2020 2020 2020 2020 2020 2020 696d  ..            im
+000021f0: 6167 655f 7369 7a65 2028 696e 7429 3a20  age_size (int): 
+00002200: 5369 7a65 206f 6620 7468 6520 696d 6167  Size of the imag
+00002210: 652e 0a20 2020 2020 2020 2020 2020 2070  e..            p
+00002220: 6174 6368 5f73 697a 6520 2869 6e74 293a  atch_size (int):
+00002230: 2053 697a 6520 6f66 2074 6865 2070 6174   Size of the pat
+00002240: 6368 2e0a 2020 2020 2020 2020 2020 2020  ch..            
+00002250: 656e 636f 6465 725f 6469 6d20 2869 6e74  encoder_dim (int
+00002260: 293a 2044 696d 656e 7369 6f6e 206f 6620  ): Dimension of 
+00002270: 7468 6520 656e 636f 6465 722e 0a20 2020  the encoder..   
+00002280: 2020 2020 2020 2020 2065 6e63 6f64 6572           encoder
+00002290: 5f64 6570 7468 2028 696e 7429 3a20 4465  _depth (int): De
+000022a0: 7074 6820 6f66 2074 6865 2065 6e63 6f64  pth of the encod
+000022b0: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
+000022c0: 656e 636f 6465 725f 6865 6164 7320 2869  encoder_heads (i
+000022d0: 6e74 293a 204e 756d 6265 7220 6f66 2068  nt): Number of h
+000022e0: 6561 6473 2069 6e20 7468 6520 656e 636f  eads in the enco
+000022f0: 6465 722e 0a20 2020 2020 2020 2020 2020  der..           
+00002300: 206e 756d 5f74 6f6b 656e 7320 2869 6e74   num_tokens (int
+00002310: 293a 204e 756d 6265 7220 6f66 2074 6f6b  ): Number of tok
+00002320: 656e 732e 0a20 2020 2020 2020 2020 2020  ens..           
+00002330: 206d 6178 5f73 6571 5f6c 656e 2028 696e   max_seq_len (in
+00002340: 7429 3a20 4d61 7869 6d75 6d20 7365 7175  t): Maximum sequ
+00002350: 656e 6365 206c 656e 6774 682e 0a20 2020  ence length..   
+00002360: 2020 2020 2020 2020 2064 6563 6f64 6572           decoder
+00002370: 5f64 696d 2028 696e 7429 3a20 4469 6d65  _dim (int): Dime
+00002380: 6e73 696f 6e20 6f66 2074 6865 2064 6563  nsion of the dec
+00002390: 6f64 6572 2e0a 2020 2020 2020 2020 2020  oder..          
+000023a0: 2020 6465 636f 6465 725f 6465 7074 6820    decoder_depth 
+000023b0: 2869 6e74 293a 2044 6570 7468 206f 6620  (int): Depth of 
+000023c0: 7468 6520 6465 636f 6465 722e 0a20 2020  the decoder..   
+000023d0: 2020 2020 2020 2020 2064 6563 6f64 6572           decoder
+000023e0: 5f68 6561 6473 2028 696e 7429 3a20 4e75  _heads (int): Nu
+000023f0: 6d62 6572 206f 6620 6865 6164 7320 696e  mber of heads in
+00002400: 2074 6865 2064 6563 6f64 6572 2e0a 2020   the decoder..  
+00002410: 2020 2020 2020 2020 2020 616c 6962 695f            alibi_
+00002420: 6e75 6d5f 6865 6164 7320 2869 6e74 293a  num_heads (int):
+00002430: 204e 756d 6265 7220 6f66 2068 6561 6473   Number of heads
+00002440: 2069 6e20 7468 6520 616c 6962 6920 6174   in the alibi at
+00002450: 7465 6e74 696f 6e2e 0a20 2020 2020 2020  tention..       
+00002460: 2020 2020 2061 7474 6e5f 6b76 5f68 6561       attn_kv_hea
+00002470: 6473 2028 696e 7429 3a20 4e75 6d62 6572  ds (int): Number
+00002480: 206f 6620 6865 6164 7320 696e 2074 6865   of heads in the
+00002490: 2061 7474 656e 7469 6f6e 206b 6579 2d76   attention key-v
+000024a0: 616c 7565 2070 726f 6a65 6374 696f 6e2e  alue projection.
+000024b0: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+000024c0: 5f61 6273 5f70 6f73 5f65 6d62 2028 626f  _abs_pos_emb (bo
+000024d0: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
+000024e0: 7573 6520 6162 736f 6c75 7465 2070 6f73  use absolute pos
+000024f0: 6974 696f 6e61 6c20 656d 6265 6464 696e  itional embeddin
+00002500: 6773 2e0a 2020 2020 2020 2020 2020 2020  gs..            
+00002510: 6372 6f73 735f 6174 7465 6e64 2028 626f  cross_attend (bo
+00002520: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
+00002530: 6372 6f73 7320 6174 7465 6e64 2069 6e20  cross attend in 
+00002540: 7468 6520 6465 636f 6465 722e 0a20 2020  the decoder..   
+00002550: 2020 2020 2020 2020 2061 6c69 6269 5f70           alibi_p
+00002560: 6f73 5f62 6961 7320 2862 6f6f 6c29 3a20  os_bias (bool): 
+00002570: 5768 6574 6865 7220 746f 2075 7365 2070  Whether to use p
+00002580: 6f73 6974 696f 6e61 6c20 6269 6173 2069  ositional bias i
+00002590: 6e20 7468 6520 616c 6962 6920 6174 7465  n the alibi atte
+000025a0: 6e74 696f 6e2e 0a20 2020 2020 2020 2020  ntion..         
+000025b0: 2020 2072 6f74 6172 795f 7870 6f73 2028     rotary_xpos (
+000025c0: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
+000025d0: 6f20 7573 6520 726f 7461 7279 2070 6f73  o use rotary pos
+000025e0: 6974 696f 6e61 6c20 656d 6265 6464 696e  itional embeddin
+000025f0: 6773 2e0a 2020 2020 2020 2020 2020 2020  gs..            
+00002600: 6174 746e 5f66 6c61 7368 2028 626f 6f6c  attn_flash (bool
+00002610: 293a 2057 6865 7468 6572 2074 6f20 7573  ): Whether to us
+00002620: 6520 6174 7465 6e74 696f 6e20 666c 6173  e attention flas
+00002630: 682e 0a20 2020 2020 2020 2020 2020 2071  h..            q
+00002640: 6b5f 6e6f 726d 2028 626f 6f6c 293a 2057  k_norm (bool): W
+00002650: 6865 7468 6572 2074 6f20 6e6f 726d 616c  hether to normal
+00002660: 697a 6520 7468 6520 7175 6572 7920 616e  ize the query an
+00002670: 6420 6b65 7920 696e 2074 6865 2061 7474  d key in the att
+00002680: 656e 7469 6f6e 206c 6179 6572 2e0a 0a20  ention layer... 
+00002690: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+000026a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026b0: 2074 6f72 6368 2e54 656e 736f 723a 2054   torch.Tensor: T
+000026c0: 6865 206f 7574 7075 7420 6f66 2074 6865  he output of the
+000026d0: 206d 6f64 656c 2e0a 0a20 2020 2020 2020   model...       
+000026e0: 2055 7361 6765 3a0a 0a20 2020 2069 6d67   Usage:..    img
+000026f0: 203d 2074 6f72 6368 2e72 616e 646e 2831   = torch.randn(1
+00002700: 2c20 332c 2032 3536 2c20 3235 3629 0a20  , 3, 256, 256). 
+00002710: 2020 2074 6578 7420 3d20 746f 7263 682e     text = torch.
+00002720: 7261 6e64 696e 7428 302c 2032 3030 3030  randint(0, 20000
+00002730: 2c20 2831 2c20 3130 3234 2929 0a20 2020  , (1, 1024)).   
+00002740: 206d 6f64 656c 203d 2050 616c 6d45 2829   model = PalmE()
+00002750: 0a20 2020 206f 7574 7075 7420 3d20 6d6f  .    output = mo
+00002760: 6465 6c28 696d 672c 2074 6578 7429 0a20  del(img, text). 
+00002770: 2020 2070 7269 6e74 286f 7574 7075 7429     print(output)
+00002780: 0a0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+00002790: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+000027a0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000027b0: 2020 2069 6d61 6765 5f73 697a 653d 3235     image_size=25
+000027c0: 362c 0a20 2020 2020 2020 2070 6174 6368  6,.        patch
+000027d0: 5f73 697a 653d 3332 2c0a 2020 2020 2020  _size=32,.      
+000027e0: 2020 656e 636f 6465 725f 6469 6d3d 3531    encoder_dim=51
+000027f0: 322c 0a20 2020 2020 2020 2065 6e63 6f64  2,.        encod
+00002800: 6572 5f64 6570 7468 3d36 2c0a 2020 2020  er_depth=6,.    
+00002810: 2020 2020 656e 636f 6465 725f 6865 6164      encoder_head
+00002820: 733d 382c 0a20 2020 2020 2020 206e 756d  s=8,.        num
+00002830: 5f74 6f6b 656e 733d 3230 3030 302c 0a20  _tokens=20000,. 
+00002840: 2020 2020 2020 206d 6178 5f73 6571 5f6c         max_seq_l
+00002850: 656e 3d31 3032 342c 0a20 2020 2020 2020  en=1024,.       
+00002860: 2064 6563 6f64 6572 5f64 696d 3d35 3132   decoder_dim=512
+00002870: 2c0a 2020 2020 2020 2020 6465 636f 6465  ,.        decode
+00002880: 725f 6465 7074 683d 362c 0a20 2020 2020  r_depth=6,.     
+00002890: 2020 2064 6563 6f64 6572 5f68 6561 6473     decoder_heads
+000028a0: 3d38 2c0a 2020 2020 2020 2020 616c 6962  =8,.        alib
+000028b0: 695f 6e75 6d5f 6865 6164 733d 342c 0a20  i_num_heads=4,. 
+000028c0: 2020 2020 2020 2061 7474 6e5f 6b76 5f68         attn_kv_h
+000028d0: 6561 6473 3d32 2c0a 2020 2020 2020 2020  eads=2,.        
+000028e0: 7573 655f 6162 735f 706f 735f 656d 623d  use_abs_pos_emb=
+000028f0: 4661 6c73 652c 0a20 2020 2020 2020 2063  False,.        c
+00002900: 726f 7373 5f61 7474 656e 643d 5472 7565  ross_attend=True
+00002910: 2c0a 2020 2020 2020 2020 616c 6962 695f  ,.        alibi_
+00002920: 706f 735f 6269 6173 3d54 7275 652c 0a20  pos_bias=True,. 
+00002930: 2020 2020 2020 2072 6f74 6172 795f 7870         rotary_xp
+00002940: 6f73 3d54 7275 652c 0a20 2020 2020 2020  os=True,.       
+00002950: 2061 7474 6e5f 666c 6173 683d 5472 7565   attn_flash=True
+00002960: 2c0a 2020 2020 2020 2020 716b 5f6e 6f72  ,.        qk_nor
+00002970: 6d3d 5472 7565 2c0a 2020 2020 293a 0a20  m=True,.    ):. 
+00002980: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+00002990: 5f69 6e69 745f 5f28 290a 0a20 2020 2020  _init__()..     
+000029a0: 2020 2023 2076 6974 2061 7263 6869 7465     # vit archite
+000029b0: 6374 7572 650a 2020 2020 2020 2020 7365  cture.        se
+000029c0: 6c66 2e65 6e63 6f64 6572 203d 2056 6954  lf.encoder = ViT
+000029d0: 7261 6e73 666f 726d 6572 5772 6170 7065  ransformerWrappe
+000029e0: 7228 0a20 2020 2020 2020 2020 2020 2069  r(.            i
+000029f0: 6d61 6765 5f73 697a 653d 696d 6167 655f  mage_size=image_
+00002a00: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
+00002a10: 2020 7061 7463 685f 7369 7a65 3d70 6174    patch_size=pat
+00002a20: 6368 5f73 697a 652c 0a20 2020 2020 2020  ch_size,.       
+00002a30: 2020 2020 2061 7474 6e5f 6c61 7965 7273       attn_layers
+00002a40: 3d45 6e63 6f64 6572 280a 2020 2020 2020  =Encoder(.      
+00002a50: 2020 2020 2020 2020 2020 6469 6d3d 656e            dim=en
+00002a60: 636f 6465 725f 6469 6d2c 2064 6570 7468  coder_dim, depth
+00002a70: 3d65 6e63 6f64 6572 5f64 6570 7468 2c20  =encoder_depth, 
+00002a80: 6865 6164 733d 656e 636f 6465 725f 6865  heads=encoder_he
+00002a90: 6164 730a 2020 2020 2020 2020 2020 2020  ads.            
+00002aa0: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00002ab0: 2020 2020 2020 2320 7061 6c6d 206d 6f64        # palm mod
+00002ac0: 656c 2061 7263 6869 7465 6374 7572 650a  el architecture.
+00002ad0: 2020 2020 2020 2020 7365 6c66 2e64 6563          self.dec
+00002ae0: 6f64 6572 203d 2054 7261 6e73 666f 726d  oder = Transform
+00002af0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+00002b00: 6e75 6d5f 746f 6b65 6e73 3d6e 756d 5f74  num_tokens=num_t
+00002b10: 6f6b 656e 732c 0a20 2020 2020 2020 2020  okens,.         
+00002b20: 2020 206d 6178 5f73 6571 5f6c 656e 3d6d     max_seq_len=m
+00002b30: 6178 5f73 6571 5f6c 656e 2c0a 2020 2020  ax_seq_len,.    
+00002b40: 2020 2020 2020 2020 7573 655f 6162 735f          use_abs_
+00002b50: 706f 735f 656d 623d 7573 655f 6162 735f  pos_emb=use_abs_
+00002b60: 706f 735f 656d 622c 0a20 2020 2020 2020  pos_emb,.       
+00002b70: 2020 2020 2061 7474 6e5f 6c61 7965 7273       attn_layers
+00002b80: 3d44 6563 6f64 6572 280a 2020 2020 2020  =Decoder(.      
+00002b90: 2020 2020 2020 2020 2020 6469 6d3d 6465            dim=de
+00002ba0: 636f 6465 725f 6469 6d2c 0a20 2020 2020  coder_dim,.     
+00002bb0: 2020 2020 2020 2020 2020 2064 6570 7468             depth
+00002bc0: 3d64 6563 6f64 6572 5f64 6570 7468 2c0a  =decoder_depth,.
+00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002be0: 6865 6164 733d 6465 636f 6465 725f 6865  heads=decoder_he
+00002bf0: 6164 732c 0a20 2020 2020 2020 2020 2020  ads,.           
+00002c00: 2020 2020 2063 726f 7373 5f61 7474 656e       cross_atten
+00002c10: 643d 6372 6f73 735f 6174 7465 6e64 2c0a  d=cross_attend,.
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 616c 6962 695f 706f 735f 6269 6173 3d61  alibi_pos_bias=a
+00002c40: 6c69 6269 5f70 6f73 5f62 6961 732c 0a20  libi_pos_bias,. 
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00002c60: 6c69 6269 5f6e 756d 5f68 6561 6473 3d61  libi_num_heads=a
+00002c70: 6c69 6269 5f6e 756d 5f68 6561 6473 2c0a  libi_num_heads,.
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 726f 7461 7279 5f78 706f 733d 726f 7461  rotary_xpos=rota
+00002ca0: 7279 5f78 706f 732c 0a20 2020 2020 2020  ry_xpos,.       
+00002cb0: 2020 2020 2020 2020 2061 7474 6e5f 6b76           attn_kv
+00002cc0: 5f68 6561 6473 3d61 7474 6e5f 6b76 5f68  _heads=attn_kv_h
+00002cd0: 6561 6473 2c0a 2020 2020 2020 2020 2020  eads,.          
+00002ce0: 2020 2020 2020 6174 746e 5f66 6c61 7368        attn_flash
+00002cf0: 3d61 7474 6e5f 666c 6173 682c 0a20 2020  =attn_flash,.   
+00002d00: 2020 2020 2020 2020 2020 2020 2071 6b5f               qk_
+00002d10: 6e6f 726d 3d71 6b5f 6e6f 726d 2c0a 2020  norm=qk_norm,.  
+00002d20: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00002d30: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00002d40: 2320 6175 746f 7265 6772 6573 7369 7665  # autoregressive
+00002d50: 2077 7261 7070 6572 2074 6f20 656e 6162   wrapper to enab
+00002d60: 6c65 2067 656e 6572 6174 696f 6e20 6f66  le generation of
+00002d70: 2074 6f6b 656e 730a 2020 2020 2020 2020   tokens.        
+00002d80: 7365 6c66 2e64 6563 6f64 6572 203d 2041  self.decoder = A
+00002d90: 7574 6f52 6567 7265 7373 6976 6557 7261  utoRegressiveWra
+00002da0: 7070 6572 2873 656c 662e 6465 636f 6465  pper(self.decode
+00002db0: 7229 0a0a 2020 2020 6465 6620 666f 7277  r)..    def forw
+00002dc0: 6172 6428 7365 6c66 2c20 696d 673a 2074  ard(self, img: t
+00002dd0: 6f72 6368 2e54 656e 736f 722c 2074 6578  orch.Tensor, tex
+00002de0: 743a 2074 6f72 6368 2e54 656e 736f 7229  t: torch.Tensor)
+00002df0: 3a0a 2020 2020 2020 2020 2222 2246 6f72  :.        """For
+00002e00: 7761 7264 2070 6173 7320 6f66 2074 6865  ward pass of the
+00002e10: 206d 6f64 656c 2e22 2222 0a20 2020 2020   model.""".     
+00002e20: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00002e30: 2020 2020 656e 636f 6465 6420 3d20 7365      encoded = se
+00002e40: 6c66 2e65 6e63 6f64 6572 2869 6d67 2c20  lf.encoder(img, 
+00002e50: 7265 7475 726e 5f65 6d62 6564 6469 6e67  return_embedding
+00002e60: 733d 5472 7565 290a 2020 2020 2020 2020  s=True).        
+00002e70: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002e80: 6465 636f 6465 7228 7465 7874 2c20 636f  decoder(text, co
+00002e90: 6e74 6578 743d 656e 636f 6465 6429 0a20  ntext=encoded). 
+00002ea0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00002eb0: 6365 7074 696f 6e20 6173 2065 7272 6f72  ception as error
+00002ec0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00002ed0: 696e 7428 6622 4661 696c 6564 2069 6e20  int(f"Failed in 
+00002ee0: 666f 7277 6172 6420 6d65 7468 6f64 3a20  forward method: 
+00002ef0: 7b65 7272 6f72 7d22 290a 2020 2020 2020  {error}").      
+00002f00: 2020 2020 2020 7261 6973 650a 0a0a 2320        raise...# 
+00002f10: 5573 6167 6520 7769 7468 2072 616e 646f  Usage with rando
+00002f20: 6d20 696e 7075 7473 0a69 6d67 203d 2074  m inputs.img = t
+00002f30: 6f72 6368 2e72 616e 646e 2831 2c20 332c  orch.randn(1, 3,
+00002f40: 2032 3536 2c20 3235 3629 0a74 6578 7420   256, 256).text 
+00002f50: 3d20 746f 7263 682e 7261 6e64 696e 7428  = torch.randint(
+00002f60: 302c 2032 3030 3030 2c20 2831 2c20 3130  0, 20000, (1, 10
+00002f70: 3234 2929 0a0a 2320 496e 6974 696c 6961  24))..# Initilia
+00002f80: 7a65 2074 6865 206d 6f64 656c 0a6d 6f64  ze the model.mod
+00002f90: 656c 203d 2050 616c 6d45 2829 0a6f 7574  el = PalmE().out
+00002fa0: 7075 7420 3d20 6d6f 6465 6c28 696d 672c  put = model(img,
+00002fb0: 2074 6578 7429 0a70 7269 6e74 286f 7574   text).print(out
+00002fc0: 7075 7429 0a60 6060 0a0a 0a23 2323 2060  put).```...### `
+00002fd0: 556e 6574 600a 556e 6574 2069 7320 6120  Unet`.Unet is a 
+00002fe0: 6661 6d6f 7573 2063 6f6e 766f 6c75 7469  famous convoluti
+00002ff0: 6f6e 616c 206e 6575 7261 6c20 6e65 7477  onal neural netw
+00003000: 6f72 6b20 6172 6368 6974 6563 7475 7265  ork architecture
+00003010: 206f 7269 6769 6e61 6c6c 7920 7573 6564   originally used
+00003020: 2066 6f72 2062 696f 6d65 6469 6361 6c20   for biomedical 
+00003030: 696d 6167 6520 7365 676d 656e 7461 7469  image segmentati
+00003040: 6f6e 2062 7574 2073 6f6f 6e20 6265 6361  on but soon beca
+00003050: 6d65 2074 6865 2062 6163 6b62 6f6e 6520  me the backbone 
+00003060: 6f66 2074 6865 2067 656e 6572 6174 6976  of the generativ
+00003070: 6520 4149 204d 6567 612d 7265 766f 6c75  e AI Mega-revolu
+00003080: 7469 6f6e 2e20 5468 6520 6172 6368 6974  tion. The archit
+00003090: 6563 7475 7265 2063 6f6d 7072 6973 6573  ecture comprises
+000030a0: 2074 776f 2070 7269 6d61 7279 2070 6174   two primary pat
+000030b0: 6877 6179 733a 2064 6f77 6e73 616d 706c  hways: downsampl
+000030c0: 696e 6720 616e 6420 7570 7361 6d70 6c69  ing and upsampli
+000030d0: 6e67 2c20 666f 6c6c 6f77 6564 2062 7920  ng, followed by 
+000030e0: 616e 206f 7574 7075 7420 636f 6e76 6f6c  an output convol
+000030f0: 7574 696f 6e2e 2044 7565 2074 6f20 6974  ution. Due to it
+00003100: 7320 552d 7368 6170 652c 2074 6865 2061  s U-shape, the a
+00003110: 7263 6869 7465 6374 7572 6520 6973 206e  rchitecture is n
+00003120: 616d 6564 2055 2d4e 6574 2e20 4974 7320  amed U-Net. Its 
+00003130: 7379 6d6d 6574 7269 6320 6172 6368 6974  symmetric archit
+00003140: 6563 7475 7265 2065 6e73 7572 6573 2074  ecture ensures t
+00003150: 6861 7420 7468 6520 636f 6e74 6578 7420  hat the context 
+00003160: 2866 726f 6d20 646f 776e 7361 6d70 6c69  (from downsampli
+00003170: 6e67 2920 616e 6420 7468 6520 6c6f 6361  ng) and the loca
+00003180: 6c69 7a61 7469 6f6e 2028 6672 6f6d 2075  lization (from u
+00003190: 7073 616d 706c 696e 6729 2061 7265 2063  psampling) are c
+000031a0: 6170 7475 7265 6420 6566 6665 6374 6976  aptured effectiv
+000031b0: 656c 792e 0a0a 6060 6070 7974 686f 6e0a  ely...```python.
+000031c0: 696d 706f 7274 2074 6f72 6368 0a0a 6672  import torch..fr
+000031d0: 6f6d 207a 6574 612e 6e6e 2069 6d70 6f72  om zeta.nn impor
+000031e0: 7420 556e 6574 0a0a 2320 496e 6974 6961  t Unet..# Initia
+000031f0: 6c69 7a65 2074 6865 2055 2d4e 6574 206d  lize the U-Net m
+00003200: 6f64 656c 0a6d 6f64 656c 203d 2055 6e65  odel.model = Une
+00003210: 7428 6e5f 6368 616e 6e65 6c73 3d31 2c20  t(n_channels=1, 
+00003220: 6e5f 636c 6173 7365 733d 3229 0a0a 2320  n_classes=2)..# 
+00003230: 5261 6e64 6f6d 2069 6e70 7574 2074 656e  Random input ten
+00003240: 736f 7220 7769 7468 2064 696d 656e 7369  sor with dimensi
+00003250: 6f6e 7320 5b62 6174 6368 5f73 697a 652c  ons [batch_size,
+00003260: 2063 6861 6e6e 656c 732c 2068 6569 6768   channels, heigh
+00003270: 742c 2077 6964 7468 5d0a 7820 3d20 746f  t, width].x = to
+00003280: 7263 682e 7261 6e64 6e28 312c 2031 2c20  rch.randn(1, 1, 
+00003290: 3537 322c 2035 3732 290a 0a23 2046 6f72  572, 572)..# For
+000032a0: 7761 7264 2070 6173 7320 7468 726f 7567  ward pass throug
+000032b0: 6820 7468 6520 6d6f 6465 6c0a 7920 3d20  h the model.y = 
+000032c0: 6d6f 6465 6c28 7829 0a0a 2320 4f75 7470  model(x)..# Outp
+000032d0: 7574 0a70 7269 6e74 2866 2249 6e70 7574  ut.print(f"Input
+000032e0: 2073 6861 7065 3a20 7b78 2e73 6861 7065   shape: {x.shape
+000032f0: 7d22 290a 7072 696e 7428 6622 4f75 7470  }").print(f"Outp
+00003300: 7574 2073 6861 7065 3a20 7b79 2e73 6861  ut shape: {y.sha
+00003310: 7065 7d22 290a 6060 600a 0a0a 2323 2320  pe}").```...### 
+00003320: 6056 6973 696f 6e45 6d62 6564 6469 6e67  `VisionEmbedding
+00003330: 7360 0a54 6865 2056 6973 696f 6e45 6d62  s`.The VisionEmb
+00003340: 6564 6469 6e67 2063 6c61 7373 2069 7320  edding class is 
+00003350: 6465 7369 676e 6564 2066 6f72 2063 6f6e  designed for con
+00003360: 7665 7274 696e 6720 696d 6167 6573 2069  verting images i
+00003370: 6e74 6f20 7061 7463 6820 656d 6265 6464  nto patch embedd
+00003380: 696e 6773 2c20 6d61 6b69 6e67 2074 6865  ings, making the
+00003390: 6d20 7375 6974 6162 6c65 2066 6f72 2070  m suitable for p
+000033a0: 726f 6365 7373 696e 6720 6279 2074 7261  rocessing by tra
+000033b0: 6e73 666f 726d 6572 2d62 6173 6564 206d  nsformer-based m
+000033c0: 6f64 656c 732e 2054 6869 7320 636c 6173  odels. This clas
+000033d0: 7320 706c 6179 7320 6120 6372 7563 6961  s plays a crucia
+000033e0: 6c20 726f 6c65 2069 6e20 7661 7269 6f75  l role in variou
+000033f0: 7320 636f 6d70 7574 6572 2076 6973 696f  s computer visio
+00003400: 6e20 7461 736b 7320 616e 6420 656e 6162  n tasks and enab
+00003410: 6c65 7320 7468 6520 696e 7465 6772 6174  les the integrat
+00003420: 696f 6e20 6f66 2076 6973 696f 6e20 6461  ion of vision da
+00003430: 7461 2069 6e74 6f20 7472 616e 7366 6f72  ta into transfor
+00003440: 6d65 7220 6172 6368 6974 6563 7475 7265  mer architecture
+00003450: 7321 0a0a 6060 6070 7974 686f 6e0a 696d  s!..```python.im
+00003460: 706f 7274 2074 6f72 6368 0a0a 6672 6f6d  port torch..from
+00003470: 207a 6574 612e 6e6e 2069 6d70 6f72 7420   zeta.nn import 
+00003480: 5669 7369 6f6e 456d 6265 6464 696e 670a  VisionEmbedding.
+00003490: 0a23 2043 7265 6174 6520 616e 2069 6e73  .# Create an ins
+000034a0: 7461 6e63 6520 6f66 2056 6973 696f 6e45  tance of VisionE
+000034b0: 6d62 6564 6469 6e67 0a76 6973 696f 6e5f  mbedding.vision_
+000034c0: 656d 6265 6464 696e 6720 3d20 5669 7369  embedding = Visi
+000034d0: 6f6e 456d 6265 6464 696e 6728 0a20 2020  onEmbedding(.   
+000034e0: 2069 6d67 5f73 697a 653d 3232 342c 0a20   img_size=224,. 
+000034f0: 2020 2070 6174 6368 5f73 697a 653d 3136     patch_size=16
+00003500: 2c0a 2020 2020 696e 5f63 6861 6e73 3d33  ,.    in_chans=3
+00003510: 2c0a 2020 2020 656d 6265 645f 6469 6d3d  ,.    embed_dim=
+00003520: 3736 382c 0a20 2020 2063 6f6e 7461 696e  768,.    contain
+00003530: 5f6d 6173 6b5f 746f 6b65 6e3d 5472 7565  _mask_token=True
+00003540: 2c0a 2020 2020 7072 6570 656e 645f 636c  ,.    prepend_cl
+00003550: 735f 746f 6b65 6e3d 5472 7565 2c0a 290a  s_token=True,.).
+00003560: 0a23 204c 6f61 6420 616e 2065 7861 6d70  .# Load an examp
+00003570: 6c65 2069 6d61 6765 2028 3320 6368 616e  le image (3 chan
+00003580: 6e65 6c73 2c20 3232 3478 3232 3429 0a69  nels, 224x224).i
+00003590: 6e70 7574 5f69 6d61 6765 203d 2074 6f72  nput_image = tor
+000035a0: 6368 2e72 616e 6428 312c 2033 2c20 3232  ch.rand(1, 3, 22
+000035b0: 342c 2032 3234 290a 0a23 2050 6572 666f  4, 224)..# Perfo
+000035c0: 726d 2069 6d61 6765 2d74 6f2d 7061 7463  rm image-to-patc
+000035d0: 6820 656d 6265 6464 696e 670a 6f75 7470  h embedding.outp
+000035e0: 7574 203d 2076 6973 696f 6e5f 656d 6265  ut = vision_embe
+000035f0: 6464 696e 6728 696e 7075 745f 696d 6167  dding(input_imag
+00003600: 6529 0a0a 2320 5468 6520 6f75 7470 7574  e)..# The output
+00003610: 206e 6f77 2063 6f6e 7461 696e 7320 7061   now contains pa
+00003620: 7463 6820 656d 6265 6464 696e 6773 2c20  tch embeddings, 
+00003630: 7265 6164 7920 666f 7220 696e 7075 7420  ready for input 
+00003640: 746f 2061 2074 7261 6e73 666f 726d 6572  to a transformer
+00003650: 206d 6f64 656c 0a60 6060 0a0a 0a23 2323   model.```...###
+00003660: 2060 6e69 7661 600a 2d20 4e69 7661 2066   `niva`.- Niva f
+00003670: 6f63 7573 6573 206f 6e20 7765 6967 6874  ocuses on weight
+00003680: 7320 6f66 2063 6572 7461 696e 206c 6179  s of certain lay
+00003690: 6572 7320 2873 7065 6369 6669 6564 2062  ers (specified b
+000036a0: 7920 7175 616e 7469 7a65 5f6c 6179 6572  y quantize_layer
+000036b0: 7329 2e20 4964 6561 6c20 666f 7220 6d6f  s). Ideal for mo
+000036c0: 6465 6c73 2077 6865 7265 2072 756e 7469  dels where runti
+000036d0: 6d65 2061 6374 6976 6174 696f 6e20 6973  me activation is
+000036e0: 2076 6172 6961 626c 652e 20f0 9f91 81ef   variable. .....
+000036f0: b88f 2045 7861 6d70 6c65 204c 6179 6572  .. Example Layer
+00003700: 733a 206e 6e2e 456d 6265 6464 696e 672c  s: nn.Embedding,
+00003710: 206e 6e2e 4c53 544d 2e20 0a0a 6060 6070   nn.LSTM. ..```p
+00003720: 7974 686f 6e0a 696d 706f 7274 2074 6f72  ython.import tor
+00003730: 6368 0a0a 6672 6f6d 207a 6574 6120 696d  ch..from zeta im
+00003740: 706f 7274 206e 6976 610a 0a23 204c 6f61  port niva..# Loa
+00003750: 6420 6120 7072 652d 7472 6169 6e65 6420  d a pre-trained 
+00003760: 6d6f 6465 6c0a 6d6f 6465 6c20 3d20 596f  model.model = Yo
+00003770: 7572 4d6f 6465 6c43 6c61 7373 2829 0a0a  urModelClass()..
+00003780: 2320 5175 616e 7469 7a65 2074 6865 206d  # Quantize the m
+00003790: 6f64 656c 2064 796e 616d 6963 616c 6c79  odel dynamically
+000037a0: 2c20 7370 6563 6966 7969 6e67 206c 6179  , specifying lay
+000037b0: 6572 7320 746f 2071 7561 6e74 697a 650a  ers to quantize.
+000037c0: 6e69 7661 280a 2020 2020 6d6f 6465 6c3d  niva(.    model=
+000037d0: 6d6f 6465 6c2c 0a20 2020 206d 6f64 656c  model,.    model
+000037e0: 5f70 6174 683d 2270 6174 685f 746f 5f70  _path="path_to_p
+000037f0: 7265 7472 6169 6e65 645f 6d6f 6465 6c5f  retrained_model_
+00003800: 7765 6967 6874 732e 7074 222c 0a20 2020  weights.pt",.   
+00003810: 206f 7574 7075 745f 7061 7468 3d22 7175   output_path="qu
+00003820: 616e 7469 7a65 645f 6d6f 6465 6c2e 7074  antized_model.pt
+00003830: 222c 0a20 2020 2071 7561 6e74 5f74 7970  ",.    quant_typ
+00003840: 653d 2264 796e 616d 6963 222c 0a20 2020  e="dynamic",.   
+00003850: 2071 7561 6e74 697a 655f 6c61 7965 7273   quantize_layers
+00003860: 3d5b 6e6e 2e4c 696e 6561 722c 206e 6e2e  =[nn.Linear, nn.
+00003870: 436f 6e76 3264 5d2c 0a20 2020 2064 7479  Conv2d],.    dty
+00003880: 7065 3d74 6f72 6368 2e71 696e 7438 2c0a  pe=torch.qint8,.
+00003890: 290a 6060 600a 0a0a 2323 2320 6046 7573  ).```...### `Fus
+000038a0: 6564 4465 6e73 6547 454c 5544 656e 7365  edDenseGELUDense
+000038b0: 600a 2d20 496e 6372 6561 7365 206d 6f64  `.- Increase mod
+000038c0: 656c 2073 7065 6564 2062 7920 3278 2077  el speed by 2x w
+000038d0: 6974 6820 7468 6973 206d 6f64 756c 6520  ith this module 
+000038e0: 7468 6174 2066 7573 6573 2074 6f67 6574  that fuses toget
+000038f0: 6865 7220 3220 6879 7065 722d 6f70 7469  her 2 hyper-opti
+00003900: 6d69 7a65 6420 6465 6e73 6520 6f70 7320  mized dense ops 
+00003910: 6672 6f6d 2062 6974 7320 616e 6420 6279  from bits and by
+00003920: 7465 7320 616e 6420 6120 6765 6c75 2074  tes and a gelu t
+00003930: 6f67 6574 6865 7221 0a0a 6060 6070 7974  ogether!..```pyt
+00003940: 686f 6e0a 696d 706f 7274 2074 6f72 6368  hon.import torch
+00003950: 0a0a 6672 6f6d 207a 6574 612e 6e6e 2069  ..from zeta.nn i
+00003960: 6d70 6f72 7420 4675 7365 6444 656e 7365  mport FusedDense
+00003970: 4745 4c55 4465 6e73 650a 0a78 203d 2074  GELUDense..x = t
+00003980: 6f72 6368 2e72 616e 646e 2831 2c20 3531  orch.randn(1, 51
+00003990: 3229 0a6d 6f64 656c 203d 2046 7573 6564  2).model = Fused
+000039a0: 4465 6e73 6547 454c 5544 656e 7365 2835  DenseGELUDense(5
+000039b0: 3132 2c20 3130 3234 290a 6f75 7420 3d20  12, 1024).out = 
+000039c0: 6d6f 6465 6c28 7829 0a6f 7574 2e73 6861  model(x).out.sha
+000039d0: 7065 0a60 6060 0a0a 0a23 2323 2060 4675  pe.```...### `Fu
+000039e0: 7365 6444 726f 706f 7574 4c61 7965 724e  sedDropoutLayerN
+000039f0: 6f72 6d60 0a2d 2046 7573 6564 4472 6f70  orm`.- FusedDrop
+00003a00: 6f75 744c 6179 6572 4e6f 726d 2069 7320  outLayerNorm is 
+00003a10: 6120 6675 7365 6420 6b65 726e 656c 206f  a fused kernel o
+00003a20: 6620 6472 6f70 6f75 7420 616e 6420 6c61  f dropout and la
+00003a30: 7965 726e 6f72 6d20 746f 2073 7065 6564  yernorm to speed
+00003a40: 2075 7020 4646 4e73 206f 7220 4d4c 5053   up FFNs or MLPS
+00003a50: 2062 7920 3258 0a0a 6060 6070 7974 686f   by 2X..```pytho
+00003a60: 6e0a 696d 706f 7274 2074 6f72 6368 0a66  n.import torch.f
+00003a70: 726f 6d20 746f 7263 6820 696d 706f 7274  rom torch import
+00003a80: 206e 6e0a 0a66 726f 6d20 7a65 7461 2e6e   nn..from zeta.n
+00003a90: 6e20 696d 706f 7274 2046 7573 6564 4472  n import FusedDr
+00003aa0: 6f70 6f75 744c 6179 6572 4e6f 726d 0a0a  opoutLayerNorm..
+00003ab0: 2320 496e 6974 6961 6c69 7a65 2074 6865  # Initialize the
+00003ac0: 206d 6f64 756c 650a 6d6f 6465 6c20 3d20   module.model = 
+00003ad0: 4675 7365 6444 726f 706f 7574 4c61 7965  FusedDropoutLaye
+00003ae0: 724e 6f72 6d28 6469 6d3d 3531 3229 0a0a  rNorm(dim=512)..
+00003af0: 2320 4372 6561 7465 2061 2073 616d 706c  # Create a sampl
+00003b00: 6520 696e 7075 7420 7465 6e73 6f72 0a78  e input tensor.x
+00003b10: 203d 2074 6f72 6368 2e72 616e 646e 2831   = torch.randn(1
+00003b20: 2c20 3531 3229 0a0a 2320 466f 7277 6172  , 512)..# Forwar
+00003b30: 6420 7061 7373 0a6f 7574 7075 7420 3d20  d pass.output = 
+00003b40: 6d6f 6465 6c28 7829 0a0a 2320 4368 6563  model(x)..# Chec
+00003b50: 6b20 6f75 7470 7574 2073 6861 7065 0a70  k output shape.p
+00003b60: 7269 6e74 286f 7574 7075 742e 7368 6170  rint(output.shap
+00003b70: 6529 2020 2320 4578 7065 6374 6564 3a20  e)  # Expected: 
+00003b80: 746f 7263 682e 5369 7a65 285b 312c 2035  torch.Size([1, 5
+00003b90: 3132 5d29 0a60 6060 0a0a 0a23 2323 2060  12]).```...### `
+00003ba0: 4d61 6d62 6160 0a2d 2050 7974 6f72 6368  Mamba`.- Pytorch
+00003bb0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00003bc0: 6f66 2074 6865 206e 6577 2053 534d 206d  of the new SSM m
+00003bd0: 6f64 656c 2061 7263 6869 7465 6374 7572  odel architectur
+00003be0: 6520 4d61 6d62 610a 0a60 6060 7079 7468  e Mamba..```pyth
+00003bf0: 6f6e 0a69 6d70 6f72 7420 746f 7263 680a  on.import torch.
+00003c00: 0a66 726f 6d20 7a65 7461 2e6e 6e20 696d  .from zeta.nn im
+00003c10: 706f 7274 204d 616d 6261 426c 6f63 6b0a  port MambaBlock.
+00003c20: 0a23 2049 6e69 7469 616c 697a 6520 4d61  .# Initialize Ma
+00003c30: 6d62 610a 626c 6f63 6b20 3d20 4d61 6d62  mba.block = Mamb
+00003c40: 6142 6c6f 636b 2864 696d 3d36 342c 2064  aBlock(dim=64, d
+00003c50: 6570 7468 3d31 290a 0a23 2052 616e 646f  epth=1)..# Rando
+00003c60: 6d20 696e 7075 740a 7820 3d20 746f 7263  m input.x = torc
+00003c70: 682e 7261 6e64 6e28 312c 2031 302c 2036  h.randn(1, 10, 6
+00003c80: 3429 0a0a 2320 4170 706c 7920 7468 6520  4)..# Apply the 
+00003c90: 6d6f 6465 6c20 746f 2074 6865 2062 6c6f  model to the blo
+00003ca0: 636b 0a79 203d 2062 6c6f 636b 2878 290a  ck.y = block(x).
+00003cb0: 0a70 7269 6e74 2879 2e73 6861 7065 290a  .print(y.shape).
+00003cc0: 2320 746f 7263 682e 5369 7a65 285b 312c  # torch.Size([1,
+00003cd0: 2031 302c 2036 345d 290a 6060 600a 0a23   10, 64]).```..#
+00003ce0: 2323 2060 4669 4c4d 600a 0a60 6060 7079  ## `FiLM`..```py
+00003cf0: 7468 6f6e 0a69 6d70 6f72 7420 746f 7263  thon.import torc
+00003d00: 680a 0a66 726f 6d20 7a65 7461 2e6e 6e20  h..from zeta.nn 
+00003d10: 696d 706f 7274 2046 696c 6d0a 0a23 2049  import Film..# I
+00003d20: 6e69 7469 616c 697a 6520 7468 6520 4669  nitialize the Fi
+00003d30: 6c6d 206c 6179 6572 0a66 696c 6d5f 6c61  lm layer.film_la
+00003d40: 7965 7220 3d20 4669 6c6d 2864 696d 3d31  yer = Film(dim=1
+00003d50: 3238 2c20 6869 6464 656e 5f64 696d 3d36  28, hidden_dim=6
+00003d60: 342c 2065 7870 616e 7365 5f72 6174 696f  4, expanse_ratio
+00003d70: 3d34 290a 0a23 2043 7265 6174 6520 736f  =4)..# Create so
+00003d80: 6d65 2064 756d 6d79 2064 6174 6120 666f  me dummy data fo
+00003d90: 7220 636f 6e64 6974 696f 6e73 2061 6e64  r conditions and
+00003da0: 2068 6964 6465 6e73 0a63 6f6e 6469 7469   hiddens.conditi
+00003db0: 6f6e 7320 3d20 746f 7263 682e 7261 6e64  ons = torch.rand
+00003dc0: 6e28 3130 2c20 3132 3829 2020 2320 4261  n(10, 128)  # Ba
+00003dd0: 7463 6820 7369 7a65 2069 7320 3130 2c20  tch size is 10, 
+00003de0: 6665 6174 7572 6520 7369 7a65 2069 7320  feature size is 
+00003df0: 3132 380a 6869 6464 656e 7320 3d20 746f  128.hiddens = to
+00003e00: 7263 682e 7261 6e64 6e28 0a20 2020 2031  rch.randn(.    1
+00003e10: 302c 2031 2c20 3132 380a 2920 2023 2042  0, 1, 128.)  # B
+00003e20: 6174 6368 2073 697a 6520 6973 2031 302c  atch size is 10,
+00003e30: 2073 6571 7565 6e63 6520 6c65 6e67 7468   sequence length
+00003e40: 2069 7320 312c 2066 6561 7475 7265 2073   is 1, feature s
+00003e50: 697a 6520 6973 2031 3238 0a0a 2320 5061  ize is 128..# Pa
+00003e60: 7373 2074 6865 2064 6174 6120 7468 726f  ss the data thro
+00003e70: 7567 6820 7468 6520 4669 6c6d 206c 6179  ugh the Film lay
+00003e80: 6572 0a6d 6f64 756c 6174 6564 5f66 6561  er.modulated_fea
+00003e90: 7475 7265 7320 3d20 6669 6c6d 5f6c 6179  tures = film_lay
+00003ea0: 6572 2863 6f6e 6469 7469 6f6e 732c 2068  er(conditions, h
+00003eb0: 6964 6465 6e73 290a 0a23 2050 7269 6e74  iddens)..# Print
+00003ec0: 2074 6865 2073 6861 7065 206f 6620 7468   the shape of th
+00003ed0: 6520 6f75 7470 7574 0a70 7269 6e74 286d  e output.print(m
+00003ee0: 6f64 756c 6174 6564 5f66 6561 7475 7265  odulated_feature
+00003ef0: 732e 7368 6170 6529 2020 2320 5368 6f75  s.shape)  # Shou
+00003f00: 6c64 2062 6520 5b31 302c 2031 2c20 3132  ld be [10, 1, 12
+00003f10: 385d 0a60 6060 0a0a 2323 2320 6068 7970  8].```..### `hyp
+00003f20: 6572 5f6f 7074 696d 697a 6560 0a2d 2041  er_optimize`.- A
+00003f30: 2073 696e 676c 6520 7772 6170 7065 7220   single wrapper 
+00003f40: 666f 7220 746f 7263 682e 6678 2c20 746f  for torch.fx, to
+00003f50: 7263 682e 7363 7269 7074 2c20 746f 7263  rch.script, torc
+00003f60: 682e 636f 6d70 696c 652c 2064 796e 616d  h.compile, dynam
+00003f70: 6963 2071 7561 6e74 697a 6174 696f 6e2c  ic quantization,
+00003f80: 206d 6978 6564 2070 7265 6369 7369 6f6e   mixed precision
+00003f90: 2074 6872 6f75 6768 2074 6f72 6368 2e61   through torch.a
+00003fa0: 6d70 2c20 7769 7468 2065 7865 6375 7469  mp, with executi
+00003fb0: 6f6e 2074 696d 6520 6d65 7472 6963 7320  on time metrics 
+00003fc0: 616c 6c20 696e 206f 6e63 6520 706c 6163  all in once plac
+00003fd0: 6521 0a60 6060 7079 7468 6f6e 0a69 6d70  e!.```python.imp
+00003fe0: 6f72 7420 746f 7263 680a 0a66 726f 6d20  ort torch..from 
+00003ff0: 7a65 7461 2e6e 6e20 696d 706f 7274 2068  zeta.nn import h
+00004000: 7970 6572 5f6f 7074 696d 697a 650a 0a0a  yper_optimize...
+00004010: 4068 7970 6572 5f6f 7074 696d 697a 6528  @hyper_optimize(
+00004020: 0a20 2020 2074 6f72 6368 5f66 783d 4661  .    torch_fx=Fa
+00004030: 6c73 652c 0a20 2020 2074 6f72 6368 5f73  lse,.    torch_s
+00004040: 6372 6970 743d 4661 6c73 652c 0a20 2020  cript=False,.   
+00004050: 2074 6f72 6368 5f63 6f6d 7069 6c65 3d54   torch_compile=T
+00004060: 7275 652c 0a20 2020 2071 7561 6e74 697a  rue,.    quantiz
+00004070: 653d 5472 7565 2c0a 2020 2020 6d69 7865  e=True,.    mixe
+00004080: 645f 7072 6563 6973 696f 6e3d 5472 7565  d_precision=True
+00004090: 2c0a 2020 2020 656e 6162 6c65 5f6d 6574  ,.    enable_met
+000040a0: 7269 6373 3d54 7275 652c 0a29 0a64 6566  rics=True,.).def
+000040b0: 206d 6f64 656c 2878 293a 0a20 2020 2072   model(x):.    r
+000040c0: 6574 7572 6e20 7820 4020 780a 0a0a 6f75  eturn x @ x...ou
+000040d0: 7420 3d20 6d6f 6465 6c28 746f 7263 682e  t = model(torch.
+000040e0: 7261 6e64 6e28 312c 2033 2c20 3332 2c20  randn(1, 3, 32, 
+000040f0: 3332 2929 0a70 7269 6e74 286f 7574 290a  32)).print(out).
+00004100: 6060 600a 0a0a 2323 2320 4450 4f20 2d20  ```...### DPO - 
+00004110: 4469 7265 6374 2050 6f6c 6963 7920 4f70  Direct Policy Op
+00004120: 7469 6d69 7a61 7469 6f6e 0a44 6972 6563  timization.Direc
+00004130: 7420 506f 6c69 6379 204f 7074 696d 697a  t Policy Optimiz
+00004140: 6174 696f 6e20 656d 706c 6f79 6564 2066  ation employed f
+00004150: 6f72 206d 616e 7920 524c 4846 2061 7070  or many RLHF app
+00004160: 6c69 6361 7469 6f6e 7320 666f 7220 4c4c  lications for LL
+00004170: 4d73 2e0a 0a60 6060 7079 7468 6f6e 0a69  Ms...```python.i
+00004180: 6d70 6f72 7420 746f 7263 680a 6672 6f6d  mport torch.from
+00004190: 2074 6f72 6368 2069 6d70 6f72 7420 6e6e   torch import nn
+000041a0: 0a0a 6672 6f6d 207a 6574 612e 726c 2069  ..from zeta.rl i
+000041b0: 6d70 6f72 7420 4450 4f0a 0a0a 2320 4465  mport DPO...# De
+000041c0: 6669 6e65 2061 2073 696d 706c 6520 706f  fine a simple po
+000041d0: 6c69 6379 206d 6f64 656c 0a63 6c61 7373  licy model.class
+000041e0: 2050 6f6c 6963 794d 6f64 656c 286e 6e2e   PolicyModel(nn.
+000041f0: 4d6f 6475 6c65 293a 0a20 2020 2064 6566  Module):.    def
+00004200: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00004210: 696e 7075 745f 6469 6d2c 206f 7574 7075  input_dim, outpu
+00004220: 745f 6469 6d29 3a0a 2020 2020 2020 2020  t_dim):.        
+00004230: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00004240: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00004250: 6663 203d 206e 6e2e 4c69 6e65 6172 2869  fc = nn.Linear(i
+00004260: 6e70 7574 5f64 696d 2c20 6f75 7470 7574  nput_dim, output
+00004270: 5f64 696d 290a 0a20 2020 2064 6566 2066  _dim)..    def f
+00004280: 6f72 7761 7264 2873 656c 662c 2078 293a  orward(self, x):
+00004290: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000042a0: 7365 6c66 2e66 6328 7829 0a0a 0a69 6e70  self.fc(x)...inp
+000042b0: 7574 5f64 696d 203d 2031 300a 6f75 7470  ut_dim = 10.outp
+000042c0: 7574 5f64 696d 203d 2035 0a70 6f6c 6963  ut_dim = 5.polic
+000042d0: 795f 6d6f 6465 6c20 3d20 506f 6c69 6379  y_model = Policy
+000042e0: 4d6f 6465 6c28 696e 7075 745f 6469 6d2c  Model(input_dim,
+000042f0: 206f 7574 7075 745f 6469 6d29 0a0a 2320   output_dim)..# 
+00004300: 496e 6974 6961 6c69 7a65 2044 504f 2077  Initialize DPO w
+00004310: 6974 6820 7468 6520 706f 6c69 6379 206d  ith the policy m
+00004320: 6f64 656c 0a64 706f 5f6d 6f64 656c 203d  odel.dpo_model =
+00004330: 2044 504f 286d 6f64 656c 3d70 6f6c 6963   DPO(model=polic
+00004340: 795f 6d6f 6465 6c2c 2062 6574 613d 302e  y_model, beta=0.
+00004350: 3129 0a0a 2320 5361 6d70 6c65 2070 7265  1)..# Sample pre
+00004360: 6665 7272 6564 2061 6e64 2075 6e70 7265  ferred and unpre
+00004370: 6665 7272 6564 2073 6571 7565 6e63 6573  ferred sequences
+00004380: 0a70 7265 6665 7272 6564 5f73 6571 203d  .preferred_seq =
+00004390: 2074 6f72 6368 2e72 616e 6469 6e74 2830   torch.randint(0
+000043a0: 2c20 6f75 7470 7574 5f64 696d 2c20 2833  , output_dim, (3
+000043b0: 2c20 696e 7075 745f 6469 6d29 290a 756e  , input_dim)).un
+000043c0: 7072 6566 6572 7265 645f 7365 7120 3d20  preferred_seq = 
+000043d0: 746f 7263 682e 7261 6e64 696e 7428 302c  torch.randint(0,
+000043e0: 206f 7574 7075 745f 6469 6d2c 2028 332c   output_dim, (3,
+000043f0: 2069 6e70 7574 5f64 696d 2929 0a0a 2320   input_dim))..# 
+00004400: 436f 6d70 7574 6520 6c6f 7373 0a6c 6f73  Compute loss.los
+00004410: 7320 3d20 6470 6f5f 6d6f 6465 6c28 7072  s = dpo_model(pr
+00004420: 6566 6572 7265 645f 7365 712c 2075 6e70  eferred_seq, unp
+00004430: 7265 6665 7272 6564 5f73 6571 290a 7072  referred_seq).pr
+00004440: 696e 7428 6c6f 7373 290a 6060 600a 0a0a  int(loss).```...
+00004450: 2323 2320 5a65 7461 436c 6f75 640a 5472  ### ZetaCloud.Tr
+00004460: 6169 6e20 6f72 2066 696e 6574 756e 6520  ain or finetune 
+00004470: 616e 7920 6d6f 6465 6c20 6f6e 2061 6e79  any model on any
+00004480: 2063 6c75 7374 6572 2069 6e20 3120 636c   cluster in 1 cl
+00004490: 6963 6b20 7769 7468 207a 6574 6163 6c6f  ick with zetaclo
+000044a0: 7564 2c20 6a75 7374 2070 6173 7320 696e  ud, just pass in
+000044b0: 2079 6f75 7220 6669 6c65 2061 6e64 2074   your file and t
+000044c0: 6865 2047 5055 2074 7970 6520 616e 6420  he GPU type and 
+000044d0: 7175 616e 7469 7479 2079 6f75 2077 616e  quantity you wan
+000044e0: 7421 2054 6f20 6761 696e 2061 6363 6573  t! To gain acces
+000044f0: 7320 6669 7273 7420 6070 6970 2069 6e73  s first `pip ins
+00004500: 7461 6c6c 207a 6574 6173 6361 6c65 6020  tall zetascale` 
+00004510: 7468 656e 2072 756e 2060 7a65 7461 202d  then run `zeta -
+00004520: 6860 2069 6e20 7468 6520 7465 726d 696e  h` in the termin
+00004530: 616c 2e20 5b48 6572 6520 6973 2074 6865  al. [Here is the
+00004540: 2064 6f63 7320 666f 7220 6d6f 7265 5d28   docs for more](
+00004550: 6874 7470 733a 2f2f 7a65 7461 2e61 7061  https://zeta.apa
+00004560: 632e 6169 2f65 6e2f 6c61 7465 7374 2f7a  c.ai/en/latest/z
+00004570: 6574 612f 636c 6f75 642f 6d61 696e 2f29  eta/cloud/main/)
+00004580: 0a0a 2d20 466c 6578 6962 6c65 2050 7269  ..- Flexible Pri
+00004590: 6369 6e67 2077 6974 6820 706f 6f6c 696e  cing with poolin
+000045a0: 6720 6672 6f6d 206d 616e 7920 636c 6f75  g from many clou
+000045b0: 6473 0a2d 2045 6173 7920 4465 706c 6f79  ds.- Easy Deploy
+000045c0: 6d65 6e74 2077 6974 6820 3120 636c 6963  ment with 1 clic
+000045d0: 6b0a 2d20 5661 7269 6f75 7320 6f70 7469  k.- Various opti
+000045e0: 6f6e 7320 666f 7220 636c 6f75 6420 7072  ons for cloud pr
+000045f0: 6f76 6964 6572 7321 0a0a 6060 6062 6173  oviders!..```bas
+00004600: 680a 5a65 7461 636c 6f75 6420 434c 490a  h.Zetacloud CLI.
+00004610: 0a6f 7074 696f 6e73 3a0a 2020 2d68 2c20  .options:.  -h, 
+00004620: 2d2d 6865 6c70 2020 2020 2020 2020 2020  --help          
+00004630: 2020 7368 6f77 2074 6869 7320 6865 6c70    show this help
+00004640: 206d 6573 7361 6765 2061 6e64 2065 7869   message and exi
+00004650: 740a 2020 2d74 2054 4153 4b5f 4e41 4d45  t.  -t TASK_NAME
+00004660: 2c20 2d2d 7461 736b 5f6e 616d 6520 5441  , --task_name TA
+00004670: 534b 5f4e 414d 450a 2020 2020 2020 2020  SK_NAME.        
+00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004690: 5461 736b 206e 616d 650a 2020 2d63 2043  Task name.  -c C
+000046a0: 4c55 5354 4552 5f4e 414d 452c 202d 2d63  LUSTER_NAME, --c
+000046b0: 6c75 7374 6572 5f6e 616d 6520 434c 5553  luster_name CLUS
+000046c0: 5445 525f 4e41 4d45 0a20 2020 2020 2020  TER_NAME.       
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2043 6c75 7374 6572 206e 616d 650a 2020   Cluster name.  
+000046f0: 2d63 6c20 434c 4f55 442c 202d 2d63 6c6f  -cl CLOUD, --clo
+00004700: 7564 2043 4c4f 5544 0a20 2020 2020 2020  ud CLOUD.       
+00004710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004720: 2043 6c6f 7564 2070 726f 7669 6465 720a   Cloud provider.
+00004730: 2020 2d67 2047 5055 532c 202d 2d67 7075    -g GPUS, --gpu
+00004740: 7320 4750 5553 2020 4750 5573 0a20 202d  s GPUS  GPUs.  -
+00004750: 6620 4649 4c45 4e41 4d45 2c20 2d2d 6669  f FILENAME, --fi
+00004760: 6c65 6e61 6d65 2046 494c 454e 414d 450a  lename FILENAME.
+00004770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004780: 2020 2020 2020 2020 4669 6c65 6e61 6d65          Filename
+00004790: 0a20 202d 732c 202d 2d73 746f 7020 2020  .  -s, --stop   
+000047a0: 2020 2020 2020 2020 2053 746f 7020 666c           Stop fl
+000047b0: 6167 0a20 202d 642c 202d 2d64 6f77 6e20  ag.  -d, --down 
+000047c0: 2020 2020 2020 2020 2020 2044 6f77 6e20             Down 
+000047d0: 666c 6167 0a20 202d 7372 2c20 2d2d 7374  flag.  -sr, --st
+000047e0: 6174 7573 5f72 6570 6f72 7420 2053 7461  atus_report  Sta
+000047f0: 7475 7320 7265 706f 7274 2066 6c61 670a  tus report flag.
+00004800: 0a60 6060 0a0a 2d20 4120 7369 6d70 6c65  .```..- A simple
+00004810: 2072 756e 2065 7861 6d70 6c65 2063 6f64   run example cod
+00004820: 6520 776f 756c 6420 6265 206c 696b 653a  e would be like:
+00004830: 0a0a 6060 6062 6173 680a 7a65 7461 202d  ..```bash.zeta -
+00004840: 6620 7472 6169 6e2e 7079 202d 6720 4131  f train.py -g A1
+00004850: 3030 3a38 0a60 6060 0a2d 2d2d 2d0a 0a0a  00:8.```.----...
+00004860: 2320 446f 6375 6d65 6e74 6174 696f 6e0a  # Documentation.
+00004870: 416c 6c20 636c 6173 7365 7320 6d75 7374  All classes must
+00004880: 2068 6176 6520 646f 6375 6d65 6e74 6174   have documentat
+00004890: 696f 6e20 6966 2079 6f75 2073 6565 2061  ion if you see a
+000048a0: 2063 6c61 7373 206f 7220 6675 6e63 7469   class or functi
+000048b0: 6f6e 2077 6974 686f 7574 2064 6f63 756d  on without docum
+000048c0: 656e 7461 7469 6f6e 2074 6865 6e20 706c  entation then pl
+000048d0: 6561 7365 2072 6570 6f72 7420 6974 2074  ease report it t
+000048e0: 6f20 6d65 2061 7420 6b79 6540 6170 6163  o me at kye@apac
+000048f0: 2e61 692c 0a0a 446f 6375 6d65 6e74 6174  .ai,..Documentat
+00004900: 696f 6e20 6973 2061 7420 5b7a 6574 612e  ion is at [zeta.
+00004910: 6170 6163 2e61 695d 2868 7474 7073 3a2f  apac.ai](https:/
+00004920: 2f7a 6574 612e 6170 6163 2e61 692f 290a  /zeta.apac.ai/).
+00004930: 0a0a 2d2d 2d2d 2d2d 2d0a 0a0a 2320 5275  ..-------...# Ru
+00004940: 6e6e 696e 6720 7465 7374 730a 596f 7520  nning tests.You 
+00004950: 7368 6f75 6c64 2069 6e73 7461 6c6c 2074  should install t
+00004960: 6865 2070 7265 2d63 6f6d 6d69 7420 686f  he pre-commit ho
+00004970: 6f6b 7320 7769 7468 2070 7265 2d63 6f6d  oks with pre-com
+00004980: 6d69 7420 696e 7374 616c 6c2e 2054 6869  mit install. Thi
+00004990: 7320 7769 6c6c 2072 756e 2074 6865 206c  s will run the l
+000049a0: 696e 7465 722c 206d 7970 792c 2061 6e64  inter, mypy, and
+000049b0: 2061 2073 7562 7365 7420 6f66 2074 6865   a subset of the
+000049c0: 2074 6573 7473 206f 6e20 6576 6572 7920   tests on every 
+000049d0: 636f 6d6d 6974 2e0a 0a46 6f72 206d 6f72  commit...For mor
+000049e0: 6520 6578 616d 706c 6573 206f 6e20 686f  e examples on ho
+000049f0: 7720 746f 2072 756e 2074 6865 2066 756c  w to run the ful
+00004a00: 6c20 7465 7374 2073 7569 7465 2070 6c65  l test suite ple
+00004a10: 6173 6520 7265 6665 7220 746f 2074 6865  ase refer to the
+00004a20: 2043 4920 776f 726b 666c 6f77 2e0a 0a53   CI workflow...S
+00004a30: 6f6d 6520 6578 616d 706c 6573 206f 6620  ome examples of 
+00004a40: 7275 6e6e 696e 6720 7465 7374 7320 6c6f  running tests lo
+00004a50: 6361 6c6c 793a 0a0a 6060 6062 6173 680a  cally:..```bash.
+00004a60: 7079 7468 6f6e 3320 2d6d 2070 6970 2069  python3 -m pip i
+00004a70: 6e73 7461 6c6c 202d 6520 272e 5b74 6573  nstall -e '.[tes
+00004a80: 7469 6e67 5d27 2020 2320 696e 7374 616c  ting]'  # instal
+00004a90: 6c20 6578 7472 6120 6465 7073 2066 6f72  l extra deps for
+00004aa0: 2074 6573 7469 6e67 0a70 7974 686f 6e33   testing.python3
+00004ab0: 202d 6d20 7079 7465 7374 2074 6573 7473   -m pytest tests
+00004ac0: 2f20 2020 2020 2020 2020 2020 2020 2020  /               
+00004ad0: 2020 2320 7768 6f6c 6520 7465 7374 2073    # whole test s
+00004ae0: 7569 7465 0a60 6060 0a2d 2d2d 2d0a 0a23  uite.```.----..#
+00004af0: 2320 436f 6d6d 756e 6974 790a 0a4a 6f69  # Community..Joi
+00004b00: 6e20 6f75 7220 6772 6f77 696e 6720 636f  n our growing co
+00004b10: 6d6d 756e 6974 7920 6172 6f75 6e64 2074  mmunity around t
+00004b20: 6865 2077 6f72 6c64 2c20 666f 7220 7265  he world, for re
+00004b30: 616c 2d74 696d 6520 7375 7070 6f72 742c  al-time support,
+00004b40: 2069 6465 6173 2c20 616e 6420 6469 7363   ideas, and disc
+00004b50: 7573 7369 6f6e 7320 6f6e 2068 6f77 2074  ussions on how t
+00004b60: 6f20 6275 696c 6420 6265 7474 6572 206d  o build better m
+00004b70: 6f64 656c 7320 f09f 988a 200a 0a2d 2056  odels .... ..- V
+00004b80: 6965 7720 6f75 7220 6f66 6669 6369 616c  iew our official
+00004b90: 205b 446f 6373 5d28 6874 7470 733a 2f2f   [Docs](https://
+00004ba0: 7a65 7461 2e61 7061 632e 6169 290a 2d20  zeta.apac.ai).- 
+00004bb0: 4368 6174 206c 6976 6520 7769 7468 2075  Chat live with u
+00004bc0: 7320 6f6e 205b 4469 7363 6f72 645d 2868  s on [Discord](h
+00004bd0: 7474 7073 3a2f 2f64 6973 636f 7264 2e67  ttps://discord.g
+00004be0: 672f 6b53 3372 774b 7333 5a43 290a 2d20  g/kS3rwKs3ZC).- 
+00004bf0: 466f 6c6c 6f77 2075 7320 6f6e 205b 5477  Follow us on [Tw
+00004c00: 6974 7465 725d 2868 7474 7073 3a2f 2f74  itter](https://t
+00004c10: 7769 7474 6572 2e63 6f6d 2f6b 7965 676f  witter.com/kyego
+00004c20: 6d65 7a29 0a2d 2043 6f6e 6e65 6374 2077  mez).- Connect w
+00004c30: 6974 6820 7573 206f 6e20 5b4c 696e 6b65  ith us on [Linke
+00004c40: 6449 6e5d 2868 7474 7073 3a2f 2f77 7777  dIn](https://www
+00004c50: 2e6c 696e 6b65 6469 6e2e 636f 6d2f 636f  .linkedin.com/co
+00004c60: 6d70 616e 792f 7468 652d 7377 6172 6d2d  mpany/the-swarm-
+00004c70: 636f 7270 6f72 6174 696f 6e29 0a2d 2056  corporation).- V
+00004c80: 6973 6974 2075 7320 6f6e 205b 596f 7554  isit us on [YouT
+00004c90: 7562 655d 2868 7474 7073 3a2f 2f77 7777  ube](https://www
+00004ca0: 2e79 6f75 7475 6265 2e63 6f6d 2f63 6861  .youtube.com/cha
+00004cb0: 6e6e 656c 2f55 4339 7958 7969 746b 6255  nnel/UC9yXyitkbU
+00004cc0: 5f57 5379 3762 645f 3431 5371 5129 0a2d  _WSy7bd_41SqQ).-
+00004cd0: 205b 4a6f 696e 2074 6865 2053 7761 726d   [Join the Swarm
+00004ce0: 7320 636f 6d6d 756e 6974 7920 6f6e 2044  s community on D
+00004cf0: 6973 636f 7264 215d 2868 7474 7073 3a2f  iscord!](https:/
+00004d00: 2f64 6973 636f 7264 2e67 672f 414a 617a  /discord.gg/AJaz
+00004d10: 426d 684b 6e72 290a 0a2d 2d2d 0a0a 2320  BmhKnr)..---..# 
+00004d20: f09f a49d 2053 6368 6564 756c 6520 6120  .... Schedule a 
+00004d30: 312d 6f6e 2d31 2053 6573 7369 6f6e 0a57  1-on-1 Session.W
+00004d40: 616e 7420 746f 2074 7261 696e 2061 2063  ant to train a c
+00004d50: 7573 746f 6d20 4149 206d 6f64 656c 2066  ustom AI model f
+00004d60: 6f72 2061 2072 6561 6c2d 776f 726c 6420  or a real-world 
+00004d70: 7461 736b 206c 696b 6520 4765 6e65 7261  task like Genera
+00004d80: 6c20 4d75 6c74 692d 4d6f 6461 6c20 4d6f  l Multi-Modal Mo
+00004d90: 6465 6c73 2c20 4661 6369 616c 2052 6563  dels, Facial Rec
+00004da0: 6f67 6e69 7469 6f6e 732c 2044 7275 6720  ognitions, Drug 
+00004db0: 4469 7363 6f76 6572 792c 2048 756d 616e  Discovery, Human
+00004dc0: 6f69 6420 526f 626f 7469 6373 3f20 4927  oid Robotics? I'
+00004dd0: 6c6c 2068 656c 7020 796f 7520 6372 6561  ll help you crea
+00004de0: 7465 2074 6865 206d 6f64 656c 2061 7263  te the model arc
+00004df0: 6869 7465 6374 7572 6520 7468 656e 2074  hitecture then t
+00004e00: 7261 696e 2074 6865 206d 6f64 656c 2061  rain the model a
+00004e10: 6e64 2074 6865 6e20 6f70 7469 6d69 7a65  nd then optimize
+00004e20: 2069 7420 746f 206d 6565 7420 796f 7572   it to meet your
+00004e30: 2071 7561 6c69 7479 2061 7373 7572 616e   quality assuran
+00004e40: 6365 2073 7461 6e64 6172 6473 2e0a 0a42  ce standards...B
+00004e50: 6f6f 6b20 6120 5b31 2d6f 6e2d 3120 5365  ook a [1-on-1 Se
+00004e60: 7373 696f 6e20 7769 7468 204b 7965 2068  ssion with Kye h
+00004e70: 6572 652e 5d28 6874 7470 733a 2f2f 6361  ere.](https://ca
+00004e80: 6c65 6e64 6c79 2e63 6f6d 2f61 7061 6361  lendly.com/apaca
+00004e90: 692f 6167 6f72 6129 2c20 7468 6520 4372  i/agora), the Cr
+00004ea0: 6561 746f 722c 2074 6f20 6469 7363 7573  eator, to discus
+00004eb0: 7320 616e 7920 6973 7375 6573 2c20 7072  s any issues, pr
+00004ec0: 6f76 6964 6520 6665 6564 6261 636b 2c20  ovide feedback, 
+00004ed0: 6f72 2065 7870 6c6f 7265 2068 6f77 2077  or explore how w
+00004ee0: 6520 6361 6e20 696d 7072 6f76 6520 5a65  e can improve Ze
+00004ef0: 7461 2066 6f72 2079 6f75 206f 7220 6865  ta for you or he
+00004f00: 6c70 2079 6f75 2062 7569 6c64 2079 6f75  lp you build you
+00004f10: 7220 6f77 6e20 6375 7374 6f6d 206d 6f64  r own custom mod
+00004f20: 656c 7321 0a0a 2323 20f0 9fab b620 436f  els!..## .... Co
+00004f30: 6e74 7269 6275 7469 6f6e 733a 0a0a 5468  ntributions:..Th
+00004f40: 6520 6561 7369 6573 7420 7761 7920 746f  e easiest way to
+00004f50: 2063 6f6e 7472 6962 7574 6520 6973 2074   contribute is t
+00004f60: 6f20 7069 636b 2061 6e79 2069 7373 7565  o pick any issue
+00004f70: 2077 6974 6820 7468 6520 6067 6f6f 6420   with the `good 
+00004f80: 6669 7273 7420 6973 7375 6560 2074 6167  first issue` tag
+00004f90: 20f0 9f92 aa2e 2052 6561 6420 7468 6520   ..... Read the 
+00004fa0: 436f 6e74 7269 6275 7469 6e67 2067 7569  Contributing gui
+00004fb0: 6465 6c69 6e65 7320 5b68 6572 655d 282f  delines [here](/
+00004fc0: 434f 4e54 5249 4255 5449 4e47 2e6d 6429  CONTRIBUTING.md)
+00004fd0: 2e20 4275 6720 5265 706f 7274 3f20 5b46  . Bug Report? [F
+00004fe0: 696c 6520 6865 7265 5d28 6874 7470 733a  ile here](https:
+00004ff0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 7965  //github.com/kye
+00005000: 676f 6d65 7a2f 7a65 7461 2f69 7373 7565  gomez/zeta/issue
+00005010: 732f 6e65 772f 6368 6f6f 7365 2920 7c20  s/new/choose) | 
+00005020: 4665 6174 7572 6520 5265 7175 6573 743f  Feature Request?
+00005030: 205b 4669 6c65 2068 6572 655d 2868 7474   [File here](htt
+00005040: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00005050: 6b79 6567 6f6d 657a 2f7a 6574 612f 6973  kyegomez/zeta/is
+00005060: 7375 6573 2f6e 6577 2f63 686f 6f73 6529  sues/new/choose)
+00005070: 0a0a 5a65 7461 2069 7320 616e 206f 7065  ..Zeta is an ope
+00005080: 6e2d 736f 7572 6365 2070 726f 6a65 6374  n-source project
+00005090: 2c20 616e 6420 636f 6e74 7269 6275 7469  , and contributi
+000050a0: 6f6e 7320 6172 6520 5645 5259 2077 656c  ons are VERY wel
+000050b0: 636f 6d65 2e20 4966 2079 6f75 2077 616e  come. If you wan
+000050c0: 7420 746f 2063 6f6e 7472 6962 7574 652c  t to contribute,
+000050d0: 2079 6f75 2063 616e 2063 7265 6174 6520   you can create 
+000050e0: 6e65 7720 6665 6174 7572 6573 2c20 6669  new features, fi
+000050f0: 7820 6275 6773 2c20 6f72 2069 6d70 726f  x bugs, or impro
+00005100: 7665 2074 6865 2069 6e66 7261 7374 7275  ve the infrastru
+00005110: 6374 7572 652e 2050 6c65 6173 6520 7265  cture. Please re
+00005120: 6665 7220 746f 2074 6865 205b 434f 4e54  fer to the [CONT
+00005130: 5249 4255 5449 4e47 2e6d 645d 2868 7474  RIBUTING.md](htt
+00005140: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00005150: 6b79 6567 6f6d 657a 2f7a 6574 612f 626c  kyegomez/zeta/bl
+00005160: 6f62 2f6d 6173 7465 722f 434f 4e54 5249  ob/master/CONTRI
+00005170: 4255 5449 4e47 2e6d 6429 2061 6e64 206f  BUTING.md) and o
+00005180: 7572 205b 636f 6e74 7269 6275 7469 6e67  ur [contributing
+00005190: 2062 6f61 7264 5d28 6874 7470 733a 2f2f   board](https://
+000051a0: 6769 7468 7562 2e63 6f6d 2f75 7365 7273  github.com/users
+000051b0: 2f6b 7965 676f 6d65 7a2f 7072 6f6a 6563  /kyegomez/projec
+000051c0: 7473 2f31 2920 746f 2070 6172 7469 6369  ts/1) to partici
+000051d0: 7061 7465 2069 6e20 526f 6164 6d61 7020  pate in Roadmap 
+000051e0: 6469 7363 7573 7369 6f6e 7321 0a0a 3c61  discussions!..<a
+000051f0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00005200: 6974 6875 622e 636f 6d2f 6b79 6567 6f6d  ithub.com/kyegom
+00005210: 657a 2f7a 6574 612f 6772 6170 6873 2f63  ez/zeta/graphs/c
+00005220: 6f6e 7472 6962 7574 6f72 7322 3e0a 2020  ontributors">.  
+00005230: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00005240: 2f2f 636f 6e74 7269 622e 726f 636b 732f  //contrib.rocks/
+00005250: 696d 6167 653f 7265 706f 3d6b 7965 676f  image?repo=kyego
+00005260: 6d65 7a2f 7a65 7461 2220 2f3e 0a3c 2f61  mez/zeta" />.</a
+00005270: 3e0a 0a2d 2d2d 2d0a 0a23 2320 4163 6365  >..----..## Acce
+00005280: 6c65 7261 7465 2042 6163 6b6c 6f67 0a48  lerate Backlog.H
+00005290: 656c 7020 7573 2061 6363 656c 6572 6174  elp us accelerat
+000052a0: 6520 6f75 7220 6261 636b 6c6f 6720 6279  e our backlog by
+000052b0: 2073 7570 706f 7274 696e 6720 7573 2066   supporting us f
+000052c0: 696e 616e 6369 616c 6c79 2120 4e6f 7465  inancially! Note
+000052d0: 2c20 7765 2772 6520 616e 206f 7065 6e20  , we're an open 
+000052e0: 736f 7572 6365 2063 6f72 706f 7261 7469  source corporati
+000052f0: 6f6e 2061 6e64 2073 6f20 616c 6c20 7468  on and so all th
+00005300: 6520 7265 7665 6e75 6520 7765 2067 656e  e revenue we gen
+00005310: 6572 6174 6520 6973 2074 6872 6f75 6768  erate is through
+00005320: 2064 6f6e 6174 696f 6e73 2061 7420 7468   donations at th
+00005330: 6520 6d6f 6d65 6e74 203b 290a 0a3c 6120  e moment ;)..<a 
+00005340: 6872 6566 3d22 6874 7470 733a 2f2f 706f  href="https://po
+00005350: 6c61 722e 7368 2f6b 7965 676f 6d65 7a22  lar.sh/kyegomez"
+00005360: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00005370: 3a2f 2f70 6f6c 6172 2e73 682f 656d 6265  ://polar.sh/embe
+00005380: 642f 6675 6e64 2d6f 7572 2d62 6163 6b6c  d/fund-our-backl
+00005390: 6f67 2e73 7667 3f6f 7267 3d6b 7965 676f  og.svg?org=kyego
+000053a0: 6d65 7a22 202f 3e3c 2f61 3e0a 0a0a 2320  mez" /></a>...# 
+000053b0: 4c69 6365 6e73 6520 0a2d 2041 7061 6368  License .- Apach
+000053c0: 650a 0a                                  e..
```

