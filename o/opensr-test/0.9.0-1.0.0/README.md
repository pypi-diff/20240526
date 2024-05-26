# Comparing `tmp/opensr_test-0.9.0.tar.gz` & `tmp/opensr_test-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensr_test-0.9.0.tar", max compression
+gzip compressed data, was "opensr_test-1.0.0.tar", max compression
```

## Comparing `opensr_test-0.9.0.tar` & `opensr_test-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-05-09 08:13:17.278355 opensr_test-0.9.0/LICENSE
--rw-r--r--   0        0        0    12100 2024-05-13 15:41:27.379466 opensr_test-0.9.0/README.md
--rw-r--r--   0        0        0      244 2024-05-18 13:08:32.084169 opensr_test-0.9.0/opensr_test/__init__.py
--rw-r--r--   0        0        0     3425 2024-05-18 12:28:54.547515 opensr_test-0.9.0/opensr_test/config.py
--rw-r--r--   0        0        0     5853 2024-05-18 14:08:52.601223 opensr_test-0.9.0/opensr_test/correctness.py
--rw-r--r--   0        0        0     2154 2024-05-14 11:04:14.042783 opensr_test-0.9.0/opensr_test/dataset.py
--rw-r--r--   0        0        0    17828 2024-05-14 14:54:26.605895 opensr_test-0.9.0/opensr_test/distance.py
--rw-r--r--   0        0        0    20870 2024-05-18 14:06:34.257202 opensr_test-0.9.0/opensr_test/main.py
--rw-r--r--   0        0        0    11321 2024-05-14 15:05:56.813535 opensr_test-0.9.0/opensr_test/plot.py
--rw-r--r--   0        0        0     2200 2024-05-12 16:32:21.798342 opensr_test-0.9.0/opensr_test/spatial.py
--rw-r--r--   0        0        0     4270 2024-05-18 12:07:37.563317 opensr_test-0.9.0/opensr_test/utils.py
--rw-r--r--   0        0        0     2076 2024-05-18 13:06:37.495411 opensr_test-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 opensr_test-0.9.0/setup.py
--rw-r--r--   0        0        0    12965 1970-01-01 00:00:00.000000 opensr_test-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-09 08:13:17.278355 opensr_test-1.0.0/LICENSE
+-rw-r--r--   0        0        0    16494 2024-05-26 11:11:06.170018 opensr_test-1.0.0/README.md
+-rw-r--r--   0        0        0      244 2024-05-18 13:08:32.084169 opensr_test-1.0.0/opensr_test/__init__.py
+-rw-r--r--   0        0        0     3464 2024-05-25 12:43:54.821618 opensr_test-1.0.0/opensr_test/config.py
+-rw-r--r--   0        0        0     6076 2024-05-25 12:43:52.649685 opensr_test-1.0.0/opensr_test/correctness.py
+-rw-r--r--   0        0        0     2154 2024-05-14 11:04:14.042783 opensr_test-1.0.0/opensr_test/dataset.py
+-rw-r--r--   0        0        0    18333 2024-05-26 11:49:28.552563 opensr_test-1.0.0/opensr_test/distance.py
+-rw-r--r--   0        0        0    21745 2024-05-25 18:56:40.876248 opensr_test-1.0.0/opensr_test/main.py
+-rw-r--r--   0        0        0    17159 2024-05-25 15:06:22.508736 opensr_test-1.0.0/opensr_test/plot.py
+-rw-r--r--   0        0        0     2273 2024-05-25 15:46:14.849087 opensr_test-1.0.0/opensr_test/spatial.py
+-rw-r--r--   0        0        0     4270 2024-05-25 08:22:20.692162 opensr_test-1.0.0/opensr_test/utils.py
+-rw-r--r--   0        0        0     2278 2024-05-25 16:12:50.531590 opensr_test-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    17881 1970-01-01 00:00:00.000000 opensr_test-1.0.0/setup.py
+-rw-r--r--   0        0        0    17538 1970-01-01 00:00:00.000000 opensr_test-1.0.0/PKG-INFO
```

### Comparing `opensr_test-0.9.0/LICENSE` & `opensr_test-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensr_test-0.9.0/opensr_test/config.py` & `opensr_test-1.0.0/opensr_test/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,19 @@
 
 
     # Synthesis parameters
     synthesis_distance: DistanceMetrics = "l1"
 
     # Correctness parameters
     correctness_distance: DistanceMetrics = "l1"
