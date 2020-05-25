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

<img src="https://lh3.googleusercontent.com/6QiBDbzh_nhP9dbKmdJ9JxLPvNgWxpNIhjiYWLwj7YgduMTrPw_zY8wQiSzHwceR_j9qj_RRpyJdYA=w2880-h1520" width="500" height="400">

## Goal 

The data is of leaf images representing 3 classes: the healthy class of images, and two disease classes including Angular Leaf Spot and Bean Rust diseases. The model should be able to distinguish between these 3 classes with high accuracy. The end goal is to build a robust, model that can be deployed on a mobile device and used in the field by a farmer.

## Base CNN Model

The CNN base model architecture consists of 3 pair of Conv-Pool layers and 1 hidden layer at fully connected layer without dropout layer(s). There is no image augmentation applied on the training images.

<img src="https://lh3.googleusercontent.com/r-hsZg6XyXaWoOj6EFLpj9Q6hj__7FC_RgHV9JsUdtNpu9AhrM-iQeW4rv1V-7c6XFL_OkffgXQ_EA=w2880-h1520" width="350" height="300">

## Improved CNN Model

The improved CNN Model architecture consists the same 3 pair of Conv-Pool layers and 1 hidden layer at fully connected layer, but with 2 dropout layers after the 1st Conv-pool layer and after 3rd Conv-Pool layer. Image augmentation is applied on the training images : rotation, width shift, height shift, shear, zoom, and horizontal flip.

<img src="https://lh3.googleusercontent.com/pqkhYbEphAHcvICLu49pMG7gJFv8QX6c_85c0Mcm0HeCJ7ZVhW4_izdB-cxwjgknig2imeU7EZNy8Q=w2880-h1520" width="350" height="300">

Image augmentation visualization

<img src="https://lh3.googleusercontent.com/XipJIYQvAXhz0_QNFs4P40P0qaVjEsvhHIqZdfDc_23w8c2NIghFfRc6niUdZ8J2yXsTzKCJTWPUTQ=w2880-h1520" width="600" height="100">

## Evaluation Comparison

Base CNN model's accuracy and loss

<img src="https://lh5.googleusercontent.com/ffSyB72tlrgCF4HxzNzmVfvXW4Ubx7ZgZQKgIDNXNvO9naVvuUzQP9V0a5Ftd3sYqAl1nyB_b9I9Mw=w2880-h1520" width="300" height="150">

Improved CNN model's accuracy and loss

<img src="https://lh6.googleusercontent.com/Po3DlSvbt2U7_BckBWL24k-RsrX4zA22ufZWJXa6iWdT3Fdy4jOISszgcc73YmoTF5t6yEzLv-TejQ=w2880-h1520" width="300" height="150">






