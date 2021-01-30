# COVID-Net
Model for COVID detection in X-Rays
Further a Flask based platform is finished for easy inference on images.

## Dataset
Augemented + Segmented + Equalized : https://drive.google.com/drive/folders/1VP-g1lDvGn-WytEFYnvoBe1oqsMtkV2n?usp=sharing

Original Data : https://github.com/ieee8023/covid-chestxray-dataset

## Pipeline
Input Image -> Augmentation -> Segmentation -> Mask Cropping -> VGG16 -> Diagnosis

## CAM results

![no-seg](https://user-images.githubusercontent.com/57294033/106353420-76482c00-6310-11eb-9b3b-092865355207.png)

CAM analysis on non-segmented images, model learns irrelevant features. Overfitting to other source semantics.

![seg](https://user-images.githubusercontent.com/57294033/106353439-9677eb00-6310-11eb-8c7e-954c43b94112.png)

CAM analysis on segmented images, model learns imporrtant features which are further verified by professional diagnosis of the same image.


