# Image-Segmentation-Seep-Detection-using-UNET

Detecting oil seeps from Satelitte (SAR) images using deep convolutional neural networks.

Creating a UNET model for performing segmentation
UNET:- It is a Deep Convolutional Neural Network. The network is based on a fully convolutional network whose architecture was modified and extended to work with fewer training images and yield more precise segmentation. It performs classification on every pixel so that the input and output share the same size. UNet is able to do image localisation by predicting the image pixel by pixel which is exactly what the problem statement demands.The model would make prediction on every pixels, resulting in the detection of oil seeps from SAR images in our case

For this image segmentation task I followed an encoder/decoder structure where we downsample the spatial resolution of the input, developing lower-resolution feature mappings which are learned to be highly efficient at discriminating between classes, and the upsample the feature representations into a full-resolution segmentation map.

In DCNN the earlier layers tend to learn low-level features while later layers develop more high-level feature mappings.Hence the need to upsample.

Evaluation Metrics Used
1) Dice Loss: The loss function used for our image segmentation task is based on the Dice coefficient, which is essentially a measure of overlap between two samples. This measure ranges from 0 to 1 where a Dice coefficient of 1 denotes perfect and complete overlap.

2) Dice Coefficient

3) IOU: The Intersection over Union metric (Jaccard index) is essentially a method to quantify the percent overlap between the target mask and our prediction output.

4) Accuracy
