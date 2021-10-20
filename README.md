# Cell Confluency Using Image Segmentation

## Project Details
Currently employed methods:  
1- U-Net CNN (Supervised Learning)  
2- K-Means Clustering (Unsupervised Learning)  

Platform IDEs:  
1- Anaconda  
2- Pycharm (Script development)  
3- Spyder (Data viewer & visualization)  

Language: Python

## Current Progress
### 1. U-Net CNN
<details open>
<summary>Methodology</summary>
<br>
 
**Step 1-** Data annotation. Cells are labelled to distinguish between the background and the cell confluency.  
  
**Step 2-** (Optional) Data/ Image patching. If your data resolutions/ dimensions are high, this step is recommended for GPU support. [[Reference 1](https://github.com/Fyzie/Cell-Confluency/blob/main/U-Net%20CNN/patch_images_masks_for_large_image.py)] [[Reference 2](https://github.com/bnsreenu/python_for_microscopists/blob/master/Tips_Tricks_5_extracting_patches_from_large_images_and_masks_for_semantic_segm.py)]
  
**Step 3-** U-Net model development. [[Reference](https://github.com/bnsreenu/python_for_microscopists/blob/master/204-207simple_unet_model.py)]  
  
**Step 4-** Data Training. [[Reference](https://github.com/bnsreenu/python_for_microscopists/blob/master/204_train_simple_unet_for_mitochondria.py)]
  
**Step 5-** Model Inference and Prediction. [[Reference](https://github.com/bnsreenu/python_for_microscopists/blob/master/204_train_simple_unet_for_mitochondria.py)]
  
**Step 6-** Model Application. [[Reference 1](https://github.com/bnsreenu/python_for_microscopists/blob/master/206_sem_segm_large_images_using_unet_with_custom_patch_inference.py)] [[Reference 2](https://github.com/bnsreenu/python_for_microscopists/blob/master/206_sem_segm_large_images_using_unet_with_patchify.py)]

</details>

<details open>
<summary>Arising Problems</summary>
<br>

1- GPU exhaustion lead to the needs for:  
  (a) batch size reduction  
  (b) dimensions reduction  
  (c) data training reduction
  
2- Bad model development lead to:  
  (a) error prediction and inference  

</details>

### 2. K-Means Clustering

<details open>
<summary>Methodology</summary>
<br>

**Step 1-** Image Normalization.
  
**Step 2-** Image Flattening.
  
**Step 3-** K-Means Clustering. Identify number of clusters accordingly to available distinct regions.
  
**Step 4-** Labeled Image Restructuring.
  
**Step 5-** Data Reshaping.
  
[[Reference](https://github.com/Fyzie/Cell-Confluency/blob/main/K-means/Kmeans_sklearn_for_image_segmentation.py)]
  
</details>

<details open>
<summary>Arising Problems</summary>
<br>
  
1- Bad clustering may due to:  
  (a) irregular brightness of image datasets (trying to normalize them in Step 1) 
  
</details>

## Image Segmentation
Image segmentation is a process of partitioning images into multiple distinguished regions containing each pixel with similar features/ attributes.