-    correctness_norm: Literal["softmax", "standard", "percent"] = "softmax"
+    correctness_norm: Literal["softmin", "percent"] = "softmin"
     im_score: Optional[float] = 0.80
     om_score: Optional[float] = 0.80
-    ha_score: Optional[float] = 0.30 # be quiet conservative about hallucinations
+    ha_score: Optional[float] = 0.40 # be quiet conservative about hallucinations
+    correctness_temperature: Optional[float] = 1.5
 
 
     # General parameters - validator ----------------------------
     @field_validator("device")
     def check_device(cls, value) -> str:
         return torch.device(value)
```

### Comparing `opensr_test-0.9.0/opensr_test/dataset.py` & `opensr_test-1.0.0/opensr_test/dataset.py`

 * *Files identical despite different names*

### Comparing `opensr_test-0.9.0/opensr_test/distance.py` & `opensr_test-1.0.0/opensr_test/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,15 @@
                     x_batch, y_batch
                 )
 
         # Go back to the original size
         metric_result = torch.nn.functional.interpolate(
             metric_result[None, None],
             size=self.x.shape[-2:],
-            mode="bicubic",
-            antialias=True,
-            align_corners=False
+            mode="nearest"
         ).squeeze()
 
         return metric_result
 
     def compute_pixel(self) -> torch.Tensor:
         return self._compute_pixel(self.x, self.y)
 
@@ -288,44 +286,58 @@
     """Learned Perceptual Image Patch Similarity between two tensors"""
 
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
-        patch_size: int = 32,
+        patch_size: int = 16,
         device: Union[str, torch.device] = "cpu",
     ):
         if method == "patch":
-            if patch_size < 32:
-                raise ValueError("The patch size must be at least 32.")
+            if patch_size < 16:
+                raise ValueError("The patch size must be at least 16.")
 
-        # if extra_requires (setup.py) is not fulfilled, raise error
         check_lpips()
         import lpips
 
-        if method == "patch":
-            if patch_size < 32:
-                raise ValueError("The patch size must be at least 32.")
-
         # Set the model
         self.model = lpips.LPIPS(net="alex", verbose=False).to(device)
+        self.model.eval()
 
         # Normalize the tensors to [-1, 1]
-        y = (y - y.min()) / (y.max() - y.min())
         y = y * 2 - 1
-
-        x = (x - x.min()) / (x.max() - x.min())
         x = x * 2 - 1
 
         super().__init__(x=x, y=y, method=method, patch_size=patch_size)
 
     @torch.no_grad()
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        return self.model(x, y).mean()
+        # Scale image is lower than 64
+        if (x.shape[1] < 64) or (x.shape[2] < 64):
+            x = torch.nn.functional.interpolate(
+                x[None],
+                size=(64, 64),
+                mode="bilinear",
+                antialias=True
+            ).squeeze()
+            
+        
+        if (y.shape[1] < 64) or (y.shape[2] < 64):
+            y = torch.nn.functional.interpolate(
+                y[None],
+                size=(64, 64),
+                mode="bilinear",
+                antialias=True
+            ).squeeze()
+
+        with torch.no_grad():
+            result = self.model(x, y).mean()
+
+        return result
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError("LPIPS cannot be computed at pixel level.")
 
 
 class CLIP(DistanceMetric):
     """Estimate the CLIP score between two tensors"""
@@ -335,72 +347,79 @@
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
         device: Union[str, torch.device] = "cpu",
     ):
         if method == "patch":
-            if patch_size < 32:
-                raise ValueError("The patch size must be at least 32.")
+            if patch_size < 16:
+                raise ValueError("The patch size must be at least 16.")
                     
         # if extra_requires (setup.py) is not fulfilled, raise error
         check_openclip()
         check_huggingface_hub()
-
         import open_clip
         from huggingface_hub import hf_hub_download
 
         # Set the model
         # Copy the pretrained model in the current directory
         checkpoint_path = hf_hub_download(
             "chendelong/RemoteCLIP",
             f"RemoteCLIP-RN50.pt",
             cache_dir='checkpoints'
         )
         ckpt = torch.load(checkpoint_path, map_location=device)
         model, _, preprocess = open_clip.create_model_and_transforms("RN50")
         model.load_state_dict(ckpt)
         model.to(device)
