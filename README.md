# Clothes Segmentation 

## Description:
The aim of the project is to teach the model to segment clothes instances from the photo and, as a bonus, then classify the category of the instance.\
Steps to implement of such a solution:
1. MNiST dataset calssificator: `ClothesClassification_v1.ipynb`
2. DeepFashion2 dataset segmentation: `U-Net-Segmentation.ipynb`
3. IMatherialist dataset segmentation: `Segmentation_v2.ipynb`

## Datasets:
1. [MNIST dataset](https://www.tensorflow.org/api_docs/python/tf/keras/datasets/fashion_mnist)
* Number of training images: 60000
* Number of testing images: 10000
* Number of classes: 10
* Images sizes: 28x28
2. [DeepFashion2](https://github.com/switchablenorms/DeepFashion2)
* Number of training images: 191961
* Number of validation images: 32153
* Number of test images: 62629
* Number of classes: 13
* Images sizes: differ
3. [IMatherialist](https://www.kaggle.com/c/imaterialist-fashion-2019-FGVC6/data)
* Number of training images: xxx
* Number of validation images: xxx
* Number of test images: xxx
* Number of classes: 46
* Images sizes: differ

## Data Augmentation
To make the model more accurate we would like to use images augmentation. We are using
 [Albumentation](https://github.com/albumentations-team/albumentations) library to do so.

## Segmentation Model:
1. For classification problem desided to use Squential with two Dense layers.
2. For segmenattion problem decided to build [U-Net Segmentation Model](https://github.com/qubvel/segmentation_models.pytorch) with the `VGG16` and `mobilenet_v2` encoder and pre-trained weights from `imagenet`.
3. For future implementation desided to try to use [U-2 Net](https://github.com/NathanUA/U-2-Net), [paper is here](https://arxiv.org/pdf/2005.09007v2.pdf)

## Author:
[Sofiia Petryshyn](https://github.com/SOFIAshyn/)
