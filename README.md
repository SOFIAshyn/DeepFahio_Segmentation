# Clothes Segmentation 

## Description:
Segment clothes instances from the photo, classify the category of the instance.

## Dataset:
We used [DeepFashion2](https://github.com/switchablenorms/DeepFashion2) dataset. Main description of the dataset:
* Number of training images: 191961
* Number of validation images: 32153
* Number of test images: 62629
* Number of classes: 13
* Images sizes: differ

## Data Augmentation
To make the model more accurate we would like to use images augmentation. We are using
 [Albumentation](https://github.com/albumentations-team/albumentations) library to do so.

## Segmentation Model:
Decided to build [U-Net Segmentation Model](https://github.com/qubvel/segmentation_models.pytorch) with the `VGG16` 
encoder and pre-trained weights from `imagenet`.

## Author:
[Sofiia Petryshyn](https://github.com/SOFIAshyn/)