+        model.eval()
 
         # desactivate the gradients
         for param in model.parameters():
             param.requires_grad = False
 
         # Scale the tensors values to [0, 1]
-        # we found better results with this normalization
-        x_norm = (x - x.min()) / (x.max() - x.min())
-        y_norm = (y - y.min()) / (y.max() - y.min())
+        x_norm = x.clamp(0, 1)
+        y_norm = y.clamp(0, 1)
         self.model = model
         super().__init__(
             x=x_norm, y=y_norm, method=method, patch_size=patch_size
         )
 
     @torch.no_grad()
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         # Scale image to be always Bx3x224x224
         if x.shape != (3, 224, 224):
             x = torch.nn.functional.interpolate(
                 x[None],
                 size=224,
                 mode="bilinear",
                 antialias=True
-            )
+            ).squeeze()
+            
         
         if y.shape != (3, 224, 224):
             y = torch.nn.functional.interpolate(
                 y[None],
                 size=224,
                 mode="bilinear",
                 antialias=True
-            )
+            ).squeeze()
         
+        # normalize
+        means = torch.tensor([0.48145466, 0.4578275, 0.40821073]).view(3, 1, 1).to(x.device)
+        stds = torch.tensor([0.26862954, 0.26130258, 0.27577711]).view(3, 1, 1).to(x.device)
+
+        x = (x - means) / stds
+        y = (y - means) / stds
+
         # Run the CLIP model
         with torch.no_grad():
-            x_emb = self.model.encode_image(x).squeeze()
-            y_emb = self.model.encode_image(y).squeeze()
+            x_emb = self.model.encode_image(x[None]).squeeze()
+            y_emb = self.model.encode_image(y[None]).squeeze()
 
         return torch.nn.functional.l1_loss(x_emb, y_emb)
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError("CLIP cannot be computed at pixel level.")
 
 
@@ -416,16 +435,16 @@
         scale: int = 4,
     ):
         super().__init__(
             x=x, y=y, method=method, patch_size=patch_size
         )
 
         if method == "patch":
-            if patch_size < 32:
-                raise ValueError("The patch size must be at least 32.")
+            if patch_size < 16:
+                raise ValueError("The patch size must be at least 16.")
 
         self.scale = scale
 
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         # do computation in cpu to avoid problems with fft
         x = x.cpu()
         y = y.cpu()
@@ -445,15 +464,14 @@
 
         return torch.mean(torch.clamp(mtf, 0, 1))
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError("MTF cannot be computed at pixel level.")
 
 
-
 def get_distance(
     x: torch.Tensor,
     y: torch.Tensor,
     method: str,
     agg_method: str,
     patch_size: int = 32,
     scale: int = 4,
```

### Comparing `opensr_test-0.9.0/opensr_test/main.py` & `opensr_test-1.0.0/opensr_test/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,15 +403,16 @@
             agg_method=self.params.agg_method,
             scale=self.scale_factor,
             patch_size=self.params.patch_size,
             rgb_bands=self.params.rgb_bands,
             device=self.params.device
         )
 
-        # Apply the mask to remove the pixels with gradients 
+
+        # Apply the mask to remove the pixels with low gradients
         mask = self._create_mask(
             d_ref=d_ref,
             d_im=d_im,
             d_om=d_om,
             gradient_threshold=gradient_threshold
         )
         self.d_ref = d_ref * mask
