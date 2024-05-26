# Comparing `tmp/NeuroUtils-0.1.6-py3-none-any.whl.zip` & `tmp/NeuroUtils-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 22486 bytes, number of entries: 9
+Zip file size: 23791 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat    28003 b- defN 24-May-18 10:08 NeuroUtils/Architectures.py
--rw-rw-rw-  2.0 fat    52929 b- defN 24-May-23 20:16 NeuroUtils/Core.py
--rw-rw-rw-  2.0 fat    27786 b- defN 24-May-23 10:35 NeuroUtils/ML_assets.py
+-rw-rw-rw-  2.0 fat    55729 b- defN 24-May-26 18:48 NeuroUtils/Core.py
+-rw-rw-rw-  2.0 fat    31793 b- defN 24-May-26 20:27 NeuroUtils/ML_assets.py
 -rw-rw-rw-  2.0 fat       50 b- defN 24-May-10 18:38 NeuroUtils/__init__.py
--rw-rw-rw-  2.0 fat      571 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2078 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      723 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/RECORD
-9 files, 112243 bytes uncompressed, 21244 bytes compressed:  81.1%
+-rw-rw-rw-  2.0 fat      571 b- defN 24-May-26 20:37 NeuroUtils-0.1.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2078 b- defN 24-May-26 20:37 NeuroUtils-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-26 20:37 NeuroUtils-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-26 20:37 NeuroUtils-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      723 b- defN 24-May-26 20:37 NeuroUtils-0.1.7.dist-info/RECORD
+9 files, 119050 bytes uncompressed, 22549 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: NeuroUtils/ML_assets.py
 Comment: 
 
 Filename: NeuroUtils/__init__.py
 Comment: 
 
-Filename: NeuroUtils-0.1.6.dist-info/LICENSE.txt
+Filename: NeuroUtils-0.1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: NeuroUtils-0.1.6.dist-info/METADATA
+Filename: NeuroUtils-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: NeuroUtils-0.1.6.dist-info/WHEEL
+Filename: NeuroUtils-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: NeuroUtils-0.1.6.dist-info/top_level.txt
+Filename: NeuroUtils-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: NeuroUtils-0.1.6.dist-info/RECORD
+Filename: NeuroUtils-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NeuroUtils/Core.py

