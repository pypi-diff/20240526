# Comparing `tmp/patch_conv-0.0.0b0.tar.gz` & `tmp/patch_conv-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patch_conv-0.0.0b0.tar", last modified: Sun Mar 10 08:03:43 2024, max compression
+gzip compressed data, was "patch_conv-0.0.1b0.tar", last modified: Sun May 26 05:12:35 2024, max compression
```

## Comparing `patch_conv-0.0.0b0.tar` & `patch_conv-0.0.1b0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-10 08:03:43.529056 patch_conv-0.0.0b0/
--rw-r--r--   0 lmxyy      (501) staff       (20)     3402 2024-03-10 08:03:43.528790 patch_conv-0.0.0b0/PKG-INFO
--rw-r--r--   0 lmxyy      (501) staff       (20)     2965 2024-03-10 08:00:59.000000 patch_conv-0.0.0b0/README.md
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-10 08:03:43.527706 patch_conv-0.0.0b0/patch_conv/
--rw-r--r--   0 lmxyy      (501) staff       (20)       65 2024-03-06 19:01:33.000000 patch_conv-0.0.0b0/patch_conv/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)       27 2024-03-10 08:02:06.000000 patch_conv-0.0.0b0/patch_conv/__version__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     1705 2024-03-10 04:11:29.000000 patch_conv-0.0.0b0/patch_conv/module.py
--rw-r--r--   0 lmxyy      (501) staff       (20)      839 2024-03-10 02:21:04.000000 patch_conv-0.0.0b0/patch_conv/utils.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-10 08:03:43.528484 patch_conv-0.0.0b0/patch_conv.egg-info/
--rw-r--r--   0 lmxyy      (501) staff       (20)     3402 2024-03-10 08:03:43.000000 patch_conv-0.0.0b0/patch_conv.egg-info/PKG-INFO
--rw-r--r--   0 lmxyy      (501) staff       (20)      277 2024-03-10 08:03:43.000000 patch_conv-0.0.0b0/patch_conv.egg-info/SOURCES.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)        1 2024-03-10 08:03:43.000000 patch_conv-0.0.0b0/patch_conv.egg-info/dependency_links.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)        6 2024-03-10 08:03:43.000000 patch_conv-0.0.0b0/patch_conv.egg-info/requires.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)       11 2024-03-10 08:03:43.000000 patch_conv-0.0.0b0/patch_conv.egg-info/top_level.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)       38 2024-03-10 08:03:43.529106 patch_conv-0.0.0b0/setup.cfg
--rw-r--r--   0 lmxyy      (501) staff       (20)      923 2024-03-10 02:22:03.000000 patch_conv-0.0.0b0/setup.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-26 05:12:35.570531 patch_conv-0.0.1b0/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1068 2024-03-11 04:12:32.000000 patch_conv-0.0.1b0/LICENSE.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)     3797 2024-05-26 05:12:35.570301 patch_conv-0.0.1b0/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)     3335 2024-05-26 05:04:21.000000 patch_conv-0.0.1b0/README.md
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-26 05:12:35.569250 patch_conv-0.0.1b0/patch_conv/
+-rw-r--r--   0 lmxyy      (501) staff       (20)       65 2024-03-06 19:01:33.000000 patch_conv-0.0.1b0/patch_conv/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)       27 2024-05-26 05:08:39.000000 patch_conv-0.0.1b0/patch_conv/__version__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2037 2024-05-26 05:11:37.000000 patch_conv-0.0.1b0/patch_conv/module.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)      839 2024-03-10 02:21:04.000000 patch_conv-0.0.1b0/patch_conv/utils.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-26 05:12:35.569953 patch_conv-0.0.1b0/patch_conv.egg-info/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     3797 2024-05-26 05:12:35.000000 patch_conv-0.0.1b0/patch_conv.egg-info/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)      289 2024-05-26 05:12:35.000000 patch_conv-0.0.1b0/patch_conv.egg-info/SOURCES.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)        1 2024-05-26 05:12:35.000000 patch_conv-0.0.1b0/patch_conv.egg-info/dependency_links.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)        6 2024-05-26 05:12:35.000000 patch_conv-0.0.1b0/patch_conv.egg-info/requires.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       11 2024-05-26 05:12:35.000000 patch_conv-0.0.1b0/patch_conv.egg-info/top_level.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       38 2024-05-26 05:12:35.570577 patch_conv-0.0.1b0/setup.cfg
+-rw-r--r--   0 lmxyy      (501) staff       (20)      923 2024-03-10 02:22:03.000000 patch_conv-0.0.1b0/setup.py
```

### Comparing `patch_conv-0.0.0b0/PKG-INFO` & `patch_conv-0.0.1b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: patch_conv
-Version: 0.0.0b0
+Version: 0.0.1b0
 Summary: Patch convolution to avoid large GPU memory usage of Conv2D
 Home-page: https://github.com/mit-han-lab/patch_conv
 Author: Muyang Li, Ligeng Zhu, and Tianle Cai
 Author-email: muyangli@mit.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: torch
 
