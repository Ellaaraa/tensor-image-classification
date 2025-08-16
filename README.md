# Image Classification with Tensors

This project demonstrates an approach to **image classification** using **tensor representations** and **Tucker decomposition**.

## What the Code Does

1. **Loads the dataset**  
   - 28 training images: 14 cats and 14 birds  
   - 12 test images to classify  

2. **Represents images as tensors**  
   Each image is treated as a tensor (multi-dimensional array), which allows us to apply tensor decomposition methods.

3. **Learns basis matrices from training data**  
   Using Tucker decomposition, the training images are broken down into smaller feature representations.  
   This reduces the dimensionality while keeping the most important information.

4. **Extracts features for test images**  
   The same learned basis is applied to the test images so they can be represented in the same feature space as the training images.

5. **Classifies test images**  
   The test image features are compared with the training image features to assign labels (cat or bird).

---

## Dataset

The dataset used is small and consists of:
- 14 cat images  
- 14 bird images  

This gives us 2 classes in total.  
The method is applied first on grayscale images, then extended to color images.
