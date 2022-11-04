# Image-and-Video-Segmentation-using-Mask-R-CNN-

Performed Instance image segmentation using Mask Region-Based Convolutional Neural Network(Mask R-CNN)  by generating  bounding boxes, extracting segmented objects and detected target class.

![PHOTO-2022-11-03-21-38-15](https://user-images.githubusercontent.com/68578215/200013571-c8732871-1fa1-4039-afae-50e4fac9779f.jpg)


## Object Detection  

Object Detection refers to the method of identifying and correctly labeling all the objects present in the image frame.

This broadly consists of two steps :

**Object Localization:** Here, a bounding box or enclosing region is determined in the tightest possible manner in order to locate the exact position of the object in the image.

**Image Classification:** The localized object is then fed to a classifier which labels the object.

![Screen Shot 2022-11-04 at 11 24 04 AM](https://user-images.githubusercontent.com/68578215/200048407-4f23438e-2da3-4949-880b-6f1e2a0418c1.png)


## Semantic Segmentation

It refers to the process of linking each pixel in the given image to a particular class label. For example in the following image the pixels are labelled as car, tree, pedestrian etc. These segments are then used to find the interactions / relations between various objects.

![Screen Shot 2022-11-04 at 11 23 54 AM](https://user-images.githubusercontent.com/68578215/200048410-1726b054-2c88-4767-9838-d989acf675d8.png)


## Instance Segmentation

Here, we associate a class label to each pixel similar to semantic segmentation, except that it treats multiple objects of the same class as individual objects / separate entities.

![Screen Shot 2022-11-04 at 11 23 48 AM](https://user-images.githubusercontent.com/68578215/200048412-3cb339a6-398a-4bec-8d89-ae9c8de07e78.png)
