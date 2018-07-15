---
layout: post
title: Importance and ways to Augment an Image for segmentation task
---

Medical Image segmentation is an important task in life-science. Counting cell in a blood slide is very time consuming and tedious.

**Data Augmentation**:
Data augmentation is the most important task in any deep learning project which involves images. I believe we should have full control on all the image augmentations as they have immense effect on training. A good augmentation not only reduces the amount of data required also improves the trained model to learn only the important pattern required to classify. 

Below is an example of segmenting of blood sample, we will be segmenting white blood cells present in blood. The available data is limited only about **100** samples. 

Types of Augmentation: There are various types of augmentation possible but each depend about the underlying job and the type of data you are fitting to.
**Zoom**: Zoom is one of the augmentation which works for almost all as Convolutional neural networks are bad in learning scales unless specified.
**Rotation**: Keep in mind how much rotation is Ok for the task, e.g. It is better to not rotate too much for some objects like hmm.. Tree maybe
**Shift**: horizontal and vertical shifts make sure you object of interest is still inside. Shift don’t help much though with Convolutional nets.
**Sheer**: Shift can be applied in both Width and Height. For some cases sheer is not correct, just take a dummy case "training a network to learn a square shape”, sheer will destroy the main idea behind a square. example: training a network on facial landmark. excellent augmentation but make sure you have things in limit. For blood segmentation its a good augmentation.
**Channel Shift**: Channel shift works well for many objects like cars, mug etc as they can be of any colour and it works well in training.
**Flip**: Horizontal and vertical flip.



**Photometric augmentation**:
Photometric Augmentation captures the distortion and noise cased by different camera sensors and lightning conditions.
**Brightness**, **Hue Saturation**, **Contrast** etc.

 
Things to keep in mind while doing data augmentation:
TBD later
<!--![_config.yml]({{ site.baseurl }}/images/config.png)-->
