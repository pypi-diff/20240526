# Comparing `tmp/npeccv6-0.0.3.tar.gz` & `tmp/npeccv6-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npeccv6-0.0.3.tar", max compression
+gzip compressed data, was "npeccv6-0.0.4.tar", max compression
```

## Comparing `npeccv6-0.0.3.tar` & `npeccv6-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        0 2024-05-13 09:16:18.854887 npeccv6-0.0.3/LICENSE
--rw-r--r--   0        0        0      202 2024-05-13 09:16:18.854887 npeccv6-0.0.3/README.md
--rw-r--r--   0        0        0      247 2024-05-21 15:01:26.257284 npeccv6-0.0.3/npeccv6/__init__.py
--rw-r--r--   0        0        0    25551 2024-05-23 10:33:50.736931 npeccv6-0.0.3/npeccv6/data.py
--rw-r--r--   0        0        0     5756 2024-05-23 10:23:19.140355 npeccv6-0.0.3/npeccv6/log/buas_cv6.log
--rw-r--r--   0        0        0    10722 2024-05-23 10:32:58.420554 npeccv6-0.0.3/npeccv6/model.py
--rw-r--r--   0        0        0    10301 2024-05-23 10:32:55.624534 npeccv6-0.0.3/npeccv6/postprocessing.py
--rw-r--r--   0        0        0     9545 2024-05-23 10:49:09.183228 npeccv6-0.0.3/npeccv6/predict.py
--rwxr-xr-x   0        0        0     2672 2024-05-23 10:32:52.264510 npeccv6-0.0.3/npeccv6/train.py
--rw-r--r--   0        0        0     4618 2024-05-23 10:43:42.396956 npeccv6-0.0.3/npeccv6/utils.py
--rw-r--r--   0        0        0     1089 2024-05-23 10:50:05.387621 npeccv6-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 npeccv6-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-26 13:16:06.217470 npeccv6-0.0.4/LICENSE
+-rw-r--r--   0        0        0      202 2024-05-26 13:16:06.217470 npeccv6-0.0.4/README.md
+-rw-r--r--   0        0        0      252 2024-05-26 14:48:59.549652 npeccv6-0.0.4/npeccv6/__init__.py
+-rw-r--r--   0        0        0    25999 2024-05-26 14:54:45.091427 npeccv6-0.0.4/npeccv6/data.py
+-rw-r--r--   0        0        0    15132 2024-05-26 14:54:45.087427 npeccv6-0.0.4/npeccv6/model.py
+-rw-r--r--   0        0        0    15193 2024-05-26 14:54:45.099427 npeccv6-0.0.4/npeccv6/model_func.py
+-rw-r--r--   0        0        0    13670 2024-05-26 14:54:45.083427 npeccv6-0.0.4/npeccv6/postprocessing.py
+-rw-r--r--   0        0        0    10202 2024-05-26 14:48:59.553652 npeccv6-0.0.4/npeccv6/predict.py
+-rw-r--r--   0        0        0   138369 2024-05-26 14:28:22.972885 npeccv6-0.0.4/npeccv6/test_landmark_detection.ipynb
+-rw-r--r--   0        0        0     2836 2024-05-26 14:48:51.849613 npeccv6-0.0.4/npeccv6/train.py
+-rw-r--r--   0        0        0     5178 2024-05-26 14:48:51.869613 npeccv6-0.0.4/npeccv6/utils.py
+-rw-r--r--   0        0        0     1113 2024-05-26 14:17:47.457409 npeccv6-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 npeccv6-0.0.4/PKG-INFO
```

### Comparing `npeccv6-0.0.3/npeccv6/data.py` & `npeccv6-0.0.4/npeccv6/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 import os
 import random
 from typing import List, Tuple
 
 import cv2
 import numpy as np
 from patchify import patchify
-
 # from tensorflow.keras.models import Model
 from tensorflow.keras.preprocessing.image import ImageDataGenerator
-
 from tensorflow.keras.utils import Sequence
 
 # I hate this
 try:
     # Attempt relative imports (if run as a package module)
     from .utils import clear_destination_folder, setup_logger
 except ImportError:
@@ -123,52 +121,65 @@
     #     # cv2.imshow("Cropped Petri Dish", cropped_image)
     #     # cv2.waitKey(0)
     #     # cv2.destroyAllWindows()
 
     # cropped_image.shape
 
 