-# PatchConv: Patch convolution to avoid large GPU memory usage of Conv2D [[Blog]](https://hanlab.mit.edu/blog/patchconv)
+# Patch Conv: Patch convolution to avoid large GPU memory usage of Conv2D [[Blog]](https://hanlab.mit.edu/blog/patch-conv)
 
 ![patch_conv](https://github.com/mit-han-lab/patch_conv/blob/main/assets/patch_conv.jpg)
 
 ## Background
 
-For high-resolution content generation, neural networks may require applying convolution over large-size activations. Currently, PyTorch tends to consume excessive memory for these operations, potentially leading to memory shortages even on 80GB A100 GPUs. As shown in the below figure, starting with input of 1G parameters (channel×height×width), the memory demands of standard PyTorch convolutions increase significantly more rapidly with the activation size  than before. When the input is larger than 2G parameters, the convolution will use up all the 80G memory.
+In current generative models, we usually apply convolutions over large-size activations to generate high-resolution content. However, PyTorch tends to use excessive memory for these operations, potentially leading to memory shortages even on 80GB A100 GPUs. 
+
+As shown in the figure below, memory demands for standard PyTorch convolutions drastically increase when the input size reaches 1B parameters (channel×height×width). Notably, with a kernel size of 7×7, the 80GB A100 GPUs would trigger Out of Memory (OOM) errors. Inputs exceeding 2B parameters can further cause 3×3 convolutions exhaust all the memory and that’s just for one layer! This memory bottleneck prevents users and the community from scaling up the models to produce high-quality images.
 
 To bypass this issue and reduce memory consumption, we propose a simple and effective solution -- Patch Conv. As shown in the above figure, similar to [SIGE](https://github.com/lmxyy/sige), Patch Conv first divides the input into several smaller patches along the height dimension while keeping some overlap between them. These patches are then reorganized into the batch dimension and fed into the original convolution to produce output patches, which are then concatenated together to form the final output. Patch Conv can reduce memory usage by over 2.4×, providing a viable workaround for the limitations of current implementations.
 
-![background](https://github.com/mit-han-lab/patch_conv/blob/main/assets/background.jpg)
+<p align="center">
+  <img src="https://github.com/mit-han-lab/patch_conv/blob/main/assets/background.jpg" width="80%"/>
+</p>
 
 ## Installation
 
 After installing [PyTorch](https://pytorch.org), you can install `PatchConv` from PyPI:
 
 ```shell
 pip install patch_conv
@@ -37,15 +42,15 @@
 pip install git+https://github.com/mit-han-lab/patch_conv.git
 ```
 
 or locally for development:
 
 ```shell
 git clone git@github.com:mit-han-lab/patch_conv.git
-cd distrifuser
+cd patch_conv
 pip install -e .
 ```
 
 ## Usage
 
 All you need to do is use [`convert_model`](https://github.com/mit-han-lab/patch_conv/blob/main/patch_conv/utils.py#L6) to wrap all the `Conv2d` in your PyTorch model to our `PatchConv`. For example,
 
@@ -64,9 +69,10 @@
 
 ![performance](https://github.com/mit-han-lab/patch_conv/blob/main/assets/performance.jpg)
 
 Patch Conv significantly reduces memory consumption by over 2.4× across various kernel sizes and input resolutions with a marginally slower inference speed compared to vanilla convolution.
 
 ## Related Projects
 
-* [DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models](https://github.com/mit-han-lab/distrifuser), Li *et al.*, CVPR 2024
+* [MCUNetV2: Memory-Efficient Patch-based Inference for Tiny Deep Learning](https://arxiv.org/abs/2110.15352), Lin *et al.*, NeurIPS 2021
 * [Efficient Spatially Sparse Inference for Conditional GANs and Diffusion Models](https://github.com/lmxyy/sige), Li *et al.*, NeurIPS 2022
+* [DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models](https://github.com/mit-han-lab/distrifuser), Li *et al.*, CVPR 2024
```

### Comparing `patch_conv-0.0.0b0/README.md` & `patch_conv-0.0.1b0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-# PatchConv: Patch convolution to avoid large GPU memory usage of Conv2D [[Blog]](https://hanlab.mit.edu/blog/patchconv)
+# Patch Conv: Patch convolution to avoid large GPU memory usage of Conv2D [[Blog]](https://hanlab.mit.edu/blog/patch-conv)
 
 ![patch_conv](https://github.com/mit-han-lab/patch_conv/blob/main/assets/patch_conv.jpg)
 
 ## Background
 
-For high-resolution content generation, neural networks may require applying convolution over large-size activations. Currently, PyTorch tends to consume excessive memory for these operations, potentially leading to memory shortages even on 80GB A100 GPUs. As shown in the below figure, starting with input of 1G parameters (channel×height×width), the memory demands of standard PyTorch convolutions increase significantly more rapidly with the activation size  than before. When the input is larger than 2G parameters, the convolution will use up all the 80G memory.
+In current generative models, we usually apply convolutions over large-size activations to generate high-resolution content. However, PyTorch tends to use excessive memory for these operations, potentially leading to memory shortages even on 80GB A100 GPUs. 
+
+As shown in the figure below, memory demands for standard PyTorch convolutions drastically increase when the input size reaches 1B parameters (channel×height×width). Notably, with a kernel size of 7×7, the 80GB A100 GPUs would trigger Out of Memory (OOM) errors. Inputs exceeding 2B parameters can further cause 3×3 convolutions exhaust all the memory and that’s just for one layer! This memory bottleneck prevents users and the community from scaling up the models to produce high-quality images.
 
 To bypass this issue and reduce memory consumption, we propose a simple and effective solution -- Patch Conv. As shown in the above figure, similar to [SIGE](https://github.com/lmxyy/sige), Patch Conv first divides the input into several smaller patches along the height dimension while keeping some overlap between them. These patches are then reorganized into the batch dimension and fed into the original convolution to produce output patches, which are then concatenated together to form the final output. Patch Conv can reduce memory usage by over 2.4×, providing a viable workaround for the limitations of current implementations.
 
-![background](https://github.com/mit-han-lab/patch_conv/blob/main/assets/background.jpg)
+<p align="center">
+  <img src="https://github.com/mit-han-lab/patch_conv/blob/main/assets/background.jpg" width="80%"/>
+</p>
 
 ## Installation
 
 After installing [PyTorch](https://pytorch.org), you can install `PatchConv` from PyPI:
 
 ```shell
 pip install patch_conv
@@ -24,15 +28,15 @@
 pip install git+https://github.com/mit-han-lab/patch_conv.git
 ```
 
 or locally for development:
 
 ```shell
 git clone git@github.com:mit-han-lab/patch_conv.git
-cd distrifuser
+cd patch_conv
 pip install -e .
 ```
 
 ## Usage
 
 All you need to do is use [`convert_model`](https://github.com/mit-han-lab/patch_conv/blob/main/patch_conv/utils.py#L6) to wrap all the `Conv2d` in your PyTorch model to our `PatchConv`. For example,
 
@@ -51,9 +55,10 @@
 
 ![performance](https://github.com/mit-han-lab/patch_conv/blob/main/assets/performance.jpg)
 
 Patch Conv significantly reduces memory consumption by over 2.4× across various kernel sizes and input resolutions with a marginally slower inference speed compared to vanilla convolution.
 
 ## Related Projects
 
+* [MCUNetV2: Memory-Efficient Patch-based Inference for Tiny Deep Learning](https://arxiv.org/abs/2110.15352), Lin *et al.*, NeurIPS 2021
+* [Efficient Spatially Sparse Inference for Conditional GANs and Diffusion Models](https://github.com/lmxyy/sige), Li *et al.*, NeurIPS 2022
 * [DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models](https://github.com/mit-han-lab/distrifuser), Li *et al.*, CVPR 2024
-* [Efficient Spatially Sparse Inference for Conditional GANs and Diffusion Models](https://github.com/lmxyy/sige), Li *et al.*, NeurIPS 2022
```

### Comparing `patch_conv-0.0.0b0/patch_conv/module.py` & `patch_conv-0.0.1b0/patch_conv/module.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import torch
 from torch import nn
 from torch.nn import functional as F
 
 
 class PatchConv2d(nn.Module):
-    def __init__(self, splits: int = 4, conv2d: nn.Conv2d = None, *args, **kwargs):
+    def __init__(self, splits: int = 4, sequential: bool = True, conv2d: nn.Conv2d = None, *args, **kwargs):
         super(PatchConv2d, self).__init__()
+        self.splits = splits
+        self.sequential = sequential
         if conv2d is not None:
             self.conv2d = conv2d
-            self.splits = splits
         else:
             self.conv2d = nn.Conv2d(*args, **kwargs)
-            self.splits = splits
 
     def forward(self, x: torch.Tensor, *args, **kwargs) -> torch.Tensor:
         b, c, h, w = x.shape
         if c * h * w >= (1 << 30):
             assert h % self.splits == 0
             x_permuted = x.view(b, c, self.splits, h // self.splits, w).permute(0, 2, 1, 3, 4)
             x_padded = F.pad(
@@ -25,14 +25,21 @@
                 value=0,
             )
             x_padded[:, 1:, :, : self.conv2d.padding[0]] = x_permuted[:, :-1, :, -self.conv2d.padding[0] :]
             x_padded[:, :-1, :, -self.conv2d.padding[0] :] = x_permuted[:, 1:, :, : self.conv2d.padding[0]]
             x_padded = x_padded.view(b * self.splits, c, -1, w)
             padding_bak = self.conv2d.padding
             self.conv2d.padding = (0, self.conv2d.padding[1])
-            output = self.conv2d(x_padded, *args, **kwargs)
+            if self.sequential:
+                outputs = []
+                for i in range(x_padded.shape[0]):
+                    output = self.conv2d(x_padded[i : i + 1], *args, **kwargs)
+                    outputs.append(output)
+                output = torch.cat(outputs, dim=0)
+            else:
+                output = self.conv2d(x_padded, *args, **kwargs)
             self.conv2d.padding = padding_bak
             _, oc, oh, ow = output.shape
             output = output.view(b, self.splits, oc, oh, ow).permute(0, 2, 1, 3, 4).reshape(b, oc, -1, ow)
             return output
         else:
             return self.conv2d(x, *args, **kwargs)
```

### Comparing `patch_conv-0.0.0b0/patch_conv/utils.py` & `patch_conv-0.0.1b0/patch_conv/utils.py`

 * *Files identical despite different names*

### Comparing `patch_conv-0.0.0b0/patch_conv.egg-info/PKG-INFO` & `patch_conv-0.0.1b0/patch_conv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: patch-conv
-Version: 0.0.0b0
+Version: 0.0.1b0
 Summary: Patch convolution to avoid large GPU memory usage of Conv2D
 Home-page: https://github.com/mit-han-lab/patch_conv
 Author: Muyang Li, Ligeng Zhu, and Tianle Cai
 Author-email: muyangli@mit.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: torch
 
-# PatchConv: Patch convolution to avoid large GPU memory usage of Conv2D [[Blog]](https://hanlab.mit.edu/blog/patchconv)
+# Patch Conv: Patch convolution to avoid large GPU memory usage of Conv2D [[Blog]](https://hanlab.mit.edu/blog/patch-conv)
 
 ![patch_conv](https://github.com/mit-han-lab/patch_conv/blob/main/assets/patch_conv.jpg)
 
 ## Background
 
-For high-resolution content generation, neural networks may require applying convolution over large-size activations. Currently, PyTorch tends to consume excessive memory for these operations, potentially leading to memory shortages even on 80GB A100 GPUs. As shown in the below figure, starting with input of 1G parameters (channel×height×width), the memory demands of standard PyTorch convolutions increase significantly more rapidly with the activation size  than before. When the input is larger than 2G parameters, the convolution will use up all the 80G memory.
+In current generative models, we usually apply convolutions over large-size activations to generate high-resolution content. However, PyTorch tends to use excessive memory for these operations, potentially leading to memory shortages even on 80GB A100 GPUs. 
+
+As shown in the figure below, memory demands for standard PyTorch convolutions drastically increase when the input size reaches 1B parameters (channel×height×width). Notably, with a kernel size of 7×7, the 80GB A100 GPUs would trigger Out of Memory (OOM) errors. Inputs exceeding 2B parameters can further cause 3×3 convolutions exhaust all the memory and that’s just for one layer! This memory bottleneck prevents users and the community from scaling up the models to produce high-quality images.
 
 To bypass this issue and reduce memory consumption, we propose a simple and effective solution -- Patch Conv. As shown in the above figure, similar to [SIGE](https://github.com/lmxyy/sige), Patch Conv first divides the input into several smaller patches along the height dimension while keeping some overlap between them. These patches are then reorganized into the batch dimension and fed into the original convolution to produce output patches, which are then concatenated together to form the final output. Patch Conv can reduce memory usage by over 2.4×, providing a viable workaround for the limitations of current implementations.
 
-![background](https://github.com/mit-han-lab/patch_conv/blob/main/assets/background.jpg)
+<p align="center">
+  <img src="https://github.com/mit-han-lab/patch_conv/blob/main/assets/background.jpg" width="80%"/>
+</p>
 
 ## Installation
 
 After installing [PyTorch](https://pytorch.org), you can install `PatchConv` from PyPI:
 
 ```shell
 pip install patch_conv
@@ -37,15 +42,15 @@
 pip install git+https://github.com/mit-han-lab/patch_conv.git
 ```
 
 or locally for development:
 
 ```shell
 git clone git@github.com:mit-han-lab/patch_conv.git
-cd distrifuser
+cd patch_conv
 pip install -e .
 ```
 
 ## Usage
 
 All you need to do is use [`convert_model`](https://github.com/mit-han-lab/patch_conv/blob/main/patch_conv/utils.py#L6) to wrap all the `Conv2d` in your PyTorch model to our `PatchConv`. For example,
 
@@ -64,9 +69,10 @@
 
 ![performance](https://github.com/mit-han-lab/patch_conv/blob/main/assets/performance.jpg)
 
 Patch Conv significantly reduces memory consumption by over 2.4× across various kernel sizes and input resolutions with a marginally slower inference speed compared to vanilla convolution.
 
 ## Related Projects
 
-* [DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models](https://github.com/mit-han-lab/distrifuser), Li *et al.*, CVPR 2024
+* [MCUNetV2: Memory-Efficient Patch-based Inference for Tiny Deep Learning](https://arxiv.org/abs/2110.15352), Lin *et al.*, NeurIPS 2021
 * [Efficient Spatially Sparse Inference for Conditional GANs and Diffusion Models](https://github.com/lmxyy/sige), Li *et al.*, NeurIPS 2022
+* [DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models](https://github.com/mit-han-lab/distrifuser), Li *et al.*, CVPR 2024
```

### Comparing `patch_conv-0.0.0b0/setup.py` & `patch_conv-0.0.1b0/setup.py`

 * *Files identical despite different names*