@@ -445,27 +446,28 @@
 
         #  Get stats
         total_stats = get_correctness_stats(
             im_tensor=self.improvement,
             om_tensor=self.omission,
             ha_tensor=self.hallucination,
             mask=mask,
-            correctness_norm=self.params.correctness_norm
+            correctness_norm=self.params.correctness_norm,
+            temperature=self.params.correctness_temperature
         )
         
         self.classification = total_stats["classification"]
         self.improvement, self.omission, self.hallucination = total_stats["tensor_stack"]
         self.im_percentage = total_stats["stats"][0]
         self.om_percentage = total_stats["stats"][1]
         self.ha_percentage = total_stats["stats"][2]
         
         return {
-            "ha_percent": self.ha_percentage.item(),
-            "om_percent": self.om_percentage.item(),
-            "im_percent": self.im_percentage.item()
+            "ha_metric": self.ha_percentage.item(),
+            "om_metric": self.om_percentage.item(),
+            "im_metric": self.im_percentage.item()
         }
 
     def compute(
         self,
         lr: torch.Tensor,
         sr: torch.Tensor,
         hr: torch.Tensor,
@@ -599,21 +601,52 @@
             e5_subtitle=e5_subtitle,
             stretch=stretch
         )        
         return fig, axs
 
     def plot_tc(
         self,
-        log_scale: Optional[bool] = True,
+        log_scale: Optional[bool] = False,
         stretch: Optional[str] = "linear"
     ):
+        self.d_im_ref[self.d_im_ref > 5] = 5
+        self.d_om_ref[self.d_om_ref > 5] = 5
+
         return plot.display_tc_score(
             sr_rgb=self.sr_harm_RGB.to("cpu"),
+            hr_rgb=self.hr_RGB.to("cpu"),
             d_im_ref=self.d_im_ref.to("cpu"),
             d_om_ref=self.d_om_ref.to("cpu"),
             tc_score=self.classification.to("cpu"),
             log_scale=log_scale,
             stretch=stretch
         )
 
+    def plot_ternary(
+        self,
+        ha: torch.Tensor = None,
+        om: torch.Tensor = None,
+        im: torch.Tensor = None
+    ):
+        if ha is None:
+            ha = self.hallucination.flatten()
+            ha = ha[~torch.isnan(ha)]
+
+        if om is None:
+            om = self.omission.flatten()
+            om = om[~torch.isnan(om)]
+
+        if im is None:
+            im = self.improvement.flatten()
+            im = im[~torch.isnan(im)]
+
+        return plot.display_ternary(
+            ha=ha.cpu().numpy(),
+            om=om.cpu().numpy(),
+            im=im.cpu().numpy()
+        )
+    
+    def plot_histogram(self):
+        return plot.display_stats(self)
+
     def __call__(self) -> Any:
         return self.compute()
```

### Comparing `opensr_test-0.9.0/opensr_test/spatial.py` & `opensr_test-1.0.0/opensr_test/spatial.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,13 +58,14 @@
         # Run the alignment model
         image_fixed, warp = align_model.run()
         image_fixed_to_torch = torch.from_numpy(image_fixed).to(self.device)
 
 
         # Get the spatial error from the affine matrix
         spatial_error = np.sqrt(warp[0][0, 2]**2 + warp[0][1, 2]**2)
-
+        if align_model.warning_status:
+            spatial_error = np.nan
         return image_fixed_to_torch[0], torch.tensor(spatial_error).type(torch.float32)
     
     @pydantic.field_validator("device")
     def check_device(cls, value):
         return torch.device(value)
```

### Comparing `opensr_test-0.9.0/opensr_test/utils.py` & `opensr_test-1.0.0/opensr_test/utils.py`

 * *Files identical despite different names*

### Comparing `opensr_test-0.9.0/pyproject.toml` & `opensr_test-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 [tool.poetry]
 name = "opensr_test"
-version = "0.9.0"
+version = "1.0.0"
 description = "A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution"
 authors = ["Cesar Aybar <cesar.aybar@uv.es>"]
 repository = "https://github.com/csaybar/opensr-test"
 documentation = "https://csaybar.github.io/opensr-test/"
 readme = "README.md"
 packages = [
   {include = "opensr_test"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4.0"
-satalign = ">=0.1.0"
+satalign = ">=0.1.3"
 numpy = ">=1.25.2"
 matplotlib = ">=3.7.0"
 torchvision = ">=0.17.0"
 scikit-image = ">=0.19.0"
 requests = ">=2.25.0"
 kornia = ">=0.7.2"
 pydantic = ">=2.7.1"
 opencv-python = ">=4.8.0.0"
+lpips = {extras = ["perceptual"], version = ">=0.1.4"}
+openai-clip = {extras = ["perceptual"], version = ">=1.0.1"}
+open-clip-torch = {extras = ["perceptual"], version = ">=2.24.0"}
+mpltern = ">=1.0.4"
 
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.12.0"
```