```diff
@@ -10,18 +10,17 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from timeit import default_timer as timer   
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from tqdm import tqdm
 from contextlib import redirect_stdout
-from ipywidgets import interact, IntSlider
-from IPython.display import display
 from matplotlib.widgets import Slider
 import math
+import cv2
 
 class Utils:
     
     def Initialize_data(DataBase_directory, Data_directory, img_H, img_W, grayscale, Load_from_CSV):
         """
         Initializes -> Loading data from main DataBase folder and load it by classes in 
         data directory
@@ -764,21 +763,30 @@
             if train:
                 #Create callback function to save best performing model
                 
                 if starting_epoch == 0:
                     self.csv_append = False
                 else:
                     self.csv_append = True
-                
-                self.CONSTANT_NOISE = np.random.normal(0, 1, (self.SAMPLE_NUMBER, self.LATENT_DIM))
+                try:
+                    print("Loading Constant noise...")
+                    self.CONSTANT_NOISE = np.load(os.path.join(self.MODEL_DIRECTORY , "Constant_noise.npy"))
+                    
+                except:
+                    print("Failed to load constant noise, generating one...")
+                    constant_noise = np.random.normal(0, 1, (self.SAMPLE_NUMBER, self.LATENT_DIM))
+                    np.save(os.path.join(self.MODEL_DIRECTORY, "Constant_noise.npy") , constant_noise)
+                    self.CONSTANT_NOISE = constant_noise
+                    
                 
                 #Deleting images if training from scratch
-                if os.path.isdir(os.path.join(self.MODEL_DIRECTORY , "Images")) and not self.csv_append:
-                    print("Deleting remaining images from folder 'Images'... ")
-                    ml.General.delete_files_in_folder(os.path.join(self.MODEL_DIRECTORY , "Images"))
+                if os.path.isdir(os.path.join(self.MODEL_DIRECTORY , "Images")) and starting_epoch ==0:
+                    delete_imgs = True
+                else:
+                    delete_imgs = False
                 
                 timer_start = timer()
                 #To add stable noise over continued training, now its only during one session
                 with tf.device(self.DEVICE):
                     for epoch in range(starting_epoch+1 , self.EPOCHS+1):
                         print("\nEpoch:",epoch)
                         steps_per_epoch = len(self.X_TRAIN) // self.BATCH_SIZE
@@ -806,15 +814,22 @@
                                 noise = np.random.normal(0, 1, (self.BATCH_SIZE, self.LATENT_DIM))
                                 ones = np.ones((self.BATCH_SIZE, 1))
                                 generator_loss = self.MODEL.train_on_batch(noise, ones)
                                 
                                 
                         # Print the progress
                         sys.stdout.write(f"\n[D loss: {discriminator_loss[0]:.3f} | D acc: {discriminator_loss[1]:.3f}] [G loss: {generator_loss:.3f}]")    
-                       
+                        
+                        #Delete images if first iteration
+                        if delete_imgs:
+                            print("Deleting remaining images from folder 'Images'... ")
+                            ml.General.delete_files_in_folder(os.path.join(self.MODEL_DIRECTORY , "Images"))
+                            delete_imgs = False
+                            
+                        
                         # Save generated images every sample_interval
                         #gan_callback()
                         self.Callback(current_epoch = epoch,
                                       constant_noise = self.CONSTANT_NOISE
                                       )
                             
                         #To make in callbacks some kind of stable random noise to have nice animation of training
@@ -827,15 +842,15 @@
                 print("Loading model which was performing best during training...\n")
                 self.MODEL.load_weights(self.MODEL_WEIGHTS_DIRECTORY)   
 
 
 
                                 
 
-        def Initialize_history(self,plot_size = 3):
+        def Initialize_history(self,show_plot, plot_size , create_gif = False, gif_scale = 1, gif_fps = 20):
             if plot_size**2>self.SAMPLE_NUMBER:
                 print("Not enough samples, consider reducing plot size")
                 return
             #1
             #Loading most actual model to initialize results
             try:
                 print("Trying to load most actual model...")
@@ -853,79 +868,108 @@
                 sample = np.load(os.path.join(path,filename))
                 history_array.append(sample)
                 
             history_array = np.array(history_array)
             
             if len(history_array) == 0:
                 print("There is no data, try to train model a little first")
+                return
             
-            plt.subplots_adjust(bottom=0.25)
+            if create_gif:
+                grid_array = ml.General.create_image_grid(history_array , size = plot_size)
+                ml.General.create_gif(gif_array = grid_array,
+                                      gif_filepath = os.path.join(self.MODEL_DIRECTORY , "Training_history.gif"),
+                                      gif_height = int(grid_array.shape[1]*gif_scale),
+                                      gif_width = int(grid_array.shape[2]*gif_scale),
+                                      fps = gif_fps
+                                      )
             
-            def update_plot(val):
-                epoch = int(val)
-                plt.suptitle(f"Epoch {epoch}")
-                for i in range(plot_size**2):
-                    plt.axis("off")
-                    plt.subplot(plot_size,plot_size,i+1)
-                    if epoch < len(history_array):
-                        if self.GRAYSCALE:
-                            plt.imshow(history_array[epoch][i], cmap="gray")
-                        else:
-                            plt.imshow(history_array[epoch][i])
-                    else:
-                        plt.text(0,0,"No data")  # Display blank image if epoch exceeds available data
-                plt.draw()
-                    
-            ax_slider = plt.axes([0.25, 0.1, 0.65, 0.03], facecolor='lightgoldenrodyellow')
-            slider = Slider(ax_slider, 'Epoch', 0, len(history_array)-1, valinit=0, valstep=1)
             
-            # Update the plot when the slider value changes
-            slider.on_changed(update_plot)
             
-            # Initialize the first plot
-            update_plot(0)
+            def update_plot(epoch):
+                ax.clear()  # Clear the previous image
+                plt.title("Training history\nEpoch: "+str(epoch))
+                if self.GRAYSCALE:
+                    ax.imshow(grid_array[epoch], cmap="gray")
+                else:
+                    ax.imshow(grid_array[epoch])
+                    
+                # Optionally, update the title
+                ax.axis("off")
+                plt.draw()
+  
+            if show_plot:  
+                #plt.subplots_adjust(bottom=0.25)
+                # Create the figure and the axis
+                fig, ax = plt.subplots()
+                plt.subplots_adjust(left=0.25, bottom=0.25)
+                
+                ax_slider = plt.axes([0.25, 0.1, 0.65, 0.03], facecolor='lightgoldenrodyellow')
+                slider = Slider(ax_slider, 'Epoch', 0, len(history_array)-1, valinit=0, valstep=1)
+                
+                # Update the plot when the slider value changes
+                slider.on_changed(update_plot)
+                
+                # Initialize the first plot
             
-            plt.show()
+                update_plot(0)
+                
+                plt.show()
+            else:
+                slider = None
                 
             
             return history_array , slider
             
         
-        def Initialize_results(self,plot_size = 4):
+        def Initialize_results(self,show_plot, plot_size = 4, saveplot = False, plot_scale = 1):
             #1
             #Loading most actual model to initialize results
             try:
                 print("Trying to load most actual model...")
                 self.MODEL.load_weights(self.MODEL_WEIGHTS_DIRECTORY)  
             except:
                 print("Could not load most actual model, working with current one loaded")
             
             Gen_imgs , _ = ml.General.generate_fake_samples(gan_generator = self.GENERATOR,
                                                     latent_dim = self.LATENT_DIM,
                                                     n_samples = plot_size**2
                                                     )
             Gen_imgs = (Gen_imgs+1)/2
+            Gen_imgs = np.array(Gen_imgs*255 , dtype = np.uint8)
             
-            plt.figure()
-            plt.suptitle("Results of generator")
-            for i in range(plot_size**2):
-                plt.subplot(plot_size,plot_size,i+1)
+            Grid_img = ml.General.create_image_grid(Gen_imgs, plot_size)
+
+        
+        
+            if show_plot:
+                plt.figure()
                 plt.axis("off")
+                plt.title("Model Results")
                 if self.GRAYSCALE:
-                    plt.imshow(Gen_imgs[i] , cmap = 'gray')
+                    plt.imshow(Grid_img , cmap = 'gray')
                 else:
-                    plt.imshow(Gen_imgs[i])
+                    plt.imshow(Grid_img)
+            if saveplot:
+                save_dir = os.path.join(self.MODEL_DIRECTORY , 'Generator_results.png')
+                Resized_grid_img = cv2.resize(Grid_img, (int(Grid_img.shape[0]*plot_scale), int(Grid_img.shape[1]*plot_scale)), interpolation=cv2.INTER_NEAREST)
+                cv2.imwrite(save_dir,Resized_grid_img)
+                
+            return Gen_imgs
+                
+
                     
             
-        def Initialize_results_interpolation(self,n_variations = 10, steps_to_variation = 50):
+        def Initialize_results_interpolation(self,n_variations, steps_to_variation, create_gif = False, gif_scale = 1,gif_fps = 20):
             gen_img_list = []
             n_vectors = n_variations
             steps = steps_to_variation
             #Interpolated latent vectors for smooth transition effect
-            latent_vectors = [np.random.randn(self.LATENT_DIM) for _ in range(n_vectors)]
+            latent_vectors = [np.random.randn(self.LATENT_DIM) for _ in range(n_vectors-1)]
+            latent_vectors.append(latent_vectors[0])
             interpolated_latent_vectors = []
             for i in range(len(latent_vectors)-1):
                 for alpha in np.linspace(0, 1, steps, endpoint=False):
                     interpolated_vector = latent_vectors[i] * (1 - alpha) + latent_vectors[i + 1] * alpha
                     interpolated_latent_vectors.append(interpolated_vector)
             # Add the last vector to complete the sequence
 
@@ -943,15 +987,26 @@
                 gen_img_list.append(gen_img)
                 ##########
 
 
                 
                 
             gen_img_list = np.array(gen_img_list)
-            
+            if create_gif:
+                try:
+                    ml.General.create_gif(gif_array = (gen_img_list*255).astype(np.uint8),
+                                          gif_filepath = os.path.join(self.MODEL_DIRECTORY , "Model_interpolation.gif"),
+                                          gif_height = int(gen_img_list.shape[1]*gif_scale) ,
+                                          gif_width = int(gen_img_list.shape[2]*gif_scale),
+                                          fps = gif_fps
+                                          )
+                    print("Interpolation gif created!")
+                    
+                except:
+                    print("Could not create gif file")
             #Plot
             
             def update_interpol(i):
                 ax.clear()  # Clear the previous image
                 if self.GRAYSCALE:
                     ax.imshow(gen_img_list[i], cmap="gray")
                 else:
```

