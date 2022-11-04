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


## Bounding Box
It is a tight rectangle used to enclose the object of interest. It is generally described by four values : (bx, by, bh, bw) .
Where (bx, by) are the co-ordinates of the center of the box and bh, bw are the height and width of the box respectively measured on a scale of 0 to 1.

## Anchor Boxes
These are a set of predefined bounding boxes of a certain height and width. These boxes are defined to capture the scale and aspect ratio of specific object classes you want to detect and are typically chosen based on object sizes in your training data-sets. During detection, the predefined anchor boxes are tiled across the image. The network predicts the probability and other attributes, such as background, intersection over union (IoU) and offsets for every tiled anchor box. The predictions are used to refine each individual anchor box. You can define several anchor boxes, each for a different object size.



Thus the network refines these anchor boxes to finally output the tight bounding boxes. These are defined by the scale and aspect ratio.

Aspect Ratio is the width / height of the box.

Size is the height and width of the box. eg (256 x 256)

Scale is the multiplying factor of the required box w.r.t to base box

Intersection over Union (IOU) :

It is an evaluation metric used to check the accuracy of the predicted bounding box w.r.t the actual ground truth.



An IOU of > 0.5 is considered as a good prediction and is used for further evaluation.

