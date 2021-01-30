# COVID-Net
Model for COVID detection in X-Rays

## Dataset
Augemented + Segmented + Equalized : https://drive.google.com/drive/folders/1VP-g1lDvGn-WytEFYnvoBe1oqsMtkV2n?usp=sharing

Original Data : https://github.com/ieee8023/covid-chestxray-dataset

## Pipeline
Input Image -> Augmentation -> Segmentation -> Mask Cropping -> VGG16 -> Diagnosis

## CAM results

![no-seg](https://user-images.githubusercontent.com/57294033/106353307-8f9ca880-630f-11eb-891c-dc0492903bef.png) 

CAM analysis on non-segmented images, model learns irrelevant features. Overfitting to other source semantics.

![seg](https://user-images.githubusercontent.com/57294033/106353309-91ff0280-630f-11eb-9d36-378a59178a52.png) 

CAM analysis on segmented images, model learns imporrtant features which are further verified by professional diagnosis of the same image.