## NeuroUtils/ML_assets.py

```diff
@@ -7,15 +7,15 @@
 from tqdm import tqdm
 import random
 from scipy.ndimage import rotate
 import pandas as pd
 import matplotlib.pyplot as plt
 import sklearn as skl
 import itertools
-os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
+from PIL import Image
 
 
 class DataSets:
     #Scenario 1
     #If it is classification data
     ################################################
     
@@ -714,9 +714,121 @@
             file_path = os.path.join(folder_path, filename)
             # Check if the path is a file (not a subdirectory)
             if os.path.isfile(file_path):
                 # Delete the file
                 os.remove(file_path)
     
     
+    # Function to create and save a GIF
+    def create_gif(gif_array, gif_filepath, gif_height, gif_width, fps=5):
+        if not isinstance(gif_array, np.ndarray):
+            raise ValueError("Input must be a numpy array")
+        
+        if gif_array.dtype != np.uint8:
+            raise ValueError("Array must be in np.uint8 format; [0-255] range")
+    
+        # Convert numpy arrays to PIL Images
+        images = [Image.fromarray(frame) for frame in gif_array]
+        images = [img.resize((gif_width,gif_height), Image.Resampling.NEAREST) for img in images]
+        
+        # Save the images as a GIF
+        images[0].save(
+            gif_filepath, 
+            save_all=True, 
+            append_images=images[1:], 
+            duration=int(1000 / fps), 
+            loop=0
+        )    
+
+
+    def create_image_grid(img_array, size, RGB = False):
+        #To improve so it can handle rgb images as well, also describe required array configuration to work
+        
+        if len(img_array.shape) == 3 and not RGB:
+            single_iteration = True
+            
+        elif len(img_array.shape) == 4 and RGB:
+            single_iteration = True
+
+        else:
+            single_iteration = False
+            
+              
+        try:
+            if RGB:
+                if single_iteration:
+                    img_array = img_array[0:size**2,:,:,:]
+                else:
+                    img_array = img_array[:,0:size**2,:,:,:]
+                
+            else:
+                if single_iteration:
+                    img_array = img_array[0:size**2,:,:]
+                else:
+                    img_array = img_array[:,0:size**2,:,:]
+                
+        except:
+            print("Size is too big for given array, increase number of samples or decrease size of grid")
+            return
+            
+        # Calculate grid size (e.g., 5x5 for 25 images)
+        if single_iteration:
+            iterations = 1
+            num_images = img_array.shape[0]
+            cell_height = img_array.shape[1]
+            cell_width = img_array.shape[2]
+
+        else:
+            iterations = img_array.shape[0]
+            num_images = img_array.shape[1]
+            cell_height = img_array.shape[2]
+            cell_width = img_array.shape[3]
+            
+        grid_size = int(np.ceil(np.sqrt(num_images)))
+        
+        # Determine the size of each cell in the grid
+        grid_array = []
+        # Create an empty grid image
+        for i in range(iterations):
+            if RGB:
+                grid_img = np.zeros((grid_size * cell_height, grid_size * cell_width,3), dtype=np.uint8)
+            else:
+                grid_img = np.zeros((grid_size * cell_height, grid_size * cell_width), dtype=np.uint8)
+                
+            
+            for idx in range(num_images):
+                row = idx // grid_size
+                col = idx % grid_size
+                if RGB:
+                    if single_iteration:
+                        grid_img[row * cell_height: (row + 1) * cell_height, col * cell_width: (col + 1) * cell_width,:] = img_array[idx]
+                    else:
+                        grid_img[row * cell_height: (row + 1) * cell_height, col * cell_width: (col + 1) * cell_width,:] = img_array[i][idx]
+                else:
+                    if single_iteration:
+                        grid_img[row * cell_height: (row + 1) * cell_height, col * cell_width: (col + 1) * cell_width] = img_array[idx]
+                    else:
+                        grid_img[row * cell_height: (row + 1) * cell_height, col * cell_width: (col + 1) * cell_width] = img_array[i][idx]
+            
+            grid_array.append(grid_img)   
+        grid_array = np.array(grid_array)
+        
+        if single_iteration:
+            grid_array = grid_array[0]
+            
+        return grid_array    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+
```