-def padder(image, patch_size):
+def padder(image: np.ndarray, patch_size: int) -> np.ndarray:
     """
     Adds padding to an image to make its dimensions divisible by a specified patch size.
 
-    This function calculates the amount of padding needed for both the height and width of an image so that its dimensions become divisible by the given patch size. The padding is applied evenly to both sides of each dimension (top and bottom for height, left and right for width). If the padding amount is odd, one extra pixel is added to the bottom or right side. The padding color is set to black (0, 0, 0).
+    This function calculates the amount of padding needed for both the height and width of an image
+    so that its dimensions become divisible by the given patch size. The padding is applied evenly to both sides
+    of each dimension (top and bottom for height, left and right for width). If the padding amount is odd,
+    one extra pixel is added to the bottom or right side. The padding color is set to black (0, 0, 0).
 
     Parameters:
-        - image (numpy.ndarray): The input image as a NumPy array. Expected shape is (height, width, channels).
+        - image (np.ndarray): The input image as a NumPy array. Expected shape is (height, width, channels).
         - patch_size (int): The patch size to which the image dimensions should be divisible. It's applied to both height and width.
 
     Returns:
-        - numpy.ndarray: The padded image as a NumPy array with the same number of channels as the input. Its dimensions are adjusted to be divisible by the specified patch size.
+        - np.ndarray: The padded image as a NumPy array with the same number of channels as the input.
+          Its dimensions are adjusted to be divisible by the specified patch size.
 
     Example:
         - padded_image = padder(cv2.imread('example.jpg'), 128)
-
     """
