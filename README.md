# Beans

Bangkit Academy Final Project

## Dataset Description

Dataset from : https://github.com/AI-Lab-Makerere/ibean/

This dataset is of leaf images taken in the field in different districts in Uganda by the Makerere AI lab in collaboration with the National Crops Resources Research Institute (NaCRRI), the national body in charge of research in agriculture in Uganda.

| Class             | Total Examples|
| ----------------- | ------------- |
| Healthy class     | 428           |
| Angular Leaf Spot | 432           |
| CBean Rust        | 436           |
| Total             | 1,296         |

## Dataset Sample

<img src="https://ibb.co/xCSHRtV" width="500" height="400">

## Goal 

The data is of leaf images representing 3 classes: the healthy class of images, and two disease classes including Angular Leaf Spot and Bean Rust diseases. The model should be able to distinguish between these 3 classes with high accuracy. The end goal is to build a robust, model that can be deployed on a mobile device and used in the field by a farmer.

## Base CNN Model

The CNN base model architecture consists of 3 pair of Conv-Pool layers and 1 hidden layer at fully connected layer without dropout layer(s). There is no image augmentation applied on the training images.

<img src="https://ibb.co/V9QQk3W" width="350" height="300">

## Improved CNN Model

The improved CNN Model architecture consists the same 3 pair of Conv-Pool layers and 1 hidden layer at fully connected layer, but with 2 dropout layers after the 1st Conv-pool layer and after 3rd Conv-Pool layer. Image augmentation is applied on the training images : rotation, width shift, height shift, shear, zoom, and horizontal flip.

<img src="https://ibb.co/98R7fBk" width="350" height="300">

Image augmentation visualization

<img src="https://ibb.co/GWpZtQ4" width="600" height="100">

## Evaluation Comparison

Base CNN model's accuracy and loss

<img src="https://ibb.co/VjYqKfG" width="450" height="300">

Improved CNN model's accuracy and loss

<img src="https://ibb.co/svgDK58" width="450" height="300">