## Comparing `NeuroUtils-0.1.6.dist-info/LICENSE.txt` & `NeuroUtils-0.1.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `NeuroUtils-0.1.6.dist-info/METADATA` & `NeuroUtils-0.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroUtils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library for neural network projects organisation
 Author-email: Sebastian Borukało <Ciapserr@gmail.com>
 Project-URL: Homepage, https://github.com/Ciapser/NeuroUtils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `NeuroUtils-0.1.6.dist-info/RECORD` & `NeuroUtils-0.1.7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 NeuroUtils/Architectures.py,sha256=SlgWVuAhl0n9_WeBiDkl11WSd3Sw2Fd41Jlq522nrlw,28003
-NeuroUtils/Core.py,sha256=YM8X3uERKNFp3l5Z-GXy-hUXa4Zsbi8gsxTv3TKIN6M,52929
-NeuroUtils/ML_assets.py,sha256=t73ByEeZLNbmFuhrAkeFN6PTyzuw-TZjLXkGFq_t0eg,27786
+NeuroUtils/Core.py,sha256=C2cSSnywizl5d-F8Fr6MmT40zmm4czILcT_rprx0LNw,55729
+NeuroUtils/ML_assets.py,sha256=GEI3HE7A5gZ3xaqmRIiucQ02QdCGsZ8K5leFPkDn09g,31793
 NeuroUtils/__init__.py,sha256=M19PlxWTqxnYsQc03A3XCzFoFFNRpV0uBG0B-76TLBQ,50