-    h = image.shape[0]
-    w = image.shape[1]
+    logger = setup_logger()
+    logger.debug(
+        f"Starting padding for image of shape {image.shape} to make dimensions divisible by {patch_size}."
+    )
+
+    h, w = image.shape[:2]
     height_padding = ((h // patch_size) + 1) * patch_size - h
     width_padding = ((w // patch_size) + 1) * patch_size - w
 
-    top_padding = int(height_padding / 2)
+    top_padding = height_padding // 2
     bottom_padding = height_padding - top_padding
 
-    left_padding = int(width_padding / 2)
+    left_padding = width_padding // 2
     right_padding = width_padding - left_padding
 
+    logger.debug(
+        f"Calculated padding: top={top_padding}, bottom={bottom_padding}, left={left_padding}, right={right_padding}"
+    )
+
     padded_image = cv2.copyMakeBorder(
         image,
         top_padding,
         bottom_padding,
         left_padding,
         right_padding,
         cv2.BORDER_CONSTANT,
         value=[0, 0, 0],
     )
 
+    logger.debug(f"Padding completed. New image shape is {padded_image.shape}.")
+
     return padded_image
 
 
 def save_mask_patches(
     path: str,
     mask: np.ndarray,
     patch_size: int,
@@ -353,18 +364,18 @@
         i,
     )
     return 0
 
 
 def patch_and_save(
     model_name: str = "test",
-    root_path: str = "../data/",
+    root_path: str = "./data/",
     patch_size: int = 256,
     scaling_factor: float = 1,
-    patch_dir: str = "../data_patched/",
+    patch_dir: str = "./data_patched/",
     test_split: float = 0.3,
 ) -> None:
     """
     Generate and save patches for images and corresponding masks.
 
     Parameters:
         - model_name (str): Name of the model or dataset.
@@ -424,15 +435,15 @@
     if all(name in folder_list for name in valid_names_train_test):
         # log("detected train, test, and masks.")
         logger.info("Processing pre-split dataset")
 
         train_folder = root_path + model_name + "/train"
         test_folder = root_path + model_name + "/test"
         masks_folder = root_path + model_name + "/masks"
-      
+
         logger.info("Cleaining folders")
         compare_and_remove(train_folder, masks_folder)
         compare_and_remove(test_folder, masks_folder)
         logger.info("Folders cleaned")
         # Get a list of all files for train and test
         # Masks will be handled later alongside images
         train_file_list = glob.glob(train_folder + "/*")
@@ -502,27 +513,29 @@
             split,
         )
         if response == 1:
             return 1
         i += 1
     return 0
 
+
 class DataGenerator(Sequence):
     def __init__(self, image_gen, mask_gen):
         self.image_gen = image_gen
         self.mask_gen = mask_gen
 
     def __len__(self):
         return min(len(self.image_gen), len(self.mask_gen))
 
     def __getitem__(self, index):
         x = self.image_gen[index]
         y = self.mask_gen[index]
         return x[0], y[0]
 
+
 def load_and_preprocess_data(
     classes: List[str],
     model_name: str = "test",
     patch_size: int = 256,
     patch_dir: str = "../data_patched/",
     seed: int = 42,
     batch_size: int = 16,
@@ -648,15 +661,16 @@
 
     if num_channels != 1:
         im_gray = cv2.cvtColor(im, cv2.COLOR_BGR2GRAY)
     else:
         im_gray = im
 
     logger.info("Cropping image to petri dish.")
-    cropped_im, roiX, roiY, roiW, roiH = crop_to_petri(im_gray)
+    _, roiX, roiY, roiW, roiH = crop_to_petri(im_gray)
+    cropped_im = im[roiX : roiX + roiW, roiY : roiY + roiH]
 
     logger.info("Padding cropped image.")
     padded_im = padder(cropped_im, patch_size)
 
     if scaling_factor != 1:
         logger.info(f"Scaling image by a factor of {scaling_factor}.")
         padded_im = cv2.resize(padded_im, (0, 0), fx=scaling_factor, fy=scaling_factor)
@@ -666,14 +680,15 @@
     i = patches.shape[0]
     j = patches.shape[1]
     patches = patches.reshape(-1, patch_size, patch_size, 1 if num_channels == 1 else 3)
 
     logger.info("Image preprocessing completed.")
     return patches, i, j, padded_im
 
+
 def main():
     parser = argparse.ArgumentParser(
         description="Preprocess data using predefinded folder struncture, /data/model_name/ train, test, masks or images, masks. If more flexible solution is needed please use process_image_and_mask function in this module to create a custom loop"
     )
     parser.add_argument(
         "model_name",
         default="test",
```

### Comparing `npeccv6-0.0.3/npeccv6/postprocessing.py` & `npeccv6-0.0.4/npeccv6/postprocessing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 #!/bin/python3
+import math
 from typing import Any, Dict, List, Tuple
 
 import cv2
 import networkx as nx
 import numpy as np
 import pandas as pd
-from skimage.morphology import remove_small_holes, remove_small_objects
+from skan import Skeleton, summarize
+from skan.csr import skeleton_to_csgraph
+from skimage.morphology import (remove_small_holes, remove_small_objects,
+                                skeletonize)
 
 try:
     # Attempt relative imports (if run as a package module)
     from .utils import setup_logger
-    
+
 except ImportError:
     # Fallback to absolute imports (if run as a standalone script)
     from utils import setup_logger
 
 
 # Configure logging
 logging = setup_logger()
@@ -41,17 +45,16 @@
             - segmented_roots_image = segment_roots(image = image_to_be_segmented, expected_nr_plants = 5)
 
     Note:
         - This function assumes that the input image contains plant roots.
         - This function will consider overlaping roots as one singular root.
         - The function will ignore roots smaller than 64 pixels.
     """
-    # Define the logger
-    logger = setup_logger()
-
+    if image.dtype != np.uint8:
+        image = image.astype(np.uint8)
     # Get components
     _, labels, stats, _ = cv2.connectedComponentsWithStats(image)
 
     # Remove objects with area smaller than 64
     removed_small_obj = remove_small_objects(labels, 64)
     removed_small_obj[removed_small_obj != 0] = 1
     removed_small_obj = removed_small_obj.astype(np.uint8)
@@ -60,19 +63,23 @@
     # Make labeles binary
     labels = labels > 0
 
     # Remove holes with area smalle than 64
     removed_small_holes = remove_small_holes(labels, 64)
     removed_small_holes[removed_small_holes != 0] = 1
     removed_small_holes = removed_small_holes.astype(np.uint8)
-    _, labels, stats, _ = cv2.connectedComponentsWithStats(removed_small_holes)
+    _, labels, stats, centroids = cv2.connectedComponentsWithStats(removed_small_holes)
+    # Round the centroids
+    centroids = np.round(centroids).astype(int)
+    # Combine stats and centroids
+    combined_stats = np.hstack((stats, centroids))
 
     # Add id to clean canvas to only roots
-    row_indices = np.arange(len(stats))
-    stats_with_id = np.hstack((stats, row_indices.reshape(-1, 1)))
+    row_indices = np.arange(len(combined_stats))
+    stats_with_id = np.hstack((combined_stats, row_indices.reshape(-1, 1)))
 
     # Empty list with roots
     roots = []
 
     # Sort the array
     sorted_stats = stats_with_id[stats_with_id[:, 3].argsort()[::-1]]
 
@@ -81,40 +88,76 @@
     below_half_y_condition = sorted_stats[:, 1] < (labels.shape[1] / 2)
     combined_condition = above_150_condition & below_half_y_condition
 
     # Apply the combined condition to filter rows
     filtered_stats = sorted_stats[combined_condition]
     sorted_roots = filtered_stats[filtered_stats[:, 3].argsort()[::-1]]
 
-    # Leave only the expected nr of plants based on size and overwrite rest
-    if len(sorted_roots) > expected_nr_plants:
-        sorted_roots = sorted_roots[:expected_nr_plants, :]
+    # Remove elements whose centroids are below 450
+    centroids_below_450 = sorted_roots[:, 6] > 450
+    centroids_above_1800 = sorted_roots[:, 6] < 1800
+    centroids_condition = centroids_below_450 & centroids_above_1800
+
+    # Keep the roots which meet the centroid condition
+    sorted_roots = sorted_roots[centroids_condition]
+
+    # Sort the roots by size in descending order
+    sorted_roots = sorted(sorted_roots, key=lambda x: x[4])
+    sorted_roots = np.array(sorted_roots)
+
+    # Empty list to keep the good roots
+    filtered_roots = []
+
+    # Iterate over all roots
+    for i, test_root in enumerate(sorted_roots):
+        # Set up the 2 checks
+        keep_1 = True
+        keep_2 = True
+        # Go over all the root bigger than the test root
+        for j, root in enumerate(sorted_roots[i + 1 :], start=i + 1):
+            # If the roots overlap vertically, failed check
+            if root[0] <= test_root[5] <= root[0] + root[2]:
+                keep_1 = False
+            # If the roots centroids are too close, failed check
+            if (
+                math.sqrt((root[5] - test_root[5]) ** 2 + (root[6] - test_root[6]) ** 2)
+                < 300
+            ):
+                keep_2 = False
+        # If both checks passed, save the root
+        if keep_1 and keep_2:
+            filtered_roots.append(test_root)
+
+    # Sort the roots by size in descending order and make them into an array
+    roots = sorted(filtered_roots, key=lambda x: x[4], reverse=True)
+    roots = np.array(roots)
 
-    # Make the roots back to np.array
-    roots = np.array(sorted_roots)
+    # Leave only the expected nr of plants based on size and overwrite rest
+    if len(roots) > expected_nr_plants:
+        roots = roots[:expected_nr_plants, :]
 
     # Make the mask based on the roots
     mask = np.isin(labels, roots[:, -1])
 
     # Create the labels/big picture
     labels[~mask] = 0
     roots = roots[roots[:, 0].argsort()]
 
     try:
         # Get the width and size of the 2nd biggest component
-        _, _, width_1, _, size_1, _ = roots[0]
+        _, _, width_1, _, size_1, _, _, _ = roots[0]
         # Get the size of the 2nd biggest component
         size_2 = roots[1][5]
 
         # Check the width
         if width_1 > labels.shape[0] / (expected_nr_plants - 1) and size_1 / 2 > size_2:
             logger.error("Image has overlapping plants!")
             return labels
     except Exception as e:
-        print(f"An error occurred: {e}")
+        logger.error(f"An error occurred: {e}")
 
     # Check the number of roots
     if len(roots) != expected_nr_plants:
         logger.error(f"Number of detected plants is not {expected_nr_plants}!")
         logger.error(f"Detected: {len(roots)} plants")
         return labels
 
@@ -278,7 +321,54 @@
     for node in junctions:
         coord = nodes_summary.loc[
             nodes_summary["node-id-src"] == node, ["coord-src-0", "coord-src-1"]
         ].values[0]
         image = cv2.circle(image, (int(coord[1]), int(coord[0])), 15, green, 5)
 
     return image
+
+
+def process_image_for_roots(
+    image: np.ndarray, expected_nr_plants: int = 5
+) -> Tuple[pd.DataFrame, np.ndarray]:
+    """
+    Processes an image to segment roots, calculate root lengths, and mark landmarks.
+
+    Parameters:
+        - image (np.ndarray): Mask of the roots.
+        - expected_nr_plants (int): expected number of plants withing the petri dish
+
+    Returns:
+        - Tuple[pd.DataFrame, np.ndarray]: A DataFrame with root lengths and the image with landmarks.
+    """
+
+    # Segment roots from the image
+    segmented_roots = segment_roots(
+        image, expected_nr_plants
+    )  # Example value for expected_nr_plants
+
+    # Create root skeletons and supparize them
+    root_skeleton = skeletonize(segmented_roots)
+    summary = summarize(Skeleton(root_skeleton))
+
+    # Calculate root lengths
+    root_lengths = calculate_root_lengths(summary)
+
+    # Create a summary DataFrame for nodes
+    nodes_summary = pd.DataFrame(summary)
+
+    # Extract main root source and destination IDs
+    main_root_src = [info["main_root_src"] for info in root_lengths.values()]
+    main_root_dest = [info["main_root_dest"] for info in root_lengths.values()]
+
+    # Mark landmarks on the original image
+    marked_image = mark_landmarks(image, nodes_summary, main_root_src, main_root_dest)
+
+    root_tip_coords = []
+
+    for node_id in main_root_dest:
+        coords = nodes_summary[nodes_summary["node-id-dst"] == node_id][
+            ["coord-dst-0", "coord-dst-1"]
+        ].values.tolist()
+        root_tip_coords.extend(coords)
+
+    return root_lengths, root_tip_coords, marked_image
```

### Comparing `npeccv6-0.0.3/npeccv6/predict.py` & `npeccv6-0.0.4/npeccv6/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 #!/bin/python3
 import argparse
 from typing import Tuple
 
 import cv2
-import numpy as np
 import keras
+import numpy as np
 from patchify import patchify, unpatchify
-from tensorflow.keras.models import load_model, Model
+from tensorflow.keras.models import Model, load_model
+from tensorflow.keras.utils import custom_object_scope
 
 try:
     # Attempt relative imports (if run as a package module)
     from .data import crop_to_petri, padder
-    from .utils import setup_logger
-    
+    from .postprocessing import process_image_for_roots
+    from .utils import f1, iou, setup_logger
+
 except ImportError:
     # Fallback to absolute imports (if run as a standalone script)
+    from postprocessing import process_image_for_roots
+    from utils import f1, iou, setup_logger
+
     from data import crop_to_petri, padder
-    from utils import setup_logger
-    
+
 logger = setup_logger()
 
+
 def load_and_preprocess_image(
     im_path: str,
     patch_size: int = 256,
     scaling_factor: float = 1,
     num_channels: int = 1,
 ) -> Tuple[np.ndarray, int, int, np.ndarray]:
     """
@@ -52,15 +57,15 @@
 
             patches, i, j, im = load_and_preprocess_image('path/to/image.jpg', patch_size=128, scaling_factor=1, num_channels=3)
             print(patches.shape)
             (num_patches, 128, 128, 1)
             print(i, j)
             4 4
     """
-    
+
     logger.info(f"Loading image from path: {im_path}")
 
     if num_channels == 1:
         im = cv2.imread(im_path, cv2.IMREAD_GRAYSCALE)
         logger.debug(f"load_and_preprocess_image:number of channels:{num_channels}")
         logger.debug(f"load_and_preprocess_image:im.shape:{im.shape}")
     else:
@@ -144,15 +149,15 @@
         - im (np.ndarray): Original image.
         - threshold (float): Threshold value for binarizing the mask. Default is 0.8.
         - patch_size (int): Size of the patches. Default is 256.
 
     Returns:
         - np.ndarray: Post-processed binary mask.
     """
-    
+
     logger.info("Starting post-processing of predictions.")
 
     # Reshape predictions
     preds = preds.reshape(i, j, patch_size, patch_size)
 
     # Splice predictions
     predicted_mask = unpatchify(preds, (im.shape[0], im.shape[1]))
@@ -182,15 +187,15 @@
         - threshold (float): Threshold value for binarizing the mask. Default is 0.8.
         - scaling_factor (float): Scaling factor for the image. Default is 1.
         - num_channels (int): Number of channels for the image (1 for grayscale, 3 for color). Default is 1.
 
     Returns:
         - np.ndarray: Predicted binary mask.
     """
-    
+
     logger.info(f"Loading and preprocessing image from path: {im_path}")
 
     # Preprocess image
     patches, i, j, im = load_and_preprocess_image(
         im_path, patch_size, scaling_factor, num_channels
     )
 
@@ -224,14 +229,15 @@
 
 # model = DummyModel()
 # image_path = 'path_to_your_image.png'
 # save_path = 'Predictions/Image.png'
 
 # predicted_mask = predict(model, image_path, save_path)
 
+
 def main():
     parser = argparse.ArgumentParser(
         description="Predict a root mask from an image using a trained U-net model."
     )
     parser.add_argument("image_path", help="Path to the input image file.")
     parser.add_argument("save_path", help="Where to save predicted mask.")
     parser.add_argument(
@@ -270,28 +276,39 @@
         "-n",
         "--num_channels",
         # dest = "num_channels",
         default=1,
         action="store",
         help="Number of channels to use with image. Default is 1",
     )
-    
 
     args = parser.parse_args()
 
     # Load the saved model
-    model = load_model("./models/" + args.model + '.keras')
+    with custom_object_scope({"f1": f1, "iou": iou}):
+        model = load_model("./models/" + args.model + ".keras")
 
     # Predict the mask
     predicted_mask = predict(
         model,
         args.image_path,
         args.save_path,
         args.patch_size,
         args.threshold,
         args.scaling_factor,
         args.num_channels,
     )
+    # TO-DO: postprocessing
+    # TO-DO: extract information about number of expected plants
+    # PLACEHOLDER!!!
+    expected_nr_plants = 5
+
+    root_lengths, root_tip_coords, marked_image = process_image_for_roots(
+        predicted_mask, expected_nr_plants
+    )
+    logger.info(f"root lengths: {root_lengths}")
+    logger.info(f"root tips coordinates in image (px): {root_tip_coords}")
+    cv2.imwrite(args.save_path, marked_image)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `npeccv6-0.0.3/npeccv6/train.py` & `npeccv6-0.0.4/npeccv6/train.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,104 @@
 #!/bin/python3
-from typing import Iterable
 import argparse
 
 try:
     # Attempt relative imports (if run as a package module)
     from .data import load_and_preprocess_data
-    from .model import train_model
+    from .model_func import train_model
     from .utils import setup_logger
-    
+
 except ImportError:
     # Fallback to absolute imports (if run as a standalone script)
-    from data import load_and_preprocess_data
-    from model import train_model
+    from model_func import train_model
     from utils import setup_logger
 
+    from data import load_and_preprocess_data
+
 logger = setup_logger()
 
+
 def main():
     parser = argparse.ArgumentParser(
         description="Train a U-net model from images and masks."
     )
     parser.add_argument("model_name", help="name of the model.")
     parser.add_argument(
         "-c",
         "--classes",
         default=["root"],
         help="Classes to use to train the model the model. For single class(recomended): ['class'], for multiclass(not advised):['class1', 'class2']",
     )
     parser.add_argument(
         "-d",
         "--patch_dir",
-        default='./data_patched/',
-        help="Path to data root directory, should end with '/'. Default: './data_patched/'"
+        default="./data_patched/",
+        help="Path to data root directory, should end with '/'. Default: './data_patched/'",
     )
-    
+
     parser.add_argument(
         "-p",
         "--patch_size",
         default=256,
-        help="How big patches to use for the model. Default: 256"
+        help="How big patches to use for the model. Default: 256",
     )
-    
+
     parser.add_argument(
-        "-s",
-        "--seed",
-        default=42,
-        help="Seed for reading data and model training"
+        "-s", "--seed", default=42, help="Seed for reading data and model training"
     )
     parser.add_argument(
-        "-b",
-        "--batch_size",
-        default=16,
-        help="What batch size to use. Default: 16"
+        "-b", "--batch_size", default=16, help="What batch size to use. Default: 16"
     )
     parser.add_argument(
         "-o",
         "--color",
         default="grayscale",
-        help="What color mode to use. Default: 'grayscale'"
+        help="What color mode to use. Default: 'grayscale'",
     )
     parser.add_argument(
-        "-e",
-        "--epochs",
-        default=20,
-        help="Number of epochs. Default: 20"
+        "-e", "--epochs", default=20, help="Number of epochs. Default: 20"
+    )
+    # Disabled
+    parser.add_argument(
+        "-r",
+        "--roots",
+        default=5,
+        help="DISABLED!!! Number of expected plants inside petri dish. Default: 5",
     )
 
     args = parser.parse_args()
 
     patch_size = args.patch_size
-    
+
     train_generator, test_generator, steps_per_epoch, validation_steps = (
-        load_and_preprocess_data(args.classes, args.model_name, patch_size, args.patch_dir, args.seed, args.batch_size, args.color)
+        load_and_preprocess_data(
+            args.classes,
+            args.model_name,
+            patch_size,
+            args.patch_dir,
+            args.seed,
+            args.batch_size,
+            args.color,
+        )
     )
 
     logger.info(f"Training model\n{steps_per_epoch = }\n{validation_steps = }")
 
-    
-    
-    if args.color == 'grayscale':
+    if args.color == "grayscale":
         color = 1
     else:
         color = 3
 
     print(patch_size, patch_size, color)
     train_model(
         model_name=args.model_name,
         train_generator=train_generator,
         test_generator=test_generator,
         steps_per_epoch=steps_per_epoch,
         validation_steps=validation_steps,
-        input_shape = (patch_size, patch_size, color),
-        epochs = args.epochs
+        input_shape=(patch_size, patch_size, color),
+        epochs=args.epochs,
     )
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `npeccv6-0.0.3/npeccv6/utils.py` & `npeccv6-0.0.4/npeccv6/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/bin/python3
 import logging
 import os
 import shutil
 from typing import Iterable
 
+import tensorflow
 import tensorflow.keras.backend as K
 
 
-def setup_logger(folder="log"):
+def setup_logger(folder: str = "log") -> None:
     """
     Set up a logger that writes log messages to a file and the console.
 
     This function creates a logger that writes log messages to a specified
     file and the console. The log messages include a timestamp, the logger's
     name, the severity level of the log message, and the message itself.
 
@@ -23,41 +24,46 @@
 
     Example:
         .. code-block:: python
 
             logger = setup_logger()
             logger.info("This is an info message.")
     """
+    # Check if logger with the same name already exists
+    logger = logging.getLogger(__name__)
+    if logger.handlers:
+        # Logger already configured, return it
+        return logger
+
     filename = "buas_cv6.log"
     path = os.path.join(folder, filename)
     os.makedirs(folder, exist_ok=True)
 
     # Create a logger object
     logger = logging.getLogger(__name__)
 
-    if not logger.hasHandlers():
-        # Set the logging level
-        logger.setLevel(logging.INFO)
-
-        # Create a handler for writing to a file
-        file_handler = logging.FileHandler(path)
-
-        # Create a handler for writing to the console
-        console_handler = logging.StreamHandler()
-
-        # Create a formatter and add it to the handlers
-        formatter = logging.Formatter(
-            "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-        )
-        file_handler.setFormatter(formatter)
-        console_handler.setFormatter(formatter)
+    # Set the logging level
+    logger.setLevel(logging.INFO)
 
-        # Add the handlers to the logger
-        logger.addHandler(file_handler)
-        logger.addHandler(console_handler)
+    # Create a handler for writing to a file
+    file_handler = logging.FileHandler(path)
+
+    # Create a handler for writing to the console
+    console_handler = logging.StreamHandler()
+
+    # Create a formatter and add it to the handlers
+    formatter = logging.Formatter(
+        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+    )
+    file_handler.setFormatter(formatter)
+    console_handler.setFormatter(formatter)
+
+    # Add the handlers to the logger
+    logger.addHandler(file_handler)
+    logger.addHandler(console_handler)
 
     return logger
 
 
 logger = setup_logger()
 
 
@@ -73,20 +79,24 @@
         - y_pred (Iterable[float]): Predicted labels.
 
     Returns:
         float: The F1 score.
     """
 
     def recall_m(y_true: Iterable[float], y_pred: Iterable[float]) -> float:
+        y_true = tensorflow.cast(y_true, tensorflow.float32)
+        y_pred = tensorflow.cast(y_pred, tensorflow.float32)
         TP = K.sum(K.round(K.clip(y_true * y_pred, 0, 1)))
         Positives = K.sum(K.round(K.clip(y_true, 0, 1)))
         recall = TP / (Positives + K.epsilon())
         return recall
 
     def precision_m(y_true: Iterable[float], y_pred: Iterable[float]) -> float:
+        y_true = tensorflow.cast(y_true, tensorflow.float32)
+        y_pred = tensorflow.cast(y_pred, tensorflow.float32)
         TP = K.sum(K.round(K.clip(y_true * y_pred, 0, 1)))
         Pred_Positives = K.sum(K.round(K.clip(y_pred, 0, 1)))
         precision = TP / (Pred_Positives + K.epsilon())
         return precision
 
     try:
         precision, recall = precision_m(y_true, y_pred), recall_m(y_true, y_pred)
@@ -113,30 +123,32 @@
         - y_pred (Iterable[float]): Predicted labels.
 
     Returns:
         float: The IoU score.
     """
 
     def f(y_true: Iterable[float], y_pred: Iterable[float]) -> float:
+        y_true = tensorflow.cast(y_true, tensorflow.float32)
+        y_pred = tensorflow.cast(y_pred, tensorflow.float32)
         intersection = K.sum(K.abs(y_true * y_pred), axis=[1, 2, 3])
         total = K.sum(K.square(y_true), [1, 2, 3]) + K.sum(K.square(y_pred), [1, 2, 3])
         union = total - intersection
         return (intersection + K.epsilon()) / (union + K.epsilon())
 
     try:
         iou_ = K.mean(f(y_true, y_pred), axis=-1)
+        logger.debug(f"iou return value - {iou_}")
     except ValueError:
         logger.error(
             f"An ValueError occurred while calculating iou due to mismatched shapes between {y_true.shape = } and {y_pred.shape =}."
         )
-
     return iou_
 
 
-def clear_destination_folder(image_patch_path):
+def clear_destination_folder(image_patch_path: str) -> None:
     folder_path = os.path.dirname(image_patch_path)
     if os.path.exists(folder_path):
         logger.info("Clearing destination folder")
         shutil.rmtree(folder_path)
         # print(f'Removing folder: {folder_path}')
     # Create the folder if it doesn't exist
     os.makedirs(folder_path)
```

### Comparing `npeccv6-0.0.3/pyproject.toml` & `npeccv6-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "npeccv6"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python package for root recognition and robot controll"
 authors = ["Hubert Waleńczak <220817@buas.nl>", "Nick Belterman <225538@buas.nl>", "Amyr Lourensz <221264@buas.nl>", "Marwa Rouah <223256@buas.nl>", "Cristian Stîngă <223385@buas.nl>"]
 readme = "README.md"
 packages = [{include = "npeccv6"}]
 
 [tool.poetry.dependencies]
-python = "^3.10 <3.11"
+python = ">=3.10, <3.11"
 keras = "^2.12.0 <2.13"
 datetime = "^5.5"
 opencv-python = "^4.9.0.80"
 patchify = "^0.2.3"
 numpy = "^1.22.0 <=1.24.3"
 isort = "^5.13.2"
 black = "^24.4.2"
@@ -22,14 +22,15 @@
 wandb = "^0.17.0"
 pytest-cov = "^5.0.0"
 networkx = "^3.3"
 skan = "^0.11.1"
 sphinx = "^7.3.7"
 sphinx-rtd-theme = "^2.0.0"
 
+streamlit = "^1.35.0"
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = [
   ".", "npeccv6",
```

### Comparing `npeccv6-0.0.3/PKG-INFO` & `npeccv6-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npeccv6
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for root recognition and robot controll
 Author: Hubert Waleńczak
 Author-email: 220817@buas.nl
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: black (>=24.4.2,<25.0.0)
@@ -17,14 +17,15 @@
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: patchify (>=0.2.3,<0.3.0)
 Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Requires-Dist: skan (>=0.11.1,<0.12.0)
 Requires-Dist: sphinx (>=7.3.7,<8.0.0)
 Requires-Dist: sphinx-rtd-theme (>=2.0.0,<3.0.0)
+Requires-Dist: streamlit (>=1.35.0,<2.0.0)
 Requires-Dist: tensorflow (>=2.12.0,<3.0.0)
 Requires-Dist: tensorflow-io-gcs-filesystem (==0.27.0)
 Requires-Dist: wandb (>=0.17.0,<0.18.0)
 Description-Content-Type: text/markdown
 
 [![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/N8yudTb1)
```

