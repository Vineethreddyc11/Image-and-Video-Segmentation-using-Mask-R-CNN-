# Image-and-Video-Segmentation-using-Mask-R-CNN-

Performed Instance image segmentation using Mask Region-Based Convolutional Neural Network(Mask R-CNN)  by generating  bounding boxes, extracting segmented objects and detected target class.

![PHOTO-2022-11-03-21-38-15](https://user-images.githubusercontent.com/68578215/200013571-c8732871-1fa1-4039-afae-50e4fac9779f.jpg)


## Object Detection  

Object Detection refers to the method of identifying and correctly labeling all the objects present in the image frame.

This broadly consists of two steps :

**Object Localization:** Here, a bounding box or enclosing region is determined in the tightest possible manner in order to locate the exact position of the object in the image.

**Image Classification:** The localized object is then fed to a classifier which labels the object.

## Semantic Segmentation

It refers to the process of linking each pixel in the given image to a particular class label. For example in the following image the pixels are labelled as car, tree, pedestrian etc. These segments are then used to find the interactions / relations between various objects.

## Instance Segmentation

Here, we associate a class label to each pixel similar to semantic segmentation, except that it treats multiple objects of the same class as individual objects / separate entities.