-NeuroUtils-0.1.6.dist-info/LICENSE.txt,sha256=aUncEakBCK32RA3QKKi4TV-y1cb4gwGer68lX2Z7NBE,571
-NeuroUtils-0.1.6.dist-info/METADATA,sha256=z9Rjqz-2aOKYUYqBJv27JSyGQuumLTj3_BfgGeovZ0w,2078
-NeuroUtils-0.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-NeuroUtils-0.1.6.dist-info/top_level.txt,sha256=1PAx5XIE5jUM7BcxFhiGFXZ0ZpFhT5BzUQn8nwtSs_Q,11
-NeuroUtils-0.1.6.dist-info/RECORD,,
+NeuroUtils-0.1.7.dist-info/LICENSE.txt,sha256=aUncEakBCK32RA3QKKi4TV-y1cb4gwGer68lX2Z7NBE,571
+NeuroUtils-0.1.7.dist-info/METADATA,sha256=f6YzGod_z7QfoOqqPsWxbohHqF-8YLzHFtpfAUdesmU,2078
+NeuroUtils-0.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+NeuroUtils-0.1.7.dist-info/top_level.txt,sha256=1PAx5XIE5jUM7BcxFhiGFXZ0ZpFhT5BzUQn8nwtSs_Q,11
+NeuroUtils-0.1.7.dist-info/RECORD,,
```

