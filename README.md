# Without Pre-Process
# Brain-Tumor-Detection-for-MRI-Images
Upload the Brain Tumor Images from the Kaggle Dataset. There are total number of 253 images with Yes-192 and No-99.
Images go into the Xlabels and Numbers goes in to the Y label. 
Plot the images.
Label Encoding and one hot encodeing for the y labels.
Build the VGG16 model with frozen the upper layer that tell the model to keep the pre trained weights of these layers unchanges. This is useful when we want to use the pre trained network as feature extractor and only want to train the new layers added.
The new layers are added at the bottom of VGG 16 and the upper layers are frozen i.e Convolution, Pooling, dense, etc.
The model accuracy for the test images in brain tumer detection is around 86%.

# With Pre Process 
CLAHE (Contrast Limited Adaptive Histogram Equalization): Enhances the contrast of the images.
Gaussian Blur: Applies Gaussian blur to reduce noise.
Histogram Equalization: Improves the contrast of the image.
Normalization: Normalizes pixel values to zero mean and unit variance.
PCA (Principal Component Analysis): Reduces the dimensionality of the images to retain variance.
Data Augmentation: Using image Data Generator to produce images of different shapes and scales.

These preprocessing steps can help improve the accuracy of your model by enhancing image quality, reducing noise, and normalizing data. Adjust the parameters and preprocessing techniques as needed based on your specific dataset and requirement.

# Results
The accuracy of the model is increased by 86% from 91% with the use of pre-processing steps for brain tumor detection from MRI images.